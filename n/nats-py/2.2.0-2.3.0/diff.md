# Comparing `tmp/nats-py-2.2.0.tar.gz` & `tmp/nats-py-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-py-2.2.0.tar", last modified: Sat Oct  1 06:37:21 2022, max compression
+gzip compressed data, was "nats-py-2.3.0.tar", last modified: Sat Jun  3 03:17:03 2023, max compression
```

## Comparing `nats-py-2.2.0.tar` & `nats-py-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,47 @@
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.076866 nats-py-2.2.0/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11357 2022-10-01 06:36:07.000000 nats-py-2.2.0/LICENSE
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    20923 2022-10-01 06:37:21.076975 nats-py-2.2.0/PKG-INFO
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7181 2022-10-01 06:36:07.000000 nats-py-2.2.0/README.md
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.072171 nats-py-2.2.0/nats/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1288 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/__init__.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.073299 nats-py-2.2.0/nats/aio/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    76140 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/client.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4014 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/errors.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8091 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/msg.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11458 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/subscription.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8489 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/aio/transport.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4269 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/errors.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.075424 nats-py-2.2.0/nats/js/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      729 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    16398 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/api.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    37701 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/client.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     5826 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/errors.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    14658 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/kv.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11830 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/js/manager.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2174 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/nuid.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.075930 nats-py-2.2.0/nats/protocol/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/protocol/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      789 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/protocol/command.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7371 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/protocol/parser.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats/py.typed
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:37:21.076646 nats-py-2.2.0/nats_py.egg-info/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    20923 2022-10-01 06:37:21.000000 nats-py-2.2.0/nats_py.egg-info/PKG-INFO
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      591 2022-10-01 06:37:21.000000 nats-py-2.2.0/nats_py.egg-info/SOURCES.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2022-10-01 06:37:21.000000 nats-py-2.2.0/nats_py.egg-info/dependency_links.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)       15 2022-10-01 06:37:21.000000 nats-py-2.2.0/nats_py.egg-info/requires.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        5 2022-10-01 06:37:21.000000 nats-py-2.2.0/nats_py.egg-info/top_level.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2022-10-01 06:36:07.000000 nats-py-2.2.0/nats_py.egg-info/zip-safe
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1237 2022-10-01 06:36:07.000000 nats-py-2.2.0/pyproject.toml
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      591 2022-10-01 06:37:21.077296 nats-py-2.2.0/setup.cfg
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      196 2022-10-01 06:36:07.000000 nats-py-2.2.0/setup.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.448949 nats-py-2.3.0/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11357 2022-10-01 06:36:07.000000 nats-py-2.3.0/LICENSE
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21002 2023-06-03 03:17:03.449064 nats-py-2.3.0/PKG-INFO
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7209 2023-06-03 03:16:18.000000 nats-py-2.3.0/README.md
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.442594 nats-py-2.3.0/nats/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1282 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/__init__.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.444033 nats-py-2.3.0/nats/aio/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/aio/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    77099 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4050 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/errors.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8450 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/msg.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    12256 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/subscription.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8164 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/transport.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4269 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/errors.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.445350 nats-py-2.3.0/nats/js/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      765 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    19338 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/api.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    40535 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6913 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/errors.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    14722 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/kv.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11923 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/manager.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    17500 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/object_store.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2210 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/nuid.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.445878 nats-py-2.3.0/nats/protocol/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/protocol/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      825 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/protocol/command.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7401 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/protocol/parser.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/py.typed
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.446976 nats-py-2.3.0/nats_py.egg-info/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21002 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/PKG-INFO
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      808 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/SOURCES.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/dependency_links.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)       65 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/requires.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        5 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/top_level.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats_py.egg-info/zip-safe
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1816 2023-06-03 03:16:18.000000 nats-py-2.3.0/pyproject.toml
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)       70 2023-06-03 03:17:03.449296 nats-py-2.3.0/setup.cfg
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      273 2023-06-03 03:16:18.000000 nats-py-2.3.0/setup.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.448817 nats-py-2.3.0/tests/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    84977 2023-06-03 03:16:18.000000 nats-py-2.3.0/tests/test_client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6309 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_async_await.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3944 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_nkeys.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2927 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_v2.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3530 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_websocket.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)   106446 2023-06-03 03:16:18.000000 nats-py-2.3.0/tests/test_js.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2398 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_nuid.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6805 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_parser.py
```

### Comparing `nats-py-2.2.0/LICENSE` & `nats-py-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nats-py-2.2.0/PKG-INFO` & `nats-py-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: NATS client for Python
 Author-email: Waldemar Quevedo <wally@synadia.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,14 +214,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: nkeys
