# Comparing `tmp/multidyndnscli-0.1.5.tar.gz` & `tmp/multidyndnscli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.5.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.6.tar", max compression
```

## Comparing `multidyndnscli-0.1.5.tar` & `multidyndnscli-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/LICENSE
--rw-r--r--   0        0        0     6930 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/README.md
--rw-r--r--   0        0        0    34179 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     2331 2023-06-03 15:11:28.096271 multidyndnscli-0.1.5/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6907 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2771 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3844 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/multidyndnscli/util.py
--rw-r--r--   0        0        0     1287 2023-06-03 15:11:28.100271 multidyndnscli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 multidyndnscli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 16:23:39.266312 multidyndnscli-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7362 2023-06-03 16:23:39.266312 multidyndnscli-0.1.6/README.md
+-rw-r--r--   0        0        0    34179 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2331 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6907 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2771 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1287 2023-06-03 16:23:39.270312 multidyndnscli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 multidyndnscli-0.1.6/PKG-INFO
```

### Comparing `multidyndnscli-0.1.5/LICENSE` & `multidyndnscli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/README.md` & `multidyndnscli-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -74,15 +74,26 @@
 
 You can find a complete example configuration file [here](config.example.yaml).
 
 For further information, have a look at the documentation: https://ethaden.github.io/multidyndnscli/.
 
 ### Running multidyndnscli
 
-Once the Python package is installed, run it by executing `multidyndnscli <your-config-file>`.
+This project generates a command line script `multidyndnscli` in either your virtual env's `bin` folder, 
+in the well-known locations in the user's home directory (e.g. ``$HOME/.local/bin``) or in a system-wide bin folder (e.g. `/usr/local/bin`).
+Make sure the respective path is in your `$PATH`.
+
+Once the Python package is installed, run it by executing 
+
+```bash
+multidyndnscli <your-config-file>
+```
+
+Use a cronjob or systemd to run the tool periodically.
+It is highly recommended not to run the tool with root privileges.
 
 ## Development
 
 ### Using a dev container
 If using Visual Studio Code, you'll can make use of a working dev container setup specified in `.devcontainer` which should be found automatically. Make sure to adapt the WAN interface used for testing - if any - to the one configure within the running container.
 
 ### Local development `pyenv`
```

#### html2text {}

```diff
@@ -36,42 +36,47 @@
 the last update for the domain has been done less tehn `delay` seconds ago, the
 current update will be skipped. This is particularly useful for DNSSEC-enabled
 domains, where the domain has to be resigned after any updates. Resigning may
 take quite a while and no further updates should be done until the updated
 values have become visible. You can find a complete example configuration file
 [here](config.example.yaml). For further information, have a look at the
 documentation: https://ethaden.github.io/multidyndnscli/. ### Running
