# Comparing `tmp/multidyndnscli-0.1.2.tar.gz` & `tmp/multidyndnscli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidyndnscli-0.1.2.tar", max compression
+gzip compressed data, was "multidyndnscli-0.1.3.tar", max compression
```

## Comparing `multidyndnscli-0.1.2.tar` & `multidyndnscli-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/LICENSE
--rw-r--r--   0        0        0     6702 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/README.md
--rw-r--r--   0        0        0    34104 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/cli.py
--rw-r--r--   0        0        0     6951 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/nc_dnsapi.py
--rw-r--r--   0        0        0     2771 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/schemata.py
--rw-r--r--   0        0        0     3844 2023-06-02 22:42:09.386575 multidyndnscli-0.1.2/multidyndnscli/util.py
--rw-r--r--   0        0        0     1254 2023-06-02 22:42:09.390575 multidyndnscli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7721 1970-01-01 00:00:00.000000 multidyndnscli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 12:23:05.988350 multidyndnscli-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6702 2023-06-03 12:23:05.988350 multidyndnscli-0.1.3/README.md
+-rw-r--r--   0        0        0    34180 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/__init__.py
+-rw-r--r--   0        0        0     2311 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/cli.py
+-rw-r--r--   0        0        0     6951 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/nc_dnsapi.py
+-rw-r--r--   0        0        0     2771 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/schemata.py
+-rw-r--r--   0        0        0     3844 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/multidyndnscli/util.py
+-rw-r--r--   0        0        0     1285 2023-06-03 12:23:05.992350 multidyndnscli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7773 1970-01-01 00:00:00.000000 multidyndnscli-0.1.3/PKG-INFO
```

### Comparing `multidyndnscli-0.1.2/LICENSE` & `multidyndnscli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.2/README.md` & `multidyndnscli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.2/multidyndnscli/__init__.py` & `multidyndnscli-0.1.3/multidyndnscli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 import fritzconnection.lib.fritzstatus  # type: ignore
 import fritzconnection.core.exceptions  # type: ignore
 # Module imports
 from . import util
 from .schemata import get_config_file_schema
 from .nc_dnsapi import Client, DNSRecord  # type: ignore
 
+from importlib_metadata import version
+
+__version__ = version(__package__)
+
 CACHE_FILE_NAME = 'multidyndns.cache'
 """The name used for the updater cache file if a (valid) cache dir has been configured"""
 KEY_DOMAINS: Final[str] = 'domains'
 """The key used to store domain statuses in the updater cache"""
 KEY_LAST_UPDATE: Final[str] = 'last_updated'
 """The key used to store the datetime of the last update into the updater cache"""
