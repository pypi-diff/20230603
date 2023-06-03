# Comparing `tmp/urllib3_ext_hface-0.2.9.tar.gz` & `tmp/urllib3_ext_hface-0.3.0.tar.gz`

## Comparing `urllib3_ext_hface-0.2.9.tar` & `urllib3_ext_hface-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,45 @@
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/dev-requirements.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/changelog.rst
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/cli.rst
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/common.rst
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/conf.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/connections.rst
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/facade.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/index.rst
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/install.rst
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/intro.rst
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/license.rst
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/protocols.rst
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/_static/custom.css
--rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/docs/_static/hface.png
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_factories.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_protocol.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http2/_factories.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http2/_protocol.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/_factories.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/_protocol.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/_quic.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/tests/helpers.py
--rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/tests/test_http1.py
--rw-r--r--   0        0        0    16185 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/tests/test_http2.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/NOTICE
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/dev-requirements.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/cli.rst
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/common.rst
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/connections.rst
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/facade.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/install.rst
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/intro.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/license.rst
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/protocols.rst
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    33109 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/docs/_static/hface.png
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/_aioquic.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/helpers.py
+-rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_http1.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_http2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/NOTICE
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.0/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.2.9/CHANGELOG.rst` & `urllib3_ext_hface-0.3.0/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,33 @@
+v0.3.0 (2023-06-03)
+-------------------
+
+* Breaking: Conception simplification. Remove HTTPFactories in favor of a single unified HTTPFactory.
+* Lazy import HTTPProtocol implementation.
+
+v0.2.12 (2023-05-25)
+--------------------
+
+* Remove ``InvalidPacket``, ``PacketInfo`` from protocols.http3.
+* Fix an error trying to unset previously unknown connection id in quic event handler.
+
+v0.2.11 (2023-05-24)
+--------
+
+* Add keyfile, certfile and keypassword in ``ClientTLSConfig`` to be passed down the QUIC configuration.
+
+v0.2.10 (2023-05-23)
+--------
+
+* Add staticmethod ``exceptions`` on ``HTTPProtocol`` that return sub-dependency-protocol specific exceptions.
+
 v0.2.9 (2023-05-23)
 --------
 
-* No longer alter (lower) header name case in h11 response event.
+* No longer lower (twice) header name case in h11 response event.
 
 v0.2.8 (2023-05-21)
 --------
 
 * Add method ``has_pending_event`` across protocols impl.
 
 v0.2.7 (2023-05-21)
