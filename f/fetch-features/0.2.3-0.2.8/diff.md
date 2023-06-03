# Comparing `tmp/fetch_features-0.2.3.tar.gz` & `tmp/fetch_features-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch_features-0.2.3.tar", last modified: Sun May 28 23:59:38 2023, max compression
+gzip compressed data, was "fetch_features-0.2.8.tar", last modified: Sat Jun  3 21:34:55 2023, max compression
```

## Comparing `fetch_features-0.2.3.tar` & `fetch_features-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.408218 fetch_features-0.2.3/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.3/LICENSE.md
--rw-r--r--   0 msp        (501) staff       (20)     3259 2023-05-28 23:59:38.407515 fetch_features-0.2.3/PKG-INFO
--rwxr-xr-x   0 msp        (501) staff       (20)     2533 2023-05-28 22:29:31.000000 fetch_features-0.2.3/README.md
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.382464 fetch_features-0.2.3/images/
--rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.3/images/fetch_features_gui.png
--rw-r--r--   0 msp        (501) staff       (20)     1137 2023-05-28 23:34:25.000000 fetch_features-0.2.3/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-05-28 23:59:38.408374 fetch_features-0.2.3/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.377710 fetch_features-0.2.3/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.390154 fetch_features-0.2.3/src/fetch_features.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     3259 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      466 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       57 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)      146 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        8 2023-05-28 23:59:38.000000 fetch_features-0.2.3/src/fetch_features.egg-info/top_level.txt
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-05-28 23:59:38.405568 fetch_features-0.2.3/src/fetcher/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.3/src/fetcher/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)     1239 2023-05-13 22:48:30.000000 fetch_features-0.2.3/src/fetcher/__main__.py
--rwx------   0 msp        (501) staff       (20)    16594 2023-05-28 22:51:12.000000 fetch_features-0.2.3/src/fetcher/access_genbank.py
--rwx------   0 msp        (501) staff       (20)    32983 2023-05-28 18:16:08.000000 fetch_features-0.2.3/src/fetcher/database.py
--rw-r--r--   0 msp        (501) staff       (20)    17348 2023-05-13 22:50:35.000000 fetch_features-0.2.3/src/fetcher/gui.py
--rw-r--r--   0 msp        (501) staff       (20)    10405 2023-05-26 21:57:12.000000 fetch_features-0.2.3/src/fetcher/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.372066 fetch_features-0.2.8/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.8/LICENSE.md
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-06-03 21:34:55.371508 fetch_features-0.2.8/PKG-INFO
+-rwxr-xr-x   0 msp        (501) staff       (20)     2533 2023-05-28 22:29:31.000000 fetch_features-0.2.8/README.md
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.357366 fetch_features-0.2.8/images/
+-rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.8/images/fetch_features_gui.png
+-rw-r--r--   0 msp        (501) staff       (20)     1159 2023-06-03 01:07:37.000000 fetch_features-0.2.8/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-06-03 21:34:55.372233 fetch_features-0.2.8/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.353469 fetch_features-0.2.8/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.363245 fetch_features-0.2.8/src/fetch_features.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      463 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       57 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)      162 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        8 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.369835 fetch_features-0.2.8/src/fetcher/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.8/src/fetcher/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)     1239 2023-06-03 21:19:35.000000 fetch_features-0.2.8/src/fetcher/__main__.py
+-rwx------   0 msp        (501) staff       (20)    18653 2023-06-03 21:21:01.000000 fetch_features-0.2.8/src/fetcher/access_genbank.py
+-rw-r--r--   0 msp        (501) staff       (20)    17556 2023-06-03 21:18:22.000000 fetch_features-0.2.8/src/fetcher/gui.py
+-rw-r--r--   0 msp        (501) staff       (20)    10902 2023-06-02 17:44:42.000000 fetch_features-0.2.8/src/fetcher/user_input.py
+-rwx------   0 msp        (501) staff       (20)    27324 2023-06-01 03:19:25.000000 fetch_features-0.2.8/src/fetcher/utils.py
```

### Comparing `fetch_features-0.2.3/LICENSE.md` & `fetch_features-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.3/PKG-INFO` & `fetch_features-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch_features
-Version: 0.2.3
+Version: 0.2.8
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fetch_features-0.2.3/README.md` & `fetch_features-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.3/images/fetch_features_gui.png` & `fetch_features-0.2.8/images/fetch_features_gui.png`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.3/pyproject.toml` & `fetch_features-0.2.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fetch_features"
-version = "0.2.3"
+version = "0.2.8"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Fetch features from a list of accession or BioSample numbers."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
@@ -29,14 +29,15 @@
     "darkdetect==0.8.0",
     "numpy==1.24.3",
     "pandas==2.0.1",
     "python-dateutil==2.8.2",
     "pytz==2023.3",
     "six==1.16.0",
     "tzdata==2023.3",
+    "openpyxl==3.1.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ivanmugu/fetch_features"
 
 [project.scripts]
 fetch_features = "fetcher.__main__:main"
```