```

### Comparing `multidyndnscli-0.1.2/multidyndnscli/cli.py` & `multidyndnscli-0.1.3/multidyndnscli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
     :param args: list of command line arguments (i.e. args), defaults to None
     :type args: Optional[List[str]], optional
     :return: Returns 0 if update was successful, otherwise 1
     :rtype: int
     """
     if sys.version_info >= (3, 9):
-        parser = argparse.ArgumentParser(exit_on_error=False) # type: ignore  # pragma: no cover
+        parser = argparse.ArgumentParser(prog='multidyndnscli', exit_on_error=False) # type: ignore  # pragma: no cover
     else:
-        parser = argparse.ArgumentParser() # type: ignore  # pragma: no cover
+        parser = argparse.ArgumentParser(prog='multidyndnscli') # type: ignore  # pragma: no cover
     parser.add_argument("config_file")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--dry-run", "-n", action="store_true")
+    parser.add_argument('--version', action='version', version=f'%(prog)s {multidyndnscli.__version__}')
     try:
         parsed_args = parser.parse_args(args=args)
         config_file = parsed_args.config_file
         dry_run = parsed_args.dry_run
         log_format = "%(asctime)s - %(levelname)s: %(message)s"
         logging.basicConfig(format=log_format)
         if parsed_args.verbose >= 2:
```

### Comparing `multidyndnscli-0.1.2/multidyndnscli/nc_dnsapi.py` & `multidyndnscli-0.1.3/multidyndnscli/nc_dnsapi.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.2/multidyndnscli/schemata.py` & `multidyndnscli-0.1.3/multidyndnscli/schemata.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.2/multidyndnscli/util.py` & `multidyndnscli-0.1.3/multidyndnscli/util.py`

 * *Files identical despite different names*

### Comparing `multidyndnscli-0.1.2/pyproject.toml` & `multidyndnscli-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "multidyndnscli"
-version = "0.1.2"
+version = "0.1.3"
 description = "DynDNS Command-line Client"
 authors = ["Eike Thaden <eike.thaden@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://ethaden.github.io/multidyndnscli/"
 repository = "https://github.com/ethaden/multidyndnscli/"
 documentation = "https://ethaden.github.io/multidyndnscli/"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 dnspython = "^2.3.0"
 pyyaml = "^6.0"
 netaddr = "^0.8.0"
-netifaces = "^0.11.0"
 requests = "^2.28.2"
 fritzconnection = "^1.12.0"
 schema = "^0.7.5"
+netifaces2 = "^0.0.16"
+importlib-metadata = "^6.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 black = "^23.3.0"
 pytest-cov = "^4.0.0"
```

### Comparing `multidyndnscli-0.1.2/PKG-INFO` & `multidyndnscli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: multidyndnscli
-Version: 0.1.2
+Version: 0.1.3
 Summary: DynDNS Command-line Client
 Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later
 Author: Eike Thaden
 Author-email: eike.thaden@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
 Requires-Dist: fritzconnection (>=1.12.0,<2.0.0)
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: netaddr (>=0.8.0,<0.9.0)
-Requires-Dist: netifaces (>=0.11.0,<0.12.0)
+Requires-Dist: netifaces2 (>=0.0.16,<0.0.17)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Project-URL: Documentation, https://ethaden.github.io/multidyndnscli/
 Project-URL: Repository, https://github.com/ethaden/multidyndnscli/
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.2 Summary: DynDNS
+Metadata-Version: 2.1 Name: multidyndnscli Version: 0.1.3 Summary: DynDNS
 Command-line Client Home-page: https://ethaden.github.io/multidyndnscli/
 License: GPL-3.0-or-later Author: Eike Thaden Author-email:
 eike.thaden@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: dnspython
 (>=2.3.0,<3.0.0) Requires-Dist: fritzconnection (>=1.12.0,<2.0.0) Requires-
-Dist: netaddr (>=0.8.0,<0.9.0) Requires-Dist: netifaces (>=0.11.0,<0.12.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: schema (>=0.7.5,<0.8.0) Project-URL: Documentation, https://
-ethaden.github.io/multidyndnscli/ Project-URL: Repository, https://github.com/
-ethaden/multidyndnscli/ Description-Content-Type: text/markdown # DynDNS
-Command Line Tool
+Dist: importlib-metadata (>=6.6.0,<7.0.0) Requires-Dist: netaddr
+(>=0.8.0,<0.9.0) Requires-Dist: netifaces2 (>=0.0.16,<0.0.17) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
+schema (>=0.7.5,<0.8.0) Project-URL: Documentation, https://ethaden.github.io/
+multidyndnscli/ Project-URL: Repository, https://github.com/ethaden/
+multidyndnscli/ Description-Content-Type: text/markdown # DynDNS Command Line
+Tool
 [Test_Status] [Docs_Status] [License:_GPL_v3] [Pypi_Version] [Python_Versions]
 [Code_style:_black]
 ## Installation Install the package from Pypi (https://pypi.org/project/
 multidyndnscli) by running `pip install multidyndnscli`. It requires Python
 3.8+. ## Installation on OpenWRT First, install the required packages on
 OpenWRT: ```bash opkg install python3 python3-yaml python3-dns python3-netaddr
 python3-netifaces ``` Then install the Pypi packages as described above. ##
```