+Provides-Extra: aiohttp
+Provides-Extra: fast_parse
 License-File: LICENSE
 
 # NATS - Python3 Client for Asyncio
 
 An [asyncio](https://docs.python.org/3/library/asyncio.html) Python client for the [NATS messaging system](https://nats.io).
 
 [![docs](https://img.shields.io/static/v1?label=docs&message=docs&color=informational)](https://nats-io.github.io/nats.py/)
@@ -336,14 +338,15 @@
     # Create pull based consumer on 'foo'.
     psub = await js.pull_subscribe("foo", "psub")
 
     # Fetch and ack messagess from consumer.
     for i in range(0, 10):
         msgs = await psub.fetch(1)
         for msg in msgs:
+            await msg.ack()
             print(msg)
 
     # Create single ephemeral push based subscriber.
     sub = await js.subscribe("foo")
     msg = await sub.next_msg()
     await msg.ack()
```

### Comparing `nats-py-2.2.0/README.md` & `nats-py-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     # Create pull based consumer on 'foo'.
     psub = await js.pull_subscribe("foo", "psub")
 
     # Fetch and ack messagess from consumer.
     for i in range(0, 10):
         msgs = await psub.fetch(1)
         for msg in msgs:
+            await msg.ack()
             print(msg)
 
     # Create single ephemeral push based subscriber.
     sub = await js.subscribe("foo")
     msg = await sub.next_msg()
     await msg.ack()
```

### Comparing `nats-py-2.2.0/nats/__init__.py` & `nats-py-2.3.0/nats/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import List, Union
+from __future__ import annotations
 
 from .aio.client import Client as NATS
 
 
 async def connect(
-    servers: Union[str, List[str]] = ["nats://localhost:4222"],
-    **options
+    servers: str | list[str] = ["nats://localhost:4222"], **options
 ) -> NATS:
     """
     :param servers: List of servers to connect.
     :param options: NATS connect options.
 
     ::
```

### Comparing `nats-py-2.2.0/nats/aio/__init__.py` & `nats-py-2.3.0/nats/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.2.0/nats/aio/client.py` & `nats-py-2.3.0/nats/aio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-# Copyright 2016-2022 The NATS Authors
+# Copyright 2016-2023 The NATS Authors
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 import asyncio
 import base64
 import ipaddress
 import json
 import logging
 import ssl
-import sys
 import time
-from secrets import token_hex
+import string
 from dataclasses import dataclass
 from email.parser import BytesParser
 from random import shuffle
+from secrets import token_hex
 from typing import (
     Any,
     Awaitable,
     Callable,
-    Dict,
-    List,
-    Optional,
     Tuple,
-    Type,
     Union,
 )
 from urllib.parse import ParseResult, urlparse
 
+try:
+    from fast_mail_parser import parse_email
+except ImportError:
+    parse_email = None
+
 import nats.js
 from nats import errors
 from nats.nuid import NUID
 from nats.protocol import command as prot_command
 from nats.protocol.parser import (
     AUTHORIZATION_VIOLATION,
     PERMISSIONS_ERR,
@@ -52,17 +55,17 @@
 from .errors import ErrInvalidUserCredentials, ErrStaleConnection
 from .msg import Msg
 from .subscription import (
     DEFAULT_SUB_PENDING_BYTES_LIMIT,
     DEFAULT_SUB_PENDING_MSGS_LIMIT,
     Subscription,
 )
-from .transport import Transport, TcpTransport, WebSocketTransport
+from .transport import TcpTransport, Transport, WebSocketTransport
 
-__version__ = '2.2.0'
+__version__ = '2.3.0'
 __lang__ = 'python3'
 _logger = logging.getLogger(__name__)
 PROTOCOL = 1
 
 INFO_OP = b'INFO'
 CONNECT_OP = b'CONNECT'
 PING_OP = b'PING'
@@ -108,70 +111,67 @@
 @dataclass
 class Srv:
     """
     Srv is a helper data structure to hold state of a server.
     """
     uri: ParseResult
     reconnects: int = 0
-    last_attempt: Optional[float] = None
+    last_attempt: float | None = None
     did_connect: bool = False
     discovered: bool = False
-    tls_name: Optional[str] = None
-    server_version: Optional[str] = None
+    tls_name: str | None = None
+    server_version: str | None = None
 
 
 class ServerVersion:
 
-    def __init__(self, server_version: str):
+    def __init__(self, server_version: str) -> None:
         self._server_version = server_version
-        self._major_version = None
-        self._minor_version = None
-        self._patch_version = None
-        self._dev_version = None
+        self._major_version: int | None = None
+        self._minor_version: int | None = None
+        self._patch_version: int | None = None
+        self._dev_version: str | None = None
 
-    def parse_version(self):
+    # TODO(@orsinium): use cached_property
+    def parse_version(self) -> None:
         v = (self._server_version).split('-')
         if len(v) > 1:
             self._dev_version = v[1]
         tokens = v[0].split('.')
         n = len(tokens)
         if n > 1:
             self._major_version = int(tokens[0])
         if n > 2:
             self._minor_version = int(tokens[1])
         if n > 3:
             self._patch_version = int(tokens[2])
 
     @property
     def major(self) -> int:
-        version = self._major_version
-        if not version:
+        if not self._major_version:
             self.parse_version()
-        return self._major_version
+        return self._major_version or 0
 
     @property
     def minor(self) -> int:
-        version = self._minor_version
-        if not version:
+        if not self._minor_version:
             self.parse_version()
-        return self._minor_version
+        return self._minor_version or 0
 
     @property
     def patch(self) -> int:
-        version = self._patch_version
-        if not version:
+        if not self._patch_version:
             self.parse_version()
-        return self._patch_version
+        return self._patch_version or 0
 
     @property
-    def dev(self) -> int:
-        version = self._dev_version
-        if not version:
+    def dev(self) -> str:
+        if not self._dev_version:
             self.parse_version()
-        return self._dev_version
+        return self._dev_version or ''
 
     def __repr__(self) -> str:
         return f"<nats server v{self._server_version}>"
 
 
 async def _default_error_callback(ex: Exception) -> None:
     """
@@ -182,140 +182,140 @@
 
 
 class Client:
     """
     Asyncio based client for NATS.
     """
 
-    msg_class: Type[Msg] = Msg
+    msg_class: type[Msg] = Msg
 
     # FIXME: Use an enum instead.
     DISCONNECTED = 0
     CONNECTED = 1
     CLOSED = 2
     RECONNECTING = 3
     CONNECTING = 4
     DRAINING_SUBS = 5
     DRAINING_PUBS = 6
 
     def __repr__(self) -> str:
         return f"<nats client v{__version__}>"
 
     def __init__(self) -> None:
-        self._current_server: Optional[Srv] = None
-        self._server_info: Dict[str, Any] = {}
-        self._server_pool: List[Srv] = []
-        self._reading_task: Optional[asyncio.Task] = None
-        self._ping_interval_task: Optional[asyncio.Task] = None
+        self._current_server: Srv | None = None
+        self._server_info: dict[str, Any] = {}
+        self._server_pool: list[Srv] = []
+        self._reading_task: asyncio.Task | None = None
+        self._ping_interval_task: asyncio.Task | None = None
         self._pings_outstanding: int = 0
         self._pongs_received: int = 0
-        self._pongs: List[asyncio.Future] = []
-        self._transport: Optional[Transport] = None
-        self._err: Optional[Exception] = None
+        self._pongs: list[asyncio.Future] = []
+        self._transport: Transport | None = None
+        self._err: Exception | None = None
 
         # callbacks
         self._error_cb: ErrorCallback = _default_error_callback
-        self._disconnected_cb: Optional[Callback] = None
-        self._closed_cb: Optional[Callback] = None
-        self._discovered_server_cb: Optional[Callback] = None
-        self._reconnected_cb: Optional[Callback] = None
+        self._disconnected_cb: Callback | None = None
+        self._closed_cb: Callback | None = None
+        self._discovered_server_cb: Callback | None = None
+        self._reconnected_cb: Callback | None = None
 
-        self._reconnection_task: Union[asyncio.Task[None], None] = None
-        self._reconnection_task_future: Optional[asyncio.Future] = None
+        self._reconnection_task: asyncio.Task[None] | None = None
+        self._reconnection_task_future: asyncio.Future | None = None
         self._max_payload: int = DEFAULT_MAX_PAYLOAD_SIZE
 
         # client id that the NATS server knows about.
-        self._client_id: Optional[str] = None
+        self._client_id: int | None = None
         self._sid: int = 0
-        self._subs: Dict[int, Subscription] = {}
+        self._subs: dict[int, Subscription] = {}
         self._status: int = Client.DISCONNECTED
         self._ps: Parser = Parser(self)
 
         # pending queue of commands that will be flushed to the server.
-        self._pending: List[bytes] = []
+        self._pending: list[bytes] = []
 
         # current size of pending data in total.
         self._pending_data_size: int = 0
 
         # max pending size is the maximum size of the data that can be buffered.
         self._max_pending_size: int = 0
 
-        self._flush_queue: Optional["asyncio.Queue[asyncio.Future[Any]]"
-                                    ] = None
-        self._flusher_task: Optional[asyncio.Task] = None
-        self._flush_timeout: Optional[float] = 0
+        self._flush_queue: asyncio.Queue[asyncio.Future[Any]] | None = None
+        self._flusher_task: asyncio.Task | None = None
+        self._flush_timeout: float | None = 0
         self._hdr_parser: BytesParser = BytesParser()
 
         # New style request/response
-        self._resp_map: Dict[str, asyncio.Future] = {}
-        self._resp_sub_prefix: Optional[bytearray] = None
+        self._resp_map: dict[str, asyncio.Future] = {}
+        self._resp_sub_prefix: bytearray | None = None
         self._nuid = NUID()
         self._inbox_prefix = bytearray(DEFAULT_INBOX_PREFIX)
+        self._auth_configured: bool = False
 
         # NKEYS support
         #
         # user_jwt_cb is used to fetch and return the account
         # signed JWT for this user.
-        self._user_jwt_cb: Optional[JWTCallback] = None
+        self._user_jwt_cb: JWTCallback | None = None
 
         # signature_cb is used to sign a nonce from the server while
         # authenticating with nkeys. The user should sign the nonce and
         # return the base64 encoded signature.
-        self._signature_cb: Optional[SignatureCallback] = None
+        self._signature_cb: SignatureCallback | None = None
 
         # user credentials file can be a tuple or single file.
-        self._user_credentials: Optional[Credentials] = None
+        self._user_credentials: Credentials | None = None
 
         # file that contains the nkeys seed and its public key as a string.
-        self._nkeys_seed: Optional[str] = None
-        self._public_nkey: Optional[str] = None
+        self._nkeys_seed: str | None = None
+        self._public_nkey: str | None = None
 
-        self.options: Dict[str, Any] = {}
+        self.options: dict[str, Any] = {}
         self.stats = {
             'in_msgs': 0,
             'out_msgs': 0,
             'in_bytes': 0,
             'out_bytes': 0,
             'reconnects': 0,
             'errors_received': 0,
         }
 
     async def connect(
         self,
-        servers: Union[str, List[str]] = ["nats://localhost:4222"],
-        error_cb: Optional[ErrorCallback] = None,
-        disconnected_cb: Optional[Callback] = None,
-        closed_cb: Optional[Callback] = None,
-        discovered_server_cb: Optional[Callback] = None,
-        reconnected_cb: Optional[Callback] = None,
-        name: Optional[str] = None,
+        servers: str | list[str] = ["nats://localhost:4222"],
+        error_cb: ErrorCallback | None = None,
+        disconnected_cb: Callback | None = None,
+        closed_cb: Callback | None = None,
+        discovered_server_cb: Callback | None = None,
+        reconnected_cb: Callback | None = None,
+        name: str | None = None,
         pedantic: bool = False,
         verbose: bool = False,
         allow_reconnect: bool = True,
         connect_timeout: int = DEFAULT_CONNECT_TIMEOUT,
         reconnect_time_wait: int = DEFAULT_RECONNECT_TIME_WAIT,
         max_reconnect_attempts: int = DEFAULT_MAX_RECONNECT_ATTEMPTS,
         ping_interval: int = DEFAULT_PING_INTERVAL,
         max_outstanding_pings: int = DEFAULT_MAX_OUTSTANDING_PINGS,
         dont_randomize: bool = False,
         flusher_queue_size: int = DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
         no_echo: bool = False,
-        tls: Optional[ssl.SSLContext] = None,
-        tls_hostname: Optional[str] = None,
-        user: Optional[str] = None,
-        password: Optional[str] = None,
-        token: Optional[str] = None,
+        tls: ssl.SSLContext | None = None,
+        tls_hostname: str | None = None,
+        user: str | None = None,
+        password: str | None = None,
+        token: str | None = None,
         drain_timeout: int = DEFAULT_DRAIN_TIMEOUT,
-        signature_cb: Optional[SignatureCallback] = None,
-        user_jwt_cb: Optional[JWTCallback] = None,
-        user_credentials: Optional[Credentials] = None,
-        nkeys_seed: Optional[str] = None,
-        inbox_prefix: Union[str, bytes] = DEFAULT_INBOX_PREFIX,
+        signature_cb: SignatureCallback | None = None,
+        user_jwt_cb: JWTCallback | None = None,
+        user_credentials: Credentials | None = None,
+        nkeys_seed: str | None = None,
+        inbox_prefix: str | bytes = DEFAULT_INBOX_PREFIX,
         pending_size: int = DEFAULT_PENDING_SIZE,
-        flush_timeout: Optional[float] = None,
+        flush_timeout: float | None = None,
     ) -> None:
         """
         Establishes a connection to NATS.
 
         :param servers: NATS Connection
         :param name: Label the connection with name (shown in NATS monitoring)
         :param error_cb: Callback to report errors.
@@ -444,15 +444,19 @@
         self.options["drain_timeout"] = drain_timeout
 
         if tls:
             self.options['tls'] = tls
         if tls_hostname:
             self.options['tls_hostname'] = tls_hostname
 
+        if user or password or token:
+            self._auth_configured = True
+
         if self._user_credentials is not None or self._nkeys_seed is not None:
+            self._auth_configured = True
             self._setup_nkeys_connect()
 
         # Queue used to trigger flushes to the socket.
         self._flush_queue = asyncio.Queue(maxsize=flusher_queue_size)
 
         # Max size of buffer used for flushing commands to the server.
         self._max_pending_size = pending_size
@@ -669,19 +673,25 @@
                 self._pending = []
                 self._pending_data_size = 0
                 await self._transport.drain()
 
         # Cleanup subscriptions since not reconnecting so no need
         # to replay the subscriptions anymore.
         for sub in self._subs.values():
-            # FIXME: Should we clear the pending queue here?
+            # Async subs use join when draining already so just cancel here.
             if sub._wait_for_msgs_task and not sub._wait_for_msgs_task.done():
                 sub._wait_for_msgs_task.cancel()
             if sub._message_iterator:
                 sub._message_iterator._cancel()
+            # Sync subs may have some inflight next_msg calls that could be blocking
+            # so cancel them here to unblock them.
+            if sub._pending_next_msgs_calls:
+                for fut in sub._pending_next_msgs_calls.values():
+                    fut.cancel("nats: connection is closed")
+                sub._pending_next_msgs_calls.clear()
         self._subs.clear()
 
         if self._transport is not None:
             self._transport.close()
             try:
                 await self._transport.wait_closed()
             except Exception as e:
@@ -743,15 +753,15 @@
             await self._close(Client.CLOSED)
 
     async def publish(
         self,
         subject: str,
         payload: bytes = b'',
         reply: str = '',
-        headers: Optional[Dict[str, str]] = None
+        headers: dict[str, str] | None = None
     ) -> None:
         """
         Publishes a NATS message.
 
         :param subject: Subject to which the message will be published.
         :param payload: Message data.
         :param reply: Inbox to which a responder can respond.
@@ -814,15 +824,15 @@
 
     async def _send_publish(
         self,
         subject: str,
         reply: str,
         payload: bytes,
         payload_size: int,
-        headers: Optional[Dict[str, Any]],
+        headers: dict[str, Any] | None,
     ) -> None:
         """
         Sends PUB command to the NATS server.
         """
         if subject == "":
             # Avoid sending messages with empty replies.
             raise errors.BadSubjectError
@@ -853,16 +863,16 @@
         if self._flush_queue is not None and self._flush_queue.empty():
             await self._flush_pending()
 
     async def subscribe(
         self,
         subject: str,
         queue: str = "",
-        cb: Optional[Callable[[Msg], Awaitable[None]]] = None,
-        future: Optional[asyncio.Future] = None,
+        cb: Callable[[Msg], Awaitable[None]] | None = None,
+        future: asyncio.Future | None = None,
         max_msgs: int = 0,
         pending_msgs_limit: int = DEFAULT_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_SUB_PENDING_BYTES_LIMIT,
     ) -> Subscription:
         """
         subscribe registers interest in a given subject.
 
@@ -942,15 +952,15 @@
 
     async def request(
         self,
         subject: str,
         payload: bytes = b'',
         timeout: float = 0.5,
         old_style: bool = False,
-        headers: Dict[str, Any] = None,
+        headers: dict[str, Any] | None = None,
     ) -> Msg:
         """
         Implements the request/response pattern via pub/sub
         using a single wildcard subscription that handles
         the responses.
 
         """
@@ -969,15 +979,15 @@
         return msg
 
     async def _request_new_style(
         self,
         subject: str,
         payload: bytes,
         timeout: float = 1,
-        headers: Dict[str, Any] = None,
+        headers: dict[str, Any] | None = None,
     ) -> Msg:
         if self.is_draining_pubs:
             raise errors.ConnectionDrainingError
 
         if not self._resp_sub_prefix:
             await self._init_request_sub()
         assert self._resp_sub_prefix
@@ -1079,50 +1089,50 @@
             await self._send_ping(future)
             await asyncio.wait_for(future, timeout)
         except asyncio.TimeoutError:
             future.cancel()
             raise errors.FlushTimeoutError
 
     @property
-    def connected_url(self) -> Optional[ParseResult]:
+    def connected_url(self) -> ParseResult | None:
         if self._current_server and self.is_connected:
             return self._current_server.uri
         return None
 
     @property
-    def servers(self) -> List[str]:
+    def servers(self) -> list[ParseResult]:
         servers = []
         for srv in self._server_pool:
-            servers.append(str(srv.uri))
+            servers.append(srv.uri)
         return servers
 
     @property
-    def discovered_servers(self) -> List[str]:
+    def discovered_servers(self) -> list[ParseResult]:
         servers = []
         for srv in self._server_pool:
             if srv.discovered:
-                servers.append(str(srv.uri))
+                servers.append(srv.uri)
         return servers
 
     @property
     def max_payload(self) -> int:
         """
         Returns the max payload which we received from the servers INFO
         """
         return self._max_payload
 
     @property
-    def client_id(self) -> Optional[str]:
+    def client_id(self) -> int | None:
         """
         Returns the client id which we received from the servers INFO
         """
         return self._client_id
 
     @property
-    def last_error(self) -> Optional[Exception]:
+    def last_error(self) -> Exception | None:
         """
         Returns the last error which may have occurred.
         """
         return self._err
 
     @property
     def pending_data_size(self) -> int:
@@ -1163,15 +1173,15 @@
         """
         if self._current_server and self._current_server.server_version:
             return ServerVersion(self._current_server.server_version)
         return ServerVersion("0.0.0-unknown")
 
     @property
     def ssl_context(self) -> ssl.SSLContext:
-        ssl_context: Optional[ssl.SSLContext] = None
+        ssl_context: ssl.SSLContext | None = None
         if "tls" in self.options:
             ssl_context = self.options.get('tls')
         else:
             ssl_context = ssl.create_default_context()
         if ssl_context is None:
             raise errors.Error('nats: no ssl context provided')
         return ssl_context
@@ -1188,15 +1198,15 @@
 
     async def _flush_pending(
         self,
         force_flush: bool = False,
     ) -> Any:
         assert self._flush_queue, "Client.connect must be called first"
         try:
-            future: "asyncio.Future" = asyncio.Future()
+            future: asyncio.Future = asyncio.Future()
             if not self.is_connected:
                 future.set_result(None)
                 return future
 
             # kick the flusher!
             await self._flush_queue.put(future)
 
@@ -1206,15 +1216,15 @@
                 except asyncio.TimeoutError:
                     # Report to the async callback that there was a timeout.
                     await self._error_cb(errors.FlushTimeoutError())
 
         except asyncio.CancelledError:
             pass
 
-    def _setup_server_pool(self, connect_url: Union[str, List[str]]) -> None:
+    def _setup_server_pool(self, connect_url: str | list[str]) -> None:
         if isinstance(connect_url, str):
             try:
                 if "nats://" in connect_url or "tls://" in connect_url:
                     # Closer to how the Go client handles this.
                     # e.g. nats://localhost:4222
                     uri = urlparse(connect_url)
                 elif "ws://" in connect_url or "wss://" in connect_url:
@@ -1226,15 +1236,16 @@
                 else:
                     # Just use the endpoint with the default NATS port.
                     # e.g. demo.nats.io
                     uri = urlparse(f"nats://{connect_url}:4222")
 
                 # In case only endpoint with scheme was set.
                 # e.g. nats://demo.nats.io or localhost:
-                if uri.port is None:
+                # the ws and wss do not need a default port as the transport will assume 80 and 443, respectively
+                if uri.port is None and uri.scheme not in ("ws", "wss"):
                     uri = urlparse(f"nats://{uri.hostname}:4222")
             except ValueError:
                 raise errors.Error("nats: invalid connect url option")
 
             if uri.hostname is None or uri.hostname == "none":
                 raise errors.Error("nats: invalid hostname in connect url")
             self._server_pool.append(Srv(uri))
@@ -1314,15 +1325,14 @@
                 continue
 
     async def _process_err(self, err_msg: str) -> None:
         """
         Processes the raw error message sent by the server
         and close connection with current server.
         """
-        assert self._error_cb, "Client.connect must be called first"
         if STALE_CONNECTION in err_msg:
             await self._process_op_err(errors.StaleConnectionError())
             return
 
         if AUTHORIZATION_VIOLATION in err_msg:
             self._err = errors.AuthorizationError()
         else:
@@ -1493,40 +1503,38 @@
             "version": __version__,
             "protocol": PROTOCOL
         }
         if "headers" in self._server_info:
             options["headers"] = self._server_info["headers"]
             options["no_responders"] = self._server_info["headers"]
 
-        if "auth_required" in self._server_info:
-            if self._server_info["auth_required"]:
-                if "nonce" in self._server_info and self._signature_cb is not None:
-                    sig = self._signature_cb(self._server_info["nonce"])
-                    options["sig"] = sig.decode()
-
-                    if self._user_jwt_cb is not None:
-                        jwt = self._user_jwt_cb()
-                        options["jwt"] = jwt.decode()
-                    elif self._public_nkey is not None:
-                        options["nkey"] = self._public_nkey
-                # In case there is no password, then consider handle
-                # sending a token instead.
-                elif self.options["user"] is not None and self.options[
-                        "password"] is not None:
-                    options["user"] = self.options["user"]
-                    options["pass"] = self.options["password"]
-                elif self.options["token"] is not None:
-                    options["auth_token"] = self.options["token"]
-                elif self._current_server and self._current_server.uri.username is not None:
-                    if self._current_server.uri.password is None:
-                        options["auth_token"
-                                ] = self._current_server.uri.username
-                    else:
-                        options["user"] = self._current_server.uri.username
-                        options["pass"] = self._current_server.uri.password
+        if self._auth_configured:
+            if "nonce" in self._server_info and self._signature_cb is not None:
+                sig = self._signature_cb(self._server_info["nonce"])
+                options["sig"] = sig.decode()
+
+                if self._user_jwt_cb is not None:
+                    jwt = self._user_jwt_cb()
+                    options["jwt"] = jwt.decode()
+                elif self._public_nkey is not None:
+                    options["nkey"] = self._public_nkey
+            # In case there is no password, then consider handle
+            # sending a token instead.
+            elif self.options["user"] is not None and self.options[
+                    "password"] is not None:
+                options["user"] = self.options["user"]
+                options["pass"] = self.options["password"]
+            elif self.options["token"] is not None:
+                options["auth_token"] = self.options["token"]
+            elif self._current_server and self._current_server.uri.username is not None:
+                if self._current_server.uri.password is None:
+                    options["auth_token"] = self._current_server.uri.username
+                else:
+                    options["user"] = self._current_server.uri.username
+                    options["pass"] = self._current_server.uri.password
 
         if self.options["name"] is not None:
             options["name"] = self.options["name"]
         if self.options["no_echo"] is not None:
             options["echo"] = not self.options["no_echo"]
 
         connect_opts = json.dumps(options, sort_keys=True)
@@ -1545,28 +1553,27 @@
         """
         if len(self._pongs) > 0:
             future = self._pongs.pop(0)
             future.set_result(True)
             self._pongs_received += 1
             self._pings_outstanding = 0
 
-    def _is_control_message(self, data, header: Dict[str,
-                                                     str]) -> Optional[str]:
+    def _is_control_message(self, data, header: dict[str, str]) -> str | None:
         if len(data) > 0:
             return None
         status = header.get(nats.js.api.Header.STATUS)
         if status == CTRL_STATUS:
             return header.get(nats.js.api.Header.DESCRIPTION)
         return None
 
-    async def _process_headers(self, headers) -> Optional[Dict[str, str]]:
+    async def _process_headers(self, headers) -> dict[str, str] | None:
         if not headers:
             return None
 
-        hdr = None
+        hdr: dict[str, str] | None = None
         raw_headers = headers[NATS_HDR_LINE_SIZE:]
 
         # If the first character is an empty space, then this is
         # an inline status message sent by the server.
         #
         # NATS/1.0 404\r\n\r\n
         # NATS/1.0 503\r\n\r\n
@@ -1583,15 +1590,15 @@
             status = line[:STATUS_MSG_LEN]
             desc = line[STATUS_MSG_LEN + 1:len(line) - _CRLF_LEN_ - _CRLF_LEN_]
             stripped_status = status.strip().decode()
 
             # Process as status only when it is a valid integer.
             hdr = {}
             if stripped_status.isdigit():
-                hdr[nats.js.api.Header.STATUS] = stripped_status
+                hdr[nats.js.api.Header.STATUS.value] = stripped_status
 
             # Move the raw_headers to end of line
             i = raw_headers.find(_CRLF_)
             raw_headers = raw_headers[i + _CRLF_LEN_:]
 
             if len(desc) > 0:
                 # Heartbeat messages can have both headers and inline status,
@@ -1614,40 +1621,52 @@
         #
         # Example header without status:
         #
         # NATS/1.0\r\nfoo: bar\r\nhello: world
         #
         raw_headers = headers[NATS_HDR_LINE_SIZE + _CRLF_LEN_:]
         try:
-            parsed_hdr = self._hdr_parser.parsebytes(raw_headers)
-            if len(parsed_hdr.items()) == 0:
-                return hdr
+            if parse_email:
+                parsed_hdr = parse_email(raw_headers).headers
             else:
-                if not hdr:
-                    hdr = {}
-                for k, v in parsed_hdr.items():
-                    hdr[k.strip()] = v.strip()
+                parsed_hdr = {
+                    k.strip(): v.strip()
+                    for k, v in self._hdr_parser.parsebytes(raw_headers
+                                                            ).items()
+                }
+            if hdr:
+                hdr.update(parsed_hdr)
+            else:
+                hdr = parsed_hdr
+
+            if parse_email:
+                to_delete = []
+                for k in hdr.keys():
+                    if any(c in k for c in string.whitespace):
+                        to_delete.append(k)
+                for k in to_delete:
+                    del hdr[k]
+
         except Exception as e:
             await self._error_cb(e)
             return hdr
 
-        return hdr
+        return hdr or None
 
     async def _process_msg(
         self,
         sid: int,
         subject: bytes,
         reply: bytes,
         data: bytes,
         headers: bytes,
     ) -> None:
         """
         Process MSG sent by server.
         """
-        assert self._error_cb, "Client.connect must be called first"
         payload_size = len(data)
         self.stats['in_msgs'] += 1
         self.stats['in_bytes'] += payload_size
 
         sub = self._subs.get(sid)
         if not sub:
             # Skip in case no subscription present.
@@ -1658,15 +1677,15 @@
             # Enough messages so can throwaway subscription now, the
             # pending messages will still be in the subscription
             # internal queue and the task will finish once the last
             # message is processed.
             self._subs.pop(sid, None)
 
         hdr = await self._process_headers(headers)
-        msg = self._build_message(subject, reply, data, hdr)
+        msg = self._build_message(sid, subject, reply, data, hdr)
         if not msg:
             return
 
         # Process flow control messages in case of using a JetStream context.
         ctrl_msg = None
         fcReply = None
         if sub._jsi:
@@ -1763,36 +1782,38 @@
 
         if ctrl_msg and not msg.reply and ctrl_msg.startswith("Idle"):
             if sub._jsi:
                 await sub._jsi.check_for_sequence_mismatch(msg)
 
     def _build_message(
         self,
+        sid: int,
         subject: bytes,
         reply: bytes,
         data: bytes,
-        headers: Optional[Dict[str, str]],
+        headers: dict[str, str] | None,
     ):
         return self.msg_class(
             subject=subject.decode(),
             reply=reply.decode(),
             data=data,
             headers=headers,
             _client=self,
+            _sid=sid,
         )
 
     def _process_disconnect(self) -> None:
         """
         Process disconnection from the server and set client status
         to DISCONNECTED.
         """
         self._status = Client.DISCONNECTED
 
     def _process_info(
-        self, info: Dict[str, Any], initial_connection: bool = False
+        self, info: dict[str, Any], initial_connection: bool = False
     ) -> None:
         """
         Process INFO lines sent by the server to reconfigure client
         with latest updates from cluster to enable server discovery.
         """
         assert self._current_server, "Client.connect must be called first"
         if 'connect_urls' in info:
@@ -1826,15 +1847,17 @@
                     shuffle(connect_urls)
                 for srv in connect_urls:
                     self._server_pool.append(srv)
 
                 if not initial_connection and connect_urls and self._discovered_server_cb:
                     self._discovered_server_cb()
 
-    def _host_is_ip(self, connect_url: Optional[str]) -> bool:
+    def _host_is_ip(self, connect_url: str | None) -> bool:
+        if connect_url is None:
+            return False
         try:
             ipaddress.ip_address(connect_url)
             return True
         except Exception:
             return False
 
     async def _process_connect_init(self) -> None:
@@ -1848,26 +1871,31 @@
         self._status = Client.CONNECTING
 
         connection_completed = self._transport.readline()
         info_line = await asyncio.wait_for(
             connection_completed, self.options["connect_timeout"]
         )
         if INFO_OP not in info_line:
+            # FIXME: Handle PING/PONG arriving first as well.
             raise errors.Error(
                 "nats: empty response from server when expecting INFO message"
             )
 
         _, info = info_line.split(INFO_OP + _SPC_, 1)
 
         try:
             srv_info = json.loads(info.decode())
+            self._server_info = srv_info
         except Exception:
             raise errors.Error("nats: info message, json parse error")
 
-        self._server_info = srv_info
+        # In case 'auth_required' is part of INFO, then need to send credentials.
+        if srv_info.get("auth_required", False):
+            self._auth_configured = True
+
         self._process_info(srv_info, initial_connection=True)
 
         if 'version' in self._server_info:
             self._current_server.server_version = self._server_info['version']
 
         if 'max_payload' in self._server_info:
             self._max_payload = self._server_info["max_payload"]
@@ -1953,29 +1981,28 @@
         )
 
         # Task for kicking the flusher queue
         self._flusher_task = asyncio.get_running_loop().create_task(
             self._flusher()
         )
 
-    async def _send_ping(self, future: asyncio.Future = None) -> None:
+    async def _send_ping(self, future: asyncio.Future | None = None) -> None:
         assert self._transport, "Client.connect must be called first"
         if future is None:
             future = asyncio.Future()
         self._pongs.append(future)
         self._transport.write(PING_PROTO)
         self._pending_data_size += len(PING_PROTO)
         await self._flush_pending()
 
     async def _flusher(self) -> None:
         """
         Coroutine which continuously tries to consume pending commands
         and then flushes them to the socket.
         """
-        assert self._error_cb, "Client.connect must be called first"
         assert self._transport, "Client.connect must be called first"
         assert self._flush_queue, "Client.connect must be called first"
         while True:
             if not self.is_connected or self.is_connecting:
                 break
 
             future: asyncio.Future = await self._flush_queue.get()
```

### Comparing `nats-py-2.2.0/nats/aio/errors.py` & `nats-py-2.3.0/nats/aio/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 import nats.errors
 
 
 class NatsError(nats.errors.Error):
     """
     .. deprecated:: v2.0.0
```

### Comparing `nats-py-2.2.0/nats/aio/msg.py` & `nats-py-2.3.0/nats/aio/msg.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,52 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 import datetime
 import json
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import TYPE_CHECKING
 
 from nats.errors import Error, MsgAlreadyAckdError, NotJSMessageError
 
 if TYPE_CHECKING:
     from nats import NATS
 
+# Subject without domain:
+# $JS.ACK.<stream>.<consumer>.<delivered>.<sseq>.<cseq>.<tm>.<pending>
+#
+_V1_TOKEN_COUNT = 9
+
+# Subject with domain:
+# $JS.ACK.<domain>.<account hash>.<stream>.<consumer>.<delivered>.<sseq>.
+#   <cseq>.<tm>.<pending>.<a token with a random value>
+#
+_V2_TOKEN_COUNT = 12
+
 
 @dataclass
 class Msg:
     """
     Msg represents a message delivered by NATS.
     """
-    _client: "NATS"
+    _client: NATS
     subject: str = ''
     reply: str = ''
     data: bytes = b''
-    headers: Optional[Dict[str, str]] = None
+    headers: dict[str, str] | None = None
 
-    _metadata: Optional["Metadata"] = None
+    _metadata: Metadata | None = None
     _ackd: bool = False
+    _sid: int | None = None
 
     class Ack:
         Ack = b"+ACK"
         Nak = b"-NAK"
         Progress = b"+WPI"
         Term = b"+TERM"
 
@@ -51,32 +65,30 @@
         Consumer = 5
         NumDelivered = 6
         StreamSeq = 7
         ConsumerSeq = 8
         Timestamp = 9
         NumPending = 10
 
-        # Subject without domain:
-        # $JS.ACK.<stream>.<consumer>.<delivered>.<sseq>.<cseq>.<tm>.<pending>
-        #
-        V1TokenCount = 9
-
-        # Subject with domain:
-        # $JS.ACK.<domain>.<account hash>.<stream>.<consumer>.<delivered>.<sseq>.
-        #   <cseq>.<tm>.<pending>.<a token with a random value>
-        #
-        V2TokenCount = 12
-
     @property
-    def header(self) -> Optional[dict]:
+    def header(self) -> dict | None:
         """
         header returns the headers from a message.
         """
         return self.headers
 
+    @property
+    def sid(self) -> int:
+        """
+        sid returns the subscription ID from a message.
+        """
+        if self._sid is None:
+            raise Error('sid not set')
+        return self._sid
+
     async def respond(self, data: bytes) -> None:
         """
         respond replies to the inbox of the message if there is one.
         """
         if not self.reply:
             raise Error('no reply subject available')
         if not self._client:
@@ -97,15 +109,15 @@
         ack_sync waits for the acknowledgement to be processed by the server.
         """
         self._check_reply()
         resp = await self._client.request(self.reply, timeout=timeout)
         self._ackd = True
         return resp
 
-    async def nak(self, delay: Optional[Union[int, float]] = None) -> None:
+    async def nak(self, delay: int | float | None = None) -> None:
         """
         nak negatively acknowledges a message delivered by JetStream triggering a redelivery.
         if `delay` is provided, redelivery is delayed for `delay` seconds
         """
         self._check_reply()
         payload = Msg.Ack.Nak
         json_args = dict()
@@ -133,111 +145,113 @@
 
         await self._client.publish(self.reply, Msg.Ack.Term)
         self._ackd = True
 
     # TODO(@orsinium): use a cached_property. Available in functools since 3.8,
     # as a package (backports.cached-property), or can be just copy-pasted in the project.
     @property
-    def metadata(self) -> "Metadata":
+    def metadata(self) -> Metadata:
         """
         metadata returns the Metadata of a JetStream message.
         """
-        msg = self
         # Memoize the parsed metadata.
-        metadata = msg._metadata
+        metadata = self._metadata
         if metadata is not None:
             return metadata
-
-        tokens = Msg.Metadata._get_metadata_fields(msg.reply)
-
-        if len(tokens) == Msg.Ack.V1TokenCount:
-            t = datetime.datetime.fromtimestamp(
-                int(tokens[7]) / 1_000_000_000.0
-            )
-            metadata = Msg.Metadata(
-                sequence=Msg.Metadata.SequencePair(
-                    stream=int(tokens[5]),
-                    consumer=int(tokens[6]),
-                ),
-                num_delivered=int(tokens[4]),
-                num_pending=int(tokens[8]),
-                timestamp=t,
-                stream=tokens[2],
-                consumer=tokens[3],
-            )
-        else:
-            t = datetime.datetime.fromtimestamp(
-                int(tokens[Msg.Ack.Timestamp]) / 1_000_000_000.0
-            )
-
-            # Underscore indicate no domain is set. Expose as empty string
-            # to client.
-            domain = tokens[Msg.Ack.Domain]
-            if domain == "_":
-                domain = ""
-
-            metadata = Msg.Metadata(
-                sequence=Msg.Metadata.SequencePair(
-                    stream=int(tokens[Msg.Ack.StreamSeq]),
-                    consumer=int(tokens[Msg.Ack.ConsumerSeq]),
-                ),
-                num_delivered=int(tokens[Msg.Ack.NumDelivered]),
-                num_pending=int(tokens[Msg.Ack.NumPending]),
-                timestamp=t,
-                stream=tokens[Msg.Ack.Stream],
-                consumer=tokens[Msg.Ack.Consumer],
-                domain=domain,
-            )
-
-        msg._metadata = metadata
+        metadata = Msg.Metadata._from_reply(self.reply)
+        self._metadata = metadata
         return metadata
 
-    def _get_metadata_fields(self, reply: Optional[str]) -> List[str]:
+    def _get_metadata_fields(self, reply: str | None) -> list[str]:
         return Msg.Metadata._get_metadata_fields(reply)
 
     def _check_reply(self) -> None:
         if self.reply is None or self.reply == '':
             raise NotJSMessageError
         if self._ackd:
             raise MsgAlreadyAckdError(self)
 
-    @dataclass
+    @dataclass(frozen=True)
     class Metadata:
         """
         Metadata is the metadata from a JetStream message.
 
         - num_pending is the number of available messages in the Stream that have not been
           consumed yet.
         - num_delivered is the number of times that this message has been delivered.
           For example, num_delivered higher than one means that there have been redeliveries.
         - timestamp is the time at which the message was delivered.
         - stream is the name of the stream.
         - consumer is the name of the consumer.
 
         """
-        sequence: Optional["SequencePair"] = None
-        num_pending: Optional[int] = None
-        num_delivered: Optional[int] = None
-        timestamp: Optional[datetime.datetime] = None
-        stream: Optional[str] = None
-        consumer: Optional[str] = None
-        domain: Optional[str] = None
+        sequence: SequencePair
+        num_pending: int
+        num_delivered: int
+        timestamp: datetime.datetime
+        stream: str
+        consumer: str
+        domain: str | None = None
 
-        @dataclass
+        @dataclass(frozen=True)
         class SequencePair:
             """
             SequencePair represents a pair of consumer and stream sequence.
             """
             consumer: int
             stream: int
 
         @classmethod
-        def _get_metadata_fields(cls, reply: Optional[str]) -> List[str]:
+        def _get_metadata_fields(cls, reply: str | None) -> list[str]:
             if not reply:
                 raise NotJSMessageError
             tokens = reply.split('.')
-            if (len(tokens) == Msg.Ack.V1TokenCount or
-                    len(tokens) >= Msg.Ack.V2TokenCount-1) and \
+            if (len(tokens) == _V1_TOKEN_COUNT or
+                    len(tokens) >= _V2_TOKEN_COUNT-1) and \
                     tokens[0] == Msg.Ack.Prefix0 and \
                     tokens[1] == Msg.Ack.Prefix1:
                 return tokens
             raise NotJSMessageError
+
+        @classmethod
+        def _from_reply(cls, reply: str) -> Msg.Metadata:
+            """Construct the metadata from the reply string
+            """
+            tokens = cls._get_metadata_fields(reply)
+            if len(tokens) == _V1_TOKEN_COUNT:
+                t = datetime.datetime.fromtimestamp(
+                    int(tokens[7]) / 1_000_000_000.0
+                )
+                return cls(
+                    sequence=Msg.Metadata.SequencePair(
+                        stream=int(tokens[5]),
+                        consumer=int(tokens[6]),
+                    ),
+                    num_delivered=int(tokens[4]),
+                    num_pending=int(tokens[8]),
+                    timestamp=t,
+                    stream=tokens[2],
+                    consumer=tokens[3],
+                )
+            else:
+                t = datetime.datetime.fromtimestamp(
+                    int(tokens[Msg.Ack.Timestamp]) / 1_000_000_000.0
+                )
+
+                # Underscore indicate no domain is set. Expose as empty string
+                # to client.
+                domain = tokens[Msg.Ack.Domain]
+                if domain == "_":
+                    domain = ""
+
+                return cls(
+                    sequence=Msg.Metadata.SequencePair(
+                        stream=int(tokens[Msg.Ack.StreamSeq]),
+                        consumer=int(tokens[Msg.Ack.ConsumerSeq]),
+                    ),
+                    num_delivered=int(tokens[Msg.Ack.NumDelivered]),
+                    num_pending=int(tokens[Msg.Ack.NumPending]),
+                    timestamp=t,
+                    stream=tokens[Msg.Ack.Stream],
+                    consumer=tokens[Msg.Ack.Consumer],
+                    domain=domain,
+                )
```

### Comparing `nats-py-2.2.0/nats/aio/subscription.py` & `nats-py-2.3.0/nats/aio/subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 import asyncio
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
     Awaitable,
     Callable,
-    List,
-    Optional,
 )
 
 from nats import errors
 # Default Pending Limits of Subscriptions
 from nats.aio.msg import Msg
 
 if TYPE_CHECKING:
@@ -58,16 +58,16 @@
 
     def __init__(
         self,
         conn,
         id: int = 0,
         subject: str = '',
         queue: str = '',
-        cb: Optional[Callable[['Msg'], Awaitable[None]]] = None,
-        future: Optional[asyncio.Future] = None,
+        cb: Callable[[Msg], Awaitable[None]] | None = None,
+        future: asyncio.Future | None = None,
         max_msgs: int = 0,
         pending_msgs_limit: int = DEFAULT_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_SUB_PENDING_BYTES_LIMIT,
     ) -> None:
         self._conn = conn
         self._id = id
         self._subject = subject
@@ -77,23 +77,29 @@
         self._cb = cb
         self._future = future
         self._closed = False
 
         # Per subscription message processor.
         self._pending_msgs_limit = pending_msgs_limit
         self._pending_bytes_limit = pending_bytes_limit
-        self._pending_queue: "asyncio.Queue[Msg]" = asyncio.Queue(
+        self._pending_queue: asyncio.Queue[Msg] = asyncio.Queue(
             maxsize=pending_msgs_limit
         )
+        # If no callback, then this is a sync subscription which will
+        # require tracking the next_msg calls inflight for cancelling.
+        if cb is None:
+            self._pending_next_msgs_calls = {}
+        else:
+            self._pending_next_msgs_calls = None
         self._pending_size = 0
         self._wait_for_msgs_task = None
         self._message_iterator = None
 
         # For JetStream enabled subscriptions.
-        self._jsi: Optional["JetStreamContext._JSI"] = None
+        self._jsi: JetStreamContext._JSI | None = None
 
     @property
     def subject(self) -> str:
         """
         Returns the subject of the `Subscription`.
         """
         return self._subject
@@ -102,15 +108,15 @@
     def queue(self) -> str:
         """
         Returns the queue name of the `Subscription` if part of a queue group.
         """
         return self._queue
 
     @property
-    def messages(self) -> AsyncIterator['Msg']:
+    def messages(self) -> AsyncIterator[Msg]:
         """
         Retrieves an async iterator for the messages from the subscription.
 
         This is only available if a callback isn't provided when creating a
         subscription.
         """
         if not self._message_iterator:
@@ -139,47 +145,62 @@
     @property
     def delivered(self) -> int:
         """
         Number of delivered messages to this subscription so far.
         """
         return self._received
 
-    async def next_msg(self, timeout: Optional[float] = 1.0) -> Msg:
+    async def next_msg(self, timeout: float | None = 1.0) -> Msg:
         """
         :params timeout: Time in seconds to wait for next message before timing out.
         :raises nats.errors.TimeoutError:
 
-        next_msg can be used to retrieve the next message
-        from a stream of messages using await syntax, this
-        only works when not passing a callback on `subscribe`::
+        next_msg can be used to retrieve the next message from a stream of messages using
+        await syntax, this only works when not passing a callback on `subscribe`::
 
             sub = await nc.subscribe('hello')
             msg = await sub.next_msg(timeout=1)
 
         """
-        future: asyncio.Future[Msg] = asyncio.Future()
+        if self._conn.is_closed:
+            raise errors.ConnectionClosedError
 
-        async def _next_msg() -> None:
-            msg = await self._pending_queue.get()
-            self._pending_size -= len(msg.data)
-            future.set_result(msg)
+        if self._cb:
+            raise errors.Error(
+                'nats: next_msg cannot be used in async subscriptions'
+            )
 
-        task = asyncio.get_running_loop().create_task(_next_msg())
+        msg = None
+        future = None
+        task_name = None
         try:
-            msg = await asyncio.wait_for(future, timeout)
+            future = asyncio.create_task(
+                asyncio.wait_for(self._pending_queue.get(), timeout)
+            )
+            task_name = future.get_name()
+            self._pending_next_msgs_calls[task_name] = future
+            msg = await future
+            self._pending_size -= len(msg.data)
             return msg
         except asyncio.TimeoutError:
-            future.cancel()
-            task.cancel()
+            if self._conn.is_closed:
+                raise errors.ConnectionClosedError
             raise errors.TimeoutError
         except asyncio.CancelledError:
-            future.cancel()
-            task.cancel()
-            # Call timeout otherwise would get an empty message.
-            raise errors.TimeoutError
+            if self._conn.is_closed:
+                raise errors.ConnectionClosedError
+            raise
+        finally:
+            if self._pending_next_msgs_calls and task_name in self._pending_next_msgs_calls:
+                del self._pending_next_msgs_calls[task_name]
+            if msg:
+                # For sync subscriptions we will consider a message
+                # to be done once it has been consumed by the client
+                # regardless of whether it has been processed.
+                self._pending_queue.task_done()
 
     def _start(self, error_cb):
         """
         Creates the resources for the subscription to start processing messages.
         """
         if self._cb:
             if not asyncio.iscoroutinefunction(self._cb) and \
@@ -227,17 +248,15 @@
             # stop waiting for messages
             self._stop_processing()
 
             # Subscription is done and won't be receiving further
             # messages so can throw it away now.
             self._conn._remove_sub(self._id)
         except asyncio.CancelledError:
-            # In case draining of a connection times out then
-            # the sub per task will be canceled as well.
-            pass
+            raise
         finally:
             self._closed = True
 
     async def unsubscribe(self, limit: int = 0):
         """
         :param limit: Max number of messages to receive before unsubscribing.
 
@@ -294,42 +313,41 @@
                     break
                 except Exception as e:
                     # All errors from calling a handler
                     # are async errors.
                     if error_cb:
                         await error_cb(e)
                 finally:
-                    # indicate the message finished processing so drain can continue
+                    # indicate the message finished processing so drain can continue.
                     self._pending_queue.task_done()
 
                 # Apply auto unsubscribe checks after having processed last msg.
                 if self._max_msgs > 0 and self._received >= self._max_msgs and self._pending_queue.empty:
                     self._stop_processing()
-
             except asyncio.CancelledError:
                 break
 
 
 class _SubscriptionMessageIterator:
 
     def __init__(self, sub: Subscription) -> None:
         self._sub: Subscription = sub
-        self._queue: "asyncio.Queue[Msg]" = sub._pending_queue
+        self._queue: asyncio.Queue[Msg] = sub._pending_queue
         self._unsubscribed_future: asyncio.Future[bool] = asyncio.Future()
 
     def _cancel(self) -> None:
         if not self._unsubscribed_future.done():
             self._unsubscribed_future.set_result(True)
 
-    def __aiter__(self) -> "_SubscriptionMessageIterator":
+    def __aiter__(self) -> _SubscriptionMessageIterator:
         return self
 
     async def __anext__(self) -> Msg:
         get_task = asyncio.get_running_loop().create_task(self._queue.get())
-        tasks: List[asyncio.Future] = [get_task, self._unsubscribed_future]
+        tasks: list[asyncio.Future] = [get_task, self._unsubscribed_future]
         finished, _ = await asyncio.wait(
             tasks, return_when=asyncio.FIRST_COMPLETED
         )
         sub = self._sub
 
         if get_task in finished:
             self._queue.task_done()
```

### Comparing `nats-py-2.2.0/nats/aio/transport.py` & `nats-py-2.3.0/nats/aio/transport.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from __future__ import annotations
+
 import abc
 import asyncio
-import sys
 import ssl
-from typing import Optional, Union, List
-from nats import errors
 from urllib.parse import ParseResult
+
 try:
     import aiohttp
 except ImportError:
-    aiohttp = None
+    aiohttp = None  # type: ignore[assignment]
+
+from nats.errors import ProtocolError
 
 
 class Transport(abc.ABC):
 
     @abc.abstractmethod
     async def connect(
         self, uri: ParseResult, buffer_size: int, connect_timeout: int
@@ -22,15 +24,15 @@
         obtained calling urllib.parse.urlparse.
         """
         pass
 
     @abc.abstractmethod
     async def connect_tls(
         self,
-        uri: Union[str, ParseResult],
+        uri: str | ParseResult,
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
     ):
         """
         connect_tls is similar to connect except it tries to connect to a secure endpoint, using the provided ssl
         context. The uri can be provided as string in case the hostname differs from the uri hostname, in case it
@@ -42,15 +44,15 @@
     def write(self, payload: bytes):
         """
         Write bytes to underlying transport. Needs a call to drain() to be successfully written.
         """
         pass
 
     @abc.abstractmethod
-    def writelines(self, payload: List[bytes]):
+    def writelines(self, payload: list[bytes]):
         """
         Writes a list of bytes, one by one, to the underlying transport. Needs a call to drain() to be successfully
         written.
         """
         pass
 
     @abc.abstractmethod
@@ -103,18 +105,18 @@
         """
         pass
 
 
 class TcpTransport(Transport):
 
     def __init__(self):
-        self._bare_io_reader: Optional[asyncio.StreamReader] = None
-        self._io_reader: Optional[asyncio.StreamReader] = None
-        self._bare_io_writer: Optional[asyncio.StreamWriter] = None
-        self._io_writer: Optional[asyncio.StreamWriter] = None
+        self._bare_io_reader: asyncio.StreamReader | None = None
+        self._io_reader: asyncio.StreamReader | None = None
+        self._bare_io_writer: asyncio.StreamWriter | None = None
+        self._io_writer: asyncio.StreamWriter | None = None
 
     async def connect(
         self, uri: ParseResult, buffer_size: int, connect_timeout: int
     ):
         r, w = await asyncio.wait_for(
             asyncio.open_connection(
                 host=uri.hostname,
@@ -130,64 +132,45 @@
         #
         # See https://github.com/nats-io/asyncio-nats/issues/43
         self._bare_io_reader = self._io_reader = r
         self._bare_io_writer = self._io_writer = w
 
     async def connect_tls(
         self,
-        uri: Union[str, ParseResult],
+        uri: str | ParseResult,
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
-    ):
-        # loop.start_tls was introduced in python 3.7
-        # the previous method is removed in 3.9
-        if sys.version_info.minor >= 7:
-            # manually recreate the stream reader/writer with a tls upgraded transport
-            reader = asyncio.StreamReader()
-            protocol = asyncio.StreamReaderProtocol(reader)
-            transport_future = asyncio.get_running_loop().start_tls(
-                self._io_writer.transport,
-                protocol,
-                ssl_context,
-                # hostname here will be passed directly as string
-                server_hostname=uri if isinstance(uri, str) else uri.hostname
-            )
-            transport = await asyncio.wait_for(
-                transport_future, connect_timeout
-            )
-            writer = asyncio.StreamWriter(
-                transport, protocol, reader, asyncio.get_running_loop()
-            )
-            self._io_reader, self._io_writer = reader, writer
-        else:
-            transport = self._io_writer.transport
-            sock = transport.get_extra_info('socket')
-            if not sock:
-                # This shouldn't happen
-                raise errors.Error('nats: unable to get socket')
+    ) -> None:
+        assert self._io_writer, f'{type(self).__name__}.connect must be called first'
 
-            connection_future = asyncio.open_connection(
-                limit=buffer_size,
-                sock=sock,
-                ssl=ssl_context,
-                # hostname here will be passed directly as string
-                server_hostname=uri if isinstance(uri, str) else uri.hostname,
-            )
-            self._io_reader, self._io_writer = await asyncio.wait_for(
-                connection_future, connect_timeout
-            )
+        # manually recreate the stream reader/writer with a tls upgraded transport
+        reader = asyncio.StreamReader()
+        protocol = asyncio.StreamReaderProtocol(reader)
+        transport_future = asyncio.get_running_loop().start_tls(
+            self._io_writer.transport,
+            protocol,
+            ssl_context,
+            # hostname here will be passed directly as string
+            server_hostname=uri if isinstance(uri, str) else uri.hostname
+        )
+        transport = await asyncio.wait_for(transport_future, connect_timeout)
+        writer = asyncio.StreamWriter(
+            transport, protocol, reader, asyncio.get_running_loop()
+        )
+        self._io_reader, self._io_writer = reader, writer
 
     def write(self, payload):
         return self._io_writer.write(payload)
 
     def writelines(self, payload):
         return self._io_writer.writelines(payload)
 
     async def read(self, buffer_size: int):
+        assert self._io_reader, f'{type(self).__name__}.connect must be called first'
         return await self._io_reader.read(buffer_size)
 
     async def readline(self):
         return await self._io_reader.readline()
 
     async def drain(self):
         return await self._io_writer.drain()
@@ -208,52 +191,63 @@
 class WebSocketTransport(Transport):
 
     def __init__(self):
         if not aiohttp:
             raise ImportError(
                 "Could not import aiohttp transport, please install it with `pip install aiohttp`"
             )
-        self._ws: Optional[aiohttp.ClientWebSocketResponse] = None
-        self._client: Optional[aiohttp.ClientSession] = aiohttp.ClientSession()
+        self._ws: aiohttp.ClientWebSocketResponse | None = None
+        self._client: aiohttp.ClientSession = aiohttp.ClientSession()
         self._pending = asyncio.Queue()
         self._close_task = asyncio.Future()
+        self._using_tls: bool | None = None
 
     async def connect(
         self, uri: ParseResult, buffer_size: int, connect_timeout: int
     ):
         # for websocket library, the uri must contain the scheme already
         self._ws = await self._client.ws_connect(
             uri.geturl(), timeout=connect_timeout
         )
+        self._using_tls = False
 
     async def connect_tls(
         self,
-        uri: Union[str, ParseResult],
+        uri: str | ParseResult,
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
     ):
+        if self._ws and not self._ws.closed:
+            if self._using_tls:
+                return
+            raise ProtocolError("ws: cannot upgrade to TLS")
+
         self._ws = await self._client.ws_connect(
             uri if isinstance(uri, str) else uri.geturl(),
             ssl=ssl_context,
             timeout=connect_timeout
         )
+        self._using_tls = True
 
     def write(self, payload):
         self._pending.put_nowait(payload)
 
     def writelines(self, payload):
         for message in payload:
             self.write(message)
 
     async def read(self, buffer_size: int):
         return await self.readline()
 
     async def readline(self):
         data = await self._ws.receive()
+        if data.type == aiohttp.WSMsgType.CLOSE:
+            # if the connection terminated abruptly, return empty binary data to raise unexpected EOF
+            return b''
         return data.data
 
     async def drain(self):
         # send all the messages pending
         while not self._pending.empty():
             message = self._pending.get_nowait()
             await self._ws.send_bytes(message)
@@ -263,11 +257,11 @@
         await self._client.close()
         self._ws = self._client = None
 
     def close(self):
         self._close_task = asyncio.create_task(self._ws.close())
 
     def at_eof(self):
-        return self._ws._reader.at_eof()
+        return self._ws.closed
 
     def __bool__(self):
-        return bool(self._ws)
+        return bool(self._client)
```

### Comparing `nats-py-2.2.0/nats/errors.py` & `nats-py-2.3.0/nats/errors.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.2.0/nats/js/__init__.py` & `nats-py-2.3.0/nats/js/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 from . import api
 from .client import JetStreamContext
 from .manager import JetStreamManager
 
 __all__ = ["api", "JetStreamManager", "JetStreamContext"]
```

### Comparing `nats-py-2.2.0/nats/js/api.py` & `nats-py-2.3.0/nats/js/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 from dataclasses import dataclass, fields, replace
 from enum import Enum
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, Dict, Optional, TypeVar
 
 _NANOSECOND = 10**9
 
 
 class Header(str, Enum):
     CONSUMER_STALLED = "Nats-Consumer-Stalled"
     DESCRIPTION = "Description"
@@ -51,45 +53,45 @@
 @dataclass
 class Base:
     """
     Helper dataclass to filter unknown fields from the API.
     """
 
     @staticmethod
-    def _convert(resp: Dict[str, Any], field: str, type: Type["Base"]) -> None:
+    def _convert(resp: dict[str, Any], field: str, type: type[Base]) -> None:
         """Convert the field into the given type in place.
         """
         data = resp.get(field, None)
         if data is None:
             resp[field] = None
         elif isinstance(data, list):
             resp[field] = [type.from_response(item) for item in data]
         else:
             resp[field] = type.from_response(data)
 
     @staticmethod
-    def _convert_nanoseconds(resp: Dict[str, Any], field: str) -> None:
+    def _convert_nanoseconds(resp: dict[str, Any], field: str) -> None:
         """Convert the given field from nanoseconds to seconds in place.
         """
         val = resp.get(field, None)
         if val is not None:
             val = val / _NANOSECOND
         resp[field] = val
 
     @staticmethod
-    def _to_nanoseconds(val: Optional[float]) -> Optional[int]:
+    def _to_nanoseconds(val: float | None) -> int | None:
         """Convert the value from seconds to nanoseconds.
         """
         if val is None:
             # We use 0 to avoid sending null to Go servers.
             return 0
         return int(val * _NANOSECOND)
 
     @classmethod
-    def from_response(cls: Type[_B], resp: Dict[str, Any]) -> _B:
+    def from_response(cls: type[_B], resp: dict[str, Any]) -> _B:
         """Read the class instance from a server response.
 
         Unknown fields are ignored ("open-world assumption").
         """
         params = {}
         for field in fields(cls):
             if field.name in resp:
@@ -97,15 +99,15 @@
         return cls(**params)
 
     def evolve(self: _B, **params) -> _B:
         """Return a copy of the instance with the passed values replaced.
         """
         return replace(self, **params)
 
-    def as_dict(self) -> Dict[str, object]:
+    def as_dict(self) -> dict[str, object]:
         """Return the object converted into an API-friendly dict.
         """
         result = {}
         for field in fields(self):
             val = getattr(self, field.name)
             if val is None:
                 continue
@@ -118,74 +120,74 @@
 @dataclass
 class PubAck(Base):
     """
     PubAck is the response of publishing a message to JetStream.
     """
     stream: str
     seq: int
-    domain: Optional[str] = None
-    duplicate: Optional[bool] = None
+    domain: str | None = None
+    duplicate: bool | None = None
 
 
 @dataclass
 class Placement(Base):
     """Placement directives to consider when placing replicas of this stream"""
 
-    cluster: Optional[str] = None
-    tags: Optional[List[str]] = None
+    cluster: str | None = None
+    tags: list[str] | None = None
 
 
 @dataclass
 class ExternalStream(Base):
     api: str
-    deliver: Optional[str] = None
+    deliver: str | None = None
 
 
 @dataclass
 class StreamSource(Base):
     name: str
-    opt_start_seq: Optional[int] = None
+    opt_start_seq: int | None = None
     # FIXME: Handle time type, omit for now.
     # opt_start_time: Optional[str] = None
-    filter_subject: Optional[str] = None
-    external: Optional[ExternalStream] = None
+    filter_subject: str | None = None
+    external: ExternalStream | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'external', ExternalStream)
         return super().from_response(resp)
 
 
 @dataclass
 class StreamSourceInfo(Base):
     name: str
-    lag: Optional[int] = None
-    active: Optional[int] = None
-    error: Optional[Dict[str, Any]] = None
+    lag: int | None = None
+    active: int | None = None
+    error: dict[str, Any] | None = None
 
 
 @dataclass
 class LostStreamData(Base):
-    msgs: Optional[List[int]] = None
-    bytes: Optional[int] = None
+    msgs: list[int] | None = None
+    bytes: int | None = None
 
 
 @dataclass
 class StreamState(Base):
     messages: int
     bytes: int
     first_seq: int
     last_seq: int
     consumer_count: int
-    deleted: Optional[List[int]] = None
-    num_deleted: Optional[int] = None
-    lost: Optional[LostStreamData] = None
+    deleted: list[int] | None = None
+    num_deleted: int | None = None
+    lost: LostStreamData | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'lost', LostStreamData)
         return super().from_response(resp)
 
 
 class RetentionPolicy(str, Enum):
     """How message retention is considered"""
 
@@ -210,110 +212,111 @@
 
 @dataclass
 class RePublish(Base):
     """
     RePublish is for republishing messages once committed to a stream. The original
     subject cis remapped from the subject pattern to the destination pattern.
     """
-    src: Optional[str] = None
-    dest: Optional[str] = None
-    headers_only: Optional[bool] = None
+    src: str | None = None
+    dest: str | None = None
+    headers_only: bool | None = None
 
 
 @dataclass
 class StreamConfig(Base):
     """
     StreamConfig represents the configuration of a stream.
     """
-    name: Optional[str] = None
-    description: Optional[str] = None
-    subjects: Optional[List[str]] = None
-    retention: Optional[RetentionPolicy] = None
-    max_consumers: Optional[int] = None
-    max_msgs: Optional[int] = None
-    max_bytes: Optional[int] = None
-    discard: Optional[DiscardPolicy] = DiscardPolicy.OLD
-    max_age: Optional[float] = None  # in seconds
+    name: str | None = None
+    description: str | None = None
+    subjects: list[str] | None = None
+    retention: RetentionPolicy | None = None
+    max_consumers: int | None = None
+    max_msgs: int | None = None
+    max_bytes: int | None = None
+    discard: DiscardPolicy | None = DiscardPolicy.OLD
+    max_age: float | None = None  # in seconds
     max_msgs_per_subject: int = -1
-    max_msg_size: Optional[int] = -1
-    storage: Optional[StorageType] = None
-    num_replicas: Optional[int] = None
+    max_msg_size: int | None = -1
+    storage: StorageType | None = None
+    num_replicas: int | None = None
     no_ack: bool = False
-    template_owner: Optional[str] = None
-    duplicate_window: int = 0
-    placement: Optional[Placement] = None
-    mirror: Optional[StreamSource] = None
-    sources: Optional[List[StreamSource]] = None
+    template_owner: str | None = None
+    duplicate_window: float = 0
+    placement: Placement | None = None
+    mirror: StreamSource | None = None
+    sources: list[StreamSource] | None = None
     sealed: bool = False
     deny_delete: bool = False
     deny_purge: bool = False
     allow_rollup_hdrs: bool = False
 
     # Allow republish of the message after being sequenced and stored.
-    republish: Optional[RePublish] = None
+    republish: RePublish | None = None
 
     # Allow higher performance, direct access to get individual messages. E.g. KeyValue
-    allow_direct: Optional[bool] = None
+    allow_direct: bool | None = None
 
     # Allow higher performance and unified direct access for mirrors as well.
-    mirror_direct: Optional[bool] = None
+    mirror_direct: bool | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert_nanoseconds(resp, 'max_age')
         cls._convert_nanoseconds(resp, 'duplicate_window')
         cls._convert(resp, 'placement', Placement)
         cls._convert(resp, 'mirror', StreamSource)
         cls._convert(resp, 'sources', StreamSource)
+        cls._convert(resp, 'republish', RePublish)
         return super().from_response(resp)
 
-    def as_dict(self) -> Dict[str, object]:
+    def as_dict(self) -> dict[str, object]:
         result = super().as_dict()
         result['duplicate_window'] = self._to_nanoseconds(
             self.duplicate_window
         )
         result['max_age'] = self._to_nanoseconds(self.max_age)
         return result
 
 
 @dataclass
 class PeerInfo(Base):
-    name: Optional[str] = None
-    current: Optional[bool] = None
-    offline: Optional[bool] = None
-    active: Optional[int] = None
-    lag: Optional[int] = None
+    name: str | None = None
+    current: bool | None = None
+    offline: bool | None = None
+    active: int | None = None
+    lag: int | None = None
 
 
 @dataclass
 class ClusterInfo(Base):
-    leader: Optional[str] = None
-    name: Optional[str] = None
-    replicas: Optional[List[PeerInfo]] = None
+    leader: str | None = None
+    name: str | None = None
+    replicas: list[PeerInfo] | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'replicas', PeerInfo)
         return super().from_response(resp)
 
 
 @dataclass
 class StreamInfo(Base):
     """
     StreamInfo is the latest information about a stream from JetStream.
     """
     config: StreamConfig
     state: StreamState
-    mirror: Optional[StreamSourceInfo] = None
-    sources: Optional[List[StreamSourceInfo]] = None
-    cluster: Optional[ClusterInfo] = None
-    did_create: Optional[bool] = None
+    mirror: StreamSourceInfo | None = None
+    sources: list[StreamSourceInfo] | None = None
+    cluster: ClusterInfo | None = None
+    did_create: bool | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'config', StreamConfig)
         cls._convert(resp, 'state', StreamState)
         cls._convert(resp, 'mirror', StreamSourceInfo)
         cls._convert(resp, 'sources', StreamSourceInfo)
         cls._convert(resp, 'cluster', ClusterInfo)
         return super().from_response(resp)
 
@@ -367,55 +370,55 @@
 @dataclass
 class ConsumerConfig(Base):
     """Consumer configuration.
 
     References:
         * `Consumers <https://docs.nats.io/jetstream/concepts/consumers>`_
     """
-    name: Optional[str] = None
-    durable_name: Optional[str] = None
-    description: Optional[str] = None
-    deliver_policy: Optional[DeliverPolicy] = DeliverPolicy.ALL
-    opt_start_seq: Optional[int] = None
-    opt_start_time: Optional[int] = None
-    ack_policy: Optional[AckPolicy] = AckPolicy.EXPLICIT
-    ack_wait: Optional[float] = None  # in seconds
-    max_deliver: Optional[int] = None
-    filter_subject: Optional[str] = None
-    replay_policy: Optional[ReplayPolicy] = ReplayPolicy.INSTANT
-    rate_limit_bps: Optional[int] = None
-    sample_freq: Optional[str] = None
-    max_waiting: Optional[int] = None
-    max_ack_pending: Optional[int] = None
-    flow_control: Optional[bool] = None
-    idle_heartbeat: Optional[float] = None
-    headers_only: Optional[bool] = None
+    name: str | None = None
+    durable_name: str | None = None
+    description: str | None = None
+    deliver_policy: DeliverPolicy | None = DeliverPolicy.ALL
+    opt_start_seq: int | None = None
+    opt_start_time: int | None = None
+    ack_policy: AckPolicy | None = AckPolicy.EXPLICIT
+    ack_wait: float | None = None  # in seconds
+    max_deliver: int | None = None
+    filter_subject: str | None = None
+    replay_policy: ReplayPolicy | None = ReplayPolicy.INSTANT
+    rate_limit_bps: int | None = None
+    sample_freq: str | None = None
+    max_waiting: int | None = None
+    max_ack_pending: int | None = None
+    flow_control: bool | None = None
+    idle_heartbeat: float | None = None
+    headers_only: bool | None = None
 
     # Push based consumers.
-    deliver_subject: Optional[str] = None
-    deliver_group: Optional[str] = None
+    deliver_subject: str | None = None
+    deliver_group: str | None = None
 
     # Ephemeral inactivity threshold
-    inactive_threshold: Optional[float] = None  # in seconds
+    inactive_threshold: float | None = None  # in seconds
 
     # Generally inherited by parent stream and other markers, now can
     # be configured directly.
-    num_replicas: Optional[int] = None
+    num_replicas: int | None = None
 
     # Force memory storage.
-    mem_storage: Optional[bool] = None
+    mem_storage: bool | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert_nanoseconds(resp, 'ack_wait')
         cls._convert_nanoseconds(resp, 'idle_heartbeat')
         cls._convert_nanoseconds(resp, 'inactive_threshold')
         return super().from_response(resp)
 
-    def as_dict(self) -> Dict[str, object]:
+    def as_dict(self) -> dict[str, object]:
         result = super().as_dict()
         result['ack_wait'] = self._to_nanoseconds(self.ack_wait)
         result['idle_heartbeat'] = self._to_nanoseconds(self.idle_heartbeat)
         result['inactive_threshold'] = self._to_nanoseconds(
             self.inactive_threshold
         )
         return result
@@ -435,25 +438,25 @@
     ConsumerInfo represents the info about the consumer.
     """
     name: str
     stream_name: str
     config: ConsumerConfig
     # FIXME: Do not handle dates for now.
     # created: datetime
-    delivered: Optional[SequenceInfo] = None
-    ack_floor: Optional[SequenceInfo] = None
-    num_ack_pending: Optional[int] = None
-    num_redelivered: Optional[int] = None
-    num_waiting: Optional[int] = None
-    num_pending: Optional[int] = None
-    cluster: Optional[ClusterInfo] = None
-    push_bound: Optional[bool] = None
+    delivered: SequenceInfo | None = None
+    ack_floor: SequenceInfo | None = None
+    num_ack_pending: int | None = None
+    num_redelivered: int | None = None
+    num_waiting: int | None = None
+    num_pending: int | None = None
+    cluster: ClusterInfo | None = None
+    push_bound: bool | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'delivered', SequenceInfo)
         cls._convert(resp, 'ack_floor', SequenceInfo)
         cls._convert(resp, 'config', ConsumerConfig)
         cls._convert(resp, 'cluster', ClusterInfo)
         return super().from_response(resp)
 
 
@@ -480,15 +483,15 @@
     memory: int
     storage: int
     streams: int
     consumers: int
     limits: AccountLimits
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'limits', AccountLimits)
         return super().from_response(resp)
 
 
 @dataclass
 class APIStats(Base):
     """API stats"""
@@ -508,67 +511,181 @@
     memory: int
     storage: int
     streams: int
     consumers: int
     limits: AccountLimits
 
     api: APIStats
-    domain: Optional[str] = None
-    tiers: Optional[Dict[str, Tier]] = None
+    domain: str | None = None
+    tiers: dict[str, Tier] | None = None
 
     @classmethod
-    def from_response(cls, resp: Dict[str, Any]):
+    def from_response(cls, resp: dict[str, Any]):
         cls._convert(resp, 'limits', AccountLimits)
         cls._convert(resp, 'api', APIStats)
         info = super().from_response(resp)
         tiers = resp.get('tiers', None)
         if tiers:
             result = {}
             for k, v in tiers.items():
                 result[k] = Tier.from_response(v)
             info.tiers = result
         return info
 
 
 @dataclass
 class RawStreamMsg(Base):
-    subject: Optional[str] = None
-    seq: Optional[int] = None
-    data: Optional[bytes] = None
-    hdrs: Optional[bytes] = None
-    headers: Optional[dict] = None
-    stream: Optional[str] = None
+    subject: str | None = None
+    seq: int | None = None
+    data: bytes | None = None
+    hdrs: bytes | None = None
+    headers: dict | None = None
+    stream: str | None = None
     # TODO: Add 'time'
 
     @property
-    def sequence(self) -> Optional[int]:
+    def sequence(self) -> int | None:
         return self.seq
 
     @property
-    def header(self) -> Optional[dict]:
+    def header(self) -> dict | None:
         """
         header returns the headers from a message.
         """
         return self.headers
 
 
 @dataclass
 class KeyValueConfig(Base):
     """
     KeyValueConfig is the configuration of a KeyValue store.
     """
     bucket: str
-    description: Optional[str] = None
-    max_value_size: Optional[int] = None
+    description: str | None = None
+    max_value_size: int | None = None
     history: int = 1
-    ttl: Optional[float] = None  # in seconds
+    ttl: float | None = None  # in seconds
+    max_bytes: int | None = None
+    storage: StorageType | None = None
+    replicas: int = 1
+    placement: Placement | None = None
+    republish: RePublish | None = None
+    direct: bool | None = None
+
+    def as_dict(self) -> dict[str, object]:
+        result = super().as_dict()
+        result['ttl'] = self._to_nanoseconds(self.ttl)
+        return result
+
+
+@dataclass
+class StreamPurgeRequest(Base):
+    """
+    StreamPurgeRequest is optional request information to the purge API.
+    """
+    # Purge up to but not including sequence.
+    seq: Optional[int] = None
+    # Subject to match against messages for the purge command.
+    filter: Optional[str] = None
+    # Number of messages to keep.
+    keep: Optional[int] = None
+
+
+@dataclass
+class ObjectStoreConfig(Base):
+    """
+    ObjectStoreConfig is the configurigation of an ObjectStore.
+    """
+    bucket: Optional[str] = None
+    description: Optional[str] = None
+    ttl: Optional[float] = None
     max_bytes: Optional[int] = None
     storage: Optional[StorageType] = None
     replicas: int = 1
     placement: Optional[Placement] = None
-    republish: Optional[RePublish] = None
-    direct: Optional[bool] = None
 
     def as_dict(self) -> Dict[str, object]:
         result = super().as_dict()
         result['ttl'] = self._to_nanoseconds(self.ttl)
         return result
+
+
+@dataclass
+class ObjectLink(Base):
+    """
+    ObjectLink is used to embed links to other buckets and objects.
+    """
+    # Bucket is the name of the other object store.
+    bucket: str
+    #  Name can be used to link to a single object.
+    # If empty means this is a link to the whole store, like a directory.
+    name: Optional[str] = None
+
+    @classmethod
+    def from_response(cls, resp: Dict[str, Any]):
+        return super().from_response(resp)
+
+
+@dataclass
+class ObjectMetaOptions(Base):
+    link: Optional[ObjectLink] = None
+    max_chunk_size: Optional[int] = None
+
+    @classmethod
+    def from_response(cls, resp: Dict[str, Any]):
+        cls._convert(resp, 'link', ObjectLink)
+        return super().from_response(resp)
+
+
+@dataclass
+class ObjectMeta(Base):
+    """
+    ObjectMeta is high level information about an object.
+    """
+    name: Optional[str] = None
+    description: Optional[str] = None
+    headers: Optional[dict] = None
+    #  Optional options.
+    options: Optional[ObjectMetaOptions] = None
+
+    @classmethod
+    def from_response(cls, resp: Dict[str, Any]):
+        cls._convert(resp, 'options', ObjectMetaOptions)
+        return super().from_response(resp)
+
+
+@dataclass
+class ObjectInfo(Base):
+    """
+    ObjectInfo is meta plus instance information.
+    """
+    name: str
+    bucket: str
+    nuid: str
+    size: Optional[int] = None
+    mtime: Optional[str] = None
+    chunks: Optional[int] = None
+    digest: Optional[str] = None
+    deleted: Optional[bool] = False
+    description: Optional[str] = None
+    headers: Optional[dict] = None
+    #  Optional options.
+    options: Optional[ObjectMetaOptions] = None
+    # NOTE: name, description, headers, options together compose
+    # what would be the ObjectMeta embedded type in Go.
+
+    @property
+    def meta(self) -> ObjectMeta:
+        return ObjectMeta(
+            name=self.name,
+            description=self.description,
+            headers=self.headers,
+            options=self.options,
+        )
+
+    def is_link(self) -> bool:
+        return self.options is not None and self.options.link is not None
+
+    @classmethod
+    def from_response(cls, resp: Dict[str, Any]):
+        cls._convert(resp, 'options', ObjectMetaOptions)
+        return super().from_response(resp)
```

### Comparing `nats-py-2.2.0/nats/js/client.py` & `nats-py-2.3.0/nats/js/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 import asyncio
 import json
 import time
-from typing import TYPE_CHECKING, Awaitable, Callable, List, Optional
 from email.parser import BytesParser
+from typing import TYPE_CHECKING, Awaitable, Callable, Optional
 
 import nats.errors
 import nats.js.errors
 from nats.aio.msg import Msg
 from nats.aio.subscription import Subscription
 from nats.js import api
-from nats.js.errors import BadBucketError, BucketNotFoundError, NotFoundError
+from nats.js.errors import BadBucketError, BucketNotFoundError, InvalidBucketNameError, NotFoundError
 from nats.js.kv import KeyValue
 from nats.js.manager import JetStreamManager
+from nats.js.object_store import (
+    VALID_BUCKET_RE, OBJ_ALL_CHUNKS_PRE_TEMPLATE, OBJ_ALL_META_PRE_TEMPLATE,
+    OBJ_STREAM_TEMPLATE, ObjectStore
+)
 
 if TYPE_CHECKING:
     from nats import NATS
 
 NATS_HDR_LINE = bytearray(b'NATS/1.0')
 NATS_HDR_LINE_SIZE = len(NATS_HDR_LINE)
 _CRLF_ = b'\r\n'
@@ -73,17 +79,17 @@
         if __name__ == '__main__':
             asyncio.run(main())
 
     """
 
     def __init__(
         self,
-        conn: "NATS",
+        conn: NATS,
         prefix: str = api.DEFAULT_PREFIX,
-        domain: Optional[str] = None,
+        domain: str | None = None,
         timeout: float = 5,
     ) -> None:
         self._prefix = prefix
         if domain is not None:
             self._prefix = f"$JS.{domain}.API"
         self._nc = conn
         self._timeout = timeout
@@ -97,17 +103,17 @@
             timeout=self._timeout,
         )
 
     async def publish(
         self,
         subject: str,
         payload: bytes = b'',
-        timeout: float = None,
-        stream: str = None,
-        headers: dict = None
+        timeout: float | None = None,
+        stream: str | None = None,
+        headers: dict | None = None
     ) -> api.PubAck:
         """
         publish emits a new message to JetStream.
         """
         hdr = headers
         if timeout is None:
             timeout = self._timeout
@@ -129,29 +135,28 @@
         if 'error' in resp:
             raise nats.js.errors.APIError.from_error(resp['error'])
         return api.PubAck.from_response(resp)
 
     async def subscribe(
         self,
         subject: str,
-        queue: Optional[str] = None,
-        cb: Optional[Callback] = None,
-        durable: Optional[str] = None,
-        stream: Optional[str] = None,
-        config: Optional[api.ConsumerConfig] = None,
+        queue: str | None = None,
+        cb: Callback | None = None,
+        durable: str | None = None,
+        stream: str | None = None,
+        config: api.ConsumerConfig | None = None,
         manual_ack: bool = False,
         ordered_consumer: bool = False,
-        idle_heartbeat: Optional[float] = None,
+        idle_heartbeat: float | None = None,
         flow_control: bool = False,
-        pending_msgs_limit: Optional[int] = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-        pending_bytes_limit: Optional[int
-                                      ] = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-        deliver_policy: Optional[api.DeliverPolicy] = None,
-        headers_only: Optional[bool] = None,
-    ) -> Subscription:
+        pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+        pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+        deliver_policy: api.DeliverPolicy | None = None,
+        headers_only: bool | None = None,
+    ) -> PushSubscription:
         """Create consumer if needed and push-subscribe to it.
 
         1. Check if consumer exists.
         2. Creates consumer if needed.
         3. Calls `subscribe_bind`.
 
         :param subject: Subject from a stream from JetStream.
@@ -287,15 +292,15 @@
             if ordered_consumer:
                 config.flow_control = True
                 config.ack_policy = api.AckPolicy.NONE
                 config.max_deliver = 1
                 config.ack_wait = 22 * 3600  # 22 hours
                 config.idle_heartbeat = idle_heartbeat
                 config.num_replicas = 1
-                config.memory_storage = True
+                config.mem_storage = True
 
             consumer_info = await self._jsm.add_consumer(stream, config=config)
             consumer = consumer_info.name
 
         if consumer is None:
             raise TypeError("cannot detect consumer")
         if config is None:
@@ -312,21 +317,20 @@
         )
 
     async def subscribe_bind(
         self,
         stream: str,
         config: api.ConsumerConfig,
         consumer: str,
-        cb: Optional[Callback] = None,
+        cb: Callback | None = None,
         manual_ack: bool = False,
         ordered_consumer: bool = False,
-        pending_msgs_limit: Optional[int] = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-        pending_bytes_limit: Optional[int
-                                      ] = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    ) -> Subscription:
+        pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+        pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+    ) -> PushSubscription:
         """Push-subscribe to an existing consumer.
         """
         # By default, async subscribers wrap the original callback and
         # auto ack the messages as they are delivered.
         #
         # In case ack policy is none then we also do not require to ack.
         #