### Comparing `fetch_features-0.2.3/src/fetch_features.egg-info/PKG-INFO` & `fetch_features-0.2.8/src/fetch_features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch-features
-Version: 0.2.3
+Version: 0.2.8
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fetch_features-0.2.3/src/fetcher/__main__.py` & `fetch_features-0.2.8/src/fetcher/__main__.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.3/src/fetcher/access_genbank.py` & `fetch_features-0.2.8/src/fetcher/access_genbank.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,198 +1,170 @@
 """Functions to fetch features of GenBank accession or BioSample numbers.
 
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 import csv
-import sys
 from pathlib import Path
 from typing import TextIO, IO
+import urllib
+import sys
 
 from Bio import Entrez
+from Bio import SeqIO
+
+from fetcher import utils
 
-from fetcher import database
+
+# TODO: test all options in MacOS, Windows, and Linux.
+# TODO: provide a set of accession and biosample numbers in the test folder.
+# Also, provide the expected results.
 
 
 def fetch_from_accession(
-        results_file: TextIO, results_fields: list, ref_results_file: TextIO,
-        ref_results_fields: list, submission_list: list
+        results_writer: TextIO, references_writer: TextIO,
+        submission_list: list
 ) -> None:
     """Fetch features from a list of accession numbers.
 
-    Use Entrez.post to ask for a list of accession numbers and Entrez.fetch
-    to retrieve the information of the posted list of accession numbers.
-    After retrieving the information, the data of every accession number is
-    parse using the parser function implemented in database.py.
-
     Parameters
     ----------
-    results_file : TextIO file object
-        Opened output file to save the fetched features of the accession
-        numbers.
-    results_fields : list
-        Headers for the `results` table. This list is the information to fetch
-        for every accession number.
-    ref_results_file : TextIO file object
-        Opened output file to save the references of the accession numbers.
-    ref_results_fields : list
-        Headers for the `references_results` table. This list is the
-        information to fetch for every accession number.
+    results_writer : TextIO file object
+        Opened file as csv.DictWriter to save the fetched features of UIDs.
+    references_writer : TextIO file object
+        Opened file as csv.DictWriter to save the references of UIDs.
     submission_list : list
-        List of strings containg accession numbers separated by commas. The
-        number of accession numbers in every string is determined by the
-        varible `batch_size` of the `make_uid_batch_list` function implemented
-        in database.py. An example of a submission_list with a batch_size of
-        three looks like the following:
-        ['CP049609.1,CP028704.1,CP043542.1',
-        'CP040107.1,CP041747.1,CP042638.1',
-        'CP015023.1,CP049163.1,CP051714.1']
+        List of batches of UIDs. An example of a submission_list with a batch
+        size of three looks like the following:
+        [['CP049609.1', 'CP028704.1', 'CP043542.1'],
+         ['CP040107.1', 'CP041747.1', 'CP042638.1'],
+         ['CP015023.1', 'CP049163.1', 'CP051714.1']]
     """
-    # Create DictWriters.
-    results_writer = csv.DictWriter(results_file, results_fields)
-    ref_results_writer = csv.DictWriter(ref_results_file, ref_results_fields)
-    # Declaring end.
+    # Iterate over list of batches of accession numbers to fetch gb sequences.
     end = 0
-
-    # Fetch the information from GenBank by batches.
-    for set_number, submission in enumerate(submission_list):
+    for set_num, submission in enumerate(submission_list):
         start = end
-        # submission_list is a list of accession numbers separated by
-        # commas. Therefore, the number of commas indicate the number of
-        # accession numbers.
-        batch_size = submission.count(',') + 1
+        batch_size = len(submission)
         end = end + batch_size
-
-        # Print download batch record.
         print(f"Going to download record {start + 1} to {end}\n")
 
-        # Post the submission_list.
-        # Because we are requesting information from a huge list of acc
-        # numbers, we have to use the ".epost" function which uploads a list of
-        # UIDs (acc numbers) for use in subsequent searches. Then, from .epost
-        # we can get the QueryKey and the WebEnv which define our history
-        # session and can be used to perform searches of data.
-        post = Entrez.epost('nuccore', id=submission)
-        search_results = use_entrez_read(post)
-
-        # Copy cookie "WebEnv" and query "QueryKey" from our history session to
-        # keep track of our batch fetching.
-        # WevEnv: Web environment string returned from a previous ESearch,
-        # EPost or ELink call
-        # QueryKey: Integer query key returned by a previous ESearch, EPost or
-        # ELink call.
-        webenv = search_results["WebEnv"]
-        query_key = search_results["QueryKey"]
-
-        # Get the batch information.
-        # db -> database, nuccore -> nuleotide, rettype -> retrieval type
-        # retmode -> determines the format of the return output
-        # retstart -> sequential index of the first UID in the retrieved
-        # set_number to be shown in the XML output
-        # retmax -> total number of UIDs from the retrieved set_number to
-        # be shown in the XML output
-        # idtype-> specifies the type of identifier to return for sequence.
-        # databases, acc -> accesion number.
-        fetch_handle = Entrez.efetch(
-            db="nuccore",
-            rettype="gb",
-            retmode="text",
-            retstart=0,
-            retmax=batch_size,
-            webenv=webenv,
-            query_key=query_key,
-            idtype="acc"
-        )
+        print("I am trying!")
+        try:
+            # db -> database, nuccore -> nuleotide, rettype -> retrieval type,
+            # retmode -> determines the format of the return output.
+            fetch_handle = Entrez.efetch(
+                db="nuccore", rettype="gb", retmode="text", id=submission,
+            )
+        except urllib.error.HTTPError as err:
+            if err.code == 400:
+                print(f"{submission} has invalid nuccore UIDs")
+                print(
+                    "If you provided a single accession number, your " +
+                    "results file is going to be empty."
+                )
+            else:
+                print(f"An error ocurred with the internet:\n{err}")
+            continue
+        except urllib.error.URLError as err:
+            if err.reason.errno == 8:
+                print(f"An error occured:\n{err}")
+                print(f"Maybe your internet is disconnected!")
+                sys.exit()
+            else:
+                print(f"An error occured with the internet:\n{err}")
+                sys.exti()
 
         # Parse the data fetched from NCBI.
-        records, ref_records = database.parser(
-            fetch_handle, set_number + 1)
-
+        records, ref_records = utils.parser(fetch_handle, set_num + 1)
         # Save the retrived data in the csv file.
-        for _, record in enumerate(records):
+        for record in records:
             results_writer.writerow(record)
-        for _, ref_record in enumerate(ref_records):
-            ref_results_writer.writerow(ref_record)
-        # Close fetch_handle.
+        for ref_record in ref_records:
+            references_writer.writerow(ref_record)
+
+        # Close fetch_handle
         fetch_handle.close()
 
 
 def fetch_from_biosample(
-        results_file: TextIO, results_fields: list, ref_results_file: TextIO,
-        ref_results_fields: list, submission_list: list
+        results_writer: TextIO, references_writer: TextIO,
+        submission_list: list
 ) -> None:
     """Fetch features from a list of BioSample numbers.
 
     Read a list of BioSample numbers to retrieve the features of all accession
     numbers associated to every BioSample number. A BioSample number can have
     one or more associated accession numbers. For example, SAMN07169263 has
     three accession numbers: CP049611.1, CP049610.1, and CP049609.1. The first
     two accession numbers belong to plasmids and the last one to a chromosome.
     In the case of SAMN07169263 this function will fetch features of the three
     above mentioned accession number.
 
     Parameters
     ----------
