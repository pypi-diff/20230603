# Comparing `tmp/aiosmtplib-2.0.1.tar.gz` & `tmp/aiosmtplib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosmtplib-2.0.1.tar", max compression
+gzip compressed data, was "aiosmtplib-2.0.2.tar", max compression
```

## Comparing `aiosmtplib-2.0.1.tar` & `aiosmtplib-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     5685 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1079 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2178 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/README.rst
--rw-r--r--   0        0        0     1270 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/__init__.py
--rw-r--r--   0        0        0      877 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/__main__.py
--rw-r--r--   0        0        0     5856 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/api.py
--rw-r--r--   0        0        0     1919 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/auth.py
--rw-r--r--   0        0        0     5417 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/email.py
--rw-r--r--   0        0        0     2980 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/errors.py
--rw-r--r--   0        0        0     2369 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/esmtp.py
--rw-r--r--   0        0        0    13547 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/protocol.py
--rw-r--r--   0        0        0       97 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/py.typed
--rw-r--r--   0        0        0      672 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/response.py
--rw-r--r--   0        0        0    54560 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/smtp.py
--rw-r--r--   0        0        0      106 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/status.py
--rw-r--r--   0        0        0     1304 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/aiosmtplib/typing.py
--rw-r--r--   0        0        0      608 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/Makefile
--rw-r--r--   0        0        0       30 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/changelog.rst
--rw-r--r--   0        0        0     6023 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/client.rst
--rw-r--r--   0        0        0     6213 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/conf.py
--rw-r--r--   0        0        0     1256 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/encryption.rst
--rw-r--r--   0        0        0      241 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/index.rst
--rw-r--r--   0        0        0       47 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/overview.rst
--rw-r--r--   0        0        0      632 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/reference.rst
--rw-r--r--   0        0        0     3835 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/docs/usage.rst
--rw-r--r--   0        0        0     2618 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/auth.py
--rw-r--r--   0        0        0    24477 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3919 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/smtpd.py
--rw-r--r--   0        0        0     6090 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/test_api.py
--rw-r--r--   0        0        0     6089 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/test_asyncio.py
--rw-r--r--   0        0        0     7635 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/test_auth_methods.py
--rw-r--r--   0        0        0     2699 2023-01-07 18:55:21.944431 aiosmtplib-2.0.1/tests/test_auth_utils.py
--rw-r--r--   0        0        0    19504 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_commands.py
--rw-r--r--   0        0        0     9232 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_config.py
--rw-r--r--   0        0        0    12621 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_connect.py
--rw-r--r--   0        0        0    10974 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_email_utils.py
--rw-r--r--   0        0        0     4413 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_errors.py
--rw-r--r--   0        0        0     1556 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_esmtp_utils.py
--rw-r--r--   0        0        0     2254 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_live.py
--rw-r--r--   0        0        0      943 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_main.py
--rw-r--r--   0        0        0     6527 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_protocol.py
--rw-r--r--   0        0        0      517 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_response.py
--rw-r--r--   0        0        0    19384 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_sendmail.py
--rw-r--r--   0        0        0      220 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_status.py
--rw-r--r--   0        0        0      677 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_sync.py
--rw-r--r--   0        0        0     5154 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_timeouts.py
--rw-r--r--   0        0        0    12443 2023-01-07 18:55:21.948431 aiosmtplib-2.0.1/tests/test_tls.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 aiosmtplib-2.0.1/setup.py
--rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 aiosmtplib-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5875 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     1079 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2178 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/README.rst
+-rw-r--r--   0        0        0     1332 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/__init__.py
+-rw-r--r--   0        0        0      877 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/__main__.py
+-rw-r--r--   0        0        0     5856 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/api.py
+-rw-r--r--   0        0        0     1919 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/auth.py
+-rw-r--r--   0        0        0     5417 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/email.py
+-rw-r--r--   0        0        0     3175 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/errors.py
+-rw-r--r--   0        0        0     2369 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/esmtp.py
+-rw-r--r--   0        0        0    13547 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/protocol.py
+-rw-r--r--   0        0        0       97 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/py.typed
+-rw-r--r--   0        0        0      672 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/response.py
+-rw-r--r--   0        0        0    54585 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/smtp.py
+-rw-r--r--   0        0        0      106 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/status.py
+-rw-r--r--   0        0        0     1304 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/aiosmtplib/typing.py
+-rw-r--r--   0        0        0      608 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/Makefile
+-rw-r--r--   0        0        0       30 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0     6023 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/client.rst
+-rw-r--r--   0        0        0     6213 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/conf.py
+-rw-r--r--   0        0        0     1256 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/encryption.rst
+-rw-r--r--   0        0        0      241 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/index.rst
+-rw-r--r--   0        0        0       47 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/overview.rst
+-rw-r--r--   0        0        0      632 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/reference.rst
+-rw-r--r--   0        0        0     3835 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/docs/usage.rst
+-rw-r--r--   0        0        0     2849 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/auth.py
+-rw-r--r--   0        0        0    24487 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     3919 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/smtpd.py
+-rw-r--r--   0        0        0     6090 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_api.py
+-rw-r--r--   0        0        0     6089 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_asyncio.py
+-rw-r--r--   0        0        0     7635 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_auth_methods.py
+-rw-r--r--   0        0        0     2699 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_auth_utils.py
+-rw-r--r--   0        0        0    19503 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_commands.py
+-rw-r--r--   0        0        0     9232 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_config.py
+-rw-r--r--   0        0        0    12629 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_connect.py
+-rw-r--r--   0        0        0    10974 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_email_utils.py
+-rw-r--r--   0        0        0     4413 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_errors.py
+-rw-r--r--   0        0        0     1556 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_esmtp_utils.py
+-rw-r--r--   0        0        0     2254 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_live.py
+-rw-r--r--   0        0        0      943 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_main.py
+-rw-r--r--   0        0        0     6527 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_protocol.py
+-rw-r--r--   0        0        0      517 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_response.py
+-rw-r--r--   0        0        0    19384 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_sendmail.py
+-rw-r--r--   0        0        0      220 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_status.py
+-rw-r--r--   0        0        0      677 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_sync.py
+-rw-r--r--   0        0        0     5154 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_timeouts.py
+-rw-r--r--   0        0        0    12443 2023-06-03 19:44:59.071944 aiosmtplib-2.0.2/tests/test_tls.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 aiosmtplib-2.0.2/setup.py
+-rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 aiosmtplib-2.0.2/PKG-INFO
```

### Comparing `aiosmtplib-2.0.1/CHANGELOG.rst` & `aiosmtplib-2.0.2/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0.2
+-----
+
+- Bugfix: don't send extra EHLO/HELO before QUIT (credit @ikrivosheev)
+- Change: added SMTPConnectionResponseError for invalid response on
+  connect only (credit @ikrivosheev)
+
 2.0.1
 -----
 
 - Bugfix: "tests" and "docs" in the sdist should be includes, not packages,
   so that they do not get put in ``site-packages``.
