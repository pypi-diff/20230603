# Comparing `tmp/apertium2ud-0.0.3.tar.gz` & `tmp/apertium2ud-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium2ud-0.0.3.tar", last modified: Fri Jun  2 03:59:03 2023, max compression
+gzip compressed data, was "apertium2ud-0.0.4.tar", last modified: Fri Jun  2 23:08:37 2023, max compression
```

## Comparing `apertium2ud-0.0.3.tar` & `apertium2ud-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.731982 apertium2ud-0.0.3/
--rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.3/LICENSE
--rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.3/MANIFEST.in
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 03:59:03.725988 apertium2ud-0.0.3/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2095 2023-05-26 10:57:10.000000 apertium2ud-0.0.3/README.md
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.329879 apertium2ud-0.0.3/apertium2ud/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1884 2023-06-01 16:50:15.000000 apertium2ud-0.0.3/apertium2ud/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1818 2023-05-25 10:21:43.000000 apertium2ud-0.0.3/apertium2ud/_map_processing.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1129 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/apertium2ud/convert.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/apertium2ud/meta.py
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.680919 apertium2ud-0.0.3/apertium2ud/resources/
--rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.3/apertium2ud/resources/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.3/apertium2ud/resources/tags_map.json
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.586528 apertium2ud-0.0.3/apertium2ud.egg-info/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)      380 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/SOURCES.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/dependency_links.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 03:59:01.000000 apertium2ud-0.0.3/apertium2ud.egg-info/not-zip-safe
--rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/top_level.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-06-02 03:59:03.733986 apertium2ud-0.0.3/setup.cfg
--rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/setup.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.397187 apertium2ud-0.0.4/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.4/LICENSE
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.4/MANIFEST.in
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 23:08:37.388741 apertium2ud-0.0.4/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2095 2023-05-26 10:57:10.000000 apertium2ud-0.0.4/README.md
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:36.715796 apertium2ud-0.0.4/apertium2ud/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2529 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/apertium2ud/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1856 2023-06-02 22:12:01.000000 apertium2ud-0.0.4/apertium2ud/_map_processing.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1816 2023-06-02 22:50:42.000000 apertium2ud-0.0.4/apertium2ud/convert.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/apertium2ud/meta.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.317320 apertium2ud-0.0.4/apertium2ud/resources/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.4/apertium2ud/resources/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     4037 2023-06-01 17:05:34.000000 apertium2ud-0.0.4/apertium2ud/resources/custom.udx
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.4/apertium2ud/resources/tags_map.json
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 23:08:37.010610 apertium2ud-0.0.4/apertium2ud.egg-info/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      413 2023-06-02 23:08:36.000000 apertium2ud-0.0.4/apertium2ud.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 23:08:34.000000 apertium2ud-0.0.4/apertium2ud.egg-info/not-zip-safe
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-06-02 23:08:35.000000 apertium2ud-0.0.4/apertium2ud.egg-info/top_level.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-06-02 23:08:37.402189 apertium2ud-0.0.4/setup.cfg
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-06-02 23:07:37.000000 apertium2ud-0.0.4/setup.py
```

### Comparing `apertium2ud-0.0.3/LICENSE` & `apertium2ud-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.3/PKG-INFO` & `apertium2ud-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `apertium2ud-0.0.3/README.md` & `apertium2ud-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.3/apertium2ud/_map_processing.py` & `apertium2ud-0.0.4/apertium2ud/_map_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 
     while len(queue) > 0:
         name, item = queue.pop(0)
 
         # if 'terminal' node (essentially, leaf node)
         if "t" in item:
             tags = item.get("tags", [])
+
             # ...add the rule to ud2a
             key = tuple(tags + sorted(item.get("feats", [])))
             value = name
             ud_combination2apertium[key].append(value)
+
             # ... add the rule to a2ud
             if len(tags) < 2:
                 apertium2ud_combination[name].append({"tag": item["tags"] if "tags" in item else [],
                                                       "feats": item["feats"] if "feats" in item else []})
             elif len(tags) == 2:
                 for tag in tags:
                     apertium2ud_combination[name].append({"tag": tag,
@@ -42,8 +44,8 @@
         else:
             # ...go deeper
             for k in item:
                 queue.append((k, item[k]))
 
     ud2a_results = sorted(list(ud_combination2apertium.items()), key=lambda x: len(x[0]), reverse=True)
 
-    return ud2a_results, dict(apertium2ud_combination)
+    return ud2a_results, {frozenset({k}): v for k, v in apertium2ud_combination.items()}
```

### Comparing `apertium2ud-0.0.3/apertium2ud/resources/tags_map.json` & `apertium2ud-0.0.4/apertium2ud/resources/tags_map.json`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.3/apertium2ud.egg-info/PKG-INFO` & `apertium2ud-0.0.4/apertium2ud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `apertium2ud-0.0.3/setup.py` & `apertium2ud-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apertium2ud",
     packages=setuptools.find_packages(),
-    version="0.0.3",
+    version="0.0.4",
     description="Converting universal tags to Apertium tags.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Anton Alekseev",
     author_email="anton.m.alexeye@gmail.com",
     url="https://github.com/alexeyev/apertium2ud",
     keywords=["natural language processing", "apertium", "morphology"],
```

