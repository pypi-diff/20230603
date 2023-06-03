# Comparing `tmp/thumbor_hsl-0.0.2.tar.gz` & `tmp/thumbor_hsl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thumbor_hsl-0.0.2.tar", last modified: Sat Jun  3 12:32:55 2023, max compression
+gzip compressed data, was "thumbor_hsl-0.0.3.tar", last modified: Sat Jun  3 12:59:56 2023, max compression
```

## Comparing `thumbor_hsl-0.0.2.tar` & `thumbor_hsl-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-03 12:32:39.000000 thumbor_hsl-0.0.2/thumbor_hsl/loaders/http_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:32:55.914669 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 12:32:55.000000 thumbor_hsl-0.0.2/thumbor_hsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/thumbor_hsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/thumbor_hsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/thumbor_hsl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/thumbor_hsl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-03 12:59:40.000000 thumbor_hsl-0.0.3/thumbor_hsl/loaders/http_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:59:56.448292 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-03 12:59:56.000000 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-03 12:59:56.000000 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:59:56.000000 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 12:59:56.000000 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 12:59:56.000000 thumbor_hsl-0.0.3/thumbor_hsl.egg-info/top_level.txt
```

### Comparing `thumbor_hsl-0.0.2/LICENSE` & `thumbor_hsl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbor_hsl-0.0.2/PKG-INFO` & `thumbor_hsl-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbor_hsl
-Version: 0.0.2
+Version: 0.0.3
 Summary: A modified `http` loader for thumbor which provides additional statistics (like width, height and url parsing)
 Home-page: https://github.com/BowlingX/thumbor-http-stats-loader
 Author: David Heidrich
 Author-email: me@bowlingx.com
 License: MIT
 License-File: LICENSE
```

### Comparing `thumbor_hsl-0.0.2/README.md` & `thumbor_hsl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `thumbor_hsl-0.0.2/setup.py` & `thumbor_hsl-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """print long description"""
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='thumbor_hsl',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     url='https://github.com/BowlingX/thumbor-http-stats-loader',
     license='MIT',
     author='David Heidrich',
     author_email='me@bowlingx.com',
     install_requires=['thumbor>=7.0.0a2,<8'],
     description='A modified `http` loader for thumbor which provides additional statistics '
```

### Comparing `thumbor_hsl-0.0.2/thumbor_hsl/loaders/http_loader.py` & `thumbor_hsl-0.0.3/thumbor_hsl/loaders/http_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     regex_match = context.config.HSL_REGEX_MATCH_URL
 
     def callback():
         return http_loader.return_contents(response, url, context, req_start)
 
     if req_start:
         res = urlparse(url)
-        netloc = res.netloc.replace(".", "_")
+        netloc = res.netloc
         code = response.code
 
         has_width_and_height = bool(context.request.width) and bool(context.request.height)
 
         if not has_width_and_height and regex_match is None:
             return callback()
 
@@ -25,23 +25,23 @@
         if regex_match:
             parsed_match = re.search(regex_match, url)
             parsed_match = parsed_match.group(1) if parsed_match and parsed_match.group(1) else ''
 
         finish = datetime.datetime.now()
 
         # make sure to have placeholders in case the values are empty. This way we can parse it easier later
-        extra = f"{context.request.width}x{context.request.height}.{parsed_match}" \
-            if has_width_and_height else f".{parsed_match}"
+        extra = f"{context.request.width}x{context.request.height}%{parsed_match}" \
+            if has_width_and_height else f"%{parsed_match}"
 
         context.metrics.timing(
-            f"original_image_with_size.fetch.{code}.{netloc}.{extra}",
+            f"original_image_with_size.fetch.{code}%{netloc}%{extra}",
             (finish - req_start).total_seconds() * 1000,
         )
         context.metrics.incr(
-            f"original_image_with_size.fetch.{code}.{netloc}.{extra}",
+            f"original_image_with_size.fetch.{code}%{netloc}%{extra}",
         )
 
     return callback()
 
 
 async def load(context, url):
     return await http_loader.load(context, url, return_contents_fn=return_contents)
```

### Comparing `thumbor_hsl-0.0.2/thumbor_hsl.egg-info/PKG-INFO` & `thumbor_hsl-0.0.3/thumbor_hsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbor-hsl
-Version: 0.0.2
+Version: 0.0.3
 Summary: A modified `http` loader for thumbor which provides additional statistics (like width, height and url parsing)
 Home-page: https://github.com/BowlingX/thumbor-http-stats-loader
 Author: David Heidrich
 Author-email: me@bowlingx.com
 License: MIT
 License-File: LICENSE
```

