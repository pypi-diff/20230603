# Comparing `tmp/lazylines-0.0.1.tar.gz` & `tmp/lazylines-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazylines-0.0.1.tar", last modified: Wed Feb 22 16:37:26 2023, max compression
+gzip compressed data, was "lazylines-0.0.2.tar", last modified: Sat Jun  3 12:31:54 2023, max compression
```

## Comparing `lazylines-0.0.1.tar` & `lazylines-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-22 16:37:26.402721 lazylines-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      862 2023-02-22 16:37:26.402721 lazylines-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      686 2023-02-22 16:32:10.000000 lazylines-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-22 16:37:26.402721 lazylines-0.0.1/lazylines/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8083 2023-02-22 16:35:47.000000 lazylines-0.0.1/lazylines/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-02-22 16:37:26.402721 lazylines-0.0.1/lazylines.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      862 2023-02-22 16:37:26.000000 lazylines-0.0.1/lazylines.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      204 2023-02-22 16:37:26.000000 lazylines-0.0.1/lazylines.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-22 16:37:26.000000 lazylines-0.0.1/lazylines.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      199 2023-02-22 16:37:26.000000 lazylines-0.0.1/lazylines.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2023-02-22 16:37:26.000000 lazylines-0.0.1/lazylines.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-02-22 16:37:26.402721 lazylines-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      792 2023-02-22 16:32:11.000000 lazylines-0.0.1/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.993568 lazylines-0.0.2/
+-rw-r--r--   0 vincent    (501) staff       (20)     1076 2023-06-03 12:12:42.000000 lazylines-0.0.2/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)     1135 2023-06-03 12:31:54.993307 lazylines-0.0.2/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      620 2023-06-03 12:12:42.000000 lazylines-0.0.2/README.md
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.991451 lazylines-0.0.2/lazylines/
+-rw-r--r--   0 vincent    (501) staff       (20)     8306 2023-06-03 12:27:05.000000 lazylines-0.0.2/lazylines/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      323 2023-06-03 12:12:42.000000 lazylines-0.0.2/lazylines/functions.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.993128 lazylines-0.0.2/lazylines.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)     1135 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      235 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      173 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       10 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-03 12:31:54.993606 lazylines-0.0.2/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)     1178 2023-06-03 12:31:26.000000 lazylines-0.0.2/setup.py
```

### Comparing `lazylines-0.0.1/lazylines/__init__.py` & `lazylines-0.0.2/lazylines/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,18 +89,21 @@
             for item in self.g:
                 for func in args:
                     if func(item):
                         yield item
 
         return LazyLines(g=new_gen())
 
-    def unnest(self, key) -> LazyLines:
+    def unnest(self, key: str) -> LazyLines:
         """
         Explodes a key, effectively un-nesting it.
 
+        Arguments:
+            key: the key to use while nesting
+
         **Usage**:
 
         ```python
         from lazylines import LazyLines
 
         data = [{'annotator': 'a',
                  'subset': [{'accept': True, 'text': 'foo'},
@@ -243,33 +246,39 @@
         srsly.write_jsonl(path, self.g, append=append, append_new_line=append_new_line)
 
     def select(self, *args) -> LazyLines:
         """Only select specific keys from each dictionary."""
 
         def new_gen():
             for ex in self.g:
-                yield {k: v for k, v in ex.items() if v in args}
+                yield {k: v for k, v in ex.items() if k in args}
 
         return LazyLines(g=new_gen())
 
     def drop(self, *args) -> LazyLines:
         """Drop specific keys from each dictionary."""
 
         def new_gen():
             for ex in self.g:
                 yield {k: v for k, v in ex.items() if k not in args}
 
         return LazyLines(g=new_gen())
 
     def pipe(self, func, *args, **kwargs) -> LazyLines:
         """Call a function over the entire generator."""
-        return LazyLines(g=func(self.g, *args, **kwargs))
+        return LazyLines(g=func(self, *args, **kwargs))
 
     def foreach(self, func, *args, **kwargs) -> LazyLines:
         """Just call a function on each dictionary, but pass the original forward."""
 
         def new_gen():
             for ex in self.g:
                 func(ex, *args, **kwargs)
                 yield ex
 
         return LazyLines(g=new_gen())
+    
+    def agg(self, **kwargs):
+        data = [ex for ex in self.g]
+        return {
+            k: func(data) for k, func in kwargs.items()
+        }
```

