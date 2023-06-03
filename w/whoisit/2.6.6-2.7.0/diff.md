# Comparing `tmp/whoisit-2.6.6.tar.gz` & `tmp/whoisit-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoisit-2.6.6.tar", last modified: Tue Dec  6 10:31:52 2022, max compression
+gzip compressed data, was "whoisit-2.7.0.tar", last modified: Sat Jun  3 11:00:02 2023, max compression
```

## Comparing `whoisit-2.6.6.tar` & `whoisit-2.7.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2022-12-06 10:31:52.251929 whoisit-2.6.6/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.6.6/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.6.6/MANIFEST.in
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2022-12-06 10:31:52.251929 whoisit-2.6.6/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.6.6/README.md
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.6.6/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2022-12-06 10:31:52.251929 whoisit-2.6.6/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2022-12-06 10:31:39.000000 whoisit-2.6.6/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2022-12-06 10:31:52.247929 whoisit-2.6.6/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.6.6/tests/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.6.6/tests/test_bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.6.6/tests/test_parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.6.6/tests/test_query.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2022-12-06 10:31:52.247929 whoisit-2.6.6/whoisit/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2402 2022-05-05 09:40:05.000000 whoisit-2.6.6/whoisit/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    17736 2022-07-10 15:49:04.000000 whoisit-2.6.6/whoisit/bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.6.6/whoisit/errors.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.6.6/whoisit/logger.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      949 2022-12-06 10:28:45.000000 whoisit-2.6.6/whoisit/overrides.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    15838 2022-12-06 10:28:45.000000 whoisit-2.6.6/whoisit/parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     9126 2022-12-06 10:28:45.000000 whoisit-2.6.6/whoisit/query.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3049 2022-07-12 13:37:33.000000 whoisit-2.6.6/whoisit/utils.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2022-12-06 10:31:43.000000 whoisit-2.6.6/whoisit/version.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2022-12-06 10:31:52.251929 whoisit-2.6.6/whoisit.egg-info/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2022-12-06 10:31:52.000000 whoisit-2.6.6/whoisit.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      471 2022-12-06 10:31:52.000000 whoisit-2.6.6/whoisit.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2022-12-06 10:31:52.000000 whoisit-2.6.6/whoisit.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:31:52.000000 whoisit-2.6.6/whoisit.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2022-12-06 10:31:52.000000 whoisit-2.6.6/whoisit.egg-info/top_level.txt
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.0/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.0/MANIFEST.in
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-06-03 11:00:02.365261 whoisit-2.7.0/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.0/README.md
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.0/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-06-03 11:00:02.365261 whoisit-2.7.0/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2023-06-03 10:59:42.000000 whoisit-2.7.0/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.0/tests/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.0/tests/test_bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.0/tests/test_parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.0/tests/test_query.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.0/tests/test_ssl.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/whoisit/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2359 2023-06-03 08:55:13.000000 whoisit-2.7.0/whoisit/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.0/whoisit/bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/errors.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.0/whoisit/logger.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      949 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/overrides.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    15838 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.0/whoisit/query.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3830 2023-06-03 08:54:56.000000 whoisit-2.7.0/whoisit/utils.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2023-06-03 10:59:35.000000 whoisit-2.7.0/whoisit/version.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/whoisit.egg-info/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/top_level.txt
```

### Comparing `whoisit-2.6.6/LICENSE` & `whoisit-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/PKG-INFO` & `whoisit-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.6.6
+Version: 2.7.0
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Platform: UNKNOWN
```

### Comparing `whoisit-2.6.6/README.md` & `whoisit-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/setup.py` & `whoisit-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '2.6.6'
+version = '2.7.0'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `whoisit-2.6.6/tests/test_bootstrap.py` & `whoisit-2.7.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/tests/test_parser.py` & `whoisit-2.7.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/tests/test_query.py` & `whoisit-2.7.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/whoisit/__init__.py` & `whoisit-2.7.0/whoisit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import requests
 from .bootstrap import Bootstrap
 from .query import QueryBuilder, Query
 from .parser import parse
 from .logger import get_logger
-from .utils import create_session
+from .utils import create_session, get_session
 from .version import version
 
 
 # Private methods
 
 
-_default_session = create_session()
-_bootstrap = Bootstrap(_default_session)
+_bootstrap = Bootstrap()
 _query_builder = QueryBuilder(_bootstrap)
 
 
 # Expose class methods as the public API
 
 
 is_bootstrapped = _bootstrap.is_bootstrapped
@@ -27,44 +26,40 @@
 build_query = _query_builder.build
 
 
 # Query helpers
 
 
 def asn(as_number, rir=None, raw=False, allow_insecure_ssl=False, session=None):
-    if not session:
-        session = _default_session
+    session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='asn', query_value=as_number, rir=rir)
-    q = Query(session, method, url, allow_insecure_ssl)
+    q = Query(session, method, url)
     response = q.request()
     return response if raw else parse(_bootstrap, 'autnum', as_number, response)
 
 
 def domain(domain_name, raw=False, allow_insecure_ssl=False, session=None):
-    if not session:
-        session = _default_session
+    session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='domain', query_value=domain_name)
-    q = Query(session, method, url, allow_insecure_ssl)
+    q = Query(session, method, url)
     response = q.request()
     return response if raw else parse(_bootstrap, 'domain', domain_name, response)
 
 
 def ip(ip_address_or_network, rir=None, raw=False, allow_insecure_ssl=False, session=None):
-    if not session:
-        session = _default_session
+    session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='ip', query_value=ip_address_or_network, rir=rir)
-    q = Query(session, method, url, allow_insecure_ssl)
+    q = Query(session, method, url)
     response = q.request()
     return response if raw else parse(_bootstrap, 'ip', ip_address_or_network, response)
 
 
 def entity(entity_handle, rir=None, raw=False, allow_insecure_ssl=False, session=None):
-    if not session:
-        session = _default_session
+    session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='entity', query_value=entity_handle, rir=rir)
-    q = Query(session, method, url, allow_insecure_ssl)
+    q = Query(session, method, url)
     response = q.request()
     return response if raw else parse(_bootstrap, 'entity', entity_handle, response)
```

