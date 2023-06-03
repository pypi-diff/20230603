# Comparing `tmp/ipylib-0.2.4.tar.gz` & `tmp/ipylib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipylib-0.2.4.tar", last modified: Sat Jun  3 01:57:00 2023, max compression
+gzip compressed data, was "ipylib-0.2.5.tar", last modified: Sat Jun  3 02:06:10 2023, max compression
```

## Comparing `ipylib-0.2.4.tar` & `ipylib-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.988182 ipylib-0.2.4/
--rw-rw-rw-   0        0        0     1093 2023-03-26 08:40:21.000000 ipylib-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      827 2023-06-03 01:57:00.987182 ipylib-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-26 08:45:38.000000 ipylib-0.2.4/README.md
--rw-rw-rw-   0        0        0      110 2023-03-26 08:40:21.000000 ipylib-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 01:57:00.988182 ipylib-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-06-03 01:50:13.000000 ipylib-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.958175 ipylib-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:57:00.985181 ipylib-0.2.4/src/ipylib.egg-info/
--rw-rw-rw-   0        0        0      827 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:57:00.000000 ipylib-0.2.4/src/ipylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 02:06:10.871122 ipylib-0.2.5/
+-rw-rw-rw-   0        0        0     1093 2023-03-26 08:40:21.000000 ipylib-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      827 2023-06-03 02:06:10.870121 ipylib-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-03-26 08:45:38.000000 ipylib-0.2.5/README.md
+-rw-rw-rw-   0        0        0      110 2023-03-26 08:40:21.000000 ipylib-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 02:06:10.872121 ipylib-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-06-03 02:05:35.000000 ipylib-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:06:10.803106 ipylib-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 02:06:10.841115 ipylib-0.2.5/src/ipylib/
+-rw-rw-rw-   0        0        0      195 2023-05-24 02:45:06.000000 ipylib-0.2.5/src/ipylib/__init__.py
+-rw-rw-rw-   0        0        0     2489 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/datacls.py
+-rw-rw-rw-   0        0        0     2427 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/idatetime.py
+-rw-rw-rw-   0        0        0    13815 2023-05-07 07:51:57.000000 ipylib-0.2.5/src/ipylib/idebug.py
+-rw-rw-rw-   0        0        0     8151 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/ifile.py
+-rw-rw-rw-   0        0        0      635 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/ijson.py
+-rw-rw-rw-   0        0        0      921 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/ilist.py
+-rw-rw-rw-   0        0        0     1856 2023-04-06 10:49:55.000000 ipylib-0.2.5/src/ipylib/imath.py
+-rw-rw-rw-   0        0        0     7503 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/inumber.py
+-rw-rw-rw-   0        0        0     1843 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/iparser.py
+-rw-rw-rw-   0        0        0      374 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/ipath.py
+-rw-rw-rw-   0        0        0     3012 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/ipylib/syspath.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:06:10.859119 ipylib-0.2.5/src/ipylib.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-06-03 02:06:10.000000 ipylib-0.2.5/src/ipylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-06-03 02:06:10.000000 ipylib-0.2.5/src/ipylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 02:06:10.000000 ipylib-0.2.5/src/ipylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 02:06:10.000000 ipylib-0.2.5/src/ipylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 02:06:10.868121 ipylib-0.2.5/src/test/
+-rw-rw-rw-   0        0        0        0 2023-03-26 08:41:01.000000 ipylib-0.2.5/src/test/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-03-26 08:44:19.000000 ipylib-0.2.5/src/test/_testenv.py
+-rw-rw-rw-   0        0        0    17743 2023-04-06 10:50:06.000000 ipylib-0.2.5/src/test/utest.py
+-rw-rw-rw-   0        0        0      371 2023-03-26 08:40:21.000000 ipylib-0.2.5/src/test/utestall.py
```

### Comparing `ipylib-0.2.4/LICENSE` & `ipylib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipylib-0.2.4/PKG-INFO` & `ipylib-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지
 Home-page: https://github.com/innovata/iPyLibrary
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ipylib-0.2.4/setup.py` & `ipylib-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipylib",
-    version="0.2.4",
+    version="0.2.5",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/iPyLibrary",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"":"src"},
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages('src'),
     python_requires=">=3.8",
 )
```

### Comparing `ipylib-0.2.4/src/ipylib.egg-info/PKG-INFO` & `ipylib-0.2.5/src/ipylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipylib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pure Python3 기능을 재사용하기 위해 한단계 추상화된 라이브러리 패키지
 Home-page: https://github.com/innovata/iPyLibrary
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