-    results_file : TextIO file object
-        Opened output file to save the fetched features of the accession
-        numbers.
-    results_fields : list
-        Headers for the `results` table. This list is the information to fetch
-        for every accession number associated to the BioSample number.
-    ref_results_file : TextIO file object
-        Opened output file to save the references of the accession numbers.
-    ref_results_fields : list
-        Headers for the `references_results` table. This list is the
-        information to fetch for every accession number associated to the
-        BioSample number.
+    results_writer : TextIO file object
+        Opened file as csv.DictWriter to save the fetched features of UIDs.
+    references_writer : TextIO file object
+        Opened file as csv.DictWriter to save the references of UIDs.
     submission_list : list
         List of BioSample numbers requested by the user.
 
     Notes
     -----
     Some BioSample numbers are associated to accession numbers that does not
     have any relevant information as contigs of few hundreds of nucleotides.
     Also, in addition to updated accession numbers, some BioSample numbers have
     outdated accession numbers. To clean all the fetched information from NCBI
     this program uses the `clean_features` function provided in database.py.
     """
     # Create DictWriter
-    results_writer = csv.DictWriter(results_file, results_fields)
-    ref_results_writer = csv.DictWriter(ref_results_file, ref_results_fields)
     lenght_acc_list = len(submission_list)
-
     # Iterate over the list of BioSample numbers (submission_list).
     for query, submission in enumerate(submission_list):
         # Number to keep track set_number of sequences (query), it is
         # important in case the connection to NCBI is interrupted so we can
         # know where to continue downloading
         set_number = query + 1
 
         # Print download record.
         print(f"Going to download record {query + 1} of {lenght_acc_list}\n")
         print(f"Accessing BioSample number: {submission}")
 
         # Search for the BioSample accession number. We need usehistory
         # to get the QueryKey and the WebEnv which define our history
         # session and can be used to performe searches of data.
-        search_handle = Entrez.esearch(
-            db="nuccore", term=submission, usehistory="y"
-        )
+        try:
+            search_handle = Entrez.esearch(
+                db="nuccore", term=submission, usehistory="y"
+            )
+        except urllib.error.HTTPError as err:
+            print(f"An error ocurred with the internet:\n{err}")
+            continue
+        except urllib.error.URLError as err:
+            if err.reason.errno == 8:
+                print(f"An error occured:\n{err}")
+                print(f"Maybe your internet is disconnected!")
+                sys.exit()
+            else:
+                print(f"An error occured with the internet:\n{err}")
+                sys.exit()
 
         # Copy information in computer memory.
-        # search_results = Entrez.read(search_handle)
-        search_results = use_entrez_read(search_handle)
+        search_results = Entrez.read(search_handle)
 
         # Close the handle.
         search_handle.close()
 
         # Count the number of results (number of sequences).
         count = int(search_results["Count"])
         print(f"Number of requested sequences from BioSample: {count}")
-
+        # Check if the BioSample number is valid.
+        if count == 0:
+            print(f'`{submission}` is an invalid BioSample number.\n')
+            continue
         # Copy cookie "WebEnv" and query "QueryKey" from our history session.
         # WevEnv -> Web environment string returned from a previous ESearch,
         # EPost or ELink call; QueryKey -> Integer query key returned by a
         # previous ESearch, EPost or ELink call.
         webenv = search_results["WebEnv"]
         query_key = search_results["QueryKey"]
 
@@ -232,36 +204,36 @@
                 retmax=end,
                 webenv=webenv,
                 query_key=query_key,
                 idtype="acc"
             )
 
             # Parse the data fetched from NCBI.
-            records, ref_records = database.parser(fetch_handle, set_number)
+            records, ref_records = utils.parser(fetch_handle, set_number)
 
             # Extend the records obtained in biosample_records for future
             # cleaning of the data, i.e to get the most updated data.
             biosample_records.extend(records)
             biosample_ref_records.extend(ref_records)
 
         # Use the clean_features function to clean data and obtain the
         # most updated information.
         # clean_features() returns a list of dictionaries
-        updated_features = database.clean_features(biosample_records)
+        updated_features = utils.clean_features(biosample_records)
 
         # Get references from updated accession number.
-        updated_references = database.clean_references(
+        updated_references = utils.clean_references(
             updated_features, biosample_ref_records
         )
 
         # Save the updated retrived data in the csv files.
         for updated_feature in updated_features:
             results_writer.writerow(updated_feature)
         for updated_ref in updated_references:
-            ref_results_writer.writerow(updated_ref)
+            references_writer.writerow(updated_ref)
 
         print(
             "Number of sequences saved after processing: " +
             f"{len(updated_features)}\n"
         )
 
         # Close fetch_handle.
@@ -270,21 +242,103 @@
 
 def use_entrez_read(handle: IO) -> None:
     try:
         search_result = Entrez.read(handle)
         return search_result
     except RuntimeError:
         print('Your list has invalid UIDs.')
-        sys.exit()
+
+
+def get_biosample_numbers(submission_list: list) -> list:
+    """Retrieve BioSample numbers from a list of batches of accession numbers.
+
+    This function uses Entrez.epost to upload batches of accession numbers to
+    the Entrez History server. To avoid problems with large batches of
+    accession numbers, limit the number of accession number per batch to 200.
+
+    Parameters
+    ----------
+    submission_list : list
+        List of batches of accession numbers. The following is an example of a
+        submission_list containing batches of three accession numbers per item
+        in the list:
+        [["CP049609.1", "CP028704.1", "CP043542.1"],
+         ["CP040107.1", "CP041747.1", "CP042638.1"],
+         ["CP015023.1", "CP049163.1", "CP051714.1"]]
+
+    Returns
+    -------
+    biosample_numbers : list
+        List of BioSample numbers retrieved from Entrez by using the provided
+        list of accession numbers. The following is a return list containing
+        the corresponding BioSample numbers of the example provided in the
+        Parameters section:
+        ["SAMN07169263", "SAMN08875353", "SAMEA104140560",
+        "SAMN05360217", "SAMN12302771", "SAMN12500846",
+        "SAMN04202539", "SAMN14133047", "SAMN14609782"]
+
+    Notes
+    -----
+    For more information about Entrez.epost read chapter 9.4 of Biopython
+    Tutorial and Cookbook (Biopython 1.76) and visit:
+    https://www.ncbi.nlm.nih.gov/books/NBK25499/#chapter4.EPost
+    """
+    # Create list to save BioSample numbers.
+    biosample_numbers = []
+    # Initialize last accession number.
+    end = 0
+    # Loop over batches of accession numbers to fetch BioSample numbers.
+    for _, submission in enumerate(submission_list):
+        start = end
+        batch_size = len(submission)
+        end = end + batch_size
+        # Print download batch record.
+        print(f"Retrieving BioSample numbers from record {start + 1} to {end}")
+
+        try:
+            # db -> database, nuccore -> nuleotide, rettype -> retrieval type,
+            # retmode -> determines the format of the return output.
+            fetch_handle = Entrez.efetch(
+                db="nuccore", rettype="gb", retmode="text", id=submission
+            )
+        except urllib.error.HTTPError as err:
+            if err.code == 400:
+                print(f"{submission} has invalid nuccore UIDs")
+                print(
+                    "If you provided a single accession number, your " +
+                    "results file is going to be empty."
+                )
+            else:
+                print(f"An error ocurred with the internet:\n{err}")
+            continue
+        except urllib.error.URLError as err:
+            if err.reason.errno == 8:
+                print(f"An error occured:\n{err}")
+                sys.exit(f"Maybe your internet is disconnected!")
+            else:
+                sys.exit(f"An error occured with the internet:\n{err}")
+
+        # Parse through the fetched information
+        for seq_record in SeqIO.parse(fetch_handle, "gb"):
+            # Loop over database cross-references (dbxrefs)
+            for xref in enumerate(seq_record.dbxrefs):
+                list_dbxrefs = xref[1].split(':')
+                # Get the BioSample number
+                if 'BioSample' in list_dbxrefs:
+                    biosample_numbers.append(list_dbxrefs[1])
+                    break
+
+    return biosample_numbers
 
 
 def fetch_features_manager(
         infile: Path, email_address: str, type_list: str = 'accession',
         output_folder: Path = Path('.'),
-        access_biosample_from_accession: bool = False, save_as: str = 'csv'
+        access_biosample_from_accession: bool = False, save_as: str = 'csv',
+        batch_size: int = 100
 ) -> None:
     """Fetch features from a list of accession or BioSample numbers.
 
     Read a txt or xlsx file with a list of UIDs. Then, convert the UIDs into a
     list of comma-separated UIDs to retrieve the information via Entrez.
 
     Parameters
