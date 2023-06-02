# Comparing `tmp/multidyndnscli-0.1.1.tar.gz` & `tmp/multidyndnscli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.1.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.2.tar", max compression
```

## Comparing `multidyndnscli-0.1.1.tar` & `multidyndnscli-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-02 18:43:13.277242 multidyndnscli-0.1.1/LICENSE
--rw-r--r--   0        0        0     6608 2023-06-02 18:43:13.277242 multidyndnscli-0.1.1/README.md
--rw-r--r--   0        0        0    33878 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     1935 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6784 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2545 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3618 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/multidyndnscli/util.py
--rw-r--r--   0        0        0     1337 2023-06-02 18:43:13.281242 multidyndnscli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7746 1970-01-01 00:00:00.000000 multidyndnscli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6702 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/README.md
+-rw-r--r--   0        0        0    34104 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6951 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2771 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1254 2023-06-02 22:42:09.390575 multidyndnscli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7721 1970-01-01 00:00:00.000000 multidyndnscli-0.1.2/PKG-INFO
```

### Comparing `multidyndnscli-0.1.1/LICENSE` & `multidyndnscli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.1/README.md` & `multidyndnscli-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # DynDNS Command Line Tool
 <p align="left">
 <a href="https://github.com/ethaden/multidyndnscli/actions/workflows/test.yml/"><img alt="Test Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/test.yml/badge.svg"></a>
-<a href="ttps://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/"><img alt="Docs Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/badge.svg"></a>
+<a href="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/"><img alt="Docs Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/badge.svg"></a>
 <a href="https://github.com/ethaden/multidyndnscli/blob/main/LICENSE"><img alt="License: GPL v3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
 <a href="https://img.shields.io/pypi/v/multidyndnscli"><img alt="Pypi Version" src="https://img.shields.io/pypi/v/multidyndnscli"></a>
 <a href="https://img.shields.io/pypi/pyversions/multidyndnscli"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/multidyndnscli"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ## Installation
@@ -102,15 +102,15 @@
 This project use based on `poetry`. You can install `poetry` by following the instructions on the poetry website https://python-poetry.org/.
 
 #### Install all packages with poetry
 
 For development including tools for generating documentation, use:
 
 ```
-poetry install -E docs
+poetry install
 ```
 
 For installing only the packages required to run the tool, use:
 
 ```
 poetry install --without dev
 ```
@@ -166,17 +166,23 @@
 
 #### Running code analysis with mypy
 ```
 poetry run mypy multidyndnscli
 ```
 
 ### Build the docs
-First, install the extra packages for building the docs:
-```
-poetry install --extras docs
-```
 
 Build the docs in folder `docs`:
 
 ```
 poetry run sphinx-build -b html docs/source/  docs/build/html
 ```
+
+# Contributors
+
+See [Contributors](CONTRIBUTORS.md)
+
+# License
+
+Copyright Eike Thaden, 2023.
+
+Distributed under the terms of the GPL v3 license, multidyndnscli is free and open source software.
```

#### html2text {}

```diff
@@ -49,24 +49,25 @@
 github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
 Initialize the required/desired python environments: ``` pyenv install 3.8
 pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
 version: ``` pyenv versions ``` #### Installing `poetry` This project use based
 on `poetry`. You can install `poetry` by following the instructions on the
 poetry website https://python-poetry.org/. #### Install all packages with
 poetry For development including tools for generating documentation, use: ```
