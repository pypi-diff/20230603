# Comparing `tmp/sshkey-tools-0.9.2.tar.gz` & `tmp/sshkey-tools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshkey-tools-0.9.2.tar", last modified: Tue May 30 15:40:41 2023, max compression
+gzip compressed data, was "sshkey-tools-0.9.3.tar", last modified: Sat Jun  3 20:54:00 2023, max compression
```

## Comparing `sshkey-tools-0.9.2.tar` & `sshkey-tools-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.350950 sshkey-tools-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/src/sshkey_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    49394 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:54:00.699916 sshkey-tools-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-06-03 20:54:00.699916 sshkey-tools-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:54:00.703916 sshkey-tools-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:54:00.699916 sshkey-tools-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:54:00.699916 sshkey-tools-0.9.3/src/sshkey_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20679 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49394 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29785 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-03 20:53:42.000000 sshkey-tools-0.9.3/src/sshkey_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:54:00.699916 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:54:00.000000 sshkey-tools-0.9.3/src/sshkey_tools.egg-info/zip-safe
```

### Comparing `sshkey-tools-0.9.2/LICENSE` & `sshkey-tools-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/PKG-INFO` & `sshkey-tools-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshkey-tools
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
 Home-page: https://github.com/scheiblingco/sshkey-tools
 Author: Lars Scheibling
 Author-email: lars@scheibling.se
 License: GnuPG 3.0
 Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,28 @@
 License-File: LICENSE
 
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
 # Notice
+The DSA algorithm has been deprecated and is removed in pyca/cryptography 41.x, meaning **version 0.9.* of this package will be the last to support DSA keys and certificates** for SSH. If there is any demand to reintroduce DSA support, please open an issue regarding this and we'll look into it. 
+
+For now, **0.9.* will be restricted to version <41.1 of the cryptography package** and **0.10 will have its DSA support removed**. We've introduced a deprecation notice in version 0.9.3.
+
+## Background
 The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
 
