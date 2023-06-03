# Comparing `tmp/funga-eth-0.6.7.tar.gz` & `tmp/funga-eth-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funga-eth-0.6.7.tar", last modified: Sat Jun  3 12:11:32 2023, max compression
+gzip compressed data, was "funga-eth-0.7.0.tar", last modified: Sat Jun  3 12:29:17 2023, max compression
```

## Comparing `funga-eth-0.6.7.tar` & `funga-eth-0.7.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.6.7/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.6.7/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)     2009 2023-06-03 12:11:32.779925 funga-eth-0.6.7/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.6.7/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.6.7/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.6.7/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.776592 funga-eth-0.6.7/funga/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/cli/handle.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.6.7/funga/eth/cli/http.py
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/cli/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.6.7/funga/eth/cli/socket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.776592 funga-eth-0.6.7/funga/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/data/config/database.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/data/config/signer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)     2479 2022-10-13 07:37:03.000000 funga-eth-0.6.7/funga/eth/encoding.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/keystore/
--rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.6.7/funga/eth/keystore/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.6.7/funga/eth/keystore/dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.6.7/funga/eth/keystore/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.6.7/funga/eth/keystore/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.6.7/funga/eth/keystore/sql.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1107 2023-03-29 14:12:40.000000 funga-eth-0.6.7/funga/eth/message.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2978 2022-12-16 11:44:47.000000 funga-eth-0.6.7/funga/eth/runnable/keyfile.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2104 2023-03-27 13:56:19.000000 funga-eth-0.6.7/funga/eth/runnable/msg.py
--rwxr-xr-x   0 lash      (1000) lash      (1000)     3850 2021-10-15 20:39:21.000000 funga-eth-0.6.7/funga/eth/runnable/signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga/eth/signer/
--rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.6.7/funga/eth/signer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.6.7/funga/eth/signer/defaultsigner.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.6.7/funga/eth/transaction.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/funga_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)     2009 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1006 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      151 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      187 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-03 12:11:32.000000 funga-eth-0.6.7/funga_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      157 2023-03-29 14:12:40.000000 funga-eth-0.6.7/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      400 2023-06-03 12:11:32.779925 funga-eth-0.6.7/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-06-03 12:09:00.000000 funga-eth-0.6.7/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.6.7/sql_requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.6.7/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:11:32.779925 funga-eth-0.6.7/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.6.7/tests/test_cli.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.6.7/tests/test_keystore_dict.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.6.7/tests/test_pbkdf2.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.6.7/tests/test_sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.6.7/tests/test_socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.279919 funga-eth-0.7.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:49:56.000000 funga-eth-0.7.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2023-06-03 12:07:27.000000 funga-eth-0.7.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     2009 2023-06-03 12:29:17.279919 funga-eth-0.7.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1322 2023-06-03 12:11:27.000000 funga-eth-0.7.0/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 07:51:12.000000 funga-eth-0.7.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1630 2022-11-14 07:51:25.000000 funga-eth-0.7.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3564 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/cli/handle.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2298 2021-10-15 20:57:44.000000 funga-eth-0.7.0/funga/eth/cli/http.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/cli/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1546 2021-10-15 20:39:41.000000 funga-eth-0.7.0/funga/eth/cli/socket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/data/config/database.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       82 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/data/config/signer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)     2479 2022-10-13 07:37:03.000000 funga-eth-0.7.0/funga/eth/encoding.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/keystore/
+-rw-r--r--   0 lash      (1000) lash      (1000)      209 2021-10-10 10:17:05.000000 funga-eth-0.7.0/funga/eth/keystore/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1143 2021-10-10 11:04:50.000000 funga-eth-0.7.0/funga/eth/keystore/dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1560 2022-01-24 11:37:10.000000 funga-eth-0.7.0/funga/eth/keystore/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5335 2022-01-25 09:02:00.000000 funga-eth-0.7.0/funga/eth/keystore/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2021-10-30 06:00:33.000000 funga-eth-0.7.0/funga/eth/keystore/sql.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1107 2023-03-29 14:12:40.000000 funga-eth-0.7.0/funga/eth/message.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2978 2022-12-16 11:44:47.000000 funga-eth-0.7.0/funga/eth/runnable/keyfile.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2104 2023-03-27 13:56:19.000000 funga-eth-0.7.0/funga/eth/runnable/msg.py
+-rwxr-xr-x   0 lash      (1000) lash      (1000)     4308 2023-06-03 12:25:41.000000 funga-eth-0.7.0/funga/eth/runnable/signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.276585 funga-eth-0.7.0/funga/eth/signer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       56 2023-03-13 16:41:32.000000 funga-eth-0.7.0/funga/eth/signer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3210 2023-03-28 15:47:47.000000 funga-eth-0.7.0/funga/eth/signer/defaultsigner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4693 2021-10-15 20:59:28.000000 funga-eth-0.7.0/funga/eth/transaction.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.279919 funga-eth-0.7.0/funga_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2009 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1006 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      151 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      187 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        6 2023-06-03 12:29:17.000000 funga-eth-0.7.0/funga_eth.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      157 2023-03-29 14:12:40.000000 funga-eth-0.7.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      400 2023-06-03 12:29:17.279919 funga-eth-0.7.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)     1625 2023-06-03 12:26:45.000000 funga-eth-0.7.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-10 16:05:05.000000 funga-eth-0.7.0/sql_requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 16:05:05.000000 funga-eth-0.7.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 12:29:17.279919 funga-eth-0.7.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3477 2022-01-25 09:02:00.000000 funga-eth-0.7.0/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1519 2021-10-10 10:17:05.000000 funga-eth-0.7.0/tests/test_keystore_dict.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1537 2022-01-25 09:02:00.000000 funga-eth-0.7.0/tests/test_pbkdf2.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2855 2021-10-10 10:17:05.000000 funga-eth-0.7.0/tests/test_sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      268 2021-10-10 10:17:05.000000 funga-eth-0.7.0/tests/test_socket.py
```

### Comparing `funga-eth-0.6.7/LICENSE` & `funga-eth-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/PKG-INFO` & `funga-eth-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.6.7
+Version: 0.7.0
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `funga-eth-0.6.7/README.md` & `funga-eth-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/WAIVER` & `funga-eth-0.7.0/WAIVER`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/WAIVER.asc` & `funga-eth-0.7.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/cli/handle.py` & `funga-eth-0.7.0/funga/eth/cli/handle.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/cli/http.py` & `funga-eth-0.7.0/funga/eth/cli/http.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/cli/jsonrpc.py` & `funga-eth-0.7.0/funga/eth/cli/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/cli/socket.py` & `funga-eth-0.7.0/funga/eth/cli/socket.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/encoding.py` & `funga-eth-0.7.0/funga/eth/encoding.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/keystore/dict.py` & `funga-eth-0.7.0/funga/eth/keystore/dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/keystore/interface.py` & `funga-eth-0.7.0/funga/eth/keystore/interface.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/keystore/keyfile.py` & `funga-eth-0.7.0/funga/eth/keystore/keyfile.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/keystore/sql.py` & `funga-eth-0.7.0/funga/eth/keystore/sql.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/message.py` & `funga-eth-0.7.0/funga/eth/message.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/runnable/keyfile.py` & `funga-eth-0.7.0/funga/eth/runnable/keyfile.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/runnable/msg.py` & `funga-eth-0.7.0/funga/eth/runnable/msg.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/runnable/signer.py` & `funga-eth-0.7.0/funga/eth/runnable/signer.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # external imports
 import confini
 from jsonrpc.exceptions import *
 
 # local imports
 from funga.eth.signer import EIP155Signer