-poetry install -E docs ``` For installing only the packages required to run the
-tool, use: ``` poetry install --without dev ``` #### Installing pre-commit Run
-the following to enable python pre-commit: ``` poetry run pre-commit install
-``` You can run the pre-commit scripts manually: ``` poetry run pre-commit run
---all-files ``` ### Running the development tools There are basically three
-ways to run tools. You can use `tox`, run the commands directly on the command
-line or - if using Visual Studio Code - use some VS code preconfigured tasks.
-#### Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
+poetry install ``` For installing only the packages required to run the tool,
+use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
+following to enable python pre-commit: ``` poetry run pre-commit install ```
+You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
+all-files ``` ### Running the development tools There are basically three ways
+to run tools. You can use `tox`, run the commands directly on the command line
+or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
+Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
 `pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
 term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
 poetry run black --skip-string-normalization . ``` Alternatively, run formatter
 with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
 multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
 #### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
-Build the docs First, install the extra packages for building the docs: ```
-poetry install --extras docs ``` Build the docs in folder `docs`: ``` poetry
-run sphinx-build -b html docs/source/ docs/build/html ```
+Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
+b html docs/source/ docs/build/html ``` # Contributors See [Contributors]
+(CONTRIBUTORS.md) # License Copyright Eike Thaden, 2023. Distributed under the
+terms of the GPL v3 license, multidyndnscli is free and open source software.
```

### Comparing `multidyndnscli-0.1.1/multidyndnscli/__init__.py` & `multidyndnscli-0.1.2/multidyndnscli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the GPL v3: https://www.gnu.org/licenses/gpl-3.0
+# For details: https://github.com/ethaden/multidyndnscli/blob/main/LICENSE
+# Copyright (c) https://github.com/ethaden/multidyndnscli/blob/main/CONTRIBUTORS.md
+
 """
 Yet another python module for router-based multi-domain, multi-host dynamic dns (dyndns), 
 with support for IPv4 and IPv6.
 This project currently only supports Netcup, but might be extended in the future.
 
 """
 import logging
```

### Comparing `multidyndnscli-0.1.1/multidyndnscli/cli.py` & `multidyndnscli-0.1.2/multidyndnscli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Licensed under the GPL v3: https://www.gnu.org/licenses/gpl-3.0
+# For details: https://github.com/ethaden/multidyndnscli/blob/main/LICENSE
+# Copyright (c) https://github.com/ethaden/multidyndnscli/blob/main/CONTRIBUTORS.md
+
+
 """Command-line interface for multidnscli"""
 import logging
 import sys
 import argparse
 from typing import List, Optional
 import yaml
 import multidyndnscli
```

### Comparing `multidyndnscli-0.1.1/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.2/multidyndnscli/nc_dnsapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Licensed under the GPL v3: https://www.gnu.org/licenses/gpl-3.0
+# Copyright (c) Nicolai Buchwitz (nbuchwitz), Thomas G. (coldfix), ? (tuxmaster5000), ? (jp-coding)
+
 """Netcup DNS API v0.1.6
 
 Because version 0.1.6 has never been released on pypi, 
 this file has been copied from the original Netcup DNS API project found here:
 https://github.com/nbuchwitz/nc_dnsapi
 
 Original License: GPL v3
```

### Comparing `multidyndnscli-0.1.1/multidyndnscli/schemata.py` & `multidyndnscli-0.1.2/multidyndnscli/schemata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the GPL v3: https://www.gnu.org/licenses/gpl-3.0
+# For details: https://github.com/ethaden/multidyndnscli/blob/main/LICENSE
+# Copyright (c) https://github.com/ethaden/multidyndnscli/blob/main/CONTRIBUTORS.md
+
 """Defines the config file schema for multidyndnscli"""
 from schema import Schema, And, Or, Optional, Use  # type: ignore
 
 def get_config_file_schema()->Schema:
     """Create the config file schema
 
     :return: Config file schema
```

### Comparing `multidyndnscli-0.1.1/multidyndnscli/util.py` & `multidyndnscli-0.1.2/multidyndnscli/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Licensed under the GPL v3: https://www.gnu.org/licenses/gpl-3.0
+# For details: https://github.com/ethaden/multidyndnscli/blob/main/LICENSE
+# Copyright (c) https://github.com/ethaden/multidyndnscli/blob/main/CONTRIBUTORS.md
+
 """Utility methods for multidyndnscli"""
 from typing import List
 import netaddr  # type: ignore
 import netifaces  # type: ignore
 
 ipv4_private_net_192_168 = netaddr.IPNetwork("192.168.0.0/16")
 ipv4_private_net_172_16 = netaddr.IPNetwork("172.16.0.0/12")
