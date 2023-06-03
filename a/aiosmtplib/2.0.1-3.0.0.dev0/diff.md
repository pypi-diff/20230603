# Comparing `tmp/aiosmtplib-2.0.1.tar.gz` & `tmp/aiosmtplib-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosmtplib-2.0.1.tar", max compression
+gzip compressed data, was "aiosmtplib-3.0.0.dev0.tar", max compression
```

## Comparing `aiosmtplib-2.0.1.tar` & `aiosmtplib-3.0.0.dev0.tar`

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
+-rw-r--r--   0        0        0     6154 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1079 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/LICENSE.txt
+-rw-r--r--   0        0        0     2178 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/README.rst
+-rw-r--r--   0        0        0     1336 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/__init__.py
+-rw-r--r--   0        0        0      877 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/__main__.py
+-rw-r--r--   0        0        0     5863 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/api.py
+-rw-r--r--   0        0        0     1940 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/auth.py
+-rw-r--r--   0        0        0     5447 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/email.py
+-rw-r--r--   0        0        0     3190 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/errors.py
+-rw-r--r--   0        0        0     2369 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/esmtp.py
+-rw-r--r--   0        0        0    13547 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/protocol.py
+-rw-r--r--   0        0        0       97 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/py.typed
+-rw-r--r--   0        0        0      672 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/response.py
+-rw-r--r--   0        0        0    54922 2023-06-03 19:39:45.143750 aiosmtplib-3.0.0.dev0/aiosmtplib/smtp.py
+-rw-r--r--   0        0        0      106 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/aiosmtplib/status.py
+-rw-r--r--   0        0        0     1304 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/aiosmtplib/typing.py
+-rw-r--r--   0        0        0      608 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/Makefile
+-rw-r--r--   0        0        0       30 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/changelog.rst
+-rw-r--r--   0        0        0     6002 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/client.rst
+-rw-r--r--   0        0        0     6213 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/conf.py
+-rw-r--r--   0        0        0     1256 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/encryption.rst
+-rw-r--r--   0        0        0      241 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/index.rst
+-rw-r--r--   0        0        0       47 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/overview.rst
+-rw-r--r--   0        0        0      632 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/reference.rst
+-rw-r--r--   0        0        0     3835 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/docs/usage.rst
+-rw-r--r--   0        0        0     2853 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/auth.py
+-rw-r--r--   0        0        0    24487 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/conftest.py
+-rw-r--r--   0        0        0     3919 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/smtpd.py
+-rw-r--r--   0        0        0     6090 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_api.py
+-rw-r--r--   0        0        0     6089 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     7635 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_auth_methods.py
+-rw-r--r--   0        0        0     2699 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_auth_utils.py
+-rw-r--r--   0        0        0    19503 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_commands.py
+-rw-r--r--   0        0        0     9227 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_config.py
+-rw-r--r--   0        0        0    12629 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_connect.py
+-rw-r--r--   0        0        0    10974 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_email_utils.py
+-rw-r--r--   0        0        0     4413 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_errors.py
+-rw-r--r--   0        0        0     1556 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_esmtp_utils.py
+-rw-r--r--   0        0        0     2254 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_live.py
+-rw-r--r--   0        0        0      943 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_main.py
+-rw-r--r--   0        0        0     6527 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_protocol.py
+-rw-r--r--   0        0        0      517 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_response.py
+-rw-r--r--   0        0        0    19384 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_sendmail.py
+-rw-r--r--   0        0        0      220 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_status.py
+-rw-r--r--   0        0        0      677 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_sync.py
+-rw-r--r--   0        0        0     5154 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_timeouts.py
+-rw-r--r--   0        0        0    12443 2023-06-03 19:39:45.147750 aiosmtplib-3.0.0.dev0/tests/test_tls.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 aiosmtplib-3.0.0.dev0/setup.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 aiosmtplib-3.0.0.dev0/PKG-INFO
```

### Comparing `aiosmtplib-2.0.1/CHANGELOG.rst` & `aiosmtplib-3.0.0.dev0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changelog
 =========
 
+3.0.0 (unreleased)
+------------------
+
+- **BREAKING**: Drop Python 3.7 support.
+- **BREAKING**: Positional and keyword argument usage is now enforced.
+- Change: added SMTPConnectionResponseError for invalid response on
+  connect only (credit @ikrivosheev)
+- Change: don't use timeout value passed to ``connect`` everywhere,
+  only for the initial connection (credit @wombatonfire)
+
+
+2.0.2
+-----
+
+- Bugfix: don't send extra EHLO/HELO before QUIT (credit @ikrivosheev)
+
+
 2.0.1
 -----
 
 - Bugfix: "tests" and "docs" in the sdist should be includes, not packages,
   so that they do not get put in ``site-packages``.