@@ -368,20 +372,20 @@
 
         return new_callback
 
     async def pull_subscribe(
         self,
         subject: str,
         durable: str,
-        stream: Optional[str] = None,
-        config: Optional[api.ConsumerConfig] = None,
-        pending_msgs_limit: Optional[int] = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-        pending_bytes_limit: Optional[int
-                                      ] = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    ) -> "JetStreamContext.PullSubscription":
+        stream: str | None = None,
+        config: api.ConsumerConfig | None = None,
+        pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+        pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+        inbox_prefix: bytes = api.INBOX_PREFIX,
+    ) -> JetStreamContext.PullSubscription:
         """Create consumer and pull subscription.
 
         1. Find stream name by subject if `stream` is not passed.
         2. Create consumer with the given `config` if not created.
         3. Call `pull_subscribe_bind`.
 
         ::
@@ -420,27 +424,27 @@
             config.filter_subject = subject
             config.durable_name = durable
             await self._jsm.add_consumer(stream, config=config)
 
         return await self.pull_subscribe_bind(
             durable=durable,
             stream=stream,
+            inbox_prefix=inbox_prefix,
             pending_bytes_limit=pending_bytes_limit,
             pending_msgs_limit=pending_msgs_limit,
         )
 
     async def pull_subscribe_bind(
         self,
         durable: str,
         stream: str,
         inbox_prefix: bytes = api.INBOX_PREFIX,
-        pending_msgs_limit: Optional[int] = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-        pending_bytes_limit: Optional[int
-                                      ] = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    ) -> "JetStreamContext.PullSubscription":
+        pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+        pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+    ) -> JetStreamContext.PullSubscription:
         """
         pull_subscribe returns a `PullSubscription` that can be delivered messages
         from a JetStream pull based consumer by calling `sub.fetch`.
 
         ::
 
             import asyncio