```

### Comparing `urllib3_ext_hface-0.2.9/docs/cli.rst` & `urllib3_ext_hface-0.3.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/common.rst` & `urllib3_ext_hface-0.3.0/docs/common.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/conf.py` & `urllib3_ext_hface-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/connections.rst` & `urllib3_ext_hface-0.3.0/docs/connections.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/facade.rst` & `urllib3_ext_hface-0.3.0/docs/facade.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/index.rst` & `urllib3_ext_hface-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/install.rst` & `urllib3_ext_hface-0.3.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/intro.rst` & `urllib3_ext_hface-0.3.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/protocols.rst` & `urllib3_ext_hface-0.3.0/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/docs/_static/hface.png` & `urllib3_ext_hface-0.3.0/docs/_static/hface.png`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import dataclasses
-
-from aioquic.tls import CipherSuite, SessionTicket
+from typing import Any
 
 
 @dataclasses.dataclass
-class ClientTLSConfig:
+class QuicTLSConfig:
     """
     Client TLS configuration.
     """
 
     #: Allows to proceed for server without valid TLS certificates.
     insecure: bool = False
 
@@ -33,18 +32,22 @@
 
     #: Directory with CA certificates to trust for server verification
     capath: str | None = None
 
     #: Blob with CA certificates to trust for server verification
     cadata: bytes | None = None
 
-    #: Manually set ciphers to be used in your DTLS
-    cipher_suites: list[CipherSuite] | None = None
+    #: If provided, will trigger an additional load_cert_chain() upon the QUIC Configuration
+    certfile: str | None = None
+
+    keyfile: str | None = None
+
+    keypassword: str | bytes | None = None
 
     #: The DTLS session ticket which should be used for session resumption
-    session_ticket: SessionTicket | None = None
+    session_ticket: Any | None = None
 
-    def clone(self) -> ClientTLSConfig:
+    def clone(self) -> QuicTLSConfig:
         """
         Clone this instance.
         """
         return dataclasses.replace(self)
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,21 @@
     GoawayReceived,
     HandshakeCompleted,
     HeadersReceived,
     StreamEvent,
     StreamReset,
     StreamResetReceived,
     StreamResetSent,
-    UnclassifiedData,
 )
 
 __all__ = (
     "Event",
     "ConnectionTerminated",
     "GoawayReceived",
     "StreamEvent",
     "StreamReset",
     "StreamResetReceived",
     "StreamResetSent",
     "HeadersReceived",
     "DataReceived",
     "HandshakeCompleted",
-    "UnclassifiedData",
 )
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/events/_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,35 +144,14 @@
 
     def __repr__(self) -> str:
         cls = type(self).__name__
         return f"{cls}(alpn={self.alpn_protocol})"
 
 
 @dataclass
-class UnclassifiedData(StreamEvent):
-    """
-    A frame containing unclassified data was received.
-    This is only useful for debug purposes.
-
-    Extends :class:`.StreamEvent`.
-    """
-
-    data: bytes
-
-    end_stream: bool = False
-
-    def __repr__(self) -> str:
-        cls = type(self).__name__
-        return (
-            f"{cls}(stream_id={self.stream_id!r}, "
-            f"len(data)={len(self.data)}, end_stream={self.end_stream!r})"
-        )
-
-
-@dataclass
 class HeadersReceived(StreamEvent):
     """
     A frame with HTTP headers was received.
 
     Extends :class:`.StreamEvent`.
     """
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from ._factories import ALPNHTTPFactory, HTTPOverQUICClientFactory, HTTPOverTCPFactory
+from ._factories import HTTPProtocolFactory
 from ._protocols import (
     HTTP1Protocol,
     HTTP2Protocol,
     HTTP3Protocol,
     HTTPOverQUICProtocol,
     HTTPOverTCPProtocol,
     HTTPProtocol,
 )
-from .http1 import HTTP1ClientFactory
-from .http2 import HTTP2ClientFactory
-from .http3 import HTTP3ClientFactory
 
 __all__ = (
-    "ALPNHTTPFactory",
-    "HTTPOverQUICClientFactory",
-    "HTTPOverTCPFactory",
-    "HTTP1ClientFactory",
-    "HTTP2ClientFactory",
-    "HTTP2ClientFactory",
-    "HTTP3ClientFactory",
     "HTTP1Protocol",
     "HTTP2Protocol",
     "HTTP3Protocol",
     "HTTPOverQUICProtocol",
     "HTTPOverTCPProtocol",
     "HTTPProtocol",
+    "HTTPProtocolFactory",
 )
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Sequence
+from typing import Any, Sequence
 
 from .._error_codes import HTTPErrorCodes
 from .._typing import HeadersType
 from ..events import Event
 
 
 class BaseProtocol(metaclass=ABCMeta):
@@ -116,24 +116,31 @@
 
         :return: a sequence of connection IDs
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def session_ticket(self) -> object | None:
+    def session_ticket(self) -> Any | None:
         raise NotImplementedError
 
 
 class HTTPProtocol(metaclass=ABCMeta):
     """
     Sans-IO representation of an HTTP connection
-
     """
 
+    implementation: str
+
+    @staticmethod
+    @abstractmethod
+    def exceptions() -> tuple[type[BaseException], ...]:
+        """Return exception types that should be handled in your application."""
+        raise NotImplementedError
+
     @property
     @abstractmethod
     def http_version(self) -> str:
         """
         An HTTP version as a string.
         """
         raise NotImplementedError
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from ._factories import HTTP1ClientFactory
+from ._h11 import HTTP1ProtocolHyperImpl
 
-__all__ = ("HTTP1ClientFactory",)
+__all__ = ("HTTP1ProtocolHyperImpl",)
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_factories.py` & `urllib3_ext_hface-0.3.0/tests/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,38 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import h11
+from urllib3_ext_hface._typing import HeaderType
 
-from .._factories import HTTPOverTCPFactory
-from .._protocols import HTTP1Protocol
-from ._protocol import HTTP1ProtocolImpl
 
-ALPN_PROTOCOL = "http/1.1"
-
-
-class HTTP1ClientFactory(HTTPOverTCPFactory):
-    """
-    Creates a default HTTP/1 protocol for client-side usage.
-
-    The HTTP/1 implementation is built on the top of the h11_ library.
-
-    .. _h11: https://h11.readthedocs.io/
-
-    Implements :class:`.HTTPOverTCPFactory`.
-    """
-
-    alpn_protocols = [ALPN_PROTOCOL]
-
-    def __call__(
-        self,
-        *,
-        tls_version: str | None = None,
-        alpn_protocol: str | None = None,
-    ) -> HTTP1Protocol:
-        connection = h11.Connection(our_role=h11.CLIENT)
-        scheme = "http" if tls_version is None else "https"
-        return HTTP1ProtocolImpl(connection, scheme=scheme)
+def build_request_headers(
+    *extra_headers: HeaderType,
+    method: bytes = b"GET",
+    scheme: bytes = b"https",
+    authority: bytes = b"example.com",
+    path: bytes = b"/",
+) -> list[HeaderType]:
+    return [
+        (b":method", method),
+        (b":scheme", scheme),
+        (b":authority", authority),
+        (b":path", path),
+    ] + list(extra_headers)
+
+
+def build_response_headers(
+    *extra_headers: HeaderType,
+    status: bytes = b"200",
+) -> list[HeaderType]:
+    return [
+        (b":status", status),
+    ] + list(extra_headers)
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http1/_protocol.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http1/_h11.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,35 +156,34 @@
             raise ValueError("Pseudo header not allowed in HTTP/1: " + name.decode())
         regular_headers.append((name, value))
 
     pseudo_headers = [(b":status", str(response.status_code).encode())]
     return pseudo_headers + regular_headers
 
 
-class HTTP1ProtocolImpl(HTTP1Protocol):
-    _scheme: bytes
-
-    _connection: h11.Connection
-    _current_stream_id: int = 1
-
-    _data_buffer: list[bytes]
-    _event_buffer: deque[Event]
-
-    _terminated: bool = False
+class HTTP1ProtocolHyperImpl(HTTP1Protocol):
+    implementation: str = "h11"
 
     def __init__(
         self,
-        connection: h11.Connection,
         *,
         scheme: str = "http",
     ) -> None:
-        self._connection = connection
-        self._scheme = scheme.encode()
-        self._data_buffer = []
-        self._event_buffer = deque()
+        self._connection: h11.Connection = h11.Connection(h11.CLIENT)
+        self._scheme: bytes = scheme.encode()
+        self._data_buffer: list[bytes] = []
+        self._event_buffer: deque[Event] = deque()
+        self._terminated: bool = False
+        self._switched: bool = False
+
+        self._current_stream_id: int = 1
+
+    @staticmethod
+    def exceptions() -> tuple[type[BaseException], ...]:
+        return h11.LocalProtocolError, h11.ProtocolError, h11.RemoteProtocolError
 
     @property
     def http_version(self) -> str:
         their_http_version = self._connection.their_http_version
         if their_http_version is None:
             return super().http_version
         return their_http_version.decode()
@@ -205,15 +204,15 @@
             raise RuntimeError(
                 "Cannot generate a new stream ID because the connection is not idle. "
                 "HTTP/1.1 is not multiplexed and we do not support HTTP pipelining."
             )
         return self._current_stream_id
 
     def submit_close(self, error_code: int = 0) -> None:
-        pass  # noop
+        pass  # no-op
 
     def submit_headers(
         self, stream_id: int, headers: HeadersType, end_stream: bool = False
     ) -> None:
         if stream_id != self._current_stream_id:
             raise ValueError("Invalid stream ID.")
         if self._connection.our_role == h11.CLIENT:
@@ -348,16 +347,14 @@
 
     def _connection_terminated(
         self, error_code: int = 0, message: str | None = None
     ) -> Event:
         self._terminated = True
         return ConnectionTerminated(error_code, message)
 
-    _switched: bool = False
-
     def _maybe_start_next_cycle(self) -> None:
         if h11.DONE == self._connection.our_state == self._connection.their_state:
             self._connection.start_next_cycle()
             self._current_stream_id += 1
         if h11.SWITCHED_PROTOCOL == self._connection.their_state and not self._switched:
             data, closed = self._connection.trailing_data
             if data:
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from ._factories import HTTP2ClientFactory
+from ._h2 import HTTP2ProtocolHyperImpl
 
-__all__ = ("HTTP2ClientFactory",)
+__all__ = ("HTTP2ProtocolHyperImpl",)
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http2/_protocol.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http2/_h2.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections import deque
 from typing import Iterator, cast
 
+import h2.config
 import h2.connection
 import h2.events
 import h2.exceptions
 
 from ..._typing import HeadersType
 from ...events import (
     ConnectionTerminated,
@@ -30,35 +31,43 @@
     HeadersReceived,
     StreamResetReceived,
     StreamResetSent,
 )
 from .._protocols import HTTP2Protocol
 
 
-class HTTP2ProtocolImpl(HTTP2Protocol):
-    _connection: h2.connection.H2Connection
-    _events: deque[Event]
-    _terminated: bool = False
+class HTTP2ProtocolHyperImpl(HTTP2Protocol):
+    implementation: str = "h2"
 
-    def __init__(self, connection: h2.connection.H2Connection) -> None:
-        self._connection = connection
+    def __init__(self) -> None:
+        self._connection: h2.connection.H2Connection = h2.connection.H2Connection(
+            h2.config.H2Configuration(
+                client_side=True,
+                validate_outbound_headers=False,
+                validate_inbound_headers=False,
+            )
+        )
         self._connection.initiate_connection()
-        self._events = deque()
+        self._events: deque[Event] = deque()
+        self._terminated: bool = False
+
+    @staticmethod
+    def exceptions() -> tuple[type[BaseException], ...]:
+        return h2.exceptions.ProtocolError, h2.exceptions.H2Error
 
     def is_available(self) -> bool:
-        # TODO: check concurrent stream limit
+        # TODO: check that we do not run out of stream IDs.
         return not self._terminated
 
     def has_expired(self) -> bool:
         # TODO: check that we do not run out of stream IDs.
         return self._terminated
 
     def get_available_stream_id(self) -> int:
-        stream_id: int = self._connection.get_next_available_stream_id()
-        return stream_id
+        return self._connection.get_next_available_stream_id()  # type: ignore[no-any-return]
 
     def submit_close(self, error_code: int = 0) -> None:
         self._connection.close_connection(error_code)
 
     def submit_headers(
         self, stream_id: int, headers: HeadersType, end_stream: bool = False
     ) -> None:
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,11 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from ._factories import HTTP3ClientFactory
-from ._quic import InvalidPacket, PacketInfo
+from ._aioquic import HTTP3ProtocolAioQuicImpl
 
-__all__ = ("HTTP3ClientFactory", "InvalidPacket", "PacketInfo")
+__all__ = ("HTTP3ProtocolAioQuicImpl",)
```