```

### Comparing `aiosmtplib-2.0.1/LICENSE.txt` & `aiosmtplib-3.0.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/README.rst` & `aiosmtplib-3.0.0.dev0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     message.set_content("Sent via aiosmtplib")
 
     asyncio.run(aiosmtplib.send(message, hostname="127.0.0.1", port=25))
 
 
 Requirements
 ------------
-Python 3.7+, compiled with SSL support, is required.
+Python 3.8+, compiled with SSL support, is required.
 
 
 Bug Reporting
 -------------
 Bug reports (and feature requests) are welcome via `Github issues`_.
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/__init__.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/__init__.py`

 * *Files 2% similar despite different names*

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
+__version__ = "3.0.0dev0"
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

### Comparing `aiosmtplib-2.0.1/aiosmtplib/__main__.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/__main__.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/api.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 __all__ = ("send",)
 
 
 async def send(
     message: Union[email.message.EmailMessage, email.message.Message, str, bytes],
+    /,
     sender: Optional[str] = None,
     recipients: Optional[Union[str, Sequence[str]]] = None,
     mail_options: Optional[Sequence[str]] = None,
     rcpt_options: Optional[Sequence[str]] = None,
     hostname: Optional[str] = "localhost",
     port: Optional[int] = None,
     username: Optional[Union[str, bytes]] = None,
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/auth.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     return value.encode("utf-8")
 
 
 def auth_crammd5_verify(
     username: Union[str, bytes],
     password: Union[str, bytes],
     challenge: Union[str, bytes],
+    /,
 ) -> bytes:
     """
     CRAM-MD5 auth uses the password as a shared secret to MD5 the server's
     response, and sends the username combined with that (base64 encoded).
     """
     username_bytes = _ensure_bytes(username)
     password_bytes = _ensure_bytes(password)
@@ -35,14 +36,15 @@
 
     return encoded_verification
 
 
 def auth_plain_encode(
     username: Union[str, bytes],
     password: Union[str, bytes],
+    /,
 ) -> bytes:
     """
     PLAIN auth base64 encodes the username and password together.
     """
     username_bytes = _ensure_bytes(username)
     password_bytes = _ensure_bytes(password)
 
@@ -51,14 +53,15 @@
 
     return encoded
 
 
 def auth_login_encode(
     username: Union[str, bytes],
     password: Union[str, bytes],
+    /,
 ) -> Tuple[bytes, bytes]:
     """
     LOGIN auth base64 encodes the username and password and sends them
     in sequence.
     """
     username_bytes = _ensure_bytes(username)
     password_bytes = _ensure_bytes(password)
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/email.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             return f"{quotes}{name}{quotes} <{address}>"
 
     return address
 
 
 def flatten_message(
     message: Union[email.message.EmailMessage, email.message.Message],
+    /,
     utf8: bool = False,
     cte_type: str = "8bit",
 ) -> bytes:
     # Make a local copy so we can delete the bcc headers.
     message_copy = copy.copy(message)
     del message_copy["Bcc"]
     del message_copy["Resent-Bcc"]
@@ -99,14 +100,15 @@
         flat_message = messageio.getvalue()
 
     return flat_message
 
 
 def extract_addresses(
     header: Union[str, email.headerregistry.AddressHeader, email.header.Header],
+    /,
 ) -> List[str]:
     """
     Convert address headers into raw email addresses, suitable for use in
     low level SMTP commands.
     """
     addresses = []
     if isinstance(header, email.headerregistry.AddressHeader):
@@ -125,15 +127,16 @@
     else:
         addresses.extend(addr for _, addr in email.utils.getaddresses([header]))
 
     return addresses
 
 
 def extract_sender(
-    message: Union[email.message.EmailMessage, email.message.Message]
+    message: Union[email.message.EmailMessage, email.message.Message],
+    /,
 ) -> Optional[str]:
     """
     Extract the sender from the message object given.
     """
     resent_dates = message.get_all("Resent-Date")
 
     if resent_dates is not None and len(resent_dates) > 1:
@@ -154,15 +157,16 @@
     if sender_header is None:
         return None
 
     return extract_addresses(sender_header)[0]
 
 
 def extract_recipients(
-    message: Union[email.message.EmailMessage, email.message.Message]
+    message: Union[email.message.EmailMessage, email.message.Message],
+    /,
 ) -> List[str]:
     """
     Extract the recipients from the message object given.
     """
     recipients: List[str] = []
 
     resent_dates = message.get_all("Resent-Date")
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/errors.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
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
 
-    def __init__(self, message: str) -> None:
+    def __init__(self, message: str, /) -> None:
         self.message = message
         self.args = (message,)
 
 
 class SMTPServerDisconnected(SMTPException, ConnectionError):
     """
     The connection was lost unexpectedly, or a command was run that requires
@@ -68,20 +69,26 @@
 
 
 class SMTPResponseException(SMTPException):
     """
     Base class for all server responses with error codes.
     """
 
-    def __init__(self, code: int, message: str) -> None:
+    def __init__(self, code: int, message: str, /) -> None:
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
@@ -97,34 +104,34 @@
 
 
 class SMTPSenderRefused(SMTPResponseException):
     """
     SMTP server refused the message sender.
     """
 
-    def __init__(self, code: int, message: str, sender: str) -> None:
+    def __init__(self, code: int, message: str, sender: str, /) -> None:
         self.code = code
         self.message = message
         self.sender = sender
         self.args = (code, message, sender)
 
 
 class SMTPRecipientRefused(SMTPResponseException):
     """
     SMTP server refused a message recipient.
     """
 
-    def __init__(self, code: int, message: str, recipient: str) -> None:
+    def __init__(self, code: int, message: str, recipient: str, /) -> None:
         self.code = code
         self.message = message
         self.recipient = recipient
         self.args = (code, message, recipient)
 
 
 class SMTPRecipientsRefused(SMTPException):
     """
     SMTP server refused multiple recipients.
     """
 
-    def __init__(self, recipients: List[SMTPRecipientRefused]) -> None:
+    def __init__(self, recipients: List[SMTPRecipientRefused], /) -> None:
         self.recipients = recipients
         self.args = (recipients,)
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/esmtp.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/esmtp.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/protocol.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/response.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/response.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/aiosmtplib/smtp.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/smtp.py`

 * *Files 2% similar despite different names*

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
 
 
@@ -60,28 +61,31 @@
         >>> recipients = ["somebody@localhost"]
         >>> message = "Hello World"
         >>> send = smtp.sendmail(sender, recipients, "Hello World")
         >>> event_loop.run_until_complete(send)
         ({}, 'OK')
 
     Keyword arguments can be provided either on :meth:`__init__` or when
-    calling the :meth:`connect` method. Note that in both cases these options
-    are saved for later use; subsequent calls to :meth:`connect` will use the
-    same options, unless new ones are provided.
+    calling the :meth:`connect` method. Note that in both cases these options,
+    except for ``timeout``, are saved for later use; subsequent calls to
+    :meth:`connect` will use the same options, unless new ones are provided.
+    ``timeout`` is saved for later use when provided on :meth:`__init__`, but
+    not when calling the :meth:`connect` method.
     """
 
     # Preferred methods first
     AUTH_METHODS: Tuple[str, ...] = (
         "cram-md5",
         "plain",
         "login",
     )
 
     def __init__(
         self,
+        /,
         hostname: Optional[str] = "localhost",
         port: Optional[int] = None,
         username: Optional[Union[str, bytes]] = None,
         password: Optional[Union[str, bytes]] = None,
         local_hostname: Optional[str] = None,
         source_address: Optional[Tuple[str, int]] = None,
         timeout: Optional[float] = DEFAULT_TIMEOUT,
@@ -245,15 +249,14 @@
         self,
         hostname: Optional[Union[str, Default]] = _default,
         port: Optional[Union[int, Default]] = _default,
         username: Optional[Union[str, bytes, Default]] = _default,
         password: Optional[Union[str, bytes, Default]] = _default,
         local_hostname: Optional[Union[str, Default]] = _default,
         source_address: Optional[Union[Tuple[str, int], Default]] = _default,
-        timeout: Optional[Union[float, Default]] = _default,
         use_tls: Optional[bool] = None,
         start_tls: Optional[Union[bool, Default]] = _default,
         validate_certs: Optional[bool] = None,
         client_cert: Optional[Union[str, Default]] = _default,
         client_key: Optional[Union[str, Default]] = _default,
         tls_context: Optional[Union[ssl.SSLContext, Default]] = _default,
         cert_bundle: Optional[Union[str, Default]] = _default,
@@ -275,16 +278,14 @@
         if port is not _default:
             self.port = port
         if username is not _default:
             self._login_username = username
         if password is not _default:
             self._login_password = password
 
-        if timeout is not _default:
-            self.timeout = timeout
         if local_hostname is not _default:
             self._local_hostname = local_hostname
         if source_address is not _default:
             if isinstance(source_address, str):
                 warnings.warn(
                     "The source_address keyword has been renamed to local_hostname "
                     "to match smtplib more closely.",
@@ -349,14 +350,15 @@
         elif self._start_tls_on_connect:
             return SMTP_STARTTLS_PORT
 
         return SMTP_PORT
 
     async def connect(
         self,
+        /,
         hostname: Optional[Union[str, Default]] = _default,
         port: Optional[Union[int, Default]] = _default,
         username: Optional[Union[str, bytes, Default]] = _default,
         password: Optional[Union[str, bytes, Default]] = _default,
         local_hostname: Optional[Union[str, Default]] = _default,
         source_address: Optional[Union[Tuple[str, int], Default]] = _default,
         timeout: Optional[Union[float, Default]] = _default,
@@ -412,15 +414,14 @@
         :raises ValueError: mutually exclusive options provided
         """
         self._update_settings_from_kwargs(
             hostname=hostname,
             port=port,
             local_hostname=local_hostname,
             source_address=source_address,
-            timeout=timeout,
             use_tls=use_tls,
             start_tls=start_tls,
             validate_certs=validate_certs,
             client_cert=client_cert,
             client_key=client_key,
             tls_context=tls_context,
             cert_bundle=cert_bundle,
@@ -438,46 +439,48 @@
 
         # Set default port last in case use_tls or start_tls is provided,
         # and only if we're not using a socket.
         if self.port is None and self.sock is None and self.socket_path is None:
             self.port = self._get_default_port()
 
         try:
-            response = await self._create_connection()
+            response = await self._create_connection(
+                timeout=self.timeout if timeout is _default else timeout
+            )
         except Exception as exc:
             self.close()  # Reset our state to disconnected
             raise exc
 
         await self._maybe_start_tls_on_connect()
         await self._maybe_login_on_connect()
 
         return response
 
-    async def _create_connection(self) -> SMTPResponse:
+    async def _create_connection(self, timeout: Optional[float]) -> SMTPResponse:
         if self.loop is None:
             raise RuntimeError("No event loop set")
 
         protocol = SMTPProtocol(
             loop=self.loop, connection_lost_callback=self._connection_lost
         )
 
         tls_context: Optional[ssl.SSLContext] = None
         ssl_handshake_timeout: Optional[float] = None
         if self.use_tls:
             tls_context = self._get_tls_context()
-            ssl_handshake_timeout = self.timeout
+            ssl_handshake_timeout = timeout
 
-        if self.sock:
+        if self.sock is not None:
             connect_coro = self.loop.create_connection(
                 lambda: protocol,
                 sock=self.sock,
                 ssl=tls_context,
                 ssl_handshake_timeout=ssl_handshake_timeout,
             )
-        elif self.socket_path:
+        elif self.socket_path is not None:
             connect_coro = self.loop.create_unix_connection(
                 lambda: protocol,
                 path=self.socket_path,  # type: ignore
                 ssl=tls_context,
                 ssl_handshake_timeout=ssl_handshake_timeout,
             )
         else:
@@ -492,40 +495,40 @@
                 port=self.port,
                 ssl=tls_context,
                 ssl_handshake_timeout=ssl_handshake_timeout,
                 local_addr=self.source_address,
             )
 
         try:
-            transport, _ = await asyncio.wait_for(connect_coro, timeout=self.timeout)
+            transport, _ = await asyncio.wait_for(connect_coro, timeout=timeout)
         except (TimeoutError, asyncio.TimeoutError) as exc:
             raise SMTPConnectTimeoutError(
                 f"Timed out connecting to {self.hostname} on port {self.port}"
             ) from exc
         except OSError as exc:
             raise SMTPConnectError(
                 f"Error connecting to {self.hostname} on port {self.port}: {exc}"
             ) from exc
 
         self.protocol = protocol
         self.transport = transport
 
         try:
-            response = await protocol.read_response(timeout=self.timeout)
+            response = await protocol.read_response(timeout=timeout)
         except SMTPServerDisconnected as exc:
             raise SMTPConnectError(
                 f"Error connecting to {self.hostname} on port {self.port}: {exc}"
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
 
@@ -636,14 +639,15 @@
 
         return self.transport.get_extra_info(key)
 
     # Base SMTP commands #
 
     async def helo(
         self,
+        /,
         hostname: Optional[str] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send the SMTP HELO command.
         Hostname to send for this command defaults to the FQDN of the local
         host.
@@ -655,15 +659,15 @@
         )
 
         if response.code != SMTPStatus.completed:
             raise SMTPHeloError(response.code, response.message)
 
         return response
 
-    async def help(self, timeout: Optional[Union[float, Default]] = _default) -> str:
+    async def help(self, /, timeout: Optional[Union[float, Default]] = _default) -> str:
         """
         Send the SMTP HELP command, which responds with help text.
 
         :raises SMTPResponseException: on unexpected server response code
         """
         await self._ehlo_or_helo_if_needed()
 
@@ -674,15 +678,15 @@
             SMTPStatus.completed,
         ):
             raise SMTPResponseException(response.code, response.message)
 
         return response.message
 
     async def rset(
-        self, timeout: Optional[Union[float, Default]] = _default
+        self, /, timeout: Optional[Union[float, Default]] = _default
     ) -> SMTPResponse:
         """
         Send an SMTP RSET command, which resets the server's envelope
         (the envelope contains the sender, recipient, and mail data).
 
         :raises SMTPResponseException: on unexpected server response code
         """
@@ -691,15 +695,15 @@
         response = await self.execute_command(b"RSET", timeout=timeout)
         if response.code != SMTPStatus.completed:
             raise SMTPResponseException(response.code, response.message)
 
         return response
 
     async def noop(
-        self, timeout: Optional[Union[float, Default]] = _default
+        self, /, timeout: Optional[Union[float, Default]] = _default
     ) -> SMTPResponse:
         """
         Send an SMTP NOOP command, which does nothing.
 
         :raises SMTPResponseException: on unexpected server response code
         """
         await self._ehlo_or_helo_if_needed()
@@ -709,14 +713,15 @@
             raise SMTPResponseException(response.code, response.message)
 
         return response
 
     async def vrfy(
         self,
         address: str,
+        /,
         options: Optional[Iterable[str]] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send an SMTP VRFY command, which tests an address for validity.
         Not many servers support this command.
 
@@ -748,14 +753,15 @@
             raise SMTPResponseException(response.code, response.message)
 
         return response
 
     async def expn(
         self,
         address: str,
+        /,
         options: Optional[Iterable[str]] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send an SMTP EXPN command, which expands a mailing list.
         Not many servers support this command.
 
@@ -781,36 +787,34 @@
 
         if response.code != SMTPStatus.completed:
             raise SMTPResponseException(response.code, response.message)
 
         return response
 
     async def quit(
-        self, timeout: Optional[Union[float, Default]] = _default
+        self, /, timeout: Optional[Union[float, Default]] = _default
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
 
     async def mail(
         self,
         sender: str,
+        /,
         options: Optional[Iterable[str]] = None,
         encoding: str = "ascii",
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send an SMTP MAIL command, which specifies the message sender and
         begins a new mail transfer session ("envelope").
@@ -834,14 +838,15 @@
             raise SMTPSenderRefused(response.code, response.message, sender)
 
         return response
 
     async def rcpt(
         self,
         recipient: str,
+        /,
         options: Optional[Iterable[str]] = None,
         encoding: str = "ascii",
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send an SMTP RCPT command, which specifies a single recipient for
         the message. This command is sent once per recipient and must be
@@ -866,14 +871,15 @@
             raise SMTPRecipientRefused(response.code, response.message, recipient)
 
         return response
 
     async def data(
         self,
         message: Union[str, bytes],
+        /,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send an SMTP DATA command, followed by the message given.
         This method transfers the actual email content to the server.
 
         :raises SMTPDataError: on unexpected server response code
@@ -893,14 +899,15 @@
 
         return await self.protocol.execute_data_command(message, timeout=timeout)
 
     # ESMTP commands #
 
     async def ehlo(
         self,
+        /,
         hostname: Optional[str] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Send the SMTP EHLO command.
         Hostname to send for this command defaults to the FQDN of the local
         host.
@@ -916,15 +923,15 @@
         self.last_ehlo_response = response
 
         if response.code != SMTPStatus.completed:
             raise SMTPHeloError(response.code, response.message)
 
         return response
 
-    def supports_extension(self, extension: str) -> bool:
+    def supports_extension(self, extension: str, /) -> bool:
         """
         Tests if the server supports the ESMTP service extension given.
         """
         return extension.lower() in self.esmtp_extensions
 
     async def _ehlo_or_helo_if_needed(self) -> None:
         """
@@ -950,14 +957,15 @@
         self._last_ehlo_response = None
         self.esmtp_extensions = {}
         self.supports_esmtp = False
         self.server_auth_methods = []
 
     async def starttls(
         self,
+        /,
         server_hostname: Optional[str] = None,
         validate_certs: Optional[bool] = None,
         client_cert: Optional[Union[str, Default]] = _default,
         client_key: Optional[Union[str, Default]] = _default,
         cert_bundle: Optional[Union[str, Default]] = _default,
         tls_context: Optional[Union[ssl.SSLContext, Default]] = _default,
         timeout: Optional[Union[float, Default]] = _default,
@@ -990,28 +998,30 @@
 
         self._update_settings_from_kwargs(
             validate_certs=validate_certs,
             client_cert=client_cert,
             client_key=client_key,
             cert_bundle=cert_bundle,
             tls_context=tls_context,
-            timeout=timeout,
         )
         self._validate_config()
 
         if server_hostname is None:
             server_hostname = self.hostname
 
+        if timeout is _default:
+            timeout = self.timeout
+
         tls_context = self._get_tls_context()
 
         if not self.supports_extension("starttls"):
             raise SMTPException("SMTP STARTTLS extension not supported by server.")
 
         response = await self.protocol.start_tls(
-            tls_context, server_hostname=server_hostname, timeout=self.timeout
+            tls_context, server_hostname=server_hostname, timeout=timeout
         )
         if self.protocol is None:
             raise SMTPServerDisconnected("Connection lost")
         # Update our transport reference
         self.transport = self.protocol.transport
 
         # RFC 3207 part 4.2:
@@ -1024,14 +1034,15 @@
 
     # Auth commands
 
     async def login(
         self,
         username: Union[str, bytes],
         password: Union[str, bytes],
+        /,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         Tries to login with supported auth methods.
 
         Some servers advertise authentication methods they don't really
         support, so if authentication fails, we continue until we've tried
@@ -1051,16 +1062,18 @@
 
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
@@ -1070,14 +1083,15 @@
 
         return response
 
     async def auth_crammd5(
         self,
         username: Union[str, bytes],
         password: Union[str, bytes],
+        /,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         CRAM-MD5 auth uses the password as a shared secret to MD5 the server's
         response.
 
         Example::
@@ -1107,14 +1121,15 @@
 
         return response
 
     async def auth_plain(
         self,
         username: Union[str, bytes],
         password: Union[str, bytes],
+        /,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         PLAIN auth encodes the username and password in one Base64 encoded
         string. No verification message is required.
 
         Example::
@@ -1134,14 +1149,15 @@
 
         return response
 
     async def auth_login(
         self,
         username: Union[str, bytes],
         password: Union[str, bytes],
+        /,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> SMTPResponse:
         """
         LOGIN auth sends the Base64 encoded username and password in sequence.
 
         Example::
 
@@ -1181,14 +1197,15 @@
         return response
 
     async def sendmail(
         self,
         sender: str,
         recipients: Union[str, Sequence[str]],
         message: Union[str, bytes],
+        /,
         mail_options: Optional[Iterable[str]] = None,
         rcpt_options: Optional[Iterable[str]] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> Tuple[Dict[str, SMTPResponse], str]:
         """
         This command performs an entire mail transaction.
 
@@ -1336,14 +1353,15 @@
         }
 
         return formatted_errors
 
     async def send_message(
         self,
         message: Union[email.message.EmailMessage, email.message.Message],
+        /,
         sender: Optional[str] = None,
         recipients: Optional[Union[str, Sequence[str]]] = None,
         mail_options: Optional[Iterable[str]] = None,
         rcpt_options: Optional[Iterable[str]] = None,
         timeout: Optional[Union[float, Default]] = _default,
     ) -> Tuple[Dict[str, SMTPResponse], str]:
         r"""
```

### Comparing `aiosmtplib-2.0.1/aiosmtplib/typing.py` & `aiosmtplib-3.0.0.dev0/aiosmtplib/typing.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/Makefile` & `aiosmtplib-3.0.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/client.rst` & `aiosmtplib-3.0.0.dev0/docs/client.rst`

 * *Files 1% similar despite different names*

```diff
@@ -186,17 +186,17 @@
 
 
 Timeouts
 --------
 
 All commands accept a ``timeout`` keyword argument of a numerical value in
 seconds. This value is used for all socket operations, and will raise
-:exc:`.SMTPTimeoutError` if exceeded. Timeout values passed to :func:`send`,
-:meth:`SMTP.__init__` or :meth:`SMTP.connect` will be used as the default
-value for commands executed on the connection.
+:exc:`.SMTPTimeoutError` if exceeded. Timeout values passed to :func:`send` and
+:meth:`SMTP.__init__` will be used as the default value for commands executed
+on the connection.
 
 The default timeout is 60 seconds.
 
 
 Parallel Execution
 ------------------
```

#### html2text {}

```diff
@@ -60,18 +60,17 @@
 ["somebody@example.com"] message = """To: somebody@example.com From:
 root@localhost Subject: Hello World! Sent via aiosmtplib """ async def
 send_with_sendmail(): smtp_client = SMTP(hostname="127.0.0.1", port=1025) await
 smtp_client.connect() await smtp_client.sendmail(sender, recipients, message)
 await smtp_client.quit() asyncio.run(send_with_sendmail()) Timeouts -------
 - All commands accept a ``timeout`` keyword argument of a numerical value in
 seconds. This value is used for all socket operations, and will raise :exc:
-`.SMTPTimeoutError` if exceeded. Timeout values passed to :func:`send`, :meth:
-`SMTP.__init__` or :meth:`SMTP.connect` will be used as the default value for
-commands executed on the connection. The default timeout is 60 seconds.
-Parallel Execution ------------------ SMTP is a sequential protocol. Multiple
-commands must be sent to send an email, and they must be sent in the correct
-sequence. As a consequence of this, executing multiple :meth:
-`SMTP.send_message` tasks in parallel (i.e. with :py:func:`asyncio.gather`) is
-not any more efficient than executing in sequence, as the client must wait
-until one mail is sent before beginning the next. If you have a lot of emails
-to send, consider creating multiple connections (:class:`SMTP` instances) and
-splitting the work between them.
+`.SMTPTimeoutError` if exceeded. Timeout values passed to :func:`send` and :
+meth:`SMTP.__init__` will be used as the default value for commands executed on
+the connection. The default timeout is 60 seconds. Parallel Execution ---------
+--------- SMTP is a sequential protocol. Multiple commands must be sent to send
+an email, and they must be sent in the correct sequence. As a consequence of
+this, executing multiple :meth:`SMTP.send_message` tasks in parallel (i.e. with
+:py:func:`asyncio.gather`) is not any more efficient than executing in
+sequence, as the client must wait until one mail is sent before beginning the
+next. If you have a lot of emails to send, consider creating multiple
+connections (:class:`SMTP` instances) and splitting the work between them.
```

### Comparing `aiosmtplib-2.0.1/docs/conf.py` & `aiosmtplib-3.0.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/encryption.rst` & `aiosmtplib-3.0.0.dev0/docs/encryption.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/reference.rst` & `aiosmtplib-3.0.0.dev0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/docs/usage.rst` & `aiosmtplib-3.0.0.dev0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/auth.py` & `aiosmtplib-3.0.0.dev0/tests/auth.py`

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

### Comparing `aiosmtplib-2.0.1/tests/conftest.py` & `aiosmtplib-3.0.0.dev0/tests/conftest.py`

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

### Comparing `aiosmtplib-2.0.1/tests/smtpd.py` & `aiosmtplib-3.0.0.dev0/tests/smtpd.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_api.py` & `aiosmtplib-3.0.0.dev0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_asyncio.py` & `aiosmtplib-3.0.0.dev0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_auth_methods.py` & `aiosmtplib-3.0.0.dev0/tests/test_auth_methods.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_auth_utils.py` & `aiosmtplib-3.0.0.dev0/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_commands.py` & `aiosmtplib-3.0.0.dev0/tests/test_commands.py`

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

### Comparing `aiosmtplib-2.0.1/tests/test_config.py` & `aiosmtplib-3.0.0.dev0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,24 +156,24 @@
     await client.connect(port=smtpd_server_port)
 
     assert client.port == smtpd_server_port
 
     await client.quit()
 
 
-async def test_connect_timeout_takes_precedence(
+async def test_connect_timeout_is_reverted(
     hostname: str,
     smtpd_server_port: int,
 ) -> None:
     client = SMTP(
         hostname=hostname, port=smtpd_server_port, timeout=0.66, start_tls=False
     )
     await client.connect(timeout=0.99)
 
-    assert client.timeout == 0.99
+    assert client.timeout == 0.66
 
     await client.quit()
 
 
 async def test_connect_source_address_takes_precedence(
     bind_address: str,
     unused_tcp_port: int,
```

### Comparing `aiosmtplib-2.0.1/tests/test_connect.py` & `aiosmtplib-3.0.0.dev0/tests/test_connect.py`

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

### Comparing `aiosmtplib-2.0.1/tests/test_email_utils.py` & `aiosmtplib-3.0.0.dev0/tests/test_email_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_errors.py` & `aiosmtplib-3.0.0.dev0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_esmtp_utils.py` & `aiosmtplib-3.0.0.dev0/tests/test_esmtp_utils.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_live.py` & `aiosmtplib-3.0.0.dev0/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_main.py` & `aiosmtplib-3.0.0.dev0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_protocol.py` & `aiosmtplib-3.0.0.dev0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_response.py` & `aiosmtplib-3.0.0.dev0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_sendmail.py` & `aiosmtplib-3.0.0.dev0/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_sync.py` & `aiosmtplib-3.0.0.dev0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_timeouts.py` & `aiosmtplib-3.0.0.dev0/tests/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/tests/test_tls.py` & `aiosmtplib-3.0.0.dev0/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `aiosmtplib-2.0.1/setup.py` & `aiosmtplib-3.0.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,23 @@
                                                                'uvloop>=0.14,<0.15'],
  'uvloop:python_version >= "3.9" and python_version < "4.0"': ['uvloop>=0.17,<0.18',
                                                                'uvloop>=0.17,<0.18',
                                                                'uvloop>=0.17,<0.18']}
 
 setup_kwargs = {
     'name': 'aiosmtplib',
-    'version': '2.0.1',
+    'version': '3.0.0.dev0',
     'description': 'asyncio SMTP client',
-    'long_description': 'aiosmtplib\n==========\n\n|circleci| |precommit.ci| |codecov| |pypi-version| |pypi-status| |downloads| |pypi-python-versions|\n|pypi-license|\n\n------------\n\naiosmtplib is an asynchronous SMTP client for use with asyncio.\n\nFor documentation, see `Read The Docs`_.\n\nQuickstart\n----------\n\n.. code-block:: python\n\n    import asyncio\n    from email.message import EmailMessage\n\n    import aiosmtplib\n\n    message = EmailMessage()\n    message["From"] = "root@localhost"\n    message["To"] = "somebody@example.com"\n    message["Subject"] = "Hello World!"\n    message.set_content("Sent via aiosmtplib")\n\n    asyncio.run(aiosmtplib.send(message, hostname="127.0.0.1", port=25))\n\n\nRequirements\n------------\nPython 3.7+, compiled with SSL support, is required.\n\n\nBug Reporting\n-------------\nBug reports (and feature requests) are welcome via `Github issues`_.\n\n\n\n.. |circleci| image:: https://circleci.com/gh/cole/aiosmtplib/tree/main.svg?style=shield\n           :target: https://circleci.com/gh/cole/aiosmtplib/tree/main\n           :alt: "aiosmtplib CircleCI build status"\n.. |pypi-version| image:: https://img.shields.io/pypi/v/aiosmtplib.svg\n                 :target: https://pypi.python.org/pypi/aiosmtplib\n                 :alt: "aiosmtplib on the Python Package Index"\n.. |pypi-python-versions| image:: https://img.shields.io/pypi/pyversions/aiosmtplib.svg\n.. |pypi-status| image:: https://img.shields.io/pypi/status/aiosmtplib.svg\n.. |pypi-license| image:: https://img.shields.io/pypi/l/aiosmtplib.svg\n.. |codecov| image:: https://codecov.io/gh/cole/aiosmtplib/branch/main/graph/badge.svg\n             :target: https://codecov.io/gh/cole/aiosmtplib\n.. |downloads| image:: https://pepy.tech/badge/aiosmtplib\n               :target: https://pepy.tech/project/aiosmtplib\n               :alt: "aiosmtplib on pypy.tech"\n.. |precommit.ci| image:: https://results.pre-commit.ci/badge/github/cole/aiosmtplib/main.svg\n                  :target: https://results.pre-commit.ci/latest/github/cole/aiosmtplib/main\n                  :alt: "pre-commit.ci status"\n.. _Read The Docs: https://aiosmtplib.readthedocs.io/en/stable/overview.html\n.. _Github issues: https://github.com/cole/aiosmtplib/issues\n',
+    'long_description': 'aiosmtplib\n==========\n\n|circleci| |precommit.ci| |codecov| |pypi-version| |pypi-status| |downloads| |pypi-python-versions|\n|pypi-license|\n\n------------\n\naiosmtplib is an asynchronous SMTP client for use with asyncio.\n\nFor documentation, see `Read The Docs`_.\n\nQuickstart\n----------\n\n.. code-block:: python\n\n    import asyncio\n    from email.message import EmailMessage\n\n    import aiosmtplib\n\n    message = EmailMessage()\n    message["From"] = "root@localhost"\n    message["To"] = "somebody@example.com"\n    message["Subject"] = "Hello World!"\n    message.set_content("Sent via aiosmtplib")\n\n    asyncio.run(aiosmtplib.send(message, hostname="127.0.0.1", port=25))\n\n\nRequirements\n------------\nPython 3.8+, compiled with SSL support, is required.\n\n\nBug Reporting\n-------------\nBug reports (and feature requests) are welcome via `Github issues`_.\n\n\n\n.. |circleci| image:: https://circleci.com/gh/cole/aiosmtplib/tree/main.svg?style=shield\n           :target: https://circleci.com/gh/cole/aiosmtplib/tree/main\n           :alt: "aiosmtplib CircleCI build status"\n.. |pypi-version| image:: https://img.shields.io/pypi/v/aiosmtplib.svg\n                 :target: https://pypi.python.org/pypi/aiosmtplib\n                 :alt: "aiosmtplib on the Python Package Index"\n.. |pypi-python-versions| image:: https://img.shields.io/pypi/pyversions/aiosmtplib.svg\n.. |pypi-status| image:: https://img.shields.io/pypi/status/aiosmtplib.svg\n.. |pypi-license| image:: https://img.shields.io/pypi/l/aiosmtplib.svg\n.. |codecov| image:: https://codecov.io/gh/cole/aiosmtplib/branch/main/graph/badge.svg\n             :target: https://codecov.io/gh/cole/aiosmtplib\n.. |downloads| image:: https://pepy.tech/badge/aiosmtplib\n               :target: https://pepy.tech/project/aiosmtplib\n               :alt: "aiosmtplib on pypy.tech"\n.. |precommit.ci| image:: https://results.pre-commit.ci/badge/github/cole/aiosmtplib/main.svg\n                  :target: https://results.pre-commit.ci/latest/github/cole/aiosmtplib/main\n                  :alt: "pre-commit.ci status"\n.. _Read The Docs: https://aiosmtplib.readthedocs.io/en/stable/overview.html\n.. _Github issues: https://github.com/cole/aiosmtplib/issues\n',
     'author': 'Cole Maclean',
     'author_email': 'hi@colemaclean.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cole/aiosmtplib',
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `aiosmtplib-2.0.1/PKG-INFO` & `aiosmtplib-3.0.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: aiosmtplib
-Version: 2.0.1
+Version: 3.0.0.dev0
 Summary: asyncio SMTP client
 Home-page: https://github.com/cole/aiosmtplib
 License: MIT
 Keywords: smtp,email,asyncio
 Author: Cole Maclean
 Author-email: hi@colemaclean.dev
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Software Development :: Libraries
@@ -66,15 +65,15 @@
     message.set_content("Sent via aiosmtplib")
 
     asyncio.run(aiosmtplib.send(message, hostname="127.0.0.1", port=25))
 
 
 Requirements
 ------------
-Python 3.7+, compiled with SSL support, is required.
+Python 3.8+, compiled with SSL support, is required.
 
 
 Bug Reporting
 -------------
 Bug reports (and feature requests) are welcome via `Github issues`_.
```