-from funga.eth.keystore.sql import SQLKeystore
 from funga.eth.cli.handle import SignRequestHandler
 
 logging.basicConfig(level=logging.WARNING)
 logg = logging.getLogger()
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 data_dir = os.path.join(script_dir, '..', 'data')
@@ -30,14 +29,15 @@
 socket_path = '/run/crypto-dev-signer/jsonrpc.ipc'
 
 
 argparser = argparse.ArgumentParser()
 argparser.add_argument('-c', type=str, default=config_dir, help='config file')
 argparser.add_argument('--env-prefix', default=os.environ.get('CONFINI_ENV_PREFIX'), dest='env_prefix', type=str, help='environment prefix for variables to overwrite configuration')
 argparser.add_argument('-i', type=int, help='default chain id for EIP155')
+argparser.add_argument('-k', '--keystore-type', dest='keystore_type', type=str, choices=['dict', 'sql'], default='dict', help='keystore backend type')
 argparser.add_argument('-s', type=str, help='socket path')
 argparser.add_argument('-v', action='store_true', help='be verbose')
 argparser.add_argument('-vv', action='store_true', help='be more verbose')
 args = argparser.parse_args()
 
 if args.vv:
     logging.getLogger().setLevel(logging.DEBUG)
@@ -84,15 +84,22 @@
     if secret_hex == None:
         raise MissingSecretError('please provide a valid hex value for the SIGNER_SECRET configuration variable')
 
     secret = bytes.fromhex(secret_hex)
     kw = {
             'symmetric_key': secret,
             }