@@ -474,78 +478,78 @@
             sub=sub,
             stream=stream,
             consumer=durable,
             deliver=deliver,
         )
 
     @classmethod
-    def is_status_msg(cls, msg: Optional[Msg]) -> Optional[str]:
+    def is_status_msg(cls, msg: Msg | None) -> str | None:
         if msg is None or msg.headers is None:
             return None
         return msg.headers.get(api.Header.STATUS)
 
     @classmethod
-    def _is_processable_msg(cls, status: Optional[str], msg: Msg) -> bool:
+    def _is_processable_msg(cls, status: str | None, msg: Msg) -> bool:
         if not status:
             return True
         # Skip most 4XX errors and do not raise exception.
         if JetStreamContext._is_temporary_error(status):
             return False
         raise nats.js.errors.APIError.from_msg(msg)
 
     @classmethod
-    def _is_temporary_error(cls, status: Optional[str]) -> bool:
+    def _is_temporary_error(cls, status: str | None) -> bool:
         if status == api.StatusCode.NO_MESSAGES or status == api.StatusCode.CONFLICT \
            or status == api.StatusCode.REQUEST_TIMEOUT:
             return True
         else:
             return False
 
     @classmethod
-    def _time_until(cls, timeout: Optional[float],
-                    start_time: float) -> Optional[float]:
+    def _time_until(
+        cls, timeout: float | None, start_time: float
+    ) -> float | None:
         if timeout is None:
             return None
         return timeout - (time.monotonic() - start_time)
 
     class _JSI():
 
         def __init__(
             self,
-            js: "JetStreamContext",
-            conn: "NATS",
+            js: JetStreamContext,
+            conn: NATS,
             stream: str,
-            ordered: Optional[bool],
-            psub: "JetStreamContext.PushSubscription",
+            ordered: bool | None,
+            psub: JetStreamContext.PushSubscription,
             sub: Subscription,
             ccreq: api.ConsumerConfig,
         ) -> None:
             self._conn = conn
             self._js = js
             self._stream = stream
             self._ordered = ordered
             self._psub = psub
             self._sub = sub
             self._ccreq = ccreq
 
             self._dseq = 1
             self._sseq = 0