### Comparing `urllib3_ext_hface-0.2.9/src/urllib3_ext_hface/protocols/http3/_protocol.py` & `urllib3_ext_hface-0.3.0/src/urllib3_ext_hface/protocols/http3/_aioquic.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,50 +10,75 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import ssl
 from collections import deque
 from time import monotonic
 from typing import Iterable, Sequence
 
 import aioquic.h3.events as h3_events
 import aioquic.quic.events as quic_events
-from aioquic.h3.connection import H3Connection
+from aioquic.h3.connection import H3Connection, ProtocolError
+from aioquic.h3.exceptions import H3Error
 from aioquic.quic.configuration import QuicConfiguration
-from aioquic.quic.connection import QuicConnection
+from aioquic.quic.connection import QuicConnection, QuicConnectionError
 from aioquic.tls import SessionTicket
 
+from ..._configuration import QuicTLSConfig
 from ..._typing import AddressType, HeadersType
 from ...events import ConnectionTerminated, DataReceived, Event
 from ...events import HandshakeCompleted as _HandshakeCompleted
 from ...events import HeadersReceived, StreamResetReceived
 from .._protocols import HTTP3Protocol
 
 
-class HTTP3ProtocolImpl(HTTP3Protocol):
+class HTTP3ProtocolAioQuicImpl(HTTP3Protocol):
+    implementation: str = "aioquic"
+
     def __init__(
         self,
-        configuration: QuicConfiguration,
         *,
-        remote_address: AddressType | None = None,
+        remote_address: AddressType,
+        server_name: str,
+        tls_config: QuicTLSConfig,
     ) -> None:
