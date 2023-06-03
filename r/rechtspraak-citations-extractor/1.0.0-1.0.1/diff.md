# Comparing `tmp/rechtspraak_citations_extractor-1.0.0.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.0.tar", last modified: Fri Jun  2 18:08:01 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.1.tar", last modified: Sat Jun  3 12:17:41 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.0.tar` & `rechtspraak_citations_extractor-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:08:01.198160 rechtspraak_citations_extractor-1.0.0/
--rw-rw-rw-   0        0        0     4818 2023-06-02 18:08:01.196160 rechtspraak_citations_extractor-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 18:08:01.184647 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       45 2023-05-21 11:04:08.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13896 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:08:01.194160 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-02 18:08:01.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-02 18:08:01.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:08:01.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-02 18:08:01.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-02 18:08:01.000000 rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 18:08:01.198160 rechtspraak_citations_extractor-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-05-21 11:05:01.000000 rechtspraak_citations_extractor-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.718237 rechtspraak_citations_extractor-1.0.1/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:17:41.717236 rechtspraak_citations_extractor-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.707236 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       45 2023-05-21 11:04:08.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13092 2023-06-03 12:12:21.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:17:41.715237 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-03 12:17:41.000000 rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:17:41.718237 rechtspraak_citations_extractor-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-03 12:17:36.000000 rechtspraak_citations_extractor-1.0.1/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.0/PKG-INFO` & `rechtspraak_citations_extractor-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.0
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.1
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.0/README.md` & `rechtspraak_citations_extractor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import requests
 from lxml import etree
 import urllib.request
 import rdflib
-import sys
-from os.path import dirname, abspath
 import threading
 import json
-
-sys.path.append(dirname(dirname(dirname(abspath(__file__)))))
 import pandas as pd
 from dotenv import load_dotenv
 from requests.auth import HTTPBasicAuth
 
 load_dotenv()
 
 LIDO_ENDPOINT = "http://linkeddata.overheid.nl/service/get-links"
 
 target_ecli = 'target_ecli'
 label = 'label'
 type = 'type'
 ecli = 'ecli'
-case_citations_fieldnames = [ecli, target_ecli, label, type, 'predecessor_successor_cases', 'keep1', 'keep2']
-legislation_citations_fieldnames = [ecli, 'legal_provision_url_lido', 'legal_provision_url', 'legal_provision']
+case_citations_fieldnames = [target_ecli, label, type]
+legislation_citations_fieldnames = ['legal_provision_url_lido', 'legal_provision_url', 'legal_provision']
 
 
 def remove_spaces_from_ecli(ecli):
     return ecli.replace(" ", "")
 
 
 def write_incremental_rows(filename, data):
@@ -201,18 +197,15 @@
         if stored[target_ecli] == new_ecli:
             added_sth_new = False
             duplicate = True
             break
     if not duplicate:
         already_existing_list.append({target_ecli: new_ecli,
                                       label: element.attrib['label'],
-                                      type: element.attrib['type'].split('/id/')[1],
-                                      'keep1': element.attrib['type'].split('/id/')[
-                                                   1] == 'lx-referentie',
-                                      'keep2': get_ecli(element) not in str()})
+                                      type: element.attrib['type'].split('/id/')[1]})
     return added_sth_new
 
 
 def add_legislations_no_duplicates(list, element):
     duplicate = False
     new_legislation = get_legislation_identifier(element)
     added_sth_new = True
@@ -295,31 +288,26 @@
 
 
 def extract_results_citations(list, ecli, fields):
     list_of_all_results = []
 
     for case_citation in list:
         case_law_result = {key: None for key in fields}
-        case_law_result[fields[0]] = (remove_spaces_from_ecli(ecli))  # Source ECLI
-        case_law_result[fields[1]] = (remove_spaces_from_ecli(case_citation[target_ecli]))  # Target ECLI
-        case_law_result[fields[2]] = (case_citation['label'])  # Target ECLI
-        case_law_result[fields[3]] = (case_citation['type'])  # Target ECLI
-        case_law_result[fields[4]] = ("")  # Target ECLI
-        case_law_result[fields[5]] = (case_citation['keep1'])  # Target ECLI
-        case_law_result[fields[6]] = (case_citation['keep2'])  # Target ECLI
+        case_law_result[fields[0]] = (remove_spaces_from_ecli(case_citation[target_ecli]))  # Target ECLI
+        case_law_result[fields[1]] = (case_citation['label'])  # Target ECLI
+        case_law_result[fields[2]] = (case_citation['type'])  # Target ECLI
         list_of_all_results.append(case_law_result)
     return list_of_all_results
 
 
 def extract_results_legislations(list, ecli, fields, username, password):
     list_of_all_results = []
 
     for leg_citation in list:
         legislation_result = {key: None for key in fields}
-        legislation_result[fields[0]] = (remove_spaces_from_ecli(ecli))  # Source ECLI
         legislation_result[fields[1]] = (leg_citation)  # Target article
         legislation_result[fields[2]] = (get_legislation_webpage(leg_citation))  # Target article webpage
         legislation_result[fields[3]] = (
             get_legislation_name(leg_citation, username, password))  # pref label == article name
         list_of_all_results.append(legislation_result)
     return list_of_all_results
```

### Comparing `rechtspraak_citations_extractor-1.0.0/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.1/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.0
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.1
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.0/setup.py` & `rechtspraak_citations_extractor-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.0',
+    version='1.0.1',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
-    install_requires=['rdflib', 'requests==2.26.0', 'python_dotenv==0.15.0', 'pandas','urllib','lxml'],
+    install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
     long_description_content_type='text/markdown',
     project_urls={
         "Bug Tracker": "https://github.com/maastrichtlawtech/extraction_libraries",
         "Build Source": "https://github.com/maastrichtlawtech/extraction_libraries",
```