-            self._cmeta: Optional[str] = None
+            self._cmeta: str | None = None
             self._fciseq = 0
-            self._active: Optional[bool] = None
+            self._active: bool | None = None
 
         def track_sequences(self, reply: str) -> None:
             self._fciseq += 1
             self._cmeta = reply
 
         def schedule_flow_control_response(self, reply: str) -> None:
             pass
 
-        async def check_for_sequence_mismatch(self,
-                                              msg: Msg) -> Optional[bool]:
+        async def check_for_sequence_mismatch(self, msg: Msg) -> bool | None:
             self._active = True
             if not self._cmeta:
                 return None
 
             tokens = msg._get_metadata_fields(self._cmeta)
             dseq = int(tokens[6])  # consumer sequence
             ldseq = None
@@ -564,19 +568,18 @@
                     )
                 else:
                     ecs = nats.js.errors.ConsumerSequenceMismatchError(
                         stream_resume_sequence=sseq,
                         consumer_sequence=dseq,
                         last_consumer_sequence=ldseq,
                     )
-                    if self._conn._error_cb:
-                        await self._conn._error_cb(ecs)
+                    await self._conn._error_cb(ecs)
             return did_reset
 
-        async def reset_ordered_consumer(self, sseq: Optional[int]) -> bool:
+        async def reset_ordered_consumer(self, sseq: int | None) -> bool:
             # FIXME: Handle AUTO_UNSUB called previously to this.
 
             # Replace current subscription.
             osid = self._sub._id
             self._conn._remove_sub(osid)
             new_deliver = self._conn.new_inbox()
 