@@ -298,107 +352,109 @@
     output_folder : Path
         Path to save result files.
     access_biosample_from_accession : bool
         Access the BioSample number link to an accession number and get the
         features of all the associated accession numbers.
     save_as : str
         Output file format. Options: 'csv', 'excel', or 'csv-excel'.
+    batch_size : int
+        Number of UIDs to be requested by batch. According to the documentation
+        of BioPython, it is not recommended to make batches of more than 500
+        UIDs.
     """
-    # Prove email address to NCBI
+    # Provide email address to NCBI
     Entrez.email = email_address
     # Read infile and create a list of accession or BioSample numbers.
-    list_accessions = database.make_uid_list(infile)
-    # Count the number of requested accession or BioSample numbers.
-    count = len(list_accessions)
-    print(f"\nRequested accession or BioSample numbers: {count}\n")
+    list_accessions = utils.make_uid_list(infile)
+    print(
+        f"\nRequested accession or BioSample numbers: {len(list_accessions)}\n"
+    )
 
     # Open result files to write the fetched data in csv format.
     results_path = output_folder / "results.csv"
     ref_results_path = output_folder / "ref_results.csv"
     results = open(results_path, "w")
     ref_results = open(ref_results_path, "w")
 
     # results' field names for the csv table.
     fields = [
-        "set_batch", "description", "accession", "size",
-        "molecule", "mod_date", "topology", "mol_type", "organism",
-        "strain", "isolation_source", "host", "plasmid", "country",
-        "lat_lon", "collection_date", "note", "serovar", "collected_by",
-        "genotype", "bioproject", "biosample", "assem_method",
-        "gen_coverage", "seq_technol", "gen_represent", "exp_final_ver"]
+        "set_batch", "description", "accession", "size", "molecule",
+        "mod_date", "topology", "mol_type", "organism", "strain",
+        "isolation_source", "host", "plasmid", "country", "lat_lon",
+        "collection_date", "note", "serovar", "collected_by", "genotype",
+        "bioproject", "biosample", "assem_method", "gen_coverage",
+        "seq_technol", "gen_represent", "exp_final_ver"
+    ]
     # references' field names for the csv table.
     ref_fields = [
         "accession", "reference_num", "location", "authors", "title",
         "journal", "medline_id", "pubmed_id", "comment"
     ]
     # Create DictWriter for results.
     results_writer = csv.DictWriter(results, fields)
-    ref_results_writer = csv.DictWriter(ref_results, ref_fields)
+    references_writer = csv.DictWriter(ref_results, ref_fields)
     # Write headers into csv files.
     results_writer.writeheader()
-    ref_results_writer.writeheader()
+    references_writer.writeheader()
 
-    # If user requested features from list of accession numbers use the
+    # ======================================================================= #
+    # If user requested features from a list of accession numbers use the
     # `fetch_from_accession` function.
+    # ======================================================================= #
     if type_list == 'accession' and (not access_biosample_from_accession):
-        # Formating list of accession numbers in batches. Don't make batches
-        # greater than 500.
-        submission_list = database.make_uid_batch_list(
-            uid_list=list_accessions, batch_size=200
+        # Make batches of accession numbers.
+        submission_list = utils.make_uid_batches(
+            uid_list=list_accessions, batch_size=batch_size
         )
-        # Fetching features
+        # Fetch features.
         print("\nFetching features\n")
         fetch_from_accession(
-            results_file=results,
-            results_fields=fields,
-            ref_results_file=ref_results,
-            ref_results_fields=ref_fields,
+            results_writer=results_writer,
+            references_writer=references_writer,
             submission_list=submission_list,
         )
 
-    # If user requested to access the BioSample numbers linked to accession
-    # numbers, use the `get_biosample_numbers` function to retrieve the linked
-    # BioSample numbers. Then use the `fetch_from_biosample` function.
+    # ======================================================================= #
+    # If user requested to access the BioSample numbers via the accession
+    # numbers, first use the `get_biosample_numbers` function to retrieve the
+    # linked BioSample numbers. Then use the `fetch_from_biosample` function.
+    # ======================================================================= #
     if type_list == 'accession' and access_biosample_from_accession:
-        # Formating list of accession numbers in batches. Don't make batches
-        # greater than 500.
-        submission_list = database.make_uid_batch_list(
-            uid_list=list_accessions, batch_size=200
-        )
-        # Getting BioSample numbers
-        print("Retrieving BioSample numbers from list of accession numbers")
-        list_biosamples = database.get_biosample_numbers(
-            submission_list, email_address
+        # Make batches of accession numbers.
+        submission_list = utils.make_uid_batches(
+            uid_list=list_accessions, batch_size=batch_size
         )
-        # Fetching features
+        # Get the BioSample numbers associated to accession numbers.
+        print("Retrieving BioSample numbers from list of accession numbers\n")
+        list_biosamples = get_biosample_numbers(submission_list)
+        # Fetch features.
         print("\nFetching features\n")
         fetch_from_biosample(
-            results_file=results,
-            results_fields=fields,
-            ref_results_file=ref_results,
-            ref_results_fields=ref_fields,
+            results_writer=results_writer,
+            references_writer=references_writer,
             submission_list=list_biosamples,
         )
 
+    # ======================================================================= #
     # If user requested features from a BioSample list use the
     # `fetch_from_biosample` function.
+    # ======================================================================= #
     if type_list == 'biosample':
-        # Fetching features
+        # Fetch features.
         print("\nFetching features\n")
         fetch_from_biosample(
-            results_file=results,
-            results_fields=fields,
-            ref_results_file=ref_results,
-            ref_results_fields=ref_fields,
+            results_writer=results_writer,
+            references_writer=references_writer,
+            # This list constains already the biosample numbers.
             submission_list=list_accessions,
         )
 
-    # Close result files
+    # Close result files.
     results.close()
     ref_results.close()
 
     # Save files in the requested format.
-    database.save_results_as(
+    utils.save_results_as(
         results=results_path,
         ref_results=ref_results_path,
         save_as=save_as
     )
```

### Comparing `fetch_features-0.2.3/src/fetcher/database.py` & `fetch_features-0.2.8/src/fetcher/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,50 +14,44 @@
 from Bio import Entrez
 from Bio import SeqIO
 
 
 def make_uid_list_from_txt(infile: Path) -> list:
     """Make list of UIDs from a txt file.
 
