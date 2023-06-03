# Comparing `tmp/vfxtool-0.0.3.tar.gz` & `tmp/vfxtool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfxtool-0.0.3.tar", last modified: Thu Jun  1 07:07:50 2023, max compression
+gzip compressed data, was "vfxtool-0.0.4.tar", last modified: Sat Jun  3 06:28:48 2023, max compression
```

## Comparing `vfxtool-0.0.3.tar` & `vfxtool-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:07:50.988804 vfxtool-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-28 11:30:02.000000 vfxtool-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      636 2023-06-01 07:07:50.986803 vfxtool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-05-28 09:42:04.000000 vfxtool-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 07:07:50.988804 vfxtool-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-06-01 07:07:15.000000 vfxtool-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:07:50.940809 vfxtool-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 07:07:50.983804 vfxtool-0.0.3/src/vfxtool.egg-info/
--rw-rw-rw-   0        0        0      636 2023-06-01 07:07:50.000000 vfxtool-0.0.3/src/vfxtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-01 07:07:50.000000 vfxtool-0.0.3/src/vfxtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:07:50.000000 vfxtool-0.0.3/src/vfxtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:07:50.000000 vfxtool-0.0.3/src/vfxtool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 06:28:48.317483 vfxtool-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-28 11:30:02.000000 vfxtool-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      636 2023-06-03 06:28:48.315480 vfxtool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-05-28 09:42:04.000000 vfxtool-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 06:28:48.318482 vfxtool-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-06-03 06:23:52.000000 vfxtool-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:28:48.115496 vfxtool-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 06:28:48.158491 vfxtool-0.0.4/src/vfxtool/
+-rw-rw-rw-   0        0        0        0 2023-05-28 08:52:41.000000 vfxtool-0.0.4/src/vfxtool/__init__.py
+-rw-rw-rw-   0        0        0     3742 2023-05-31 13:00:28.000000 vfxtool-0.0.4/src/vfxtool/dataIO.py
+-rw-rw-rw-   0        0        0      332 2023-05-31 05:59:28.000000 vfxtool-0.0.4/src/vfxtool/lineup.py
+-rw-rw-rw-   0        0        0       37 2023-05-28 10:12:11.000000 vfxtool-0.0.4/src/vfxtool/main.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:11:12.000000 vfxtool-0.0.4/src/vfxtool/shotsInfo.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:28:48.312480 vfxtool-0.0.4/src/vfxtool.egg-info/
+-rw-rw-rw-   0        0        0      636 2023-06-03 06:28:48.000000 vfxtool-0.0.4/src/vfxtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-03 06:28:48.000000 vfxtool-0.0.4/src/vfxtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 06:28:48.000000 vfxtool-0.0.4/src/vfxtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 06:28:48.000000 vfxtool-0.0.4/src/vfxtool.egg-info/top_level.txt
```

### Comparing `vfxtool-0.0.3/LICENSE.txt` & `vfxtool-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vfxtool-0.0.3/PKG-INFO` & `vfxtool-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfxtool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A studio Pipeline for 3d animation and VFX studio
 Home-page: https://github.com/yogendra97github/vfxpipeline.git
 Author: Yogendra Singh
 Author-email: yogendrasingh.hqvfx@gmail.com
 Project-URL: Bug Tracker, https://github.com/yogendra97github/vfxpipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vfxtool-0.0.3/setup.py` & `vfxtool-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vfxtool",
-    version="0.0.3",
+    version="0.0.4",
     author="Yogendra Singh",
     author_email="yogendrasingh.hqvfx@gmail.com",
     description="A studio Pipeline for 3d animation and VFX studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yogendra97github/vfxpipeline.git",
     project_urls={
```

### Comparing `vfxtool-0.0.3/src/vfxtool.egg-info/PKG-INFO` & `vfxtool-0.0.4/src/vfxtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfxtool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A studio Pipeline for 3d animation and VFX studio
 Home-page: https://github.com/yogendra97github/vfxpipeline.git
 Author: Yogendra Singh
 Author-email: yogendrasingh.hqvfx@gmail.com
 Project-URL: Bug Tracker, https://github.com/yogendra97github/vfxpipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