@@ -629,15 +632,15 @@
     class PushSubscription(Subscription):
         """
         PushSubscription is a subscription that is delivered messages.
         """
 
         def __init__(
             self,
-            js: "JetStreamContext",
+            js: JetStreamContext,
             sub: Subscription,
             stream: str,
             consumer: str,
         ) -> None:
             self._js = js
             self._stream = stream
             self._consumer = consumer
@@ -656,14 +659,15 @@
             # Per subscription message processor.
             self._pending_msgs_limit = sub._pending_msgs_limit
             self._pending_bytes_limit = sub._pending_bytes_limit
             self._pending_queue = sub._pending_queue
             self._pending_size = sub._pending_size
             self._wait_for_msgs_task = sub._wait_for_msgs_task
             self._message_iterator = sub._message_iterator
+            self._pending_next_msgs_calls = sub._pending_next_msgs_calls
 
         async def consumer_info(self) -> api.ConsumerInfo:
             """
             consumer_info gets the current info of the consumer from this subscription.
             """
             info = await self._js._jsm.consumer_info(
                 self._stream,
@@ -681,15 +685,15 @@
     class PullSubscription:
         """
         PullSubscription is a subscription that can fetch messages.
         """
 
         def __init__(
             self,
-            js: "JetStreamContext",
+            js: JetStreamContext,
             sub: Subscription,
             stream: str,
             consumer: str,
             deliver: bytes,
         ) -> None:
             # JS/JSM context
             self._js = js
@@ -743,15 +747,15 @@
             info = await self._js._jsm.consumer_info(
                 self._stream, self._consumer
             )
             return info
 
         async def fetch(self,
                         batch: int = 1,
-                        timeout: Optional[float] = 5) -> List[Msg]:
+                        timeout: float | None = 5) -> list[Msg]:
             """
             fetch makes a request to JetStream to be delivered a set of messages.
 
             :param batch: Number of messages to fetch from server.
             :param timeout: Max duration of the fetch request before it expires.
 
             ::
@@ -791,16 +795,16 @@
                 msg = await self._fetch_one(expires, timeout)
                 return [msg]
             msgs = await self._fetch_n(batch, expires, timeout)
             return msgs
 
         async def _fetch_one(
             self,
-            expires: Optional[int],
-            timeout: Optional[float],
+            expires: int | None,
+            timeout: float | None,
         ) -> Msg:
             queue = self._sub._pending_queue
 
             # Check the next message in case there are any.
             while not queue.empty():
                 try:
                     msg = queue.get_nowait()
@@ -841,24 +845,24 @@
                     # Any other type of status message is an error.
                     raise nats.js.errors.APIError.from_msg(msg)
             return msg
 
         async def _fetch_n(
             self,
             batch: int,
-            expires: Optional[int],
-            timeout: Optional[float],
-        ) -> List[Msg]:
+            expires: int | None,
+            timeout: float | None,
+        ) -> list[Msg]:
             msgs = []
             queue = self._sub._pending_queue
             start_time = time.monotonic()
             needed = batch
 
             # Fetch as many as needed from the internal pending queue.
-            msg: Optional[Msg]
+            msg: Msg | None
 
             while not queue.empty():
                 try:
                     msg = queue.get_nowait()
                     self._sub._pending_size -= len(msg.data)
                     status = JetStreamContext.is_status_msg(msg)
                     if status:
@@ -880,16 +884,21 @@
             await self._nc.publish(
                 self._nms,
                 json.dumps(next_req).encode(),
                 self._deliver,
             )
             await asyncio.sleep(0)
 
-            # Wait for first message or timeout.
-            msg = await self._sub.next_msg(timeout)
+            try:
+                msg = await self._sub.next_msg(timeout)
+            except asyncio.TimeoutError:
+                if msgs:
+                    return msgs
+                raise
+
             status = JetStreamContext.is_status_msg(msg)
             if JetStreamContext._is_processable_msg(status, msg):
                 # First processable message received, do not raise error from now.
                 msgs.append(msg)
                 needed -= 1
 
                 try:
@@ -987,43 +996,50 @@
     ######################
     #                    #
     # KeyValue Context   #
     #                    #
     ######################
 
     async def key_value(self, bucket: str) -> KeyValue:
+        if VALID_BUCKET_RE.match(bucket) is None:
+            raise InvalidBucketNameError
+
         stream = KV_STREAM_TEMPLATE.format(bucket=bucket)
         try:
             si = await self.stream_info(stream)
         except NotFoundError:
             raise BucketNotFoundError
         if si.config.max_msgs_per_subject < 1:
             raise BadBucketError
 
         return KeyValue(
             name=bucket,
             stream=stream,
             pre=KV_PRE_TEMPLATE.format(bucket=bucket),
             js=self,
-            direct=si.config.allow_direct
+            direct=bool(si.config.allow_direct)
         )
 
     async def create_key_value(
         self,
-        config: Optional[api.KeyValueConfig] = None,
+        config: api.KeyValueConfig | None = None,
         **params,
     ) -> KeyValue:
         """
         create_key_value takes an api.KeyValueConfig and creates a KV in JetStream.
         """
         if config is None:
             config = api.KeyValueConfig(bucket=params["bucket"])
         config = config.evolve(**params)
 
-        duplicate_window = 2 * 60  # 2 minutes
+        if VALID_BUCKET_RE.match(config.bucket) is None:
+            raise InvalidBucketNameError
+
+        duplicate_window: float = 2 * 60  # 2 minutes
+
         if config.ttl and config.ttl < duplicate_window:
             duplicate_window = config.ttl
 
         if config.history > 64:
             raise nats.js.errors.KeyHistoryTooLargeError
 
         stream = api.StreamConfig(
@@ -1049,17 +1065,101 @@
         assert stream.name is not None
 
         return KeyValue(
             name=config.bucket,
             stream=stream.name,
             pre=KV_PRE_TEMPLATE.format(bucket=config.bucket),
             js=self,
-            direct=si.config.allow_direct
+            direct=bool(si.config.allow_direct),
         )
 
     async def delete_key_value(self, bucket: str) -> bool:
         """
         delete_key_value deletes a JetStream KeyValue store by destroying
         the associated stream.
         """
+        if VALID_BUCKET_RE.match(bucket) is None:
+            raise InvalidBucketNameError
+
         stream = KV_STREAM_TEMPLATE.format(bucket=bucket)
         return await self.delete_stream(stream)
+
+    #######################
+    #                     #
+    # ObjectStore Context #
+    #                     #
+    #######################
+
+    async def object_store(self, bucket: str) -> ObjectStore:
+        if VALID_BUCKET_RE.match(bucket) is None:
+            raise InvalidBucketNameError
+
+        stream = OBJ_STREAM_TEMPLATE.format(bucket=bucket)
+        try:
+            await self.stream_info(stream)
+        except NotFoundError:
+            raise BucketNotFoundError
+
+        return ObjectStore(
+            name=bucket,
+            stream=stream,
+            js=self,
+        )
+
+    async def create_object_store(
+        self,
+        bucket: str = None,
+        config: Optional[api.ObjectStoreConfig] = None,
+        **params,
+    ) -> ObjectStore:
+        """
+        create_object_store takes an api.ObjectStoreConfig and creates a OBJ in JetStream.
+        """
+        if config is None:
+            config = api.ObjectStoreConfig(bucket=bucket)
+        else:
+            config.bucket = bucket
+        config = config.evolve(**params)
+
+        if VALID_BUCKET_RE.match(config.bucket) is None:
+            raise InvalidBucketNameError
+
+        name = config.bucket
+        chunks = OBJ_ALL_CHUNKS_PRE_TEMPLATE.format(bucket=name)
+        meta = OBJ_ALL_META_PRE_TEMPLATE.format(bucket=name)
+
+        max_bytes = config.max_bytes
+        if max_bytes == 0:
+            max_bytes = -1
+
+        stream = api.StreamConfig(
+            name=OBJ_STREAM_TEMPLATE.format(bucket=config.bucket),
+            description=config.description,
+            subjects=[chunks, meta],
+            max_age=config.ttl,
+            max_bytes=max_bytes,
+            max_consumers=0,
+            storage=config.storage,
+            num_replicas=config.replicas,
+            placement=config.placement,
+            discard=api.DiscardPolicy.NEW,
+            allow_rollup_hdrs=True,
+            allow_direct=True,
+        )
+        await self.add_stream(stream)
+
+        assert stream.name is not None
+        return ObjectStore(
+            name=config.bucket,
+            stream=stream.name,
+            js=self,
+        )
+
+    async def delete_object_store(self, bucket: str) -> bool:
+        """
+        delete_object_store will delete the underlying stream for the named object.
+        """
+        if VALID_BUCKET_RE.match(bucket) is None:
+            raise InvalidBucketNameError
+
+        stream = OBJ_STREAM_TEMPLATE.format(bucket=bucket)
+        return await self.delete_stream(stream)
```

### Comparing `nats-py-2.2.0/nats/js/errors.py` & `nats-py-2.3.0/nats/js/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,77 +8,79 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Dict, NoReturn, Optional
+from typing import TYPE_CHECKING, Any, NoReturn
 
 import nats.errors
 from nats.js import api
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
 
 
 class Error(nats.errors.Error):
     """
     An Error raised by the NATS client when using JetStream.
     """
 
-    def __init__(self, description: Optional[str] = None) -> None:
+    def __init__(self, description: str | None = None) -> None:
         self.description = description
 
     def __str__(self) -> str:
         desc = ''
         if self.description:
             desc = self.description
         return f"nats: JetStream.{self.__class__.__name__} {desc}"
 
 
 @dataclass(repr=False, init=False)
 class APIError(Error):
     """
     An Error that is the result of interacting with NATS JetStream.
     """
-    code: Optional[int]
-    err_code: Optional[int]
-    description: Optional[str]
-    stream: Optional[str]
-    seq: Optional[int]
+    code: int | None
+    err_code: int | None
+    description: str | None
+    stream: str | None
+    seq: int | None
 
     def __init__(
         self,
-        code: int = None,
-        description: Optional[str] = None,
-        err_code: Optional[int] = None,
-        stream: Optional[str] = None,
-        seq: Optional[int] = None,
+        code: int | None = None,
+        description: str | None = None,
+        err_code: int | None = None,
+        stream: str | None = None,
+        seq: int | None = None,
     ) -> None:
         self.code = code
         self.err_code = err_code
         self.description = description
         self.stream = stream
         self.seq = seq
 
     @classmethod
-    def from_msg(cls, msg: "Msg") -> NoReturn:
+    def from_msg(cls, msg: Msg) -> NoReturn:
         if msg.header is None:
             raise APIError
         code = msg.header[api.Header.STATUS]
         if code == api.StatusCode.SERVICE_UNAVAILABLE:
             raise ServiceUnavailableError
         else:
             desc = msg.header[api.Header.DESCRIPTION]
             raise APIError(code=int(code), description=desc)
 
     @classmethod
-    def from_error(cls, err: Dict[str, Any]):
+    def from_error(cls, err: dict[str, Any]):
         code = err['code']
         if code == 503:
             raise ServiceUnavailableError(**err)
         elif code == 500:
             raise ServerError(**err)
         elif code == 404:
             raise NotFoundError(**err)
@@ -221,7 +223,63 @@
         return "nats: no keys found"
 
 
 class KeyHistoryTooLargeError(KeyValueError):
 
     def __str__(self) -> str:
         return "nats: history limited to a max of 64"
+
+
+class InvalidBucketNameError(Error):
+    """
+    Raised when trying to create a KV or OBJ bucket with invalid name.
+    """
+    pass
+
+
+class InvalidObjectNameError(Error):
+    """
+    Raised when trying to put an object in Object Store with invalid key.
+    """
+    pass
+
+
+class BadObjectMetaError(Error):
+    """
+    Raised when trying to read corrupted metadata from Object Store.
+    """
+    pass
+
+
+class LinkIsABucketError(Error):
+    """
+    Raised when trying to get object from Object Store that is a bucket.
+    """
+    pass
+
+
+class DigestMismatchError(Error):
+    """
+    Raised when getting an object from Object Store that has a different digest than expected.
+    """
+    pass
+
+
+class ObjectNotFoundError(NotFoundError):
+    """
+    When attempted to lookup an Object that does not exist.
+    """
+    pass
+
+
+class ObjectDeletedError(NotFoundError):
+    """
+    When attempted to do an operation to an Object that does not exist.
+    """
+    pass
+
+
+class ObjectAlreadyExists(Error):
+    """
+    When attempted to do an operation to an Object that already exist.
+    """
+    pass
```

### Comparing `nats-py-2.2.0/nats/js/kv.py` & `nats-py-2.3.0/nats/js/kv.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 import asyncio
 import datetime
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Optional, List
+from typing import TYPE_CHECKING
 
-from nats.js import api
+import nats.errors
 import nats.js.errors
+from nats.js import api
 
 if TYPE_CHECKING:
     from nats.js import JetStreamContext
 
 KV_OP = "KV-Operation"
 KV_DEL = "DEL"
 KV_PURGE = "PURGE"
@@ -64,19 +67,19 @@
     @dataclass
     class Entry:
         """
         An entry from a KeyValue store in JetStream.
         """
         bucket: str
         key: str
-        value: Optional[bytes]
-        revision: Optional[int]
-        delta: Optional[int]
-        created: Optional[int]
-        operation: Optional[str]
+        value: bytes | None
+        revision: int | None
+        delta: int | None
+        created: int | None
+        operation: str | None
 
     @dataclass(frozen=True)
     class BucketStatus:
         """
         BucketStatus is the status of a KeyValue bucket.
         """
         stream_info: api.StreamInfo
@@ -93,48 +96,48 @@
         def history(self) -> int:
             """
             history returns the max msgs per subject.
             """
             return self.stream_info.config.max_msgs_per_subject
 
         @property
-        def ttl(self) -> Optional[float]:
+        def ttl(self) -> float | None:
             """
             ttl returns the max age in seconds.
             """
             if self.stream_info.config.max_age is None:
                 return None
             return self.stream_info.config.max_age
 
     def __init__(
         self,
         name: str,
         stream: str,
         pre: str,
-        js: "JetStreamContext",
+        js: JetStreamContext,
         direct: bool,
     ) -> None:
         self._name = name
         self._stream = stream
         self._pre = pre
         self._js = js
         self._direct = direct
 
-    async def get(self, key: str, revision: Optional[int] = None) -> Entry:
+    async def get(self, key: str, revision: int | None = None) -> Entry:
         """
         get returns the latest value for the key.
         """
         entry = None
         try:
             entry = await self._get(key, revision)
         except nats.js.errors.KeyDeletedError as err:
             raise nats.js.errors.KeyNotFoundError(err.entry, err.op)
         return entry
 
-    async def _get(self, key: str, revision: Optional[int] = None) -> Entry:
+    async def _get(self, key: str, revision: int | None = None) -> Entry:
         msg = None
         subject = f"{self._pre}{key}"
         try:
             if revision:
                 msg = await self._js.get_msg(
                     self._stream,
                     seq=revision,
@@ -209,15 +212,15 @@
                 raise err
             except nats.js.errors.KeyDeletedError as err:
                 pa = await self.update(key, value, last=err.entry.revision)
 
         return pa
 
     async def update(
-        self, key: str, value: bytes, last: Optional[int] = None
+        self, key: str, value: bytes, last: int | None = None
     ) -> int:
         """
         update will update the value iff the latest revision matches.
         """
         hdrs = {}
         if not last:
             last = 0
@@ -234,15 +237,15 @@
                 raise nats.js.errors.KeyWrongLastSequenceError(
                     description=err.description
                 )
             else:
                 raise err
         return pa.seq
 
-    async def delete(self, key: str, last: Optional[int] = None) -> bool:
+    async def delete(self, key: str, last: int | None = None) -> bool:
         """
         delete will place a delete marker and remove all previous revisions.
         """
         hdrs = {}
         hdrs[KV_OP] = KV_DEL
 
         if last and last > 0:
@@ -257,15 +260,15 @@
         """
         hdrs = {}
         hdrs[KV_OP] = KV_PURGE
         hdrs[api.Header.ROLLUP] = MSG_ROLLUP_SUBJECT
         await self._js.publish(f"{self._pre}{key}", headers=hdrs)
         return True
 