```

### Comparing `aiosmtplib-2.0.1/LICENSE.txt` & `aiosmtplib-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/README.rst` & `aiosmtplib-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/__init__.py` & `aiosmtplib-2.0.2/aiosmtplib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,23 @@
     SMTPReadTimeoutError,
     SMTPRecipientRefused,
     SMTPRecipientsRefused,
     SMTPResponseException,
     SMTPSenderRefused,
     SMTPServerDisconnected,
     SMTPTimeoutError,
+    SMTPConnectResponseError,
 )
 from .response import SMTPResponse
 from .smtp import SMTP
 from .typing import SMTPStatus
 
 
 __title__ = "aiosmtplib"
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 __author__ = "Cole Maclean"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 Cole Maclean"
 __all__ = (
     "send",
     "SMTP",
     "SMTPResponse",
@@ -51,8 +52,9 @@
     "SMTPRecipientsRefused",
     "SMTPResponseException",
     "SMTPSenderRefused",
     "SMTPServerDisconnected",
     "SMTPTimeoutError",
     "SMTPConnectTimeoutError",
     "SMTPReadTimeoutError",
+    "SMTPConnectResponseError",
 )
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/__main__.py` & `aiosmtplib-2.0.2/aiosmtplib/__main__.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/api.py` & `aiosmtplib-2.0.2/aiosmtplib/api.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/auth.py` & `aiosmtplib-2.0.2/aiosmtplib/auth.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/email.py` & `aiosmtplib-2.0.2/aiosmtplib/email.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/errors.py` & `aiosmtplib-2.0.2/aiosmtplib/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "SMTPRecipientsRefused",
     "SMTPResponseException",
     "SMTPSenderRefused",
     "SMTPServerDisconnected",
     "SMTPTimeoutError",
     "SMTPConnectTimeoutError",
     "SMTPReadTimeoutError",