-    Read a txt file that contains a list of UIDs, as accession or BioSample
-    numbers. Then, create a python list with these UIDs.
-
     Parameters
     ----------
     infile : Path
         Path to txt file that contains UIDs as accession or BioSample
         numbers. Every UID must be separated by a new line character
-        (enter). The list can be created in excell by saving the file as
+        (enter). The list can be created in Excel by saving the file as
         txt or using a text editor.
 
     Returns
     -------
     list_accessions: list
         List of accession numbers. For example, a returned list from a txt
         file with nine accession number would look like the following list:
         ['CP049609.1', 'CP028704.1', 'CP043542.1', 'CP040107.1',
         'CP041747.1', 'CP042638.1', 'CP015023.1', 'CP049163.1',
         'CP051714.1']
     """
-    # Open infile.txt.
+    # Open infile.txt and make a list of UIDs.
     with open(infile, 'r') as reader:
-        # Create a list of unique identifiers.
         uid_list = reader.readlines()
-
-    # Remove the '\n' character.
-    for i, uid in enumerate(uid_list):
-        uid_list[i] = uid.replace('\n', '')
+    # Remove the `\n` character of every uid.
+    uid_list = [uid.rstrip() for uid in uid_list]
 
     return uid_list
 
 
 def make_uid_list_from_xlsx(infile: Path) -> list:
     """Make list of UIDs from a xlsx file.
 