-    async def purge_deletes(self, olderthan: Optional[int] = 30 * 60) -> bool:
+    async def purge_deletes(self, olderthan: int = 30 * 60) -> bool:
         """
         purge will remove all current delete markers older.
         :param olderthan: time in seconds
         """
 
         watcher = await self.watchall()
         delete_markers = []
@@ -293,14 +296,15 @@
 
     class KeyWatcher:
 
         def __init__(self, js):
             self._js = js
             self._updates = asyncio.Queue(maxsize=256)
             self._sub = None
+            self._pending: int | None = None
 
             # init done means that the nil marker has been sent,
             # once this is sent it won't be sent anymore.
             self._init_done = False
 
         async def stop(self):
             """
@@ -329,15 +333,15 @@
 
     async def watchall(self, **kwargs) -> KeyWatcher:
         """
         watchall returns a KeyValue watcher that matches all the keys.
         """
         return await self.watch(">", **kwargs)
 
-    async def keys(self, **kwargs) -> List[str]:
+    async def keys(self, **kwargs) -> list[str]:
         """
         keys will return a list of the keys from a KeyValue store.
         """
         watcher = await self.watchall(
             ignore_deletes=True,
             meta_only=True,
         )
@@ -351,15 +355,15 @@
         await watcher.stop()
 
         if not keys:
             raise nats.js.errors.NoKeysError
 
         return keys
 
-    async def history(self, key: str) -> List[Entry]:
+    async def history(self, key: str) -> list[Entry]:
         """
         history retrieves a list of the entries so far.
         """
         watcher = await self.watch(key, include_history=True)
 
         entries = []
 
@@ -388,15 +392,15 @@
         watch will fire a callback when a key that matches the keys
         pattern is updated.
         The first update after starting the watch is None in case
         there are no pending updates.
         """
         subject = f"{self._pre}{keys}"
         watcher = KeyValue.KeyWatcher(self)