### Comparing `whoisit-2.6.6/whoisit/bootstrap.py` & `whoisit-2.7.0/whoisit/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import requests
 from time import time
 from urllib.parse import urlsplit
 from ipaddress import IPv4Network, IPv4Address, IPv6Network, IPv6Address
 from .logger import get_logger
-from .utils import http_request, is_subnet_of, create_session
+from .utils import http_request, is_subnet_of, create_session, get_session
 from .overrides import iana_overrides
 from .errors import BootstrapError, UnsupportedError
 
 
 log = get_logger('bootstrap')
 
 
@@ -54,19 +54,16 @@
         'ID': 'idnic',
         'LACNIC': 'lacnic',
         'BR': 'registro.br', # registro.br currently does not use entity prefixes
         'RIPE': 'ripe',
         'TW': 'twnic',
     }
 
-    def __init__(self, session=None):
-        if not session:
-            self.session = create_session()
-        else:
-            self.session = session
+    def __init__(self, session=None, allow_insecure_ssl=False):
+        self.session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
         self.bootstrap_parsers = {
             'asn': self.parse_asn_data,
             'dns': self.parse_dns_data,
             'ipv4': self.parse_ipv4_data,
             'ipv6': self.parse_ipv6_data,
             'object': self.parse_object_data,
         }
```

### Comparing `whoisit-2.6.6/whoisit/errors.py` & `whoisit-2.7.0/whoisit/errors.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/whoisit/logger.py` & `whoisit-2.7.0/whoisit/logger.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/whoisit/overrides.py` & `whoisit-2.7.0/whoisit/overrides.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/whoisit/parser.py` & `whoisit-2.7.0/whoisit/parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.6.6/whoisit/query.py` & `whoisit-2.7.0/whoisit/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,18 +160,17 @@
 class Query:
     """
         Make an HTTP request to an RDAP endpoint as a query. This is slightly more
         elaborate than a single function just to allow kwargs to be arbitrarily passed
         to both requests and the requested URL if required.
     """
 
-    def __init__(self, session, method, url, allow_insecure_ssl=False, **kwargs):
+    def __init__(self, session, method, url, **kwargs):
         self.session = session
         self.method = method.strip().upper()
-        self.allow_insecure_ssl = bool(allow_insecure_ssl)
         if kwargs:
             # kwargs are appended to the URL, such as test=123 becomes url?test=123
             self.url = self.add_url_params(url, kwargs)
         else:
             self.url = url
 
     def add_url_params(self, url, extra_params):
@@ -182,16 +181,15 @@
         for k, v in extra_params.items():
             qs[k] = str(v)
         qs_str = urlencode(qs)
         return urlunsplit((parts.scheme, parts.netloc, parts.path, qs_str, ''))
 
     def request(self, *args, **kwargs):
         # args and kwargs here are passed directly to requests.request(...)
-        response = http_request(self.session, url=self.url, method=self.method,
-                                allow_insecure_ssl=self.allow_insecure_ssl, *args, **kwargs)
+        response = http_request(self.session, url=self.url, method=self.method, *args, **kwargs)
         if response.status_code == 404:
             raise ResourceDoesNotExist(f'RDAP {self.method} request to {self.url} '
                                        f'returned a 404 error, the resource does '
                                        f'not exist')
         elif response.status_code == 429:
             raise RateLimitedError(f'RDAP {self.method} request to {self.url} '
                                    f'returned a 429 error, the resource has been '
```

### Comparing `whoisit-2.6.6/whoisit.egg-info/PKG-INFO` & `whoisit-2.7.0/whoisit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.6.6
+Version: 2.7.0
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Platform: UNKNOWN
```