-    Read an excel file that contains a list of UIDs, as accession or
+    Read an Excel file that contains a list of UIDs, as accession or
     BioSample numbers. Then, create a python list with these UIDs.
     The list must be in the first column of the first spreadsheet tab.
 
     Parameters
     ----------
     infile : Path
         Path to xlsx file that contains UIDs as accession or BioSample
@@ -86,169 +80,36 @@
     if infile_extention == 'txt':
         uid_list = make_uid_list_from_txt(infile)
     else:
         uid_list = make_uid_list_from_xlsx(infile)
     return uid_list
 
 
-def make_uid_batch_list(uid_list: list, batch_size: int = 200) -> list:
-    """Make batches of commma-delimited UIDs as accession or Biosample numbers.
-
-    Parameters
-    ----------
-    uid_list : list
-        List of UIDs to be proccessed
-    batch_size : int
-        Size of batches. NCBI suggests to request a maximum of 500
-        accession numbers.
+def make_uid_batches(uid_list: list, batch_size: int = 100) -> list:
+    """Make list of batches of UIDs."""
+    batches = []
+    for i, uid in enumerate(uid_list):
+        if (i % batch_size == 0) and (i == 0):
+            batch = [uid]
+        elif (i % batch_size == 0):
+            batches.append(batch)
+            batch = [uid]
+        else:
+            batch.append(uid)
+    batches.append(batch)
+    return batches
 
-    Returns
-    -------
-    submission_list : list
-        List of strings containg UIDs separated by commas. An example of a
-        submission_list created with accession numbers and a batch size of
-        three look like the following:
-        ['CP049609.1,CP028704.1,CP043542.1',
-        'CP040107.1,CP041747.1,CP042638.1',
-        'CP015023.1,CP049163.1,CP051714.1']
-    """
-    # Number of UIDs to process.
-    number_seq = len(uid_list)
-    # Declare the list of batches of comma-delimited UIDs to return after
-    # processing.
-    submission_list = []
-    # Counter to access the list_accessions.
-    counter_accessions = 0
-
-    # Loop to create the list of UIDs by batches
-    for start in range(0, number_seq, batch_size):
-        end = min(number_seq, start + batch_size)
-        # This list is going to save temporarily the batch of UIDs that are
-        # going to be converted into a string of comma-separated UIDs
-        set_list = []
-        # Make batches.
-        for _ in range(start, end):
-            set_list.append(uid_list[counter_accessions])
-            counter_accessions += 1
-        # Convert the list into string.
-        set_list = ','.join(set_list)
-        submission_list.append(set_list)
-
-    return submission_list
-
-
-def get_biosample_numbers(submission_list: list, email_address: str) -> list:
-    """Retrieve BioSample numbers from a list of batches of accession numbers.
-
-    This function uses Entrez.epost to upload batches of accession numbers to
-    the Entrez History server. To avoid problems with large batches of
-    accession numbers, limit the number of accession number per batch to 200.
 
-    Parameters
-    ----------
-    submission_list : list
-        List of strings containg batches of accession numbers separated by
-        commas. The following is an example of a submission_list containing
-        batches of three accession numbers per item in the list:
-        ["CP049609.1,CP028704.1,CP043542.1",
-        "CP040107.1,CP041747.1,CP042638.1",
-        "CP015023.1,CP049163.1,CP051714.1"]
-    email_address : string
-        User's email address is requested by NCBI
+class Info:
+    """"Class to store data retrieved from the nuccore database.
 
