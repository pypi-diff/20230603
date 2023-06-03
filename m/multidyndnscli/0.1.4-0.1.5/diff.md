# Comparing `tmp/multidyndnscli-0.1.4.tar.gz` & `tmp/multidyndnscli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.4.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.5.tar", max compression
```

## Comparing `multidyndnscli-0.1.4.tar` & `multidyndnscli-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/LICENSE
--rw-r--r--   0        0        0     6763 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/README.md
--rw-r--r--   0        0        0    34179 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     2331 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6951 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2771 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3844 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/multidyndnscli/util.py
--rw-r--r--   0        0        0     1285 2023-06-03 12:40:44.070040 multidyndnscli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidyndnscli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6930 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/README.md
+-rw-r--r--   0        0        0    34179 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2331 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6907 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2771 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1287 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 multidyndnscli-0.1.5/PKG-INFO
```

### Comparing `multidyndnscli-0.1.4/LICENSE` & `multidyndnscli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.4/README.md` & `multidyndnscli-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 <a href="https://github.com/ethaden/multidyndnscli/blob/main/LICENSE"><img alt="License: GPL v3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
 <a href="https://img.shields.io/pypi/v/multidyndnscli"><img alt="Pypi Version" src="https://img.shields.io/pypi/v/multidyndnscli"></a>
 <a href="https://img.shields.io/pypi/pyversions/multidyndnscli"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/multidyndnscli"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ## Installation
