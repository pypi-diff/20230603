# Comparing `tmp/funga-0.5.5.tar.gz` & `tmp/funga-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funga-0.5.5.tar", last modified: Wed Mar 29 14:16:28 2023, max compression
+gzip compressed data, was "funga-0.5.6.tar", last modified: Sat Jun  3 12:32:40 2023, max compression
```

## Comparing `funga-0.5.5.tar` & `funga-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-29 14:16:28.513243 funga-0.5.5/
--rw-r--r--   0 lash      (1000) lash      (1000)     2098 2023-03-29 14:14:39.000000 funga-0.5.5/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:45:10.000000 funga-0.5.5/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2021-10-10 10:17:05.000000 funga-0.5.5/LICENSE.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-11-14 07:48:30.000000 funga-0.5.5/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)     1692 2023-03-29 14:16:28.513243 funga-0.5.5/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1044 2022-11-14 18:49:47.000000 funga-0.5.5/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2022-11-14 07:45:18.000000 funga-0.5.5/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1617 2022-11-14 07:45:28.000000 funga-0.5.5/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-29 14:16:28.513243 funga-0.5.5/funga/
--rw-r--r--   0 lash      (1000) lash      (1000)      423 2021-10-10 16:12:47.000000 funga-0.5.5/funga/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1376 2021-10-10 16:12:47.000000 funga-0.5.5/funga/keystore.py
--rw-r--r--   0 lash      (1000) lash      (1000)      173 2021-10-10 16:12:47.000000 funga-0.5.5/funga/signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-29 14:16:28.513243 funga-0.5.5/funga.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)     1692 2023-03-29 14:16:28.000000 funga-0.5.5/funga.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      292 2023-03-29 14:16:28.000000 funga-0.5.5/funga.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-29 14:16:28.000000 funga-0.5.5/funga.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-03-29 14:16:28.000000 funga-0.5.5/funga.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:12:47.000000 funga-0.5.5/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      376 2023-03-29 14:16:28.513243 funga-0.5.5/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      956 2023-03-29 14:15:18.000000 funga-0.5.5/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:09:40.000000 funga-0.5.5/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:32:40.753251 funga-0.5.6/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2181 2023-06-03 12:31:57.000000 funga-0.5.6/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:45:10.000000 funga-0.5.6/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2021-10-10 10:17:05.000000 funga-0.5.6/LICENSE.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-11-14 07:48:30.000000 funga-0.5.6/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     1691 2023-06-03 12:32:40.753251 funga-0.5.6/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1044 2022-11-14 18:49:47.000000 funga-0.5.6/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2022-11-14 07:45:18.000000 funga-0.5.6/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1617 2022-11-14 07:45:28.000000 funga-0.5.6/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:32:40.753251 funga-0.5.6/funga/
+-rw-r--r--   0 lash      (1000) lash      (1000)      423 2021-10-10 16:12:47.000000 funga-0.5.6/funga/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1376 2021-10-10 16:12:47.000000 funga-0.5.6/funga/keystore.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      173 2021-10-10 16:12:47.000000 funga-0.5.6/funga/signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:32:40.753251 funga-0.5.6/funga.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1691 2023-06-03 12:32:40.000000 funga-0.5.6/funga.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      292 2023-06-03 12:32:40.000000 funga-0.5.6/funga.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-03 12:32:40.000000 funga-0.5.6/funga.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-03 12:32:40.000000 funga-0.5.6/funga.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:12:47.000000 funga-0.5.6/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      375 2023-06-03 12:32:40.753251 funga-0.5.6/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      956 2023-06-03 12:31:05.000000 funga-0.5.6/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:09:40.000000 funga-0.5.6/test_requirements.txt
```

### Comparing `funga-0.5.5/CHANGELOG` & `funga-0.5.6/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+* 0.5.6
+	- Upgrade to beta
+* 0.5.5
+	- Change package readme and update project uri
 * 0.5.4
 	- Update url in package file
 * 0.5.3
 	- Change license to AGPL3 and copyright waived to public domain
 * 0.4.14-unreleased
 	- Remove web3 / eth-* module dependencies
 	- Add custom keyfile handling code and cli tool
```

### Comparing `funga-0.5.5/LICENSE` & `funga-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/LICENSE.txt` & `funga-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/PKG-INFO` & `funga-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: funga
-Version: 0.5.5
+Version: 0.5.6
 Summary: A signer and keystore daemon and library for cryptocurrency software development
 Home-page: https://git.defalsify.org/funga
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CRYPTO DEV SIGNER
```

### Comparing `funga-0.5.5/README.md` & `funga-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/WAIVER` & `funga-0.5.6/WAIVER`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/WAIVER.asc` & `funga-0.5.6/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/funga/keystore.py` & `funga-0.5.6/funga/keystore.py`

 * *Files identical despite different names*

### Comparing `funga-0.5.5/funga.egg-info/PKG-INFO` & `funga-0.5.6/funga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: funga
-Version: 0.5.5
+Version: 0.5.6
 Summary: A signer and keystore daemon and library for cryptocurrency software development
 Home-page: https://git.defalsify.org/funga
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CRYPTO DEV SIGNER
```

### Comparing `funga-0.5.5/setup.py` & `funga-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     if l == '':
         break
     test_requirements.append(l.rstrip())
 f.close()
 
 setup(
         name="funga",
-        version="0.5.5",
+        version="0.5.6",
         description="A signer and keystore daemon and library for cryptocurrency software development",
         author="Louis Holbrook",
         author_email="dev@holbrook.no",
         packages=[
             'funga',
             ],
         install_requires=requirements,
```