-    Returns
-    -------
-    biosample_numbers : list
-        List of BioSample numbers retrieved from Entrez by using the provided
-        list of accession numbers. The following is a return list containing
-        the corresponding BioSample numbers of the example provided in the
-        Parameters section:
-        ["SAMN07169263", "SAMN08875353", "SAMEA104140560",
-        "SAMN05360217", "SAMN12302771", "SAMN12500846",
-        "SAMN04202539", "SAMN14133047", "SAMN14609782"]
-
-    Notes
-    -----
-    For more information about Entrez.epost read chapter 9.4 of Biopython
-    Tutorial and Cookbook (Biopython 1.76) and visit:
-    https://www.ncbi.nlm.nih.gov/books/NBK25499/#chapter4.EPost
+    All the attributes are initiated to `missing`. Hence, if a fetched
+    attribute from the GenBank file is missing we reduce the if-else statements
+    in the code.
     """
-    # Create list to save BioSample numbers.
-    biosample_numbers = []
-
-    # Provide email address to GeneBank.
-    Entrez.email = email_address
-
-    # Initialize last accession number.
-    end = 0
-
-    # Fetch BioSample numbers from GenBank by batches.
-    for _, submission in enumerate(submission_list):
-        start = end
-        # submission_list is a list of accession numbers separated by
-        # commas. Therefore, the number of commas indicate the number of
-        # accession numbers.
-        batch_size = submission.count(',') + 1
-        end = end + batch_size
-
-        # Print download batch record.
-        print(f"Retrieving BioSample numbers from record {start + 1} to {end}")
-
-        # Post the submission_list.
-        # Because we are requesting information from a huge list of acc
-        # numbers, we have to use the ".epost" function which uploads a
-        # list of UIs (acc numbers) for use in subsequent searches.
-        # From .epost we can get the QueryKey and the WebEnv which define
-        # our history session and can be used to performe searches of data.
-        posting = Entrez.epost('nuccore', id=submission)
-        search_results = Entrez.read(posting)
-
-        # Copy cookie "WebEnv" and query "QueryKey" from our history
-        # session to keep track of our batch fetching.
-        # WevEnv -> Web environment string returned from a previous
-        # ESearch, EPost or ELink call; QueryKey -> Integer query key
-        # returned by a previous ESearch, EPost or ELink call
-        webenv = search_results["WebEnv"]
-        query_key = search_results["QueryKey"]
-
-        # Get the batch information
-        # db -> database, nuccore -> nuleotide, rettype -> retrieval type
-        # retmode -> determines the format of the return output
-        # retstart -> sequential index of the first UID in the retrieved
-        # set_number to be shown in the XML output
-        # retmax -> total number of UIDs from the retrieved set_number to be
-        # shown in the XML output
-        # idtype-> specifies the type of identifier to return for sequence
-        # databases, acc -> accesion number
-        fetch_handle = Entrez.efetch(
-            db="nuccore",
-            rettype="gb",
-            retmode="text",
-            retstart=0,
-            retmax=batch_size,
-            webenv=webenv,
-            query_key=query_key,
-            idtype="acc"
-        )
-
-        # Pars throw the fetched information
-        for seq_record in SeqIO.parse(fetch_handle, "gb"):
-            # Loop over database cross-references (dbxrefs)
-            for xref in enumerate(seq_record.dbxrefs):
-                list_dbxrefs = xref[1].split(':')
-                # Get the BioSample number
-                if 'BioSample' in list_dbxrefs:
-                    biosample_numbers.append(list_dbxrefs[1])
-                    break
-
-    return biosample_numbers
-
-
-class Info:
-    """"Class to store data retrieved from the nuccore database."""
 
     def __init__(
         self, set_batch='missing', description='missing', accession='missing',
         size='missing', mod_date='missing', molecule='missing',
         topology='missing', mol_type='missing', organism='missing',
         strain='missing', isolation_source='missing', host='missing',
         plasmid='missing', country='missing', lat_lon='missing',
```

### Comparing `fetch_features-0.2.3/src/fetcher/gui.py` & `fetch_features-0.2.8/src/fetcher/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 import customtkinter
 from customtkinter import ThemeManager
 
 from fetcher.user_input import is_valid_email
 from fetcher.access_genbank import fetch_features_manager
 
+# TODO: make a cancel button to kill downloading and restore all parameters to
+# default.
+# TODO: improve the reset button to clean the display textbox.
+
 
 class App(customtkinter.CTk):
     """fetch_features GUI."""
 
     def __init__(self):
         super().__init__()
         # Parameters to run fetch_features
@@ -159,15 +163,14 @@
             self.navigation_frame,
             values=['Accession', 'BioSample'],
             variable=self.type_identifier_var,
             command=lambda _: self.update_type_of_ui()
         )
         self.type_identifier_menu.grid(
             row=4, column=0, padx=(10, 5), pady=(5, 10))
