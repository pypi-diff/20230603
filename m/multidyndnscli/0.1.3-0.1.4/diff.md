# Comparing `tmp/multidyndnscli-0.1.3.tar.gz` & `tmp/multidyndnscli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.3.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.4.tar", max compression
```

## Comparing `multidyndnscli-0.1.3.tar` & `multidyndnscli-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-03 12:23:05.988350 multidyndnscli-0.1.3/LICENSE
--rw-r--r--   0        0        0     6702 2023-06-03 12:23:05.988350 multidyndnscli-0.1.3/README.md
--rw-r--r--   0        0        0    34180 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     2311 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6951 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2771 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3844 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/util.py
--rw-r--r--   0        0        0     1285 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7773 1970-01-01 00:00:00.000000 multidyndnscli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6763 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/README.md
+-rw-r--r--   0        0        0    34179 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2331 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6951 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2771 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1285 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidyndnscli-0.1.4/PKG-INFO
```

### Comparing `multidyndnscli-0.1.3/LICENSE` & `multidyndnscli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.3/README.md` & `multidyndnscli-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## Installation
 Install the package from Pypi (https://pypi.org/project/multidyndnscli) by running `pip install multidyndnscli`. It requires Python 3.8+.
 
 ## Installation on OpenWRT
 First, install the required packages on OpenWRT:
 
 ```bash
-opkg install python3 python3-yaml python3-dns python3-netaddr python3-netifaces
+opkg install python3
 ```
 
 Then install the Pypi packages as described above.
 
 ## Usage
 
 Create a config file and customize it. A small example might look like this:
@@ -173,14 +173,19 @@
 
 Build the docs in folder `docs`:
 
 ```
 poetry run sphinx-build -b html docs/source/  docs/build/html
 ```
 
+### Increase the version
+
+Update the version in `pyproject.tom`. The tool will report this version after the release.
+
+
 # Contributors
 
 See [Contributors](CONTRIBUTORS.md)
 
 # License
 
 Copyright Eike Thaden, 2023.
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
 # DynDNS Command Line Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
 ## Installation Install the package from Pypi (https://pypi.org/project/
 multidyndnscli) by running `pip install multidyndnscli`. It requires Python
 3.8+. ## Installation on OpenWRT First, install the required packages on
-OpenWRT: ```bash opkg install python3 python3-yaml python3-dns python3-netaddr
-python3-netifaces ``` Then install the Pypi packages as described above. ##
-Usage Create a config file and customize it. A small example might look like
-this: ``` common: cache_dir: "" dns_providers: - name: "Netcup" type: "Netcup"
-userid: "" apikey: "" apipass: "" router: ipv4: method: "wan" wan_interface: ""
-ipv6: enabled: true method: "wan" wan_interface: "" domains: - name:
-"test.invalid" dns_provider: "Netcup" delay: 300 hosts: - name: "openwrt.lan"
-fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4: "router" ipv6:
-"router" - name: "server.lan" fqdn: "server.home.test.invalid"
+OpenWRT: ```bash opkg install python3 ``` Then install the Pypi packages as
+described above. ## Usage Create a config file and customize it. A small
+example might look like this: ``` common: cache_dir: "" dns_providers: - name:
+"Netcup" type: "Netcup" userid: "" apikey: "" apipass: "" router: ipv4: method:
+"wan" wan_interface: "" ipv6: enabled: true method: "wan" wan_interface: ""
+domains: - name: "test.invalid" dns_provider: "Netcup" delay: 300 hosts: -
+name: "openwrt.lan" fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4:
+"router" ipv6: "router" - name: "server.lan" fqdn: "server.home.test.invalid"
 public_ip_methods: ipv4: "router" ipv6: "local_dns" ``` Create a folder for
 caching data which is writable by the user who runs the script and specify its
 location in `cache_dir`. Configure your DNS provider. Note, that currently only
 Netcup is supported. In our example, the script is running directly on the
 router. The router's IP addresses are identified by getting the public
 addresses of the specified WAN interface. Below, one domain called
 `test.invalid` is configured which consists of two local hosts. The example
@@ -64,10 +63,12 @@
 `pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
 term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
 poetry run black --skip-string-normalization . ``` Alternatively, run formatter
 with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
 multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
 #### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
 Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
-b html docs/source/ docs/build/html ``` # Contributors See [Contributors]
-(CONTRIBUTORS.md) # License Copyright Eike Thaden, 2023. Distributed under the
-terms of the GPL v3 license, multidyndnscli is free and open source software.
+b html docs/source/ docs/build/html ``` ### Increase the version Update the
+version in `pyproject.tom`. The tool will report this version after the
+release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
+Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
+multidyndnscli is free and open source software.
```

### Comparing `multidyndnscli-0.1.3/multidyndnscli/__init__.py` & `multidyndnscli-0.1.4/multidyndnscli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 import yaml
 import dns.resolver
 from netaddr import IPAddress, AddrFormatError
 import requests
 import fritzconnection  # type: ignore
 import fritzconnection.lib.fritzstatus  # type: ignore
 import fritzconnection.core.exceptions  # type: ignore
+from importlib_metadata import version
 # Module imports
 from . import util
 from .schemata import get_config_file_schema
 from .nc_dnsapi import Client, DNSRecord  # type: ignore
 
-from importlib_metadata import version
-
 __version__ = version(__package__)
 
 CACHE_FILE_NAME = 'multidyndns.cache'
 """The name used for the updater cache file if a (valid) cache dir has been configured"""
 KEY_DOMAINS: Final[str] = 'domains'
 """The key used to store domain statuses in the updater cache"""
 KEY_LAST_UPDATE: Final[str] = 'last_updated'