-multidyndnscli Once the Python package is installed, run it by executing
-`multidyndnscli `. ## Development ### Using a dev container If using Visual
-Studio Code, you'll can make use of a working dev container setup specified in
-`.devcontainer` which should be found automatically. Make sure to adapt the WAN
-interface used for testing - if any - to the one configure within the running
-container. ### Local development `pyenv` This project can use `pyenv`, though
-using it is not mandatory. You can install `pyenv` by following the
-instructions on the pyenv website https://github.com/pyenv/pyenv. List
-installable versions ``` pyenv install -l ``` Initialize the required/desired
-python environments: ``` pyenv install 3.8 pyenv install 3.9 pyenv install 3.10
-pyenv install 3.11 ``` Show installed version: ``` pyenv versions ``` ####
-Installing `poetry` This project use based on `poetry`. You can install
-`poetry` by following the instructions on the poetry website https://python-
-poetry.org/. #### Install all packages with poetry For development including
-tools for generating documentation, use: ``` poetry install ``` For installing
-only the packages required to run the tool, use: ``` poetry install --without
-dev ``` #### Installing pre-commit Run the following to enable python pre-
-commit: ``` poetry run pre-commit install ``` You can run the pre-commit
-scripts manually: ``` poetry run pre-commit run --all-files ``` ### Running the
-development tools There are basically three ways to run tools. You can use
-`tox`, run the commands directly on the command line or - if using Visual
-Studio Code - use some VS code preconfigured tasks. #### Running tests You can
-use `tox`: ``` tox ``` Alternatively, you can run `pytest` manually: ``` poetry
-run pytest --cov-report xml:cov.xml --cov-report term-missing --
-cov=multidyndnscli tests/ ``` #### Running code formatter ``` poetry run black
---skip-string-normalization . ``` Alternatively, run formatter with tox: ```
-tox -e format ``` #### Run linter ``` poetry run pylint multidyndnscli ```
-Alternatively, run linter with tox: ``` tox -e linter ``` #### Running code
-analysis with mypy ``` poetry run mypy multidyndnscli ``` ### Build the docs
-Build the docs in folder `docs`: ``` poetry run sphinx-build -b html docs/
-source/ docs/build/html ``` ### Increase the version Update the version in
-`pyproject.tom`. The tool will report this version after the release. #
-Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright Eike
-Thaden, 2023. Distributed under the terms of the GPL v3 license, multidyndnscli
-is free and open source software.
+multidyndnscli This project generates a command line script `multidyndnscli` in
+either your virtual env's `bin` folder, in the well-known locations in the
+user's home directory (e.g. ``$HOME/.local/bin``) or in a system-wide bin
+folder (e.g. `/usr/local/bin`). Make sure the respective path is in your
+`$PATH`. Once the Python package is installed, run it by executing ```bash
+multidyndnscli  ``` Use a cronjob or systemd to run the tool periodically. It
+is highly recommended not to run the tool with root privileges. ## Development
+### Using a dev container If using Visual Studio Code, you'll can make use of a
+working dev container setup specified in `.devcontainer` which should be found
+automatically. Make sure to adapt the WAN interface used for testing - if any -
+to the one configure within the running container. ### Local development
+`pyenv` This project can use `pyenv`, though using it is not mandatory. You can
+install `pyenv` by following the instructions on the pyenv website https://
+github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
+Initialize the required/desired python environments: ``` pyenv install 3.8
+pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
+version: ``` pyenv versions ``` #### Installing `poetry` This project use based
+on `poetry`. You can install `poetry` by following the instructions on the
+poetry website https://python-poetry.org/. #### Install all packages with
+poetry For development including tools for generating documentation, use: ```
+poetry install ``` For installing only the packages required to run the tool,
+use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
+following to enable python pre-commit: ``` poetry run pre-commit install ```
+You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
+all-files ``` ### Running the development tools There are basically three ways
+to run tools. You can use `tox`, run the commands directly on the command line
+or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
+Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
+`pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
+term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
+poetry run black --skip-string-normalization . ``` Alternatively, run formatter
+with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
+multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
+#### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
+Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
+b html docs/source/ docs/build/html ``` ### Increase the version Update the
+version in `pyproject.tom`. The tool will report this version after the
+release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
+Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
+multidyndnscli is free and open source software.
```

### Comparing `multidyndnscli-0.1.5/multidyndnscli/__init__.py` & `multidyndnscli-0.1.6/multidyndnscli/__init__.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/multidyndnscli/cli.py` & `multidyndnscli-0.1.6/multidyndnscli/cli.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.6/multidyndnscli/nc_dnsapi.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/multidyndnscli/schemata.py` & `multidyndnscli-0.1.6/multidyndnscli/schemata.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/multidyndnscli/util.py` & `multidyndnscli-0.1.6/multidyndnscli/util.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.5/pyproject.toml` & `multidyndnscli-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.5"
+version = "0.1.6"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
```

### Comparing `multidyndnscli-0.1.5/PKG-INFO` & `multidyndnscli-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.5
+Version: 0.1.6
 Summary: DynDNS Command-line Client
 Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -100,15 +100,26 @@
 
 You can find a complete example configuration file [here](config.example.yaml).
 
 For further information, have a look at the documentation: https://ethaden.github.io/multidyndnscli/.
 
 ### Running multidyndnscli
 
-Once the Python package is installed, run it by executing `multidyndnscli <your-config-file>`.
+This project generates a command line script `multidyndnscli` in either your virtual env's `bin` folder, 
+in the well-known locations in the user's home directory (e.g. ``$HOME/.local/bin``) or in a system-wide bin folder (e.g. `/usr/local/bin`).
+Make sure the respective path is in your `$PATH`.
+
+Once the Python package is installed, run it by executing 
+
+```bash
+multidyndnscli <your-config-file>
+```
+
+Use a cronjob or systemd to run the tool periodically.
+It is highly recommended not to run the tool with root privileges.
 
 ## Development
 
 ### Using a dev container
 If using Visual Studio Code, you'll can make use of a working dev container setup specified in `.devcontainer` which should be found automatically. Make sure to adapt the WAN interface used for testing - if any - to the one configure within the running container.
 
 ### Local development `pyenv`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.5 Summary: DynDNS
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.6 Summary: DynDNS
 Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later Author: Eike Thaden Author-email:
 eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: dnspython
@@ -51,42 +51,47 @@
 the last update for the domain has been done less tehn `delay` seconds ago, the
 current update will be skipped. This is particularly useful for DNSSEC-enabled
 domains, where the domain has to be resigned after any updates. Resigning may
 take quite a while and no further updates should be done until the updated
 values have become visible. You can find a complete example configuration file
 [here](config.example.yaml). For further information, have a look at the
 documentation: https://ethaden.github.io/multidyndnscli/. ### Running
