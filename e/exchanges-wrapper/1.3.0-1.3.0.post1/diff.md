# Comparing `tmp/exchanges-wrapper-1.3.0.tar.gz` & `tmp/exchanges-wrapper-1.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges-wrapper-1.3.0.tar", last modified: Thu Jun  1 19:17:04 2023, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.0.post1.tar", last modified: Sat Jun  3 20:49:19 2023, max compression
```

## Comparing `exchanges-wrapper-1.3.0.tar` & `exchanges-wrapper-1.3.0.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0/.deepsource.toml
--rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0/.dockerignore
--rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0/.github/dependabot.yml
--rwxr-xr-x   0        0        0     5996 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0/Dockerfile
--rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0/README.md
--rw-r--r--   0        0        0    15398 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/example/exch_client.py
--rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0/example/ms_cfg.toml
--rw-r--r--   0        0        0     1287 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45215 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    44445 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19618 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     6048 2023-04-01 15:08:34.303021 exchanges-wrapper-1.3.0/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    61936 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-02-24 16:57:17.581054 exchanges-wrapper-1.3.0/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43798 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10270 2023-05-23 10:25:45.286853 exchanges-wrapper-1.3.0/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12097 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    22294 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      986 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/requirements.txt
--rw-r--r--   0        0        0     7577 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0.post1/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0.post1/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0.post1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0.post1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     5996 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0.post1/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0.post1/LICENSE.md
+-rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post1/README.md
+-rw-r--r--   0        0        0    15398 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/example/exch_client.py
+-rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0.post1/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1289 2023-06-03 20:48:25.969282 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19618 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6048 2023-04-01 15:08:34.303021 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61936 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-02-24 16:57:17.581054 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    43798 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10270 2023-05-23 10:25:45.286853 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22294 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0.post1/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0      986 2023-06-03 20:48:25.969282 exchanges-wrapper-1.3.0.post1/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-03 20:46:47.277312 exchanges-wrapper-1.3.0.post1/requirements.txt
+-rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0.post1/PKG-INFO
```

### Comparing `exchanges-wrapper-1.3.0/CHANGELOG.md` & `exchanges-wrapper-1.3.0.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/Dockerfile` & `exchanges-wrapper-1.3.0.post1/Dockerfile`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/LICENSE.md` & `exchanges-wrapper-1.3.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/README.md` & `exchanges-wrapper-1.3.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/example/exch_client.py` & `exchanges-wrapper-1.3.0.post1/example/exch_client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.3.0"
+__version__ = "1.3.0-1"
 
 from pathlib import Path
 import shutil
 #
 import platform
 print(f"Python {platform.python_version()}")
 #
```

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/c_structures.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.0.post1/exchanges_wrapper/web_sockets.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.3.0/pyproject.toml` & `exchanges-wrapper-1.3.0.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,16 @@
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
     "aiohttp==3.8.4",
-    "grpcio==1.54.2",
-    "grpcio-tools==1.54.2",
+    "grpcio==1.48.1",
+    "grpcio-tools==1.48.1",
     "toml==0.10.2",
     "idna==3.4",
     "pyotp~=2.8.0",
     "simplejson==3.19.1"
 ]
 
 [tool.flit.module]
```

### Comparing `exchanges-wrapper-1.3.0/PKG-INFO` & `exchanges-wrapper-1.3.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.3.0
+Version: 1.3.0.post1
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: aiohttp==3.8.4
-Requires-Dist: grpcio==1.54.2
-Requires-Dist: grpcio-tools==1.54.2
+Requires-Dist: grpcio==1.48.1
+Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: toml==0.10.2
 Requires-Dist: idna==3.4
 Requires-Dist: pyotp~=2.8.0
 Requires-Dist: simplejson==3.19.1
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0 Summary: REST API
-and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
-email: Thomas Marchand
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0.post1 Summary:
+REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
+Author-email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.54.2 Requires-Dist: grpcio-
-tools==1.54.2 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
+Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
+tools==1.48.1 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
 Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Project-URL: Source,
 https://github.com/DogsTailFarmer/exchanges-wrapper
             [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
```

