# Comparing `tmp/ipylib-0.2.3.tar.gz` & `tmp/ipylib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipylib-0.2.3.tar", last modified: Wed May 24 02:55:10 2023, max compression
+gzip compressed data, was "ipylib-0.2.4.tar", last modified: Sat Jun  3 01:57:00 2023, max compression
```

## Comparing `ipylib-0.2.3.tar` & `ipylib-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:55:10.374617 ipylib-0.2.3/
--rw-rw-rw-   0        0        0     1093 2023-03-26 08:40:21.000000 ipylib-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      827 2023-05-24 02:55:10.373617 ipylib-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-26 08:45:38.000000 ipylib-0.2.3/README.md
--rw-rw-rw-   0        0        0      110 2023-03-26 08:40:21.000000 ipylib-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 02:55:10.374617 ipylib-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-05-24 02:51:34.000000 ipylib-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:55:10.350612 ipylib-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 02:55:10.371617 ipylib-0.2.3/src/ipylib.egg-info/
--rw-rw-rw-   0        0        0      827 2023-05-24 02:55:10.000000 ipylib-0.2.3/src/ipylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-24 02:55:10.000000 ipylib-0.2.3/src/ipylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:55:10.000000 ipylib-0.2.3/src/ipylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:55:10.000000 ipylib-0.2.3/src/ipylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.988182 ipylib-0.2.4/
+-rw-rw-rw-   0        0        0     1093 2023-03-26 08:40:21.000000 ipylib-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      827 2023-06-03 01:57:00.987182 ipylib-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-03-26 08:45:38.000000 ipylib-0.2.4/README.md
+-rw-rw-rw-   0        0        0      110 2023-03-26 08:40:21.000000 ipylib-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 01:57:00.988182 ipylib-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-06-03 01:50:13.000000 ipylib-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.958175 ipylib-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.985181 ipylib-0.2.4/src/ipylib.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/top_level.txt
```

### Comparing `ipylib-0.2.3/LICENSE` & `ipylib-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipylib-0.2.3/PKG-INFO` & `ipylib-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylib
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지
 Home-page: https://github.com/innovata/iPyLibrary
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ipylib-0.2.3/setup.py` & `ipylib-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipylib",
-    version="0.2.3",
+    version="0.2.4",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/iPyLibrary",
     classifiers=[
```

### Comparing `ipylib-0.2.3/src/ipylib.egg-info/PKG-INFO` & `ipylib-0.2.4/src/ipylib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylib
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지
 Home-page: https://github.com/innovata/iPyLibrary
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