-Notice from OpenSSH:
+## Notice from OpenSSH:
 ```
 OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
 ```
 
 [ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
 
-
 # Features
 ### SSH Keys
 - Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
```

### Comparing `sshkey-tools-0.9.2/README.md` & `sshkey-tools-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
 # Notice
+The DSA algorithm has been deprecated and is removed in pyca/cryptography 41.x, meaning **version 0.9.* of this package will be the last to support DSA keys and certificates** for SSH. If there is any demand to reintroduce DSA support, please open an issue regarding this and we'll look into it. 
+
+For now, **0.9.* will be restricted to version <41.1 of the cryptography package** and **0.10 will have its DSA support removed**. We've introduced a deprecation notice in version 0.9.3.
+
+## Background
 The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
 
-Notice from OpenSSH:
+## Notice from OpenSSH:
 ```
 OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
 ```
 
 [ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
 
-
 # Features
 ### SSH Keys
 - Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
```

### Comparing `sshkey-tools-0.9.2/setup.py` & `sshkey-tools-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/__version__.py` & `sshkey-tools-0.9.3/src/sshkey_tools/__version__.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/cert.py` & `sshkey-tools-0.9.3/src/sshkey_tools/cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Raises:
     _EX.SSHCertificateException: General error in certificate
     _EX.InvalidCertificateFormatException: An error with the format of the certificate
     _EX.InvalidCertificateFieldException: An invalid field has been added to the certificate
     _EX.NoPrivateKeyException: The certificate contains no private key
     _EX.NotSignedException: The certificate is not signed and cannot be exported
 """
+import warnings
 from base64 import b64decode, b64encode
 from dataclasses import dataclass
 from typing import Tuple, Union
 
 from prettytable import PrettyTable
 
 from . import exceptions as _EX
@@ -573,17 +574,24 @@
 class RsaCertificate(SSHCertificate):
     """The RSA Certificate class"""
 
     DEFAULT_KEY_TYPE = "rsa-sha2-512-cert-v01@openssh.com"
 
 
 class DsaCertificate(SSHCertificate):
-    """The DSA Certificate class"""
+    """The DSA Certificate class (DEPRECATED)"""
 
     DEFAULT_KEY_TYPE = "ssh-dss-cert-v01@openssh.com"
+    
+    def __post_init__(self):
+        """Display the deprecation notice"""
+        warnings.warn(
+            "SSH DSA keys and certificates are deprecated and will be removed in version 0.10 of sshkey-tools",
+            stacklevel=2,
+        )
 
 
 class EcdsaCertificate(SSHCertificate):
     """The ECDSA certificate class"""
 
     DEFAULT_KEY_TYPE = "ecdsa-sha2-nistp[curve_size]-cert-v01@openssh.com"
```

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/exceptions.py` & `sshkey-tools-0.9.3/src/sshkey_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/fields.py` & `sshkey-tools-0.9.3/src/sshkey_tools/fields.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/keys.py` & `sshkey-tools-0.9.3/src/sshkey_tools/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes for handling SSH public/private keys
 """
+import warnings
 from base64 import b64decode
 from enum import Enum
 from struct import unpack
 from typing import Union
 
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.backends.openssl.dsa import _DSAPrivateKey, _DSAPublicKey
@@ -609,14 +610,19 @@
             key=key,
             comment=comment,
             key_type=key_type,
             public_numbers=key.public_numbers(),
             serialized=serialized,
         )
         self.parameters = key.parameters().parameter_numbers()
+        
+        warnings.warn(
+            "SSH DSA keys and certificates are deprecated and will be removed in version 0.10 of sshkey-tools",
+            stacklevel=2,
+        )
 
     @classmethod
     # pylint: disable=invalid-name
     def from_numbers(cls, p: int, q: int, g: int, y: int) -> "DsaPublicKey":
         """
         Create a DSA public key from public numbers and parameters
 
@@ -661,14 +667,19 @@
 
     def __init__(self, key: _DSA.DSAPrivateKey):
         super().__init__(
             key=key,
             public_key=DsaPublicKey(key.public_key()),
             private_numbers=key.private_numbers(),
         )
+        
+        warnings.warn(
+            "SSH DSA keys and certificates are deprecated and will be removed in version 0.10 of sshkey-tools",
+            stacklevel=2,
+        )
 
     @classmethod
     # pylint: disable=invalid-name,too-many-arguments
     def from_numbers(cls, p: int, q: int, g: int, y: int, x: int) -> "DsaPrivateKey":
         """
         Creates a new DsaPrivateKey object from parameters and public/private numbers
```

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools/utils.py` & `sshkey-tools-0.9.3/src/sshkey_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools.egg-info/PKG-INFO` & `sshkey-tools-0.9.3/src/sshkey_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshkey-tools
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
 Home-page: https://github.com/scheiblingco/sshkey-tools
 Author: Lars Scheibling
 Author-email: lars@scheibling.se
 License: GnuPG 3.0
 Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
 Classifier: Programming Language :: Python :: 3
@@ -15,24 +15,28 @@
 License-File: LICENSE
 
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
 # Notice
+The DSA algorithm has been deprecated and is removed in pyca/cryptography 41.x, meaning **version 0.9.* of this package will be the last to support DSA keys and certificates** for SSH. If there is any demand to reintroduce DSA support, please open an issue regarding this and we'll look into it. 
+
+For now, **0.9.* will be restricted to version <41.1 of the cryptography package** and **0.10 will have its DSA support removed**. We've introduced a deprecation notice in version 0.9.3.
+
+## Background
 The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
 
-Notice from OpenSSH:
+## Notice from OpenSSH:
 ```
 OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
 ```
 
 [ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
 
-
 # Features
 ### SSH Keys
 - Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
```

### Comparing `sshkey-tools-0.9.2/src/sshkey_tools.egg-info/SOURCES.txt` & `sshkey-tools-0.9.3/src/sshkey_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