-        if configuration.is_client and remote_address is None:
-            raise ValueError("remote_address is required for client connections.")
+        self._configuration: QuicConfiguration = QuicConfiguration(
+            is_client=True,
+            verify_mode=ssl.CERT_NONE if tls_config.insecure else ssl.CERT_REQUIRED,
+            cafile=tls_config.cafile,
+            capath=tls_config.capath,
+            cadata=tls_config.cadata,
+            alpn_protocols=["h3"],
+            session_ticket=tls_config.session_ticket,
+            server_name=server_name,
+        )
+
+        if tls_config.certfile:
+            self._configuration.load_cert_chain(
+                tls_config.certfile,  # type: ignore[arg-type]
+                tls_config.keyfile,  # type: ignore[arg-type]
+                tls_config.keypassword,
+            )
+
+        self._configuration.load_verify_locations(tls_config.cafile)
 
-        self._configuration: QuicConfiguration = configuration
         self._quic: QuicConnection = QuicConnection(configuration=self._configuration)
         self._connection_ids: set[bytes] = set()
         self._remote_address = remote_address
         self._event_buffer: deque[Event] = deque()
         self._http: H3Connection | None = None
         self._terminated: bool = False
-        self._now: float | None = None
+
+    @staticmethod
+    def exceptions() -> tuple[type[BaseException], ...]:
+        return ProtocolError, H3Error, QuicConnectionError
 
     def is_available(self) -> bool:
         # TODO: check concurrent stream limit
         return not self._terminated
 
     def has_expired(self) -> bool:
         # TODO: check that we do not run out of stream IDs.
