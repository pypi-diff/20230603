# Comparing `tmp/datasinda-0.0.0.tar.gz` & `tmp/datasinda-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\datasinda-0.0.0.tar", last modified: Sat Jun  3 00:44:39 2023, max compression
+gzip compressed data, was "dist\datasinda-0.0.1.tar", last modified: Sat Jun  3 20:35:48 2023, max compression
```

## Comparing `datasinda-0.0.0.tar` & `datasinda-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 00:44:39.029424 datasinda-0.0.0/
--rw-rw-rw-   0        0        0      535 2023-06-03 00:44:39.030402 datasinda-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 00:44:39.012826 datasinda-0.0.0/datasinda/
--rw-rw-rw-   0        0        0       56 2023-06-03 00:44:32.000000 datasinda-0.0.0/datasinda/__init__.py
--rw-rw-rw-   0        0        0       32 2023-06-02 18:48:36.000000 datasinda-0.0.0/datasinda/admin.py
--rw-rw-rw-   0        0        0      165 2023-06-02 18:46:51.000000 datasinda-0.0.0/datasinda/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:44:39.028449 datasinda-0.0.0/datasinda/migrations/
--rw-rw-rw-   0        0        0        0 2023-06-02 18:46:51.000000 datasinda-0.0.0/datasinda/migrations/__init__.py
--rw-rw-rw-   0        0        0       28 2023-06-02 18:48:51.000000 datasinda-0.0.0/datasinda/models.py
--rw-rw-rw-   0        0        0     1185 2023-06-02 18:46:51.000000 datasinda-0.0.0/datasinda/serializers.py
--rw-rw-rw-   0        0        0       60 2023-06-02 18:46:51.000000 datasinda-0.0.0/datasinda/tests.py
--rw-rw-rw-   0        0        0      752 2023-06-02 18:46:51.000000 datasinda-0.0.0/datasinda/urls.py
--rw-rw-rw-   0        0        0     7947 2023-06-02 18:54:29.000000 datasinda-0.0.0/datasinda/views.py
-drwxrwxrwx   0        0        0        0 2023-06-03 00:44:39.025522 datasinda-0.0.0/datasinda.egg-info/
--rw-rw-rw-   0        0        0      535 2023-06-03 00:44:38.000000 datasinda-0.0.0/datasinda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-03 00:44:38.000000 datasinda-0.0.0/datasinda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 00:44:38.000000 datasinda-0.0.0/datasinda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      350 2023-06-03 00:44:38.000000 datasinda-0.0.0/datasinda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-03 00:44:38.000000 datasinda-0.0.0/datasinda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1101 2023-06-03 00:44:39.032354 datasinda-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-06-02 20:33:51.000000 datasinda-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 20:35:48.120422 datasinda-0.0.1/
+-rw-rw-rw-   0        0        0     1072 2023-06-03 20:22:16.000000 datasinda-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      558 2023-06-03 20:35:48.121400 datasinda-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:23:24.000000 datasinda-0.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-03 20:35:48.103821 datasinda-0.0.1/datasinda/
+-rw-rw-rw-   0        0        0       56 2023-06-03 00:44:32.000000 datasinda-0.0.1/datasinda/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-02 18:48:36.000000 datasinda-0.0.1/datasinda/admin.py
+-rw-rw-rw-   0        0        0      165 2023-06-02 18:46:51.000000 datasinda-0.0.1/datasinda/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-03 20:35:48.119444 datasinda-0.0.1/datasinda/migrations/
+-rw-rw-rw-   0        0        0        0 2023-06-02 18:46:51.000000 datasinda-0.0.1/datasinda/migrations/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-06-02 18:48:51.000000 datasinda-0.0.1/datasinda/models.py
+-rw-rw-rw-   0        0        0       60 2023-06-03 20:31:07.000000 datasinda-0.0.1/datasinda/modulo.py
+-rw-rw-rw-   0        0        0     1185 2023-06-02 18:46:51.000000 datasinda-0.0.1/datasinda/serializers.py
+-rw-rw-rw-   0        0        0       60 2023-06-02 18:46:51.000000 datasinda-0.0.1/datasinda/tests.py
+-rw-rw-rw-   0        0        0      752 2023-06-02 18:46:51.000000 datasinda-0.0.1/datasinda/urls.py
+-rw-rw-rw-   0        0        0     7947 2023-06-02 18:54:29.000000 datasinda-0.0.1/datasinda/views.py
+drwxrwxrwx   0        0        0        0 2023-06-03 20:35:48.117493 datasinda-0.0.1/datasinda.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-06-03 20:35:47.000000 datasinda-0.0.1/datasinda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-06-03 20:35:47.000000 datasinda-0.0.1/datasinda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 20:35:47.000000 datasinda-0.0.1/datasinda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-06-03 20:35:47.000000 datasinda-0.0.1/datasinda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 20:35:47.000000 datasinda-0.0.1/datasinda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1101 2023-06-03 20:35:48.123352 datasinda-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-06-02 20:33:51.000000 datasinda-0.0.1/setup.py
```

### Comparing `datasinda-0.0.0/PKG-INFO` & `datasinda-0.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: datasinda
-Version: 0.0.0
+Version: 0.0.1
 Summary: Datasinda API
 Home-page: https://gitlab.com/alecerioli98/datasinda-api
 Author: 'Alessandro Cerioli'
 License: MIT
 Classifier: Framework :: Django
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
```

### Comparing `datasinda-0.0.0/datasinda/serializers.py` & `datasinda-0.0.1/datasinda/serializers.py`

 * *Files identical despite different names*

### Comparing `datasinda-0.0.0/datasinda/urls.py` & `datasinda-0.0.1/datasinda/urls.py`

 * *Files identical despite different names*

### Comparing `datasinda-0.0.0/datasinda/views.py` & `datasinda-0.0.1/datasinda/views.py`

 * *Files identical despite different names*

### Comparing `datasinda-0.0.0/datasinda.egg-info/PKG-INFO` & `datasinda-0.0.1/datasinda.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: datasinda
-Version: 0.0.0
+Version: 0.0.1
 Summary: Datasinda API
 Home-page: https://gitlab.com/alecerioli98/datasinda-api
 Author: 'Alessandro Cerioli'
 License: MIT
 Classifier: Framework :: Django
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
```

### Comparing `datasinda-0.0.0/setup.cfg` & `datasinda-0.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 6173 696e 6461 0d0a 7665   = datasinda..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 300d 0a64  rsion = 0.0.0..d
+00000020: 7273 696f 6e20 3d20 302e 302e 310d 0a64  rsion = 0.0.1..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2044 6174  escription = Dat
 00000040: 6173 696e 6461 2041 5049 0d0a 6c6f 6e67  asinda API..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 5245 4144 4d45 2e72 7374 0d0a  ile:README.rst..
 00000070: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
 00000080: 746c 6162 2e63 6f6d 2f61 6c65 6365 7269  tlab.com/aleceri
 00000090: 6f6c 6939 382f 6461 7461 7369 6e64 612d  oli98/datasinda-
@@ -15,15 +15,15 @@
 000000e0: 200d 0a09 4672 616d 6577 6f72 6b20 3a3a   ...Framework ::
 000000f0: 2044 6a61 6e67 6f0d 0a09 456e 7669 726f   Django...Enviro
 00000100: 6e6d 656e 7420 3a3a 2057 6562 2045 6e76  nment :: Web Env
 00000110: 6972 6f6e 6d65 6e74 0d0a 0949 6e74 656e  ironment...Inten
 00000120: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
 00000130: 4465 7665 6c6f 7065 7273 0d0a 094c 6963  Developers...Lic
 00000140: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000150: 6f76 6564 203a 3a20 4253 4420 4c69 6365  oved :: BSD Lice
+00000150: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
 00000160: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
 00000170: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 00000180: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
 00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
 000001b0: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
 000001c0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
```

