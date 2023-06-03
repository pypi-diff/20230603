# Comparing `tmp/geobatchpy-0.2.2.tar.gz` & `tmp/geobatchpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geobatchpy-0.2.2.tar", max compression
+gzip compressed data, was "geobatchpy-0.2.3.tar", max compression
```

## Comparing `geobatchpy-0.2.2.tar` & `geobatchpy-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1092 2022-09-10 20:02:04.452721 geobatchpy-0.2.2/LICENSE
--rw-r--r--   0        0        0     6238 2022-11-13 19:43:07.722636 geobatchpy-0.2.2/README.md
--rw-r--r--   0        0        0       60 2022-11-13 19:56:06.684136 geobatchpy-0.2.2/geobatchpy/__init__.py
--rw-r--r--   0        0        0    19712 2022-11-13 19:53:16.094061 geobatchpy-0.2.2/geobatchpy/batch.py
--rw-r--r--   0        0        0     3210 2022-11-01 20:25:51.585878 geobatchpy-0.2.2/geobatchpy/boundaries.py
--rw-r--r--   0        0        0     4162 2022-10-24 09:46:11.831829 geobatchpy-0.2.2/geobatchpy/cli.py
--rw-r--r--   0        0        0     8118 2022-11-13 19:56:06.684442 geobatchpy-0.2.2/geobatchpy/client.py
--rw-r--r--   0        0        0     2582 2022-11-13 19:56:06.684711 geobatchpy-0.2.2/geobatchpy/utils.py
--rw-r--r--   0        0        0      903 2022-11-13 19:56:06.684977 geobatchpy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7277 2022-11-13 19:56:11.828678 geobatchpy-0.2.2/setup.py
--rw-r--r--   0        0        0     7003 2022-11-13 19:56:11.829186 geobatchpy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-09-10 20:02:04.452721 geobatchpy-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6238 2022-11-13 19:43:07.722636 geobatchpy-0.2.3/README.md
+-rw-r--r--   0        0        0       60 2022-11-13 19:56:06.684136 geobatchpy-0.2.3/geobatchpy/__init__.py
+-rw-r--r--   0        0        0    19712 2022-11-13 19:53:16.094061 geobatchpy-0.2.3/geobatchpy/batch.py
+-rw-r--r--   0        0        0     3210 2022-11-01 20:25:51.585878 geobatchpy-0.2.3/geobatchpy/boundaries.py
+-rw-r--r--   0        0        0     4162 2022-10-24 09:46:11.831829 geobatchpy-0.2.3/geobatchpy/cli.py
+-rw-r--r--   0        0        0     8118 2022-11-13 19:56:06.684442 geobatchpy-0.2.3/geobatchpy/client.py
+-rw-r--r--   0        0        0     2582 2022-11-13 19:56:06.684711 geobatchpy-0.2.3/geobatchpy/utils.py
+-rw-r--r--   0        0        0      903 2023-06-03 08:31:29.022455 geobatchpy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7277 2023-06-03 08:34:21.362686 geobatchpy-0.2.3/setup.py
+-rw-r--r--   0        0        0     7003 2023-06-03 08:34:21.363170 geobatchpy-0.2.3/PKG-INFO
```

### Comparing `geobatchpy-0.2.2/LICENSE` & `geobatchpy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/README.md` & `geobatchpy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/geobatchpy/batch.py` & `geobatchpy-0.2.3/geobatchpy/batch.py`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/geobatchpy/boundaries.py` & `geobatchpy-0.2.3/geobatchpy/boundaries.py`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/geobatchpy/cli.py` & `geobatchpy-0.2.3/geobatchpy/cli.py`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/geobatchpy/client.py` & `geobatchpy-0.2.3/geobatchpy/client.py`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/geobatchpy/utils.py` & `geobatchpy-0.2.3/geobatchpy/utils.py`

 * *Files identical despite different names*

### Comparing `geobatchpy-0.2.2/pyproject.toml` & `geobatchpy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geobatchpy"
-version = "0.2.2"
+version = "0.2.3"
 description = "A CLI and Python Client for the Geoapify API."
 authors = ["Paul Kinsvater <paul.kinsvater@gmail.com>", "Nikita Butsch <nikitabutsch@gmail.com>"]
 keywords = ["geoapify", "geocoding", "openstreetmap", "geojson"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/huels-originals/geobatchpy"
 repository = "https://github.com/huels-originals/geobatchpy"
```

### Comparing `geobatchpy-0.2.2/setup.py` & `geobatchpy-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['geobatch = geobatchpy.cli:main']}
 
 setup_kwargs = {
     'name': 'geobatchpy',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A CLI and Python Client for the Geoapify API.',
     'long_description': '# A CLI and Python Client for the Geoapify API\n\nWe have been using the Geoapify API to **geocode millions of location records** for data validation and analytics. We built\nthis package to make this process comfortable using Python and the command line.\n\nWhy Geoapify and this package may also be a good fit for you:\n\n- You need to batch process large numbers of location records (geocode, reverse geocode, places & details).\n- The license must support commercial use without restrictions.\n- It needs to be cheap (or even for free if you don\'t need more than 6k addresses per day).\n\nSign up at [geoapify.com](https://geoapify.com/) and start with their free plan of 3k credits per day which translates\nto up to 6k address geocodings.\n\n## Install our package with `pip`\n\nThis package is available on the public PyPI:\n\n```shell\npip install geobatchpy\n```\n\n## Examples\n\nSee our documentation at [geobatchpy.readthedocs.io](https://geobatchpy.readthedocs.io/en/latest/) for a growing number of\ncomprehensive example use cases. Below we illustrate both, the Python API and the CLI, for a tiny batch geocoding\nexample.\n\n### A simple batch geocoding example using the Python API\n\nBelow we geocode multiple addresses in a single batch. There are two ways how we can provide the location data as input.\nEither we use a list of strings, one string per address. These are then taken as free text searches. Or we provide\nstructured input as a list of dictionaries, again one per address. See the\n[Geoapify API documentation](https://apidocs.geoapify.com/) for a complete list of address attributes accepted by the\ngeocoding services. Use the optional `parameters` dictionary if all your addresses have an attribute in common. E.g.,\nbelow we request results in French.\n\n```python\nfrom geobatchpy import Client\n\nclient = Client(api_key=\'<your-api-key>\')\n\naddresses = [\'Hülser Markt 1, 47839 Krefeld\',\n             \'DB Schenker, Essen, Germany\',\n             \'JCI Beteiligungs GmbH, Am Schimmersfeld 5, Ratingen\']\n\n# see the geoapify.com API docs for more optional parameters\nres = client.batch.geocode(locations=addresses, parameters={\'lang\': \'fr\'}, simplify_output=True)\n```\n\nAlternatively you can provide a list of dictionaries, with every address in a structured form. And if you still need\nthe free text search for some, you can do this with the `\'text\'` attribute. Here is the same example, with the first\ntwo address translated to structured form:\n\n```python\naddresses = [{\'city\': \'Krefeld\', \'street\': \'Hülser Markt\', \'housenumber\': 1, \'postcode\': \'47839\'},\n             {\'name\': \'DB Schenker\', \'city\': \'Essen\', \'country\': \'Germany\'},\n             {\'text\': \'JCI Beteiligungs GmbH, Am Schimmersfeld 5, Ratingen\'}]\n```\n\n```python\n# Showing the first of three result sets: res[0]\n{\n    "query": {\n        "text": "Hülser Markt 1, 47839 Krefeld",\n        "parsed": {\n            "housenumber": "1",\n            "street": "hülser markt",\n            "postcode": "47839",\n            "city": "krefeld",\n            "expected_type": "building",\n        },\n    },\n    "datasource": {\n        "sourcename": "openstreetmap",\n        "attribution": "© OpenStreetMap contributors",\n        "license": "Open Database License",\n        "url": "https://www.openstreetmap.org/copyright",\n    },\n    "name": "Metzgerei Etteldorf",\n    "housenumber": "1",\n    "street": "Hülser Markt",\n    "suburb": "Hüls",\n    "city": "Krefeld",\n    "state": "Rhénanie-du-Nord-Westphalie",\n    "postcode": "47839",\n    "country": "Allemagne",\n    "country_code": "de",\n    "lon": 6.510696417033254,\n    "lat": 51.373026800000005,\n    "formatted": "Metzgerei Etteldorf, Hülser Markt 1, 47839 Krefeld, Allemagne",\n    "address_line1": "Metzgerei Etteldorf",\n    "address_line2": "Hülser Markt 1, 47839 Krefeld, Allemagne",\n    "category": "commercial.food_and_drink.butcher",\n    "result_type": "amenity",\n    "rank": {\n        "importance": 0.31100000000000005,\n        "popularity": 5.585340759145855,\n        "confidence": 1,\n        "confidence_city_level": 1,\n        "confidence_street_level": 1,\n        "match_type": "inner_part",\n    },\n    "place_id": "516b5e6500f40a1a40590a449957bfaf4940f00102f9010ecff70d00000000c002019203134d65747a676572656920457474656c646f7266",\n}\n```\n\n### The same batch geocoding example using the CLI\n\nWe built the `geoapify` command line interface to make batch processing large numbers of records more comfortable.\n\nSteps:\n1. Prepare a JSON file as input.\n2. Use `geoapify post-batch-jobs` to submit one or more jobs to the Geoapify servers.\n3. Use `geoapify monitor-batch-jobs` for monitoring progress and data retrieval.\n\n```python\n# Step 1 - written in Python:\nfrom geobatchpy.batch import parse_geocoding_inputs\nfrom geobatchpy.utils import write_data_to_json_file\n\naddresses = [\'Hülser Markt 1, 47839 Krefeld\',\n             \'DB Schenker, Essen, Germany\',\n             \'JCI Beteiligungs GmbH, Am Schimmersfeld 5, Ratingen\']\n\ndata = {\n    \'api\': \'/v1/geocode/search\',  # see the Geoapify API docs for other APIs that work with batch processing\n    \'inputs\': parse_geocoding_inputs(locations=addresses),\n    \'batch_len\': 2,  # optional - will put first two addresses in batch 1, last address in batch 2\n    \'id\': \'my-batch-geocoding-job\'  # optional - a reference which will be reused in the output file\n}\n\nwrite_data_to_json_file(data=data, file_path=\'<path-data-in>\')\n```\n\nThe following command submits one or more jobs and stores job URLs to disk. Those URLs are required to monitor\nand retrieve results.\n\n```shell\ngeobatch submit <path-data-in> <path-post-data-out> --api-key <your-key>\n```\n\nYou can omit the `--api-key` option if you set the `GEOAPIFY_KEY` environment variable. Next we start monitoring\nprogress:\n\n```shell\ngeobatch receive <path-post-data-out> <path-results-data-out> --api-key <your-key>\n```\n\nWe can abort the monitoring at any time and restart later - provided the jobs still are in the cache of\nGeoapify servers (24 hours).\n\n## References and further reading\n\n- [geoapify.com API documentation](https://apidocs.geoapify.com/)\n- [Towards Data Science - Deduplicate and clean-up millions of location records](https://towardsdatascience.com/deduplicate-and-clean-up-millions-of-location-records-abcffb308ebf)\n',
     'author': 'Paul Kinsvater',
     'author_email': 'paul.kinsvater@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/huels-originals/geobatchpy',
```

### Comparing `geobatchpy-0.2.2/PKG-INFO` & `geobatchpy-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geobatchpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI and Python Client for the Geoapify API.
 Home-page: https://github.com/huels-originals/geobatchpy
 License: MIT
 Keywords: geoapify,geocoding,openstreetmap,geojson
 Author: Paul Kinsvater
 Author-email: paul.kinsvater@gmail.com
 Requires-Python: >=3.7.1,<4.0
```