-        # TODO: test this
         # Access BioSample from Accession number label
         self.access_bio_from_acc_label = customtkinter.CTkLabel(
             self.navigation_frame,
             text='Access BioSample from\naccession number:'
         )
         self.access_bio_from_acc_label.grid(row=3, column=1, padx=5, pady=5)
         # Access BioSample from Accession number variable
@@ -316,17 +319,19 @@
         if self.type_identifier_var.get() == 'Accession':
             self.type_of_ui = 'accession'
         else:
             self.type_of_ui = 'biosample'
 
     def update_access_biosample_from_accession(self) -> None:
         if self.access_bio_from_acc_var.get() == 'No':
-            self.access_bio_from_acc = False
+            self.access_biosample_from_accession = False
         else:
-            self.access_bio_from_acc = True
+            self.access_biosample_from_accession = True
+        print("value of access_bio_from_acc_var =",
+              self.access_biosample_from_accession)
 
     def update_save_as(self) -> None:
         if self.save_as_var.get() == 'csv':
             self.save_as = 'csv'
         elif self.save_as_var.get() == 'excel':
             self.save_as = 'excel'
         else:
@@ -425,17 +430,16 @@
             self.display_window.configure(state='disabled')
             return None
         self.display_window.configure(state='normal')
         self.display_window.insert('end', output)
         self.display_window.see('end')
         self.output.seek(0)
         self.output.truncate(0)
-        # self.display_window.configure(state='disabled')
-        # Call updtate constantly to check stdout
-        self.after(1000, self.update_textbox)
+        # Call updtate constantly to check stdout and stderr
+        self.after(500, self.update_textbox)
 
     def print_values_to_run_fetch_features(self) -> None:
         """Print values needed to run fetch features."""
         print('values for running fetch_features.py')
         print('Input paht:', self.input_path)
         print('output path:', self.output_path)
         print('type of ui:', self.type_of_ui)
```

### Comparing `fetch_features-0.2.3/src/fetcher/user_input.py` & `fetch_features-0.2.8/src/fetcher/user_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         action='store_true',
         help="Activate GUI."
     )
     # ################################################################ #
     # Parse command line arguments and store info in a UserInput class #
     # ################################################################ #
     args = parser.parse_args()
-    print(args.__dict__)
+    # print(args.__dict__)
     user_input = get_command_line_input(args)
     check_required_and_gui_arguments(user_input)
 
     return user_input
 
 
 def get_command_line_input(command_line_input: Namespace) -> UserInput:
@@ -192,32 +192,43 @@
     # Check if user wants to activate gui.
     user_input.use_gui = activate_gui(command_line_input)
 
     return user_input
 
 
 def check_required_and_gui_arguments(user_input: UserInput) -> None:
+    # If `use_gui` is selected, no mandatory arguments are needed.
     if (
         (user_input.use_gui and user_input.infile) or
         (user_input.use_gui and user_input.uid_type) or
         (user_input.use_gui and user_input.email)
     ):
         sys.exit(
             'Error: too many arguments. If you want to activate the ' +
             'GUI, only provide the `--gui` flag.'
         )
+    # If `use_gui` is not selected, all mandatory arguments are needed.
     if (
         (not user_input.use_gui and not user_input.infile) or
         (not user_input.use_gui and not user_input.uid_type) or
         (not user_input.use_gui and not user_input.email)
     ):
         sys.exit(
             'Error: the `--input`, `--type`, and `--email` arguments ' +
             'are required.'
         )
+    # If `--access-biosample-from-accession`, check that `--type` is accession
+    if (
+        (user_input.uid_type != 'accession') and
+        (user_input.access_biosample_from_accession)
+    ):
+        sys.exit(
+            'Error: when requesting `--access-biosample-from-accession` ' +
+            'the `--type` argument must be accession.'
+        )
 
 
 def get_infile(comm_line_input: Namespace) -> Union[Path, None]:
     infile = comm_line_input.input
     # If user provided input file, check if valid.
     if infile:
         infile = Path(infile)
```