-multidyndnscli Once the Python package is installed, run it by executing
-`multidyndnscli `. ## Development ### Using a dev container If using Visual
-Studio Code, you'll can make use of a working dev container setup specified in
-`.devcontainer` which should be found automatically. Make sure to adapt the WAN
-interface used for testing - if any - to the one configure within the running
-container. ### Local development `pyenv` This project can use `pyenv`, though
-using it is not mandatory. You can install `pyenv` by following the
-instructions on the pyenv website https://github.com/pyenv/pyenv. List
-installable versions ``` pyenv install -l ``` Initialize the required/desired
-python environments: ``` pyenv install 3.8 pyenv install 3.9 pyenv install 3.10
-pyenv install 3.11 ``` Show installed version: ``` pyenv versions ``` ####
-Installing `poetry` This project use based on `poetry`. You can install
-`poetry` by following the instructions on the poetry website https://python-
-poetry.org/. #### Install all packages with poetry For development including
-tools for generating documentation, use: ``` poetry install ``` For installing
-only the packages required to run the tool, use: ``` poetry install --without
-dev ``` #### Installing pre-commit Run the following to enable python pre-
-commit: ``` poetry run pre-commit install ``` You can run the pre-commit
-scripts manually: ``` poetry run pre-commit run --all-files ``` ### Running the
-development tools There are basically three ways to run tools. You can use
-`tox`, run the commands directly on the command line or - if using Visual
-Studio Code - use some VS code preconfigured tasks. #### Running tests You can
-use `tox`: ``` tox ``` Alternatively, you can run `pytest` manually: ``` poetry
-run pytest --cov-report xml:cov.xml --cov-report term-missing --
-cov=multidyndnscli tests/ ``` #### Running code formatter ``` poetry run black
---skip-string-normalization . ``` Alternatively, run formatter with tox: ```
-tox -e format ``` #### Run linter ``` poetry run pylint multidyndnscli ```
-Alternatively, run linter with tox: ``` tox -e linter ``` #### Running code
-analysis with mypy ``` poetry run mypy multidyndnscli ``` ### Build the docs
-Build the docs in folder `docs`: ``` poetry run sphinx-build -b html docs/
-source/ docs/build/html ``` ### Increase the version Update the version in
-`pyproject.tom`. The tool will report this version after the release. #
-Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright Eike
-Thaden, 2023. Distributed under the terms of the GPL v3 license, multidyndnscli
-is free and open source software.
+multidyndnscli This project generates a command line script `multidyndnscli` in
+either your virtual env's `bin` folder, in the well-known locations in the
+user's home directory (e.g. ``$HOME/.local/bin``) or in a system-wide bin
+folder (e.g. `/usr/local/bin`). Make sure the respective path is in your
+`$PATH`. Once the Python package is installed, run it by executing ```bash
+multidyndnscli  ``` Use a cronjob or systemd to run the tool periodically. It
+is highly recommended not to run the tool with root privileges. ## Development
+### Using a dev container If using Visual Studio Code, you'll can make use of a
+working dev container setup specified in `.devcontainer` which should be found
+automatically. Make sure to adapt the WAN interface used for testing - if any -
+to the one configure within the running container. ### Local development
+`pyenv` This project can use `pyenv`, though using it is not mandatory. You can
+install `pyenv` by following the instructions on the pyenv website https://
+github.com/pyenv/pyenv. List installable versions ``` pyenv install -l ```
+Initialize the required/desired python environments: ``` pyenv install 3.8
+pyenv install 3.9 pyenv install 3.10 pyenv install 3.11 ``` Show installed
+version: ``` pyenv versions ``` #### Installing `poetry` This project use based
+on `poetry`. You can install `poetry` by following the instructions on the
+poetry website https://python-poetry.org/. #### Install all packages with
+poetry For development including tools for generating documentation, use: ```
+poetry install ``` For installing only the packages required to run the tool,
+use: ``` poetry install --without dev ``` #### Installing pre-commit Run the
+following to enable python pre-commit: ``` poetry run pre-commit install ```
+You can run the pre-commit scripts manually: ``` poetry run pre-commit run --
+all-files ``` ### Running the development tools There are basically three ways
+to run tools. You can use `tox`, run the commands directly on the command line
+or - if using Visual Studio Code - use some VS code preconfigured tasks. ####
+Running tests You can use `tox`: ``` tox ``` Alternatively, you can run
+`pytest` manually: ``` poetry run pytest --cov-report xml:cov.xml --cov-report
+term-missing --cov=multidyndnscli tests/ ``` #### Running code formatter ```
+poetry run black --skip-string-normalization . ``` Alternatively, run formatter
+with tox: ``` tox -e format ``` #### Run linter ``` poetry run pylint
+multidyndnscli ``` Alternatively, run linter with tox: ``` tox -e linter ```
+#### Running code analysis with mypy ``` poetry run mypy multidyndnscli ``` ###
+Build the docs Build the docs in folder `docs`: ``` poetry run sphinx-build -
+b html docs/source/ docs/build/html ``` ### Increase the version Update the
+version in `pyproject.tom`. The tool will report this version after the
+release. # Contributors See [Contributors](CONTRIBUTORS.md) # License Copyright
+Eike Thaden, 2023. Distributed under the terms of the GPL v3 license,
+multidyndnscli is free and open source software.
```

