# Comparing `tmp/rechtspraak_citations_extractor-1.0.1.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.1.tar", last modified: Sat Jun  3 12:17:41 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.2.tar", last modified: Sat Jun  3 12:22:15 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.1.tar` & `rechtspraak_citations_extractor-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.718237 rechtspraak_citations_extractor-1.0.1/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:17:41.717236 rechtspraak_citations_extractor-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.707236 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       45 2023-05-21 11:04:08.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13092 2023-06-03 12:12:21.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.715237 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:17:41.718237 rechtspraak_citations_extractor-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-06-03 12:17:36.000000 rechtspraak_citations_extractor-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:22:15.849936 rechtspraak_citations_extractor-1.0.2/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:22:15.848937 rechtspraak_citations_extractor-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:22:15.837936 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13092 2023-06-03 12:12:21.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:22:15.846936 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:22:15.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-03 12:22:15.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:22:15.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-06-03 12:22:15.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-03 12:22:15.000000 rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:22:15.849936 rechtspraak_citations_extractor-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.2/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.1/PKG-INFO` & `rechtspraak_citations_extractor-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.1
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.2
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.1/README.md` & `rechtspraak_citations_extractor-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.2/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.1
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.2
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.1/setup.py` & `rechtspraak_citations_extractor-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.1',
+    version='1.0.2',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
     install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
```