-Install the package from Pypi (https://pypi.org/project/multidyndnscli) by running `pip install multidyndnscli`. It requires Python 3.8+.
+THis project requires Python 3.8+.
+Install the package from Pypi by running `pip install multidyndnscli`.
 
+For details, see https://pypi.org/project/multidyndnscli.
 ## Installation on OpenWRT
 First, install the required packages on OpenWRT:
 
 ```bash
 opkg install python3
 ```
 
 Then install the Pypi packages as described above.
 
 ## Usage
 
+### Config file
+
 Create a config file and customize it. A small example might look like this:
 
 ```
 common:
   cache_dir: "<existing writable folder for caching data>"
 dns_providers:
   - name: "Netcup"
@@ -68,14 +72,18 @@
 
 For every configured domain, all records to be updated will be identified and the whole domain will be changed using only one query to the DNS providers API. In the example, a `delay` of 300 seconds has been configured. If the last update for the domain has been done less tehn `delay` seconds ago, the current update will be skipped. This is particularly useful for DNSSEC-enabled domains, where the domain has to be resigned after any updates. Resigning may take quite a while and no further updates should be done until the updated values have become visible.
 
 You can find a complete example configuration file [here](config.example.yaml).
 
 For further information, have a look at the documentation: https://ethaden.github.io/multidyndnscli/.
 
+### Running multidyndnscli
+
+Once the Python package is installed, run it by executing `multidyndnscli <your-config-file>`.
+
 ## Development
 
 ### Using a dev container
 If using Visual Studio Code, you'll can make use of a working dev container setup specified in `.devcontainer` which should be found automatically. Make sure to adapt the WAN interface used for testing - if any - to the one configure within the running container.
 
 ### Local development `pyenv`
 This project can use `pyenv`, though using it is not mandatory. You can install `pyenv` by following the instructions on the pyenv website https://github.com/pyenv/pyenv.
```

#### html2text {}

```diff
@@ -1,74 +1,77 @@
 # DynDNS Command Line Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
-## Installation Install the package from Pypi (https://pypi.org/project/
-multidyndnscli) by running `pip install multidyndnscli`. It requires Python
-3.8+. ## Installation on OpenWRT First, install the required packages on
-OpenWRT: ```bash opkg install python3 ``` Then install the Pypi packages as
-described above. ## Usage Create a config file and customize it. A small
-example might look like this: ``` common: cache_dir: "" dns_providers: - name:
-"Netcup" type: "Netcup" userid: "" apikey: "" apipass: "" router: ipv4: method:
-"wan" wan_interface: "" ipv6: enabled: true method: "wan" wan_interface: ""
-domains: - name: "test.invalid" dns_provider: "Netcup" delay: 300 hosts: -
-name: "openwrt.lan" fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4:
-"router" ipv6: "router" - name: "server.lan" fqdn: "server.home.test.invalid"
-public_ip_methods: ipv4: "router" ipv6: "local_dns" ``` Create a folder for
-caching data which is writable by the user who runs the script and specify its
-location in `cache_dir`. Configure your DNS provider. Note, that currently only
-Netcup is supported. In our example, the script is running directly on the
-router. The router's IP addresses are identified by getting the public
-addresses of the specified WAN interface. Below, one domain called
-`test.invalid` is configured which consists of two local hosts. The example
-uses the DNS provder called `Netcup` (see above) for configuring the domain.
-The `name` of each host has to be equal to the fully-qualified domain name used
-internally to talk the respective hosts. The `fqdn` is the public DNS name
-which should point to the IP addresses of that host or the router. In many
-cases, there is only one public IPv4 address for the router and all internal
-hosts use private IPv4 addresses. In such a case, using `ipv4: "router"` in
-`public_ip_methods` will use the router's IPv4 address for the public FQDN. For
-IPv6, usually each host as well as the router will have public IPv6 addresses.
-Using `ipv6: "local_dns"` will make sure that the local DNS server is queried
-for each host's name and the first public IPv6 found is used for reconfiguring
-the public DNS. For every configured domain, all records to be updated will be
+## Installation THis project requires Python 3.8+. Install the package from
+Pypi by running `pip install multidyndnscli`. For details, see https://
+pypi.org/project/multidyndnscli. ## Installation on OpenWRT First, install the
+required packages on OpenWRT: ```bash opkg install python3 ``` Then install the
+Pypi packages as described above. ## Usage ### Config file Create a config file
+and customize it. A small example might look like this: ``` common: cache_dir:
+"" dns_providers: - name: "Netcup" type: "Netcup" userid: "" apikey: ""
+apipass: "" router: ipv4: method: "wan" wan_interface: "" ipv6: enabled: true
+method: "wan" wan_interface: "" domains: - name: "test.invalid" dns_provider:
+"Netcup" delay: 300 hosts: - name: "openwrt.lan" fqdn:
+"openwrt.home.test.invalid" public_ip_methods: ipv4: "router" ipv6: "router" -
+name: "server.lan" fqdn: "server.home.test.invalid" public_ip_methods: ipv4:
+"router" ipv6: "local_dns" ``` Create a folder for caching data which is
+writable by the user who runs the script and specify its location in
+`cache_dir`. Configure your DNS provider. Note, that currently only Netcup is
+supported. In our example, the script is running directly on the router. The
+router's IP addresses are identified by getting the public addresses of the
+specified WAN interface. Below, one domain called `test.invalid` is configured
+which consists of two local hosts. The example uses the DNS provder called
+`Netcup` (see above) for configuring the domain. The `name` of each host has to
+be equal to the fully-qualified domain name used internally to talk the
+respective hosts. The `fqdn` is the public DNS name which should point to the
+IP addresses of that host or the router. In many cases, there is only one
+public IPv4 address for the router and all internal hosts use private IPv4
+addresses. In such a case, using `ipv4: "router"` in `public_ip_methods` will
+use the router's IPv4 address for the public FQDN. For IPv6, usually each host
+as well as the router will have public IPv6 addresses. Using `ipv6:
+"local_dns"` will make sure that the local DNS server is queried for each
+host's name and the first public IPv6 found is used for reconfiguring the
+public DNS. For every configured domain, all records to be updated will be
 identified and the whole domain will be changed using only one query to the DNS
 providers API. In the example, a `delay` of 300 seconds has been configured. If
 the last update for the domain has been done less tehn `delay` seconds ago, the
 current update will be skipped. This is particularly useful for DNSSEC-enabled
 domains, where the domain has to be resigned after any updates. Resigning may
 take quite a while and no further updates should be done until the updated
 values have become visible. You can find a complete example configuration file
 [here](config.example.yaml). For further information, have a look at the
-documentation: https://ethaden.github.io/multidyndnscli/. ## Development ###
-Using a dev container If using Visual Studio Code, you'll can make use of a
-working dev container setup specified in `.devcontainer` which should be found
-automatically. Make sure to adapt the WAN interface used for testing - if any -
-to the one configure within the running container. ### Local development
-`pyenv` This project can use `pyenv`, though using it is not mandatory. You can
-install `pyenv` by following the instructions on the pyenv website https://
-github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
-Initialize the required/desired python environments: ``` pyenv install 3.8
-pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
-version: ``` pyenv versions ``` #### Installing `poetry` This project use based
-on `poetry`. You can install `poetry` by following the instructions on the
-poetry website https://python-poetry.org/. #### Install all packages with
-poetry For development including tools for generating documentation, use: ```
-poetry install ``` For installing only the packages required to run the tool,
-use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
-following to enable python pre-commit: ``` poetry run pre-commit install ```
-You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
-all-files ``` ### Running the development tools There are basically three ways
-to run tools. You can use `tox`, run the commands directly on the command line
-or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
-Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
-`pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
-term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
-poetry run black --skip-string-normalization . ``` Alternatively, run formatter
-with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
-multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
-#### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
-Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
-b html docs/source/ docs/build/html ``` ### Increase the version Update the
-version in `pyproject.tom`. The tool will report this version after the
-release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
-Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
-multidyndnscli is free and open source software.
+documentation: https://ethaden.github.io/multidyndnscli/. ### Running
+multidyndnscli Once the Python package is installed, run it by executing
+`multidyndnscli `. ## Development ### Using a dev container If using Visual
+Studio Code, you'll can make use of a working dev container setup specified in
+`.devcontainer` which should be found automatically. Make sure to adapt the WAN
+interface used for testing - if any - to the one configure within the running
+container. ### Local development `pyenv` This project can use `pyenv`, though
+using it is not mandatory. You can install `pyenv` by following the
+instructions on the pyenv website https://github.com/pyenv/pyenv. List
+installable versions ``` pyenv install -l ``` Initialize the required/desired
+python environments: ``` pyenv install 3.8 pyenv install 3.9 pyenv install 3.10
+pyenv install 3.11 ``` Show installed version: ``` pyenv versions ``` ####
+Installing `poetry` This project use based on `poetry`. You can install
+`poetry` by following the instructions on the poetry website https://python-
+poetry.org/. #### Install all packages with poetry For development including
+tools for generating documentation, use: ``` poetry install ``` For installing
+only the packages required to run the tool, use: ``` poetry install --without
+dev ``` #### Installing pre-commit Run the following to enable python pre-
+commit: ``` poetry run pre-commit install ``` You can run the pre-commit
+scripts manually: ``` poetry run pre-commit run --all-files ``` ### Running the
+development tools There are basically three ways to run tools. You can use
+`tox`, run the commands directly on the command line or - if using Visual
+Studio Code - use some VS code preconfigured tasks. #### Running tests You can
+use `tox`: ``` tox ``` Alternatively, you can run `pytest` manually: ``` poetry
+run pytest --cov-report xml:cov.xml --cov-report term-missing --
+cov=multidyndnscli tests/ ``` #### Running code formatter ``` poetry run black
+--skip-string-normalization . ``` Alternatively, run formatter with tox: ```
+tox -e format ``` #### Run linter ``` poetry run pylint multidyndnscli ```
+Alternatively, run linter with tox: ``` tox -e linter ``` #### Running code
+analysis with mypy ``` poetry run mypy multidyndnscli ``` ### Build the docs
+Build the docs in folder `docs`: ``` poetry run sphinx-build -b html docs/
+source/ docs/build/html ``` ### Increase the version Update the version in
+`pyproject.tom`. The tool will report this version after the release. #
+Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright Eike
+Thaden, 2023. Distributed under the terms of the GPL v3 license, multidyndnscli
+is free and open source software.
```

### Comparing `multidyndnscli-0.1.4/multidyndnscli/__init__.py` & `multidyndnscli-0.1.5/multidyndnscli/__init__.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.4/multidyndnscli/cli.py` & `multidyndnscli-0.1.5/multidyndnscli/cli.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.4/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.5/multidyndnscli/nc_dnsapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 ? (tuxmaster5000)
 ? (jp-coding)
 
 """
 
 import requests
 import json
-import pytest
-pytestmark = pytest.mark.skip
 
 name = "nc_dns"
 
 class DNSZone(object):
     def __init__(self, name, ttl, serial, refresh, retry, expire, dnssecstatus):
         self.name = name
         self.ttl = ttl
```

### Comparing `multidyndnscli-0.1.4/multidyndnscli/schemata.py` & `multidyndnscli-0.1.5/multidyndnscli/schemata.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.4/multidyndnscli/util.py` & `multidyndnscli-0.1.5/multidyndnscli/util.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.4/pyproject.toml` & `multidyndnscli-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.4"
+version = "0.1.5"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
@@ -35,15 +35,15 @@
 types-requests = "^2.29.0.0"
 pytest-mock = "^3.10.0"
 sphinx = {version = "^7.0.1"}
 furo = {version = "^2023.5.20"}
 sphinx-autoapi = {version = "^2.1.0"}
 
 [tool.poetry.scripts]
-multi-dyndns-cli = "multidyndnscli:run"
+multidyndnscli = "multidyndnscli.cli:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*"]
```

### Comparing `multidyndnscli-0.1.4/PKG-INFO` & `multidyndnscli-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.4
+Version: 0.1.5
 Summary: DynDNS Command-line Client
 Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -31,27 +31,31 @@
 <a href="https://github.com/ethaden/multidyndnscli/blob/main/LICENSE"><img alt="License: GPL v3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
 <a href="https://img.shields.io/pypi/v/multidyndnscli"><img alt="Pypi Version" src="https://img.shields.io/pypi/v/multidyndnscli"></a>
 <a href="https://img.shields.io/pypi/pyversions/multidyndnscli"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/multidyndnscli"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ## Installation
-Install the package from Pypi (https://pypi.org/project/multidyndnscli) by running `pip install multidyndnscli`. It requires Python 3.8+.
+THis project requires Python 3.8+.
+Install the package from Pypi by running `pip install multidyndnscli`.
 
+For details, see https://pypi.org/project/multidyndnscli.
 ## Installation on OpenWRT
 First, install the required packages on OpenWRT:
 
 ```bash
 opkg install python3
 ```
 
 Then install the Pypi packages as described above.
 
 ## Usage
 
+### Config file
+
 Create a config file and customize it. A small example might look like this:
 
 ```
 common:
   cache_dir: "<existing writable folder for caching data>"
 dns_providers:
   - name: "Netcup"
@@ -94,14 +98,18 @@
 
 For every configured domain, all records to be updated will be identified and the whole domain will be changed using only one query to the DNS providers API. In the example, a `delay` of 300 seconds has been configured. If the last update for the domain has been done less tehn `delay` seconds ago, the current update will be skipped. This is particularly useful for DNSSEC-enabled domains, where the domain has to be resigned after any updates. Resigning may take quite a while and no further updates should be done until the updated values have become visible.
 
 You can find a complete example configuration file [here](config.example.yaml).
 
 For further information, have a look at the documentation: https://ethaden.github.io/multidyndnscli/.
 
+### Running multidyndnscli
+
+Once the Python package is installed, run it by executing `multidyndnscli <your-config-file>`.
+
 ## Development
 
 ### Using a dev container
 If using Visual Studio Code, you'll can make use of a working dev container setup specified in `.devcontainer` which should be found automatically. Make sure to adapt the WAN interface used for testing - if any - to the one configure within the running container.
 
 ### Local development `pyenv`
 This project can use `pyenv`, though using it is not mandatory. You can install `pyenv` by following the instructions on the pyenv website https://github.com/pyenv/pyenv.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.4 Summary: DynDNS
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.5 Summary: DynDNS
 Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later Author: Eike Thaden Author-email:
 eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: dnspython
@@ -12,78 +12,81 @@
 pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
 schema (>=0.7.5,<0.8.0) Project-URL: Documentation, https://ethaden.github.io/
 multidyndnscli/ Project-URL: Repository, https://github.com/ethaden/
 multidyndnscli/ Description-Content-Type: text/markdown # DynDNS Command Line
 Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
-## Installation Install the package from Pypi (https://pypi.org/project/
-multidyndnscli) by running `pip install multidyndnscli`. It requires Python
-3.8+. ## Installation on OpenWRT First, install the required packages on
-OpenWRT: ```bash opkg install python3 ``` Then install the Pypi packages as
-described above. ## Usage Create a config file and customize it. A small
-example might look like this: ``` common: cache_dir: "" dns_providers: - name:
-"Netcup" type: "Netcup" userid: "" apikey: "" apipass: "" router: ipv4: method:
-"wan" wan_interface: "" ipv6: enabled: true method: "wan" wan_interface: ""
-domains: - name: "test.invalid" dns_provider: "Netcup" delay: 300 hosts: -
-name: "openwrt.lan" fqdn: "openwrt.home.test.invalid" public_ip_methods: ipv4:
-"router" ipv6: "router" - name: "server.lan" fqdn: "server.home.test.invalid"
-public_ip_methods: ipv4: "router" ipv6: "local_dns" ``` Create a folder for
-caching data which is writable by the user who runs the script and specify its
-location in `cache_dir`. Configure your DNS provider. Note, that currently only
-Netcup is supported. In our example, the script is running directly on the
-router. The router's IP addresses are identified by getting the public
-addresses of the specified WAN interface. Below, one domain called
-`test.invalid` is configured which consists of two local hosts. The example
-uses the DNS provder called `Netcup` (see above) for configuring the domain.
-The `name` of each host has to be equal to the fully-qualified domain name used
-internally to talk the respective hosts. The `fqdn` is the public DNS name
-which should point to the IP addresses of that host or the router. In many
-cases, there is only one public IPv4 address for the router and all internal
-hosts use private IPv4 addresses. In such a case, using `ipv4: "router"` in
-`public_ip_methods` will use the router's IPv4 address for the public FQDN. For
-IPv6, usually each host as well as the router will have public IPv6 addresses.
-Using `ipv6: "local_dns"` will make sure that the local DNS server is queried
-for each host's name and the first public IPv6 found is used for reconfiguring
-the public DNS. For every configured domain, all records to be updated will be
+## Installation THis project requires Python 3.8+. Install the package from
+Pypi by running `pip install multidyndnscli`. For details, see https://
+pypi.org/project/multidyndnscli. ## Installation on OpenWRT First, install the
+required packages on OpenWRT: ```bash opkg install python3 ``` Then install the
+Pypi packages as described above. ## Usage ### Config file Create a config file
+and customize it. A small example might look like this: ``` common: cache_dir:
+"" dns_providers: - name: "Netcup" type: "Netcup" userid: "" apikey: ""
+apipass: "" router: ipv4: method: "wan" wan_interface: "" ipv6: enabled: true
+method: "wan" wan_interface: "" domains: - name: "test.invalid" dns_provider:
+"Netcup" delay: 300 hosts: - name: "openwrt.lan" fqdn:
+"openwrt.home.test.invalid" public_ip_methods: ipv4: "router" ipv6: "router" -
+name: "server.lan" fqdn: "server.home.test.invalid" public_ip_methods: ipv4:
+"router" ipv6: "local_dns" ``` Create a folder for caching data which is
+writable by the user who runs the script and specify its location in
+`cache_dir`. Configure your DNS provider. Note, that currently only Netcup is
+supported. In our example, the script is running directly on the router. The
+router's IP addresses are identified by getting the public addresses of the
+specified WAN interface. Below, one domain called `test.invalid` is configured
+which consists of two local hosts. The example uses the DNS provder called
+`Netcup` (see above) for configuring the domain. The `name` of each host has to
+be equal to the fully-qualified domain name used internally to talk the
+respective hosts. The `fqdn` is the public DNS name which should point to the
+IP addresses of that host or the router. In many cases, there is only one
+public IPv4 address for the router and all internal hosts use private IPv4
+addresses. In such a case, using `ipv4: "router"` in `public_ip_methods` will
+use the router's IPv4 address for the public FQDN. For IPv6, usually each host
+as well as the router will have public IPv6 addresses. Using `ipv6:
+"local_dns"` will make sure that the local DNS server is queried for each
+host's name and the first public IPv6 found is used for reconfiguring the
+public DNS. For every configured domain, all records to be updated will be
 identified and the whole domain will be changed using only one query to the DNS
 providers API. In the example, a `delay` of 300 seconds has been configured. If
 the last update for the domain has been done less tehn `delay` seconds ago, the
 current update will be skipped. This is particularly useful for DNSSEC-enabled
 domains, where the domain has to be resigned after any updates. Resigning may
 take quite a while and no further updates should be done until the updated
 values have become visible. You can find a complete example configuration file
 [here](config.example.yaml). For further information, have a look at the
-documentation: https://ethaden.github.io/multidyndnscli/. ## Development ###
-Using a dev container If using Visual Studio Code, you'll can make use of a
-working dev container setup specified in `.devcontainer` which should be found
-automatically. Make sure to adapt the WAN interface used for testing - if any -
-to the one configure within the running container. ### Local development
-`pyenv` This project can use `pyenv`, though using it is not mandatory. You can
-install `pyenv` by following the instructions on the pyenv website https://
-github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
-Initialize the required/desired python environments: ``` pyenv install 3.8
-pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
-version: ``` pyenv versions ``` #### Installing `poetry` This project use based
-on `poetry`. You can install `poetry` by following the instructions on the
-poetry website https://python-poetry.org/. #### Install all packages with
-poetry For development including tools for generating documentation, use: ```
-poetry install ``` For installing only the packages required to run the tool,
-use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
-following to enable python pre-commit: ``` poetry run pre-commit install ```
-You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
-all-files ``` ### Running the development tools There are basically three ways
-to run tools. You can use `tox`, run the commands directly on the command line
-or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
-Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
-`pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
-term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
-poetry run black --skip-string-normalization . ``` Alternatively, run formatter
-with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
-multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
-#### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
-Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
-b html docs/source/ docs/build/html ``` ### Increase the version Update the
-version in `pyproject.tom`. The tool will report this version after the
-release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
-Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
-multidyndnscli is free and open source software.
+documentation: https://ethaden.github.io/multidyndnscli/. ### Running
+multidyndnscli Once the Python package is installed, run it by executing
+`multidyndnscli `. ## Development ### Using a dev container If using Visual
+Studio Code, you'll can make use of a working dev container setup specified in
+`.devcontainer` which should be found automatically. Make sure to adapt the WAN
+interface used for testing - if any - to the one configure within the running
+container. ### Local development `pyenv` This project can use `pyenv`, though
+using it is not mandatory. You can install `pyenv` by following the
+instructions on the pyenv website https://github.com/pyenv/pyenv. List
+installable versions ``` pyenv install -l ``` Initialize the required/desired
+python environments: ``` pyenv install 3.8 pyenv install 3.9 pyenv install 3.10
+pyenv install 3.11 ``` Show installed version: ``` pyenv versions ``` ####
+Installing `poetry` This project use based on `poetry`. You can install
+`poetry` by following the instructions on the poetry website https://python-
+poetry.org/. #### Install all packages with poetry For development including
+tools for generating documentation, use: ``` poetry install ``` For installing
+only the packages required to run the tool, use: ``` poetry install --without
+dev ``` #### Installing pre-commit Run the following to enable python pre-
+commit: ``` poetry run pre-commit install ``` You can run the pre-commit
+scripts manually: ``` poetry run pre-commit run --all-files ``` ### Running the
+development tools There are basically three ways to run tools. You can use
+`tox`, run the commands directly on the command line or - if using Visual
+Studio Code - use some VS code preconfigured tasks. #### Running tests You can
+use `tox`: ``` tox ``` Alternatively, you can run `pytest` manually: ``` poetry
+run pytest --cov-report xml:cov.xml --cov-report term-missing --
+cov=multidyndnscli tests/ ``` #### Running code formatter ``` poetry run black
+--skip-string-normalization . ``` Alternatively, run formatter with tox: ```
+tox -e format ``` #### Run linter ``` poetry run pylint multidyndnscli ```
+Alternatively, run linter with tox: ``` tox -e linter ``` #### Running code
+analysis with mypy ``` poetry run mypy multidyndnscli ``` ### Build the docs
+Build the docs in folder `docs`: ``` poetry run sphinx-build -b html docs/
+source/ docs/build/html ``` ### Increase the version Update the version in
+`pyproject.tom`. The tool will report this version after the release. #
+Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright Eike
+Thaden, 2023. Distributed under the terms of the GPL v3 license, multidyndnscli
+is free and open source software.
```