@@ -103,15 +128,14 @@
         return len(self._event_buffer) > 0
 
     @property
     def connection_ids(self) -> Sequence[bytes]:
         return list(self._connection_ids)
 
     def clock(self, now: float) -> None:
-        self._now = now
         timer = self._quic.get_timer()
         if timer is not None and now >= timer:
             self._quic.handle_timer(now)
             self._fetch_events()
 
     def get_timer(self) -> float | None:
         return self._quic.get_timer()
@@ -143,15 +167,20 @@
             for h3_event in self._http.handle_event(quic_event):
                 self._event_buffer += self._map_h3_event(h3_event)
 
     def _map_quic_event(self, quic_event: quic_events.QuicEvent) -> Iterable[Event]:
         if isinstance(quic_event, quic_events.ConnectionIdIssued):
             self._connection_ids.add(quic_event.connection_id)
         elif isinstance(quic_event, quic_events.ConnectionIdRetired):
-            self._connection_ids.remove(quic_event.connection_id)
+            try:
+                self._connection_ids.remove(quic_event.connection_id)
+            except (
+                KeyError
+            ):  # it is surprising, learn more about this with aioquic maintainer.
+                pass
 
         if isinstance(quic_event, quic_events.HandshakeCompleted):
             yield _HandshakeCompleted(quic_event.alpn_protocol)
         elif isinstance(quic_event, quic_events.ConnectionTerminated):
             self._terminated = True
             yield ConnectionTerminated(quic_event.error_code, quic_event.reason_phrase)
         elif isinstance(quic_event, quic_events.StreamReset):
```

### Comparing `urllib3_ext_hface-0.2.9/tests/test_http1.py` & `urllib3_ext_hface-0.3.0/tests/test_http1.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 from __future__ import annotations
 
 from typing import Any
 
 import pytest
 from helpers import build_request_headers, build_response_headers
 
-from urllib3_ext_hface import HeadersType
+from urllib3_ext_hface._typing import HeadersType
 from urllib3_ext_hface.events import ConnectionTerminated, DataReceived, HeadersReceived
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP1ClientFactory
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTPProtocolFactory, HTTP1Protocol
 
 
 @pytest.fixture(name="client")
 def _client(request: Any) -> HTTPOverTCPProtocol:
-    factory = HTTP1ClientFactory()
-    return factory(tls_version="TLS 1.2")
+    return HTTPProtocolFactory.new(HTTP1Protocol)
 
 
 def assert_connection_available(protocol: HTTPOverTCPProtocol) -> None:
     assert protocol.next_event() is None
     assert protocol.bytes_to_send() == b""
     assert protocol.is_available()
     assert not protocol.has_expired()
```

### Comparing `urllib3_ext_hface-0.2.9/tests/test_http2.py` & `urllib3_ext_hface-0.3.0/tests/test_http2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 from typing import Any, cast
 
 import hpack
 import pytest
 from helpers import build_request_headers, build_response_headers
 
-from urllib3_ext_hface import HeadersType, HeaderType
+from urllib3_ext_hface._typing import HeadersType, HeaderType
 from urllib3_ext_hface.events import (
     ConnectionTerminated,
     DataReceived,
     HeadersReceived,
     StreamResetSent,
 )
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP2ClientFactory
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTPProtocolFactory, HTTP2Protocol
 
 CLIENT_MAGIC = b"PRI * HTTP/2.0\r\n\r\nSM\r\n\r\n"
 
 
 class Frame:
     DATA = 0x00
     HEADERS = 0x01
@@ -97,16 +97,15 @@
         raise ValueError("Not a HEADERS frame.")
     decoder = hpack.Decoder()
     return cast(HeadersType, decoder.decode(frame[9:], raw=True))
 
 
 @pytest.fixture(name="client")
 def _client(request: Any) -> HTTPOverTCPProtocol:
-    factory = HTTP2ClientFactory()
-    return factory(tls_version="TLS 1.2", alpn_protocol="h2")
+    return HTTPProtocolFactory.new(HTTP2Protocol)
 
 
 def assert_connection_available(protocol: HTTPOverTCPProtocol) -> None:
     assert protocol.next_event() is None
     assert protocol.bytes_to_send() == b""
     assert protocol.is_available()
     assert not protocol.has_expired()
```

### Comparing `urllib3_ext_hface-0.2.9/tests/test_integration.py` & `urllib3_ext_hface-0.3.0/tests/test_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,39 +13,34 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import Iterator
 
 import pytest
-from helpers import build_request_headers, build_response_headers
 
 from urllib3_ext_hface.events import (
-    ConnectionTerminated,
-    DataReceived,
     Event,
-    HeadersReceived,
-    StreamResetReceived,
 )
-from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTP1ClientFactory, HTTP2ClientFactory
+from urllib3_ext_hface.protocols import HTTPOverTCPProtocol, HTTPProtocolFactory, HTTP1Protocol, HTTP2Protocol
 
 
 def _generate_http1() -> Iterator[
     tuple[str, tuple[HTTPOverTCPProtocol, HTTPOverTCPProtocol]]
 ]:
 
-    client = HTTP1ClientFactory()(tls_version="TLS 1.2")
-    yield f"http1-{HTTP1ClientFactory}", (client,)
+    client = HTTPProtocolFactory.new(HTTP1Protocol)
+    yield f"http1-{HTTP1Protocol}", (client,)
 
 
 def _generate_http2() -> Iterator[
     tuple[str, tuple[HTTPOverTCPProtocol, HTTPOverTCPProtocol]]
 ]:
-    client = HTTP2ClientFactory()(tls_version="TLS 1.2", alpn_protocol="h2")
-    yield f"http2-{HTTP2ClientFactory}", (client,)
+    client = HTTPProtocolFactory.new(HTTP2Protocol)
+    yield f"http2-{HTTP2Protocol}", (client,)
 
 
 def pytest_generate_tests(metafunc: pytest.Metafunc) -> None:
     if "client" in metafunc.fixturenames or "server" in metafunc.fixturenames:
         ids = []
         values = []
         for id, value in _generate_http1():
```

### Comparing `urllib3_ext_hface-0.2.9/LICENSE` & `urllib3_ext_hface-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/NOTICE` & `urllib3_ext_hface-0.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/README.rst` & `urllib3_ext_hface-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/pyproject.toml` & `urllib3_ext_hface-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.2.9/PKG-INFO` & `urllib3_ext_hface-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.2.9
+Version: 0.3.0
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