+    "SMTPConnectResponseError",
 )
 
 
 class SMTPException(Exception):
     """
     Base class for all SMTP exceptions.
     """
@@ -74,14 +75,20 @@
 
     def __init__(self, code: int, message: str) -> None:
         self.code = code
         self.message = message
         self.args = (code, message)
 
 
+class SMTPConnectResponseError(SMTPResponseException, SMTPConnectError):
+    """
+    The SMTP server returned an invalid response code after connecting.
+    """
+
+
 class SMTPHeloError(SMTPResponseException):
     """
     Server refused HELO or EHLO.
     """
 
 
 class SMTPDataError(SMTPResponseException):
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/esmtp.py` & `aiosmtplib-2.0.2/aiosmtplib/esmtp.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/protocol.py` & `aiosmtplib-2.0.2/aiosmtplib/protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/response.py` & `aiosmtplib-2.0.2/aiosmtplib/response.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/smtp.py` & `aiosmtplib-2.0.2/aiosmtplib/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     SMTPNotSupported,
     SMTPRecipientRefused,
     SMTPRecipientsRefused,
     SMTPResponseException,
     SMTPSenderRefused,
     SMTPServerDisconnected,
     SMTPTimeoutError,
+    SMTPConnectResponseError,
 )
 from .esmtp import parse_esmtp_extensions
 from .protocol import SMTPProtocol
 from .response import SMTPResponse
 from .typing import Default, SMTPStatus, SocketPathType, _default
 
 
@@ -517,15 +518,15 @@
             ) from exc
         except SMTPTimeoutError as exc:
             raise SMTPConnectTimeoutError(
                 "Timed out waiting for server ready message"
             ) from exc
 
         if response.code != SMTPStatus.ready:
-            raise SMTPConnectError(str(response))
+            raise SMTPConnectResponseError(response.code, response.message)
 
         return response
 
     def _connection_lost(self, waiter: "asyncio.Future[None]") -> None:
         if waiter.cancelled() or waiter.exception() is not None:
             self.close()
 
@@ -789,17 +790,14 @@
     ) -> SMTPResponse:
         """
         Send the SMTP QUIT command, which closes the connection.
         Also closes the connection from our side after a response is received.
 
         :raises SMTPResponseException: on unexpected server response code
         """
-        # Can't quit without HELO/EHLO
-        await self._ehlo_or_helo_if_needed()
-
         response = await self.execute_command(b"QUIT", timeout=timeout)
         if response.code != SMTPStatus.closing:
             raise SMTPResponseException(response.code, response.message)
 
         self.close()
 
         return response
@@ -1051,16 +1049,18 @@
 
         response: Optional[SMTPResponse] = None
         exception: Optional[SMTPAuthenticationError] = None
         for auth_name in self.supported_auth_methods:
             method_name = f'auth_{auth_name.replace("-", "")}'
             try:
                 auth_method = getattr(self, method_name)