```

### Comparing `multidyndnscli-0.1.1/pyproject.toml` & `multidyndnscli-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.1"
+version = "0.1.2"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
-license = "GPLv3"
+license = "GPL-3.0-or-later"
 readme = "README.md"
-homepage = "https://pypi.org/project/multidyndnscli/"
+homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 dnspython = "^2.3.0"
 pyyaml = "^6.0"
 netaddr = "^0.8.0"
 netifaces = "^0.11.0"
 requests = "^2.28.2"
 fritzconnection = "^1.12.0"
 schema = "^0.7.5"
-sphinx = {version = "^7.0.1", extras = ["docs"]}
-furo = {version = "^2023.5.20", extras = ["docs"]}
-sphinx-autoapi = {version = "^2.1.0", extras = ["docs"]}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
@@ -32,17 +29,17 @@
 mypy = "^1.2.0"
 pydantic = "^1.10.7"
 tox = "^4.5.1"
 coverage = {extras = ["toml"], version = "^7.2.5"}
 types-pyyaml = "^6.0.12.9"
 types-requests = "^2.29.0.0"
 pytest-mock = "^3.10.0"
-
-[tool.poetry.extras]
-docs = ["pdoc"]
+sphinx = {version = "^7.0.1"}
+furo = {version = "^2023.5.20"}
+sphinx-autoapi = {version = "^2.1.0"}
 
 [tool.poetry.scripts]
 multi-dyndns-cli = "multidyndnscli:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multidyndnscli-0.1.1/PKG-INFO` & `multidyndnscli-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.1
+Version: 0.1.2
 Summary: DynDNS Command-line Client
-Home-page: https://pypi.org/project/multidyndnscli/
-License: GPLv3
+Home-page: https://ethaden.github.io/multidyndnscli/
+License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: docs
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
 Requires-Dist: fritzconnection (>=1.12.0,<2.0.0)
-Requires-Dist: furo[docs] (>=2023.5.20,<2024.0.0)
 Requires-Dist: netaddr (>=0.8.0,<0.9.0)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
-Requires-Dist: sphinx-autoapi[docs] (>=2.1.0,<3.0.0)
-Requires-Dist: sphinx[docs] (>=7.0.1,<8.0.0)
 Project-URL: Documentation, https://ethaden.github.io/multidyndnscli/
 Project-URL: Repository, https://github.com/ethaden/multidyndnscli/
 Description-Content-Type: text/markdown
 
 # DynDNS Command Line Tool
 <p align="left">
 <a href="https://github.com/ethaden/multidyndnscli/actions/workflows/test.yml/"><img alt="Test Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/test.yml/badge.svg"></a>
-<a href="ttps://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/"><img alt="Docs Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/badge.svg"></a>
+<a href="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/"><img alt="Docs Status" src="https://github.com/ethaden/multidyndnscli/actions/workflows/docs.yml/badge.svg"></a>
 <a href="https://github.com/ethaden/multidyndnscli/blob/main/LICENSE"><img alt="License: GPL v3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
 <a href="https://img.shields.io/pypi/v/multidyndnscli"><img alt="Pypi Version" src="https://img.shields.io/pypi/v/multidyndnscli"></a>
 <a href="https://img.shields.io/pypi/pyversions/multidyndnscli"><img alt="Python Versions" src="https://img.shields.io/pypi/pyversions/multidyndnscli"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ## Installation
@@ -131,15 +127,15 @@
 This project use based on `poetry`. You can install `poetry` by following the instructions on the poetry website https://python-poetry.org/.
 
 #### Install all packages with poetry
 
 For development including tools for generating documentation, use:
 
 ```
-poetry install -E docs
+poetry install
 ```
 
 For installing only the packages required to run the tool, use:
 
 ```
 poetry install --without dev
 ```
@@ -195,18 +191,24 @@
 
 #### Running code analysis with mypy
 ```
 poetry run mypy multidyndnscli
 ```
 
 ### Build the docs
-First, install the extra packages for building the docs:
-```
-poetry install --extras docs
-```
 
 Build the docs in folder `docs`:
 
 ```
 poetry run sphinx-build -b html docs/source/  docs/build/html
 ```
 