-    SignRequestHandler.keystore = SQLKeystore(dsn, **kw)
+    if args.keystore_type == 'sql':
+        logg.info('using sql keystore: ' + dsn)
+        from funga.eth.keystore.sql import SQLKeystore
+        SignRequestHandler.keystore = SQLKeystore(dsn, **kw)
+    else:
+        logg.warning('using volatile dict keystore - all keys will be lost when you quit')
+        from funga.eth.keystore.dict import DictKeystore
+        SignRequestHandler.keystore = DictKeystore()
     SignRequestHandler.signer = EIP155Signer(SignRequestHandler.keystore)
 
     arg = None
     try:
         arg = json.loads(sys.argv[1])
     except:
         logg.info('no json rpc command detected, starting socket server {}'.format(socket_url))
```

### Comparing `funga-eth-0.6.7/funga/eth/signer/defaultsigner.py` & `funga-eth-0.7.0/funga/eth/signer/defaultsigner.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga/eth/transaction.py` & `funga-eth-0.7.0/funga/eth/transaction.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/funga_eth.egg-info/PKG-INFO` & `funga-eth-0.7.0/funga_eth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funga-eth
-Version: 0.6.7
+Version: 0.7.0
 Summary: Ethereum implementation of the funga keystore and signer
 Home-page: https://git.defalsify.org/funga-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `funga-eth-0.6.7/funga_eth.egg-info/SOURCES.txt` & `funga-eth-0.7.0/funga_eth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/setup.py` & `funga-eth-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 f = open('README.md', 'r')
 description = f.read()
 f.close()
 
 setup(
         name="funga-eth",
-        version="0.6.7",
+        version="0.7.0",
         description="Ethereum implementation of the funga keystore and signer",
         author="Louis Holbrook",
         author_email="dev@holbrook.no",
         packages=[
             'funga.eth.signer',
             'funga.eth',
             'funga.eth.cli',
```

### Comparing `funga-eth-0.6.7/tests/test_cli.py` & `funga-eth-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/tests/test_keystore_dict.py` & `funga-eth-0.7.0/tests/test_keystore_dict.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/tests/test_pbkdf2.py` & `funga-eth-0.7.0/tests/test_pbkdf2.py`

 * *Files identical despite different names*

### Comparing `funga-eth-0.6.7/tests/test_sign.py` & `funga-eth-0.7.0/tests/test_sign.py`

 * *Files identical despite different names*