-            except AttributeError:
-                raise RuntimeError(f"Missing handler for auth method {auth_name}")
+            except AttributeError as err:
+                raise RuntimeError(
+                    f"Missing handler for auth method {auth_name}"
+                ) from err
             try:
                 response = await auth_method(username, password, timeout=timeout)
             except SMTPAuthenticationError as exc:
                 exception = exc
             else:
                 # No exception means we're good
                 break
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/typing.py` & `aiosmtplib-2.0.2/aiosmtplib/typing.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/Makefile` & `aiosmtplib-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/client.rst` & `aiosmtplib-2.0.2/docs/client.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/conf.py` & `aiosmtplib-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/encryption.rst` & `aiosmtplib-2.0.2/docs/encryption.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/reference.rst` & `aiosmtplib-2.0.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/usage.rst` & `aiosmtplib-2.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/pyproject.toml` & `aiosmtplib-2.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aiosmtplib"
-version = "2.0.1"
+version = "2.0.2"
 description = "asyncio SMTP client"
 authors = ["Cole Maclean <hi@colemaclean.dev>"]
 license = "MIT"
 packages = [
     { include = "aiosmtplib" },
 ]
 readme = "README.rst"
@@ -74,28 +74,38 @@
 [tool.poetry.group.security]
 optional = true
 
 [tool.poetry.group.security.dependencies]
 bandit = "^1.7.4"
 safety = "^2.3.1"
 
+[tool.poetry.group.lint]
+optional = true
+
+[tool.poetry.group.lint.dependencies]
+ruff = "^0.0.244"
+
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 minversion = "6.0"
 junit_family = "xunit2"
 addopts = "--strict-markers"
 testpaths = [
     "tests"
 ]
 
-[tool.isort]
-profile = "black"
-lines_after_imports = 2
-default_section = "THIRDPARTY"
-known_first_party = [ "aiosmtplib" ]
+[tool.ruff]
+# Enable flake8-bugbear (`B`) rules.
+select = ["E", "F", "B"]
+# Never enforce `E501` (line length violations).
+ignore = ["E501"]
+# Avoid trying to fix flake8-bugbear (`B`) violations.
+unfixable = ["B"]
+line-length = 88
+target-version = "py37"
 
 [tool.coverage]
 
 [tool.coverage.run]
 source = [ "aiosmtplib" ]
 branch = true
 parallel = true
```

### Comparing `aiosmtplib-2.0.1/tests/auth.py` & `aiosmtplib-2.0.2/tests/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Deque, List, Tuple
 
 from aiosmtplib.response import SMTPResponse
 from aiosmtplib.smtp import SMTP
 
 
 class DummySMTPAuth(SMTP):
-
     transport = None
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
         self.received_commands: List[bytes] = []
         self.responses: Deque[Tuple[int, str]] = deque()
```

### Comparing `aiosmtplib-2.0.1/tests/conftest.py` & `aiosmtplib-2.0.2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,17 +395,17 @@
             smtpd.session.host_name = args[0]
         await smtpd.push("250 done")
 
     return mock_response_done
 
 
 @pytest.fixture(scope="session")
-def smtpd_mock_response_done_then_close() -> Callable[
-    [SMTPD], Coroutine[Any, Any, None]
-]:
+def smtpd_mock_response_done_then_close() -> (
+    Callable[[SMTPD], Coroutine[Any, Any, None]]
+):
     async def mock_response_done_then_close(
         smtpd: SMTPD, *args: Any, **kwargs: Any
     ) -> None:
         if args and args[0]:
             smtpd.session.host_name = args[0]
         await smtpd.push("250 done")
         await smtpd.push("221 bye now")
@@ -419,17 +419,17 @@
     async def mock_response_error(smtpd: SMTPD, *args: Any, **kwargs: Any) -> None:
         await smtpd.push("555 error")
 
     return mock_response_error
 
 
 @pytest.fixture(scope="session")
-def smtpd_mock_response_error_disconnect() -> Callable[
-    [SMTPD], Coroutine[Any, Any, None]
-]:
+def smtpd_mock_response_error_disconnect() -> (
+    Callable[[SMTPD], Coroutine[Any, Any, None]]
+):
     async def mock_response_error_disconnect(
         smtpd: SMTPD, *args: Any, **kwargs: Any
     ) -> None:
         await smtpd.push("501 error")
         await smtpd.transport.close()
 
     return mock_response_error_disconnect
@@ -511,27 +511,27 @@
         await smtpd.push("421 retry in 5 minutes")
         await smtpd.transport.close()
 
     return mock_response_unavailable
 
 
 @pytest.fixture(scope="session")