+# Contributors
+
+See [Contributors](CONTRIBUTORS.md)
+
+# License
+
+Copyright Eike Thaden, 2023.
+
+Distributed under the terms of the GPL v3 license, multidyndnscli is free and open source software.
+
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.1 Summary: DynDNS
-Command-line Client Home-page: https://pypi.org/project/multidyndnscli/
-License: GPLv3 Author: Eike Thaden Author-email: eike.thaden@gmail.com
-Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: Other/Proprietary
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Provides-Extra: docs
-Requires-Dist: dnspython (>=2.3.0,<3.0.0) Requires-Dist: fritzconnection
-(>=1.12.0,<2.0.0) Requires-Dist: furo[docs] (>=2023.5.20,<2024.0.0) Requires-
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.2 Summary: DynDNS
+Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
+License: GPL-3.0-or-later Author: Eike Thaden Author-email:
+eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
+OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: dnspython
+(>=2.3.0,<3.0.0) Requires-Dist: fritzconnection (>=1.12.0,<2.0.0) Requires-
 Dist: netaddr (>=0.8.0,<0.9.0) Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: schema (>=0.7.5,<0.8.0) Requires-Dist: sphinx-autoapi[docs]
-(>=2.1.0,<3.0.0) Requires-Dist: sphinx[docs] (>=7.0.1,<8.0.0) Project-URL:
-Documentation, https://ethaden.github.io/multidyndnscli/ Project-URL:
-Repository, https://github.com/ethaden/multidyndnscli/ Description-Content-
-Type: text/markdown # DynDNS Command Line Tool
+Requires-Dist: schema (>=0.7.5,<0.8.0) Project-URL: Documentation, https://
+ethaden.github.io/multidyndnscli/ Project-URL: Repository, https://github.com/
+ethaden/multidyndnscli/ Description-Content-Type: text/markdown # DynDNS
+Command Line Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
 ## Installation Install the package from Pypi (https://pypi.org/project/
 multidyndnscli) by running `pip install multidyndnscli`. It requires Python
 3.8+. ## Installation on OpenWRT First, install the required packages on
 OpenWRT: ```bash opkg install python3 python3-yaml python3-dns python3-netaddr
 python3-netifaces ``` Then install the Pypi packages as described above. ##
@@ -64,24 +63,25 @@
 github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
 Initialize the required/desired python environments: ``` pyenv install 3.8
 pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
 version: ``` pyenv versions ``` #### Installing `poetry` This project use based
 on `poetry`. You can install `poetry` by following the instructions on the
 poetry website https://python-poetry.org/. #### Install all packages with
 poetry For development including tools for generating documentation, use: ```
-poetry install -E docs ``` For installing only the packages required to run the
-tool, use: ``` poetry install --without dev ``` #### Installing pre-commit Run
-the following to enable python pre-commit: ``` poetry run pre-commit install
-``` You can run the pre-commit scripts manually: ``` poetry run pre-commit run
---all-files ``` ### Running the development tools There are basically three
-ways to run tools. You can use `tox`, run the commands directly on the command
-line or - if using Visual Studio Code - use some VS code preconfigured tasks.
-#### Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
+poetry install ``` For installing only the packages required to run the tool,
+use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
+following to enable python pre-commit: ``` poetry run pre-commit install ```
+You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
+all-files ``` ### Running the development tools There are basically three ways
+to run tools. You can use `tox`, run the commands directly on the command line
+or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
+Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
 `pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
 term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
 poetry run black --skip-string-normalization . ``` Alternatively, run formatter
 with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
 multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
 #### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
-Build the docs First, install the extra packages for building the docs: ```
-poetry install --extras docs ``` Build the docs in folder `docs`: ``` poetry
-run sphinx-build -b html docs/source/ docs/build/html ```
+Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
+b html docs/source/ docs/build/html ``` # Contributors See [Contributors]
+(CONTRIBUTORS.md) # License Copyright Eike Thaden, 2023. Distributed under the
+terms of the GPL v3 license, multidyndnscli is free and open source software.
```