-        init_setup = asyncio.Future()
+        init_setup: asyncio.Future[bool] = asyncio.Future()
 
         async def watch_updates(msg):
             if not init_setup.done():
                 await asyncio.wait_for(init_setup, timeout=self._js._timeout)
 
             meta = msg.metadata
             op = None
```

### Comparing `nats-py-2.2.0/nats/js/manager.py` & `nats-py-2.3.0/nats/js/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import json
+from __future__ import annotations
+
 import base64
+import json
 from email.parser import BytesParser
-from typing import TYPE_CHECKING, Any, Dict, Optional, List
+from typing import TYPE_CHECKING, Any
 
 from nats.errors import NoRespondersError
 from nats.js import api
-from nats.js.errors import APIError, ServiceUnavailableError, NotFoundError
+from nats.js.errors import APIError, NotFoundError, ServiceUnavailableError
 
 if TYPE_CHECKING:
     from nats import NATS
 
 NATS_HDR_LINE = bytearray(b'NATS/1.0')
 NATS_HDR_LINE_SIZE = len(NATS_HDR_LINE)
 _CRLF_ = b'\r\n'
@@ -33,15 +35,15 @@
 class JetStreamManager:
     """
     JetStreamManager exposes management APIs for JetStream.
     """
 
     def __init__(
         self,
-        conn: "NATS",
+        conn: NATS,
         prefix: str = api.DEFAULT_PREFIX,
         timeout: float = 5,
     ) -> None:
         self._prefix = prefix
         self._nc = conn
         self._timeout = timeout
         self._hdr_parser = BytesParser()
@@ -70,15 +72,17 @@
         """
         resp = await self._api_request(
             f"{self._prefix}.STREAM.INFO.{name}", timeout=self._timeout
         )
         return api.StreamInfo.from_response(resp)
 
     async def add_stream(
-        self, config: api.StreamConfig = None, **params
+        self,
+        config: api.StreamConfig | None = None,
+        **params
     ) -> api.StreamInfo:
         """
         add_stream creates a stream.
         """
         if config is None:
             config = api.StreamConfig()
         config = config.evolve(**params)
@@ -90,15 +94,17 @@
             f"{self._prefix}.STREAM.CREATE.{config.name}",
             data.encode(),
             timeout=self._timeout,
         )
         return api.StreamInfo.from_response(resp)
 
     async def update_stream(
-        self, config: api.StreamConfig = None, **params
+        self,
+        config: api.StreamConfig | None = None,
+        **params
     ) -> api.StreamInfo:
         """
         update_stream updates a stream.
         """
         if config is None:
             config = api.StreamConfig()
         config = config.evolve(**params)
@@ -121,22 +127,22 @@
             f"{self._prefix}.STREAM.DELETE.{name}", timeout=self._timeout
         )
         return resp['success']
 
     async def purge_stream(
         self,
         name: str,
-        seq: Optional[int] = None,
-        subject: Optional[str] = None,
-        keep: Optional[int] = None
+        seq: int | None = None,
+        subject: str | None = None,
+        keep: int | None = None
     ) -> bool:
         """
         Purge a stream by name.
         """
-        stream_req = {}
+        stream_req: dict[str, Any] = {}
         if seq:
             stream_req['seq'] = seq
         if subject:
             stream_req['filter'] = subject
         if keep:
             stream_req['keep'] = keep
 
@@ -145,27 +151,27 @@
             f"{self._prefix}.STREAM.PURGE.{name}",
             req.encode(),
             timeout=self._timeout
         )
         return resp['success']
 
     async def consumer_info(
-        self, stream: str, consumer: str, timeout: Optional[float] = None
+        self, stream: str, consumer: str, timeout: float | None = None
     ):
         # TODO: Validate the stream and consumer names.
         if timeout is None:
             timeout = self._timeout
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.INFO.{stream}.{consumer}",
             b'',
             timeout=timeout
         )
         return api.ConsumerInfo.from_response(resp)
 
-    async def streams_info(self) -> List[api.StreamInfo]:
+    async def streams_info(self) -> list[api.StreamInfo]:
         """
         streams_info retrieves a list of streams.
         """
         resp = await self._api_request(
             f"{self._prefix}.STREAM.LIST",
             b'',
             timeout=self._timeout,
@@ -175,16 +181,16 @@
             stream_info = api.StreamInfo.from_response(stream)
             streams.append(stream_info)
         return streams
 
     async def add_consumer(
         self,
         stream: str,
-        config: Optional[api.ConsumerConfig] = None,
-        timeout: Optional[float] = None,
+        config: api.ConsumerConfig | None = None,
+        timeout: float | None = None,
         **params,
     ) -> api.ConsumerInfo:
         if not timeout:
             timeout = self._timeout
         if config is None:
             config = api.ConsumerConfig()
         config = config.evolve(**params)
@@ -216,15 +222,15 @@
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.DELETE.{stream}.{consumer}",
             b'',
             timeout=self._timeout
         )
         return resp['success']
 
-    async def consumers_info(self, stream: str) -> List[api.ConsumerInfo]:
+    async def consumers_info(self, stream: str) -> list[api.ConsumerInfo]:
         """
         consumers_info retrieves a list of consumers.
         """
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.LIST.{stream}",
             b'',
             timeout=self._timeout,
@@ -234,24 +240,24 @@
             consumer_info = api.ConsumerInfo.from_response(consumer)
             consumers.append(consumer_info)
         return consumers
 
     async def get_msg(
         self,
         stream_name: str,
-        seq: Optional[int] = None,
-        subject: Optional[str] = None,
-        direct: Optional[bool] = False,
-        next: Optional[bool] = False,
+        seq: int | None = None,
+        subject: str | None = None,
+        direct: bool | None = False,
+        next: bool | None = False,
     ) -> api.RawStreamMsg:
         """
         get_msg retrieves a message from a stream.
         """
         req_subject = None
-        req = {}
+        req: dict[str, Any] = {}
         if seq:
             req['seq'] = seq
         if subject:
             req['seq'] = None
             req.pop('seq', None)
             req['last_by_subj'] = subject
         if next:
@@ -274,34 +280,34 @@
                 req_subject, data.encode(), timeout=self._timeout
             )
             raw_msg = JetStreamManager._lift_msg_to_raw_msg(resp)
             return raw_msg
 
         # Non Direct form
         req_subject = f"{self._prefix}.STREAM.MSG.GET.{stream_name}"
-        resp = await self._api_request(
+        resp_data = await self._api_request(
             req_subject, data.encode(), timeout=self._timeout
         )
 
-        raw_msg = api.RawStreamMsg.from_response(resp['message'])
+        raw_msg = api.RawStreamMsg.from_response(resp_data['message'])
         if raw_msg.hdrs:
             hdrs = base64.b64decode(raw_msg.hdrs)
             raw_headers = hdrs[NATS_HDR_LINE_SIZE + _CRLF_LEN_:]
             parsed_headers = self._hdr_parser.parsebytes(raw_headers)
             headers = None
             if len(parsed_headers.items()) > 0:
                 headers = {}
                 for k, v in parsed_headers.items():
                     headers[k] = v
             raw_msg.headers = headers
 
-        data = None
+        msg_data: bytes | None = None
         if raw_msg.data:
-            data = base64.b64decode(raw_msg.data)
-        raw_msg.data = data
+            msg_data = base64.b64decode(raw_msg.data)
+        raw_msg.data = msg_data
 
         return raw_msg
 
     @classmethod
     def _lift_msg_to_raw_msg(self, msg) -> api.RawStreamMsg:
         if not msg.data:
             msg.data = None
@@ -334,27 +340,27 @@
         resp = await self._api_request(req_subject, data.encode())
         return resp['success']
 
     async def get_last_msg(
         self,
         stream_name: str,
         subject: str,
-        direct: Optional[bool] = False,
+        direct: bool | None = False,
     ) -> api.RawStreamMsg:
         """
         get_last_msg retrieves the last message from a stream.
         """
         return await self.get_msg(stream_name, subject=subject, direct=direct)
 
     async def _api_request(
         self,
         req_subject: str,
         req: bytes = b'',
         timeout: float = 5,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         try:
             msg = await self._nc.request(req_subject, req, timeout=timeout)
             resp = json.loads(msg.data)
         except NoRespondersError:
             raise ServiceUnavailableError
 
         # Check for API errors.
```

### Comparing `nats-py-2.2.0/nats/nuid.py` & `nats-py-2.3.0/nats/nuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from __future__ import annotations
+
 from random import Random
+from secrets import randbelow, token_bytes
 from sys import maxsize as MaxInt
-from secrets import token_bytes, randbelow
 
 DIGITS = b'0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
 BASE = 62
 PREFIX_LENGTH = 12
 SEQ_LENGTH = 10
 MAX_SEQ = 839299365868340224  # BASE**10
 MIN_INC = 33
```

### Comparing `nats-py-2.2.0/nats/protocol/__init__.py` & `nats-py-2.3.0/nats/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.2.0/nats/protocol/command.py` & `nats-py-2.3.0/nats/protocol/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Callable
 
 PUB_OP = 'PUB'
 HPUB_OP = 'HPUB'
 SUB_OP = 'SUB'
 UNSUB_OP = 'UNSUB'
 _CRLF_ = '\r\n'
```

### Comparing `nats-py-2.2.0/nats/protocol/parser.py` & `nats-py-2.3.0/nats/protocol/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """
 NATS network protocol parser.
 """
 
+from __future__ import annotations
+
 import json
 import re
-from typing import Any, Dict
+from typing import Any
 
 from nats.errors import ProtocolError
 
 MSG_RE = re.compile(
     b'\\AMSG\\s+([^\\s]+)\\s+([^\\s]+)\\s+(([^\\s]+)[^\\S\r\n]+)?(\\d+)\r\n'
 )
 HMSG_RE = re.compile(
@@ -79,15 +81,15 @@
         return f"<nats protocol parser state={self.state}>"
 
     def reset(self) -> None:
         self.buf = bytearray()
         self.state = AWAITING_CONTROL_LINE
         self.needed = 0
         self.header_needed = 0
-        self.msg_arg: Dict[str, Any] = {}
+        self.msg_arg: dict[str, Any] = {}
 
     async def parse(self, data: bytes = b''):
         """
         Parses the wire protocol from NATS for the client
         and dispatches the subscription callbacks.
         """
         self.buf.extend(data)
```

### Comparing `nats-py-2.2.0/nats_py.egg-info/PKG-INFO` & `nats-py-2.3.0/nats_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: NATS client for Python
 Author-email: Waldemar Quevedo <wally@synadia.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,14 +214,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: nkeys
+Provides-Extra: aiohttp
+Provides-Extra: fast_parse
 License-File: LICENSE
 
 # NATS - Python3 Client for Asyncio
 
 An [asyncio](https://docs.python.org/3/library/asyncio.html) Python client for the [NATS messaging system](https://nats.io).
 
 [![docs](https://img.shields.io/static/v1?label=docs&message=docs&color=informational)](https://nats-io.github.io/nats.py/)
@@ -336,14 +338,15 @@
     # Create pull based consumer on 'foo'.
     psub = await js.pull_subscribe("foo", "psub")
 
     # Fetch and ack messagess from consumer.
     for i in range(0, 10):
         msgs = await psub.fetch(1)
         for msg in msgs:
+            await msg.ack()
             print(msg)
 
     # Create single ephemeral push based subscriber.
     sub = await js.subscribe("foo")
     msg = await sub.next_msg()
     await msg.ack()
```

### Comparing `nats-py-2.2.0/nats_py.egg-info/SOURCES.txt` & `nats-py-2.3.0/nats_py.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -15,16 +15,25 @@
 nats/aio/transport.py
 nats/js/__init__.py
 nats/js/api.py
 nats/js/client.py
 nats/js/errors.py
 nats/js/kv.py
 nats/js/manager.py
+nats/js/object_store.py
 nats/protocol/__init__.py
 nats/protocol/command.py
 nats/protocol/parser.py
 nats_py.egg-info/PKG-INFO
 nats_py.egg-info/SOURCES.txt
 nats_py.egg-info/dependency_links.txt
 nats_py.egg-info/requires.txt
 nats_py.egg-info/top_level.txt
-nats_py.egg-info/zip-safe
+nats_py.egg-info/zip-safe
+tests/test_client.py
+tests/test_client_async_await.py
+tests/test_client_nkeys.py
+tests/test_client_v2.py
+tests/test_client_websocket.py
+tests/test_js.py
+tests/test_nuid.py
+tests/test_parser.py
```

### Comparing `nats-py-2.2.0/pyproject.toml` & `nats-py-2.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -33,7 +33,32 @@
 [tool.setuptools.dynamic]
 version = {attr = "nats.aio.client.__version__"}
 
 [tool.setuptools.packages.find]
 include = ["nats*"]  # package names should match these glob patterns (["*"] by default)
 exclude = ["scripts", "tests"]  # exclude packages matching these glob patterns (empty by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
+
+[tool.mypy]
+files = ["nats"]
+python_version = "3.7"
+ignore_missing_imports = true
+follow_imports = "silent"
+show_error_codes = true
+check_untyped_defs = false
+
+[tool.pytest.ini_options]
+addopts = ["--cov=nats", "--cov-report=html"]
+
+[tool.yapf]
+split_before_first_argument = true
+dedent_closing_brackets = true
+coalesce_brackets = true
+allow_split_before_dict_value = false
+indent_dictionary_value = true
+split_before_expression_after_opening_paren = true
+
+[tool.isort]
+combine_as_imports = true
+multi_line_output = 3
+include_trailing_comma = true
+src_paths = ["nats", "tests"]
```