-def smtpd_mock_response_tls_not_available() -> Callable[
-    [SMTPD], Coroutine[Any, Any, None]
-]:
+def smtpd_mock_response_tls_not_available() -> (
+    Callable[[SMTPD], Coroutine[Any, Any, None]]
+):
     async def mock_tls_not_available(smtpd: SMTPD, *args: Any, **kwargs: Any) -> None:
         await smtpd.push("454 please login")
 
     return mock_tls_not_available
 
 
 @pytest.fixture(scope="session")
-def smtpd_mock_response_tls_ready_disconnect() -> Callable[
-    [SMTPD], Coroutine[Any, Any, None]
-]:
+def smtpd_mock_response_tls_ready_disconnect() -> (
+    Callable[[SMTPD], Coroutine[Any, Any, None]]
+):
     async def mock_response_tls_ready_disconnect(
         smtpd: SMTPD, *args: Any, **kwargs: Any
     ) -> None:
         await smtpd.push("220 go for it")
         await smtpd.transport.close()
 
     return mock_response_tls_ready_disconnect
@@ -550,17 +550,17 @@
     async def mock_response_eof(smtpd: SMTPD, *args: Any, **kwargs: Any) -> None:
         await smtpd.transport.write_eof()
 
     return mock_response_eof
 
 
 @pytest.fixture(scope="session")
-def smtpd_mock_response_error_with_code_factory() -> Callable[
-    [str], Callable[[SMTPD], Coroutine[Any, Any, None]]
-]:
+def smtpd_mock_response_error_with_code_factory() -> (
+    Callable[[str], Callable[[SMTPD], Coroutine[Any, Any, None]]]
+):
     def factory(error_code: str) -> Callable[[SMTPD], Coroutine[Any, Any, None]]:
         async def mock_error_response(smtpd: SMTPD, *args: Any, **kwargs: Any) -> None:
             await smtpd.push(f"{error_code} error")
 
         return mock_error_response
 
     return factory
```

### Comparing `aiosmtplib-2.0.1/tests/smtpd.py` & `aiosmtplib-2.0.2/tests/smtpd.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_api.py` & `aiosmtplib-2.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_asyncio.py` & `aiosmtplib-2.0.2/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_auth_methods.py` & `aiosmtplib-2.0.2/tests/test_auth_methods.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_auth_utils.py` & `aiosmtplib-2.0.2/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_commands.py` & `aiosmtplib-2.0.2/tests/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,14 @@
 async def test_ehlo_or_helo_if_needed_disconnect_after_ehlo(
     smtp_client: SMTP,
     smtpd_server: asyncio.AbstractServer,
     smtpd_class: Type[SMTPD],
     smtpd_mock_response_unavailable: Callable,
     monkeypatch: pytest.MonkeyPatch,
 ) -> None:
-
     monkeypatch.setattr(smtpd_class, "smtp_EHLO", smtpd_mock_response_unavailable)
 
     async with smtp_client:
         with pytest.raises(SMTPHeloError):
             await smtp_client._ehlo_or_helo_if_needed()
```

### Comparing `aiosmtplib-2.0.1/tests/test_config.py` & `aiosmtplib-2.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_connect.py` & `aiosmtplib-2.0.2/tests/test_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 async def test_context_manager_exception_quits(
     smtp_client: SMTP,
     smtpd_server: asyncio.AbstractServer,
     received_commands: List[Tuple[str, Tuple[Any, ...]]],
 ) -> None:
     with pytest.raises(ZeroDivisionError):
         async with smtp_client:
-            1 / 0
+            1 / 0  # noqa
 
     assert received_commands[-1][0] == "QUIT"
 
 
 async def test_context_manager_connect_exception_closes(
     smtp_client: SMTP,
     smtpd_server: asyncio.AbstractServer,
```

### Comparing `aiosmtplib-2.0.1/tests/test_email_utils.py` & `aiosmtplib-2.0.2/tests/test_email_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_errors.py` & `aiosmtplib-2.0.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_esmtp_utils.py` & `aiosmtplib-2.0.2/tests/test_esmtp_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_live.py` & `aiosmtplib-2.0.2/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_main.py` & `aiosmtplib-2.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_protocol.py` & `aiosmtplib-2.0.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_response.py` & `aiosmtplib-2.0.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_sendmail.py` & `aiosmtplib-2.0.2/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_sync.py` & `aiosmtplib-2.0.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_timeouts.py` & `aiosmtplib-2.0.2/tests/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_tls.py` & `aiosmtplib-2.0.2/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/setup.py` & `aiosmtplib-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                                                                'uvloop>=0.14,<0.15'],
  'uvloop:python_version >= "3.9" and python_version < "4.0"': ['uvloop>=0.17,<0.18',
                                                                'uvloop>=0.17,<0.18',
                                                                'uvloop>=0.17,<0.18']}
 
 setup_kwargs = {
     'name': 'aiosmtplib',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'asyncio SMTP client',
     'long_description': 'aiosmtplib\n==========\n\n|circleci| |precommit.ci| |codecov| |pypi-version| |pypi-status| |downloads| |pypi-python-versions|\n|pypi-license|\n\n------------\n\naiosmtplib is an asynchronous SMTP client for use with asyncio.\n\nFor documentation, see `Read The Docs`_.\n\nQuickstart\n----------\n\n.. code-block:: python\n\n    import asyncio\n    from email.message import EmailMessage\n\n    import aiosmtplib\n\n    message = EmailMessage()\n    message["From"] = "root@localhost"\n    message["To"] = "somebody@example.com"\n    message["Subject"] = "Hello World!"\n    message.set_content("Sent via aiosmtplib")\n\n    asyncio.run(aiosmtplib.send(message, hostname="127.0.0.1", port=25))\n\n\nRequirements\n------------\nPython 3.7+, compiled with SSL support, is required.\n\n\nBug Reporting\n-------------\nBug reports (and feature requests) are welcome via `Github issues`_.\n\n\n\n.. |circleci| image:: https://circleci.com/gh/cole/aiosmtplib/tree/main.svg?style=shield\n           :target: https://circleci.com/gh/cole/aiosmtplib/tree/main\n           :alt: "aiosmtplib CircleCI build status"\n.. |pypi-version| image:: https://img.shields.io/pypi/v/aiosmtplib.svg\n                 :target: https://pypi.python.org/pypi/aiosmtplib\n                 :alt: "aiosmtplib on the Python Package Index"\n.. |pypi-python-versions| image:: https://img.shields.io/pypi/pyversions/aiosmtplib.svg\n.. |pypi-status| image:: https://img.shields.io/pypi/status/aiosmtplib.svg\n.. |pypi-license| image:: https://img.shields.io/pypi/l/aiosmtplib.svg\n.. |codecov| image:: https://codecov.io/gh/cole/aiosmtplib/branch/main/graph/badge.svg\n             :target: https://codecov.io/gh/cole/aiosmtplib\n.. |downloads| image:: https://pepy.tech/badge/aiosmtplib\n               :target: https://pepy.tech/project/aiosmtplib\n               :alt: "aiosmtplib on pypy.tech"\n.. |precommit.ci| image:: https://results.pre-commit.ci/badge/github/cole/aiosmtplib/main.svg\n                  :target: https://results.pre-commit.ci/latest/github/cole/aiosmtplib/main\n                  :alt: "pre-commit.ci status"\n.. _Read The Docs: https://aiosmtplib.readthedocs.io/en/stable/overview.html\n.. _Github issues: https://github.com/cole/aiosmtplib/issues\n',
     'author': 'Cole Maclean',
     'author_email': 'hi@colemaclean.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cole/aiosmtplib',
```

### Comparing `aiosmtplib-2.0.1/PKG-INFO` & `aiosmtplib-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmtplib
-Version: 2.0.1
+Version: 2.0.2
 Summary: asyncio SMTP client
 Home-page: https://github.com/cole/aiosmtplib
 License: MIT
 Keywords: smtp,email,asyncio
 Author: Cole Maclean
 Author-email: hi@colemaclean.dev
 Requires-Python: >=3.7,<4.0
```