```

### Comparing `multidyndnscli-0.1.3/multidyndnscli/cli.py` & `multidyndnscli-0.1.4/multidyndnscli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
     :param args: list of command line arguments (i.e. args), defaults to None
     :type args: Optional[List[str]], optional
     :return: Returns 0 if update was successful, otherwise 1
     :rtype: int
     """
     if sys.version_info >= (3, 9):
-        parser = argparse.ArgumentParser(prog='multidyndnscli', exit_on_error=False) # type: ignore  # pragma: no cover
+        parser = argparse.ArgumentParser(prog='multidyndnscli',
+            exit_on_error=False) # type: ignore  # pragma: no cover
     else:
         parser = argparse.ArgumentParser(prog='multidyndnscli') # type: ignore  # pragma: no cover
     parser.add_argument("config_file")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--dry-run", "-n", action="store_true")
-    parser.add_argument('--version', action='version', version=f'%(prog)s {multidyndnscli.__version__}')
+    parser.add_argument('--version', action='version',
+        version=f'%(prog)s {multidyndnscli.__version__}')
     try:
         parsed_args = parser.parse_args(args=args)
         config_file = parsed_args.config_file
         dry_run = parsed_args.dry_run
         log_format = "%(asctime)s - %(levelname)s: %(message)s"
         logging.basicConfig(format=log_format)
         if parsed_args.verbose >= 2:
```

### Comparing `multidyndnscli-0.1.3/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.4/multidyndnscli/nc_dnsapi.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.3/multidyndnscli/schemata.py` & `multidyndnscli-0.1.4/multidyndnscli/schemata.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.3/multidyndnscli/util.py` & `multidyndnscli-0.1.4/multidyndnscli/util.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.3/pyproject.toml` & `multidyndnscli-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.3"
+version = "0.1.4"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
```

### Comparing `multidyndnscli-0.1.3/PKG-INFO` & `multidyndnscli-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.3
+Version: 0.1.4
 Summary: DynDNS Command-line Client
 Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -37,15 +37,15 @@
 ## Installation
 Install the package from Pypi (https://pypi.org/project/multidyndnscli) by running `pip install multidyndnscli`. It requires Python 3.8+.
 
 ## Installation on OpenWRT
 First, install the required packages on OpenWRT:
 
 ```bash
-opkg install python3 python3-yaml python3-dns python3-netaddr python3-netifaces
+opkg install python3
 ```
 
 Then install the Pypi packages as described above.
 
 ## Usage
 
 Create a config file and customize it. A small example might look like this:
@@ -199,14 +199,19 @@
 
 Build the docs in folder `docs`:
 
 ```
 poetry run sphinx-build -b html docs/source/  docs/build/html
 ```
 
+### Increase the version
+
+Update the version in `pyproject.tom`. The tool will report this version after the release.
+
+
 # Contributors
 
 See [Contributors](CONTRIBUTORS.md)
 
 # License
 
 Copyright Eike Thaden, 2023.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.3 Summary: DynDNS
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.4 Summary: DynDNS
 Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later Author: Eike Thaden Author-email:
 eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: dnspython
@@ -15,23 +15,22 @@
 multidyndnscli/ Description-Content-Type: text/markdown # DynDNS Command Line
 Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
 ## Installation Install the package from Pypi (https://pypi.org/project/
 multidyndnscli) by running `pip install multidyndnscli`. It requires Python
 3.8+. ## Installation on OpenWRT First, install the required packages on
-OpenWRT: ```bash opkg install python3 python3-yaml python3-dns python3-netaddr
-python3-netifaces ``` Then install the Pypi packages as described above. ##
-Usage Create a config file and customize it. A small example might look like
-this: ``` common: cache_dir: "" dns_providers: - name: "Netcup" type: "Netcup"
-userid: "" apikey: "" apipass: "" router: ipv4: method: "wan" wan_interface: ""
-ipv6: enabled: true method: "wan" wan_interface: "" domains: - name:
-"test.invalid" dns_provider: "Netcup" delay: 300 hosts: - name: "openwrt.lan"
-fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4: "router" ipv6:
-"router" - name: "server.lan" fqdn: "server.home.test.invalid"
+OpenWRT: ```bash opkg install python3 ``` Then install the Pypi packages as
+described above. ## Usage Create a config file and customize it. A small
+example might look like this: ``` common: cache_dir: "" dns_providers: - name:
+"Netcup" type: "Netcup" userid: "" apikey: "" apipass: "" router: ipv4: method:
+"wan" wan_interface: "" ipv6: enabled: true method: "wan" wan_interface: ""
+domains: - name: "test.invalid" dns_provider: "Netcup" delay: 300 hosts: -
+name: "openwrt.lan" fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4:
+"router" ipv6: "router" - name: "server.lan" fqdn: "server.home.test.invalid"
 public_ip_methods: ipv4: "router" ipv6: "local_dns" ``` Create a folder for
 caching data which is writable by the user who runs the script and specify its
 location in `cache_dir`. Configure your DNS provider. Note, that currently only
 Netcup is supported. In our example, the script is running directly on the
 router. The router's IP addresses are identified by getting the public
 addresses of the specified WAN interface. Below, one domain called
 `test.invalid` is configured which consists of two local hosts. The example
@@ -79,10 +78,12 @@
 `pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
 term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
 poetry run black --skip-string-normalization . ``` Alternatively, run formatter
 with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
 multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
 #### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
 Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
-b html docs/source/ docs/build/html ``` # Contributors See [Contributors]
-(CONTRIBUTORS.md) # License Copyright Eike Thaden, 2023. Distributed under the
-terms of the GPL v3 license, multidyndnscli is free and open source software.
+b html docs/source/ docs/build/html ``` ### Increase the version Update the
+version in `pyproject.tom`. The tool will report this version after the
+release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
+Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
+multidyndnscli is free and open source software.
```

