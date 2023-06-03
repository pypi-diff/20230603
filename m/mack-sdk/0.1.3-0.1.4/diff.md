# Comparing `tmp/mack_sdk-0.1.3.tar.gz` & `tmp/mack_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mack_sdk-0.1.3.tar", max compression
+gzip compressed data, was "mack_sdk-0.1.4.tar", max compression
```

## Comparing `mack_sdk-0.1.3.tar` & `mack_sdk-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      820 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/__init__.py
--rw-r--r--   0        0        0     3163 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/client.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/resources/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/resources/models.py
--rw-r--r--   0        0        0     2600 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/resources/movie.py
--rw-r--r--   0        0        0     1726 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/resources/quote.py
--rw-r--r--   0        0        0        0 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/tools/__init__.py
--rw-r--r--   0        0        0      906 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/tools/raise_for_status.py
--rw-r--r--   0        0        0      961 2023-06-03 17:41:46.691692 mack_sdk-0.1.3/mack_SDK/tools/settings.py
--rw-r--r--   0        0        0     2281 2023-06-03 17:42:04.003657 mack_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 mack_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      702 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/__init__.py
+-rw-r--r--   0        0        0     3081 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/client.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/resources/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/resources/models.py
+-rw-r--r--   0        0        0     2619 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/resources/movie.py
+-rw-r--r--   0        0        0     1745 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/resources/quote.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/tools/__init__.py
+-rw-r--r--   0        0        0      906 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/tools/raise_for_status.py
+-rw-r--r--   0        0        0      941 2023-06-03 18:42:50.748282 mack_sdk-0.1.4/mack_SDK/tools/settings.py
+-rw-r--r--   0        0        0     2330 2023-06-03 18:43:08.960744 mack_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 mack_sdk-0.1.4/PKG-INFO
```

### Comparing `mack_sdk-0.1.3/mack_SDK/client.py` & `mack_sdk-0.1.4/mack_SDK/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 import httpx
-from resources.movie import Movie
-from resources.quote import Quote
-from tools.settings import Settings
+
+from mack_SDK.resources.movie import Movie
+from mack_SDK.resources.quote import Quote
+from mack_SDK.tools.settings import Settings
 
 
 class Client(object):
     """Create LOTR API Client.
 
     This class is used to create a client for the LOTR API.
     API docs - https://the-one-api.dev/documentation.
     `BEARER_TOKEN` is required for the API to work ([get token](https://the-one-api.dev/sign-up)),
     it may be passed as an argument or set as an environment variable.
+    Currently not supported: Filtering, Sorting, Pagination (needs to be implemented by the client
+    user).
 
     Examples:
-        Initialize a client:
         ```python
-        client = Client(bearer_token="foo")
-        ```
+        # Initialize a client
+        import mack_SDK.client
+        client = mack_SDK.client.Client(bearer_token="some_token")
 
-        Work with `/movies` resources:
-        ```python
+        # Work with `/movies` resources:
         movie_client = client.create_resource_class("movie")
         movies = movie_client.get_all_movies(page=2)
         movie = movie_client.get_movie("5cd95395de30eff6ebccde5b")
         quotes = movie_client.get_quotes("5cd95395de30eff6ebccde5b", limit=10)
-        ```
 
-        Work with `/quotes` resources:
-        ```python
+        # Work with `/quotes` resources:
         movie_client = client.create_resource_class("movie")
         quote_client = client.create_resource_class("quote")
         quotes = quote_client.get_all_quotes(limit=50, page=2)
         quote = quote_client.get_quote("5cd96e05de30eff6ebcce7ea")
-        ```
+    ```
     """
 
     http_client: httpx.Client
 
     def __init__(self, base_url: str = "https://the-one-api.dev/v2", bearer_token: str = None):
         """Create instance of the LOTR API client.
 
-        Method instantiates the `httpx.Client()` and sets:
-            * base_url
-            * headers (Content-Type, Authorization)
-            * SSL verification is on and can not be changed
-        Currently not supported:
-            * Filtering
-            * Sorting
-            * Pagination (needs to be implemented by the client user)
+        Method instantiates the `httpx.Client()` and sets: `base_url`,
+        `headers` (Content-Type, Authorization), SSL verification is on and can not be changed
 
         Args:
             base_url : Base URL for the `httpx.CLient()`
             bearer_token :  Bearer auth token. Get here -https://the-one-api.dev/sign-up
         """
         settings = Settings(BEARER_TOKEN=bearer_token)
 
