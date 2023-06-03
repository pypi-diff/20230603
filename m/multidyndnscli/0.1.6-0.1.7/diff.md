# Comparing `tmp/multidyndnscli-0.1.6.tar.gz` & `tmp/multidyndnscli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.6.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.7.tar", max compression
```

## Comparing `multidyndnscli-0.1.6.tar` & `multidyndnscli-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-03 16:23:39.266312 multidyndnscli-0.1.6/LICENSE
--rw-r--r--   0        0        0     7362 2023-06-03 16:23:39.266312 multidyndnscli-0.1.6/README.md
--rw-r--r--   0        0        0    34179 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     2331 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6907 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2771 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3844 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/util.py
--rw-r--r--   0        0        0     1287 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 multidyndnscli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 19:55:35.850356 multidyndnscli-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7362 2023-06-03 19:55:35.850356 multidyndnscli-0.1.7/README.md
+-rw-r--r--   0        0        0    34610 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2331 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6907 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2865 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1287 2023-06-03 19:55:35.854356 multidyndnscli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 multidyndnscli-0.1.7/PKG-INFO
```

### Comparing `multidyndnscli-0.1.6/LICENSE` & `multidyndnscli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.6/README.md` & `multidyndnscli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.6/multidyndnscli/__init__.py` & `multidyndnscli-0.1.7/multidyndnscli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,43 +119,43 @@
     def _resolve_current_fqdn_ipv4(self):
         """Method for resolving the current IPv4 the FQDN is pointing to (if any)
         """
         try:
             result = dns.resolver.resolve(self._fqdn, rdtype=dns.rdatatype.A)
             if len(result.rrset) > 0:
                 self._current_fqdn_dns_ipv4 = IPAddress(result.rrset[0].address)
-        except (ValueError, AddrFormatError):
+        except (ValueError, AddrFormatError, dns.resolver.NXDOMAIN):
             self._current_fqdn_dns_ipv4 = None
 
     def _resolve_current_fqdn_ipv6_set(self):
         """Method for resolving the current IPv6 the FQDN is pointing to (if any)
         """
         addresses = set()
         try:
             result = dns.resolver.resolve(self._fqdn, rdtype=dns.rdatatype.AAAA)
             for rrset_address in result.rrset:
                 address = IPAddress(rrset_address.address)
                 if util.is_public_ipv6(address):
                     addresses.add(address)
             self._current_fqdn_dns_ipv6_set = addresses
-        except (ValueError, AddrFormatError):
+        except (ValueError, AddrFormatError, dns.resolver.NXDOMAIN):
             self._current_fqdn_dns_ipv6_set = set()
 
     def _resolve_host_ipv4(self, method: str):
         """Method for resolving the public IPv4 used to reach the host from the intranet
         """
         address = None
         if method == 'router':
             address = self._router.ipv4
         elif method == 'local_dns':
             try:
                 result = dns.resolver.resolve(self._name, rdtype=dns.rdatatype.A)
                 if result.rrset is not None and len(result.rrset) > 0:
                     address = result.rrset[0].address
-            except (ValueError, AddrFormatError) as exc:
+            except (ValueError, AddrFormatError, dns.resolver.NXDOMAIN) as exc:
                 raise DNSResolutionException(
                     f'Unable to find IPv4 for local hostname {self._name}') from exc
 
         if address is not None:
             self._host_ipv4 = IPAddress(address)
 
     def _resolve_host_ipv6_set(self, method: str):
@@ -170,15 +170,15 @@
                 result = dns.resolver.resolve(self._name, rdtype=dns.rdatatype.AAAA)
                 if result.rrset is None:
                     return
                 for result_addr in result.rrset:
                     address = IPAddress(result_addr.address)
                     if util.is_public_ipv6(address):
                         addresses.add(address)
-            except (ValueError, AddrFormatError) as exc:
+            except (ValueError, AddrFormatError, dns.resolver.NXDOMAIN) as exc:
                 raise DNSResolutionException(
                     f'Unable to find IPv6s for local hostname {self._name}') from exc
         if len(addresses) > 0:
             self._host_ipv6_set = addresses
 
     def needs_update(self) -> bool:
         """Indicates whether or not an update of the FQDN is required for this host
@@ -347,15 +347,18 @@
                 return
         records_ipv4 = []
         records_ipv6 = []
         needs_update = False
         for host in self._host_list:
             if host.needs_update():
                 needs_update = True
-                dns_prefix = host.fqdn.rstrip(self._domain_name).rstrip('.')
+                dns_prefix = host.fqdn
+                # Strip domain name of, if any
+                if dns_prefix.endswith(f'.{self._domain_name}'):
+                    dns_prefix = dns_prefix[:-len(f'.{self._domain_name}')]
                 if host.host_ipv4 is not None:
                     record = DNSRecord(
                         hostname=dns_prefix, type='A', destination=str(host.host_ipv4)
                     )
                     records_ipv4.append(record)
                 ipv6 = host.host_ipv6
                 if ipv6 is not None:
@@ -378,14 +381,18 @@
             for record in records_ipv6:
                 current_record_id = self._find_record_id(record.hostname, 'AAAA')
                 if current_record_id is not None:
                     record.id = current_record_id
             records = records_ipv4 + records_ipv6
             if not dry_run:
                 self._dns_provider.update_domain(self, records)
+            else:
+                print(f'Would update the following records of domain {self.domain_name}:')
+                for rec in records:
+                    print (f'  {str(rec)}')
 
     def _rebuild_domain_records_cache(self):
         """Rebuild the domain record cache from data fetched from the configure DNS provider
         """
         record_dict = {}
         records = self._dns_provider.fetch_domain(self)
         for record in records:
```

### Comparing `multidyndnscli-0.1.6/multidyndnscli/cli.py` & `multidyndnscli-0.1.7/multidyndnscli/cli.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.6/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.7/multidyndnscli/nc_dnsapi.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.6/multidyndnscli/schemata.py` & `multidyndnscli-0.1.7/multidyndnscli/schemata.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,20 @@
     """Create the config file schema
 
     :return: Config file schema
     :rtype: Schema
     """
     return Schema(
         {
-            Optional("common"): {Optional("cache_dir"): And(str)},
+            Optional("common"): Or(
+                None,
+                {
+                    Optional("cache_dir"): And(str)
+                }
+            ),
             "dns_providers": [
                 Or(
                     {
                         "name": And(str, len),
                         "type": And(str, Use(str.lower), "netcup"),
                         "userid": And(str, len),
                         "apikey": And(str, len),
```

### Comparing `multidyndnscli-0.1.6/multidyndnscli/util.py` & `multidyndnscli-0.1.7/multidyndnscli/util.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.6/pyproject.toml` & `multidyndnscli-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.6"
+version = "0.1.7"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
```

### Comparing `multidyndnscli-0.1.6/PKG-INFO` & `multidyndnscli-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.6
+Version: 0.1.7
 Summary: DynDNS Command-line Client
 Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.6 Summary: DynDNS
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.7 Summary: DynDNS
 Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later Author: Eike Thaden Author-email:
 eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: dnspython
```

