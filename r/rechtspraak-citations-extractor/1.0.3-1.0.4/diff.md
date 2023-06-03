# Comparing `tmp/rechtspraak_citations_extractor-1.0.3.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.3.tar", last modified: Sat Jun  3 12:29:55 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.4.tar", last modified: Sat Jun  3 12:36:40 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.3.tar` & `rechtspraak_citations_extractor-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:55.262176 rechtspraak_citations_extractor-1.0.3/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:29:55.261176 rechtspraak_citations_extractor-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:55.250963 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13292 2023-06-03 12:29:35.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:29:55.259176 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-03 12:29:55.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-03 12:29:55.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:29:55.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-03 12:29:55.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-03 12:29:55.000000 rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:29:55.262176 rechtspraak_citations_extractor-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-06-03 12:28:07.000000 rechtspraak_citations_extractor-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.884020 rechtspraak_citations_extractor-1.0.4/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:36:40.883020 rechtspraak_citations_extractor-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.872660 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13293 2023-06-03 12:36:33.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:36:40.880821 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-03 12:36:40.000000 rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:36:40.884020 rechtspraak_citations_extractor-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-03 12:36:33.000000 rechtspraak_citations_extractor-1.0.4/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.3/PKG-INFO` & `rechtspraak_citations_extractor-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.3
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.4
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.3/README.md` & `rechtspraak_citations_extractor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
                 for the_citations in sub.iterchildren(incoming):
                     for sub_ref in the_citations.iterchildren():
                         if is_case_law(sub_ref):
                             added_sth_new = add_citations_no_duplicates(case_law_citations_incoming, sub_ref)
 
         if not added_sth_new or start_page > 15:
-            print(start_page)
+            #print(start_page)
             end_of_pages = True
 
     # Remove duplicates empties
 
     for item in case_law_citations_incoming:
         if item[target_ecli] == "":
             case_law_citations_incoming.remove(item)
@@ -300,17 +300,17 @@
 
 
 def extract_results_legislations(list, ecli, fields, username, password):
     list_of_all_results = []
 
     for leg_citation in list:
         legislation_result = {key: None for key in fields}
-        legislation_result[fields[1]] = (leg_citation)  # Target article
-        legislation_result[fields[2]] = (get_legislation_webpage(leg_citation))  # Target article webpage
-        legislation_result[fields[3]] = (
+        legislation_result[fields[0]] = (leg_citation)  # Target article
+        legislation_result[fields[1]] = (get_legislation_webpage(leg_citation))  # Target article webpage
+        legislation_result[fields[2]] = (
             get_legislation_name(leg_citation, username, password))  # pref label == article name
         list_of_all_results.append(legislation_result)
     return list_of_all_results
 
 
 def get_citations(dataframe=None, username="", password="", threads=1):
     if dataframe is None or not username or not password:
```

### Comparing `rechtspraak_citations_extractor-1.0.3/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.4/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.3
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.4
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.3/setup.py` & `rechtspraak_citations_extractor-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.3',
+    version='1.0.4',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
     install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
```

