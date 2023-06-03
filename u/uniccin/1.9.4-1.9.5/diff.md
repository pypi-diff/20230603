# Comparing `tmp/uniccin-1.9.4.tar.gz` & `tmp/uniccin-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniccin-1.9.4.tar", last modified: Tue May 30 23:32:24 2023, max compression
+gzip compressed data, was "uniccin-1.9.5.tar", last modified: Sat Jun  3 14:05:04 2023, max compression
```

## Comparing `uniccin-1.9.4.tar` & `uniccin-1.9.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:32:24.000000 uniccin-1.9.4/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 uniccin-1.9.4/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5628 2023-05-30 23:32:24.000000 uniccin-1.9.4/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4831 2023-05-23 17:22:46.000000 uniccin-1.9.4/README.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3850 2023-05-30 23:15:18.000000 uniccin-1.9.4/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-30 23:32:24.000000 uniccin-1.9.4/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       35 2023-05-22 16:32:11.000000 uniccin-1.9.4/src/uniccin/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1628 2023-05-30 23:18:31.000000 uniccin-1.9.4/src/uniccin/block.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin/data/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       58 2023-05-22 16:32:46.000000 uniccin-1.9.4/src/uniccin/data/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    18613 2023-05-21 14:25:06.000000 uniccin-1.9.4/src/uniccin/data/block.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 uniccin-1.9.4/src/uniccin/data/ccc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    28591 2023-05-30 23:31:35.000000 uniccin-1.9.4/src/uniccin/data/html_entities.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1520 2023-05-30 23:19:30.000000 uniccin-1.9.4/src/uniccin/format.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)      677 2023-05-30 23:19:38.000000 uniccin-1.9.4/src/uniccin/html.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2623 2023-05-30 23:20:14.000000 uniccin-1.9.4/src/uniccin/search.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4997 2023-05-30 23:20:45.000000 uniccin-1.9.4/src/uniccin/uc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     7805 2023-05-30 23:23:52.000000 uniccin-1.9.4/src/uniccin/uni.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5628 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)      469 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       41 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        8 2023-05-30 23:32:23.000000 uniccin-1.9.4/src/uniccin.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-03 14:05:04.000000 uniccin-1.9.5/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 uniccin-1.9.5/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5628 2023-06-03 14:05:04.000000 uniccin-1.9.5/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4831 2023-05-23 17:22:46.000000 uniccin-1.9.5/README.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3850 2023-06-03 14:04:15.000000 uniccin-1.9.5/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-06-03 14:05:04.000000 uniccin-1.9.5/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       35 2023-05-22 16:32:11.000000 uniccin-1.9.5/src/uniccin/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1628 2023-05-30 23:18:31.000000 uniccin-1.9.5/src/uniccin/block.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin/data/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       58 2023-05-22 16:32:46.000000 uniccin-1.9.5/src/uniccin/data/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    18613 2023-05-21 14:25:06.000000 uniccin-1.9.5/src/uniccin/data/block.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 uniccin-1.9.5/src/uniccin/data/ccc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    28591 2023-05-30 23:31:35.000000 uniccin-1.9.5/src/uniccin/data/html_entities.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1520 2023-05-30 23:19:30.000000 uniccin-1.9.5/src/uniccin/format.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      677 2023-05-30 23:19:38.000000 uniccin-1.9.5/src/uniccin/html.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2623 2023-05-30 23:20:14.000000 uniccin-1.9.5/src/uniccin/search.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5459 2023-06-03 14:00:13.000000 uniccin-1.9.5/src/uniccin/uc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     7859 2023-06-03 13:55:34.000000 uniccin-1.9.5/src/uniccin/uni.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5628 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      469 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       41 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        8 2023-06-03 14:05:04.000000 uniccin-1.9.5/src/uniccin.egg-info/top_level.txt
```

### Comparing `uniccin-1.9.4/LICENSE` & `uniccin-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/PKG-INFO` & `uniccin-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniccin
-Version: 1.9.4
+Version: 1.9.5
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `uniccin-1.9.4/README.md` & `uniccin-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/pyproject.toml` & `uniccin-1.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniccin"
-version = "1.9.4"
+version = "1.9.5"
 description = "Command-line tool to display Unicode character information"
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `uniccin-1.9.4/src/uniccin/block.py` & `uniccin-1.9.5/src/uniccin/block.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/data/block.py` & `uniccin-1.9.5/src/uniccin/data/block.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/data/ccc.py` & `uniccin-1.9.5/src/uniccin/data/ccc.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/data/html_entities.py` & `uniccin-1.9.5/src/uniccin/data/html_entities.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/format.py` & `uniccin-1.9.5/src/uniccin/format.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/html.py` & `uniccin-1.9.5/src/uniccin/html.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/search.py` & `uniccin-1.9.5/src/uniccin/search.py`

 * *Files identical despite different names*

### Comparing `uniccin-1.9.4/src/uniccin/uc.py` & `uniccin-1.9.5/src/uniccin/uc.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,29 @@
         if n & m == n:
             break
         m = m >> 1
     r.append((0xFE ^ (m << 1)) | n)
     r.reverse()
     return r
 
+def sanitize(s: str, replacement: str | None = '\uFFFD') -> str:
+    """Remove or replace disallowed code points (surrogates)."""
+    try:
+        _ = bytes(s, encoding='utf-32')
+    except UnicodeEncodeError:
+        r = []
+        for c in s:
+            if ord(c) in range(0xD800, 0xE000):
+                if replacement is not None:
+                    r.append(replacement)
+            else:
+                r.append(c)
+        s = ''.join(r)
+    return s
+
 # Normalization
 
 def normalize(c: str, form: str) -> str:
     # NB: character first.
     return unicodedata.normalize(form.upper(), c)
 
 # Uniform property access functions. These all accept a ‘default’ argument,
```

### Comparing `uniccin-1.9.4/src/uniccin/uni.py` & `uniccin-1.9.5/src/uniccin/uni.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,17 @@
         args.format = [CANNED_FORMATS['short'][1]]
     sep = False
     for c in chrs:
         if sep:
             print(end=args.eol)
         sep = True
         for f in args.format:
-            print(f.format_map(uniccin.format.UniFormat(c)), end='')
+            print(
+                uniccin.uc.sanitize(f.format_map(uniccin.format.UniFormat(c))),
+                end='')
 
     if args.eol and args.eol != chr(0):
         print(end=args.eol)
 
     return error_count
 
 if __name__ == '__main__':  # pragma: no cover
```

### Comparing `uniccin-1.9.4/src/uniccin.egg-info/PKG-INFO` & `uniccin-1.9.5/src/uniccin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniccin
-Version: 1.9.4
+Version: 1.9.5
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

