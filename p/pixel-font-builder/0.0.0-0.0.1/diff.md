# Comparing `tmp/pixel-font-builder-0.0.0.tar.gz` & `tmp/pixel-font-builder-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.0.tar", last modified: Mon May  8 16:43:56 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.1.tar", last modified: Fri Jun  2 14:50:06 2023, max compression
```

## Comparing `pixel-font-builder-0.0.0.tar` & `pixel-font-builder-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 16:43:44.000000 pixel-font-builder-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 16:43:44.000000 pixel-font-builder-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-08 16:43:44.000000 pixel-font-builder-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:56.034669 pixel-font-builder-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:44.000000 pixel-font-builder-0.0.0/src/pixel_font_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 16:43:56.000000 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 16:43:56.000000 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:43:56.000000 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 16:43:56.000000 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 16:43:56.000000 pixel-font-builder-0.0.0/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:43:56.038669 pixel-font-builder-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:43:44.000000 pixel-font-builder-0.0.0/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:06.062522 pixel-font-builder-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-02 14:50:06.000000 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-02 14:50:06.000000 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:06.000000 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 14:50:06.000000 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 14:50:06.000000 pixel-font-builder-0.0.1/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:50:06.066522 pixel-font-builder-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 14:49:56.000000 pixel-font-builder-0.0.1/tests/test_demo.py
```

### Comparing `pixel-font-builder-0.0.0/LICENSE` & `pixel-font-builder-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.0/pyproject.toml` & `pixel-font-builder-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.0"
+version = "0.0.1"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
 maintainers = [
     { name = "TakWolf" },
 ]
 keywords = ["font", "pixel"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools==4.39.3",
-    "Brotli==1.0.9",
-    "bdffont==0.0.7",
+    "fonttools>=4.39.4",
+    "Brotli>=1.0.9",
+    "bdffont>=0.0.11",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/pixel-font-builder"
 source = "https://github.com/TakWolf/pixel-font-builder"
 issues = "https://github.com/TakWolf/pixel-font-builder/issues"
```