@@ -62,20 +56,16 @@
             },
         )
         self.http_client = httpx.Client(base_url=base_url, headers=headers, verify=True)
 
     def create_resource_class(self, resource_name: str) -> object:
         """Create an API resource (endpoint) class.
 
-        Following endpoints are supported:
-        * `/movie`
-        * `/movie/{id}`
-        * `/movie/{id}/quote`
-        * `/quote`
-        * `/quote/{id}`
+        Following endpoints are supported: `/movie`, `/movie/{id}`, `/movie/{id}/quote`, `/quote`,
+        `/quote/{id}`
 
         Args:
             resource_name: Name of the resource (endpoint) class to create
 
         Returns:
             object: Resource class
```

### Comparing `mack_sdk-0.1.3/mack_SDK/resources/models.py` & `mack_sdk-0.1.4/mack_SDK/resources/models.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.3/mack_SDK/resources/movie.py` & `mack_sdk-0.1.4/mack_SDK/resources/movie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import httpx
-from resources import models
-from tools.raise_for_status import raise_for_status
+
+from mack_SDK.resources import models
+from mack_SDK.tools.raise_for_status import raise_for_status
 
 
 class Movie(object):
     """Movie resource class.
 
     This class is responsible for making requests to the /movie resource (endpoint)
     """
```

### Comparing `mack_sdk-0.1.3/mack_SDK/resources/quote.py` & `mack_sdk-0.1.4/mack_SDK/resources/quote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import httpx
-from resources import models
-from tools.raise_for_status import raise_for_status
+
+from mack_SDK.resources import models
+from mack_SDK.tools.raise_for_status import raise_for_status
 
 
 class Quote(object):
     """Quote resource class.
 
     This class is responsible for making requests to the /quote resource (endpoint)
     """
```

### Comparing `mack_sdk-0.1.3/mack_SDK/tools/raise_for_status.py` & `mack_sdk-0.1.4/mack_SDK/tools/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `mack_sdk-0.1.3/mack_SDK/tools/settings.py` & `mack_sdk-0.1.4/mack_SDK/tools/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
     """Settings for the LOTR API client."""
 
     BEARER_TOKEN: str
 
     class Config(BaseSettings.Config):
         """Settings configuration.
 
-        Main purpose is to change the order of the settings sources to (in order):
-        * Init value
-        * Environment variable
-        * Secret File (secret) (not tested)
+        Main purpose is to change the order of the settings sources to (in order): Init value,
+        Environment variable, Secret File (secret) (not tested)
 
         Please see base class for more information
         Docs - https://docs.pydantic.dev/latest/usage/settings/#customise-settings-sources
         """
 
         @classmethod
         def customise_sources(  # noqa: D102
```

### Comparing `mack_sdk-0.1.3/pyproject.toml` & `mack_sdk-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mack-SDK"
 version = "0.1.0"
 description = "LOTR SDK"
 requires-python = ">=3.11"
 
 [tool.poetry]
 name = "mack-SDK"
-version = "0.1.3"
+version = "0.1.4"
 description = "LOTR SDK"
 authors = ["Maksym Iv <maxim.ivaschenko@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "mack_SDK" }]
 
 [tool.poetry.dependencies]
 python = "~3.11"
@@ -33,22 +33,23 @@
 flake8-isort = "^6.0"
 flake8-bandit = "^4.1.1"
 wemake-python-styleguide = "^0.18.0"
 lazydocs = "^0.4.8"
 pydocstyle = "^6.3.0"
 
 [tool.pytest.ini_options]
-pythonpath = ["mack_SDK"]
+pythonpath = ["./"]
 
 [tool.flake8]
 max_line_length = 100
 inline-quotes = '"'
 max-line-complexity=20
 # https://wemake-python-styleguide.readthedocs.io/en/latest/pages/usage/violations/index.html
-ignore = ["WPS305", "WPS115", "I003", "D104", "ANN101", "ANN102", "ANN204", "D100"]
+# TODO: Fix RST2* errors
+ignore = ["WPS305", "WPS115", "I003", "D104", "ANN101", "ANN102", "ANN204", "D100", "RST203", "RST214", "RST215"]
 per-file-ignores = ["tests/*.py: S101 S105 S106 ANN001 ANN201 D100 D103 WPS111 WPS114 WPS226 WPS432"]
 
 
 [tool.black]
 exclude = '''
 /(
     \.git
```

### Comparing `mack_sdk-0.1.3/PKG-INFO` & `mack_sdk-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: mack-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: LOTR SDK
 Author: Maksym Iv
 Author-email: maxim.ivaschenko@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
 This is a Python SDK for the [The One API](https://the-one-api.dev/) (not fully implemented).
+
 API Overview is [here](./docs/README.md).
-Example usage may be found [here](./docs/client.md#class-client).
+
+Example usage may be found [here](./docs/client.md#Examples).
+
+**Rate limit retry is not implemented, you may get 429 errors**
 
 # Install
-TODO
+`pip install mack-sdk`
 
 # Development
 `pre-commit` hooks is heavily used for various linting and formatting tasks.
 We rely on [poetry](https://python-poetry.org/) for dependency management.
 `make` is used to spin-up local environment:
 * `make development` to install all dependencies
-* `make test` to run all tests
 * `make lint` to run linting
-
-# Acknowledgements
-* Docs are generated with [lazydocs](https://github.com/ml-tooling/lazydocs) and process needs to be improved.
-  [MkDocs](mkdocs.org) may be used to improve the documentation, [guide](https://realpython.com/python-project-documentation-with-mkdocs/)
+* `make test` to run all tests
+* `make test TESTS=tests/unit/client_test.py` to run tests from a file
```

