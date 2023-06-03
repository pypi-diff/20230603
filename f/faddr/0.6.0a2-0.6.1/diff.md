# Comparing `tmp/faddr-0.6.0a2.tar.gz` & `tmp/faddr-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faddr-0.6.0a2.tar", max compression
+gzip compressed data, was "faddr-0.6.1.tar", max compression
```

## Comparing `faddr-0.6.0a2.tar` & `faddr-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2021-10-22 00:59:56.250890 faddr-0.6.0a2/LICENSE
--rw-r--r--   0        0        0     1106 2022-03-20 09:43:28.125493 faddr-0.6.0a2/README.md
--rw-r--r--   0        0        0       92 2022-12-23 13:20:36.170000 faddr-0.6.0a2/faddr/__init__.py
--rw-r--r--   0        0        0     9956 2022-12-19 23:19:49.370000 faddr-0.6.0a2/faddr/database.py
--rw-r--r--   0        0        0     3381 2022-12-02 10:06:38.900000 faddr-0.6.0a2/faddr/exceptions.py
--rw-r--r--   0        0        0     5428 2022-12-02 10:06:38.900000 faddr-0.6.0a2/faddr/faddr.py
--rw-r--r--   0        0        0     5736 2022-12-19 23:19:49.340000 faddr-0.6.0a2/faddr/faddr_db.py
--rw-r--r--   0        0        0     3240 2022-12-19 23:19:49.310000 faddr-0.6.0a2/faddr/faddr_rest.py
--rw-r--r--   0        0        0      247 2022-12-02 10:06:38.900000 faddr-0.6.0a2/faddr/logging.py
--rw-r--r--   0        0        0     5225 2022-12-02 10:06:38.900000 faddr-0.6.0a2/faddr/models.py
--rw-r--r--   0        0        0     3116 2022-12-19 23:19:49.310000 faddr-0.6.0a2/faddr/parser.py
--rw-r--r--   0        0        0     7021 2022-12-23 12:28:05.810000 faddr-0.6.0a2/faddr/rancid.py
--rw-r--r--   0        0        0     3232 2022-12-19 23:19:14.470000 faddr-0.6.0a2/faddr/repo.py
--rw-r--r--   0        0        0     1336 2022-12-02 10:06:38.900000 faddr-0.6.0a2/faddr/results.py
--rw-r--r--   0        0        0     5509 2022-12-19 22:05:48.830000 faddr-0.6.0a2/faddr/schemas.py
--rw-r--r--   0        0        0     1460 2022-12-19 22:53:19.310000 faddr-0.6.0a2/faddr/settings.py
--rw-r--r--   0        0        0   996086 2022-05-14 16:03:26.396325 faddr-0.6.0a2/faddr/static/redoc.standalone.js
--rw-r--r--   0        0        0  1096221 2022-05-14 16:03:26.416325 faddr-0.6.0a2/faddr/static/swagger-ui-bundle.js
--rw-r--r--   0        0        0   143980 2022-05-14 16:03:26.416325 faddr-0.6.0a2/faddr/static/swagger-ui.css
--rw-r--r--   0        0        0     2897 2022-12-19 22:05:48.830000 faddr-0.6.0a2/faddr/templates/cisco-ios.ttp
--rw-r--r--   0        0        0     3194 2022-12-19 22:05:48.830000 faddr-0.6.0a2/faddr/templates/cisco-iosxr.ttp
--rw-r--r--   0        0        0     2838 2022-12-19 22:05:48.830000 faddr-0.6.0a2/faddr/templates/cisco-nxos.ttp
--rw-r--r--   0        0        0     2962 2022-12-19 22:05:48.840000 faddr-0.6.0a2/faddr/templates/huawei-vrp.ttp
--rw-r--r--   0        0        0     2844 2022-12-19 22:05:48.840000 faddr-0.6.0a2/faddr/templates/juniper-junos.ttp
--rw-r--r--   0        0        0     1446 2022-12-23 13:20:36.170000 faddr-0.6.0a2/pyproject.toml
--rw-r--r--   0        0        0     2304 1970-01-01 00:00:00.000000 faddr-0.6.0a2/setup.py
--rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 faddr-0.6.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-10-22 00:59:56.250890 faddr-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1106 2022-03-20 09:43:28.125493 faddr-0.6.1/README.md
+-rw-r--r--   0        0        0       90 2023-06-03 02:18:30.305757 faddr-0.6.1/faddr/__init__.py
+-rw-r--r--   0        0        0    10215 2023-01-14 17:04:23.980000 faddr-0.6.1/faddr/database.py
+-rw-r--r--   0        0        0     3381 2022-12-02 10:06:38.900000 faddr-0.6.1/faddr/exceptions.py
+-rw-r--r--   0        0        0     7385 2023-06-03 02:18:30.309090 faddr-0.6.1/faddr/faddr.py
+-rw-r--r--   0        0        0     5736 2023-01-14 17:04:23.940000 faddr-0.6.1/faddr/faddr_db.py
+-rw-r--r--   0        0        0     3240 2023-01-14 17:04:23.920000 faddr-0.6.1/faddr/faddr_rest.py
+-rw-r--r--   0        0        0      247 2022-12-02 10:06:38.900000 faddr-0.6.1/faddr/logging.py
+-rw-r--r--   0        0        0     5225 2022-12-02 10:06:38.900000 faddr-0.6.1/faddr/models.py
+-rw-r--r--   0        0        0     3116 2023-01-14 17:04:23.910000 faddr-0.6.1/faddr/parser.py
+-rw-r--r--   0        0        0     7021 2022-12-23 12:28:05.810000 faddr-0.6.1/faddr/rancid.py
+-rw-r--r--   0        0        0     3232 2022-12-19 23:19:14.470000 faddr-0.6.1/faddr/repo.py
+-rw-r--r--   0        0        0     1336 2022-12-02 10:06:38.900000 faddr-0.6.1/faddr/results.py
+-rw-r--r--   0        0        0     5509 2022-12-19 22:05:48.830000 faddr-0.6.1/faddr/schemas.py
+-rw-r--r--   0        0        0     1460 2022-12-19 22:53:19.310000 faddr-0.6.1/faddr/settings.py
+-rw-r--r--   0        0        0   996086 2022-05-14 16:03:26.396325 faddr-0.6.1/faddr/static/redoc.standalone.js
+-rw-r--r--   0        0        0  1096221 2022-05-14 16:03:26.416325 faddr-0.6.1/faddr/static/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   143980 2022-05-14 16:03:26.416325 faddr-0.6.1/faddr/static/swagger-ui.css
+-rw-r--r--   0        0        0     2897 2022-12-19 22:05:48.830000 faddr-0.6.1/faddr/templates/cisco-ios.ttp
+-rw-r--r--   0        0        0     3194 2022-12-19 22:05:48.830000 faddr-0.6.1/faddr/templates/cisco-iosxr.ttp
+-rw-r--r--   0        0        0     2838 2022-12-19 22:05:48.830000 faddr-0.6.1/faddr/templates/cisco-nxos.ttp
+-rw-r--r--   0        0        0     2962 2022-12-19 22:05:48.840000 faddr-0.6.1/faddr/templates/huawei-vrp.ttp
+-rw-r--r--   0        0        0     2844 2022-12-19 22:05:48.840000 faddr-0.6.1/faddr/templates/juniper-junos.ttp
+-rw-r--r--   0        0        0     1444 2023-06-03 02:18:30.312423 faddr-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 faddr-0.6.1/setup.py
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 faddr-0.6.1/PKG-INFO
```

### Comparing `faddr-0.6.0a2/LICENSE` & `faddr-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/README.md` & `faddr-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/database.py` & `faddr-0.6.1/faddr/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,39 +189,44 @@
 
         with Session(self.engine) as session:
             session.add(device)
             session.commit()
 
         logger.debug(f"Inserted device: '{device_data['name']}'")
 
-    def find_networks(self, queries, network_types=None):
+    def find_networks(self, queries, network_types=None, no_shutdown=False):
         """Find provided networks."""
 
         if network_types is None:
             network_types = ["direct"]
         for network_type in network_types:
             if network_type not in ("direct", "static"):
                 raise FaddrDatabaseUnknownQueryType(network_type)
 
         result = {}
 
         for query in queries:
-            result.update(self.find_network(query, network_types))
+            result.update(self.find_network(query, network_types, no_shutdown))
 
         return result
 
-    def find_network(self, query, network_types=None):
+    def find_network(self, query, network_types=None, no_shutdown=False):
         """Find provided network."""
 
         if network_types is None:
             network_types = ["direct"]
         for network_type in network_types:
             if network_type not in ("direct", "static"):
                 raise FaddrDatabaseUnknownQueryType(network_type)
 
+        if no_shutdown:
+            shutdown_status_query = (False,)
+        else:
+            shutdown_status_query = (True, False)
+
         if self.revision_id is None:
             self.get_active_revision()
 
         logger.debug(f"Using revision_id {self.revision_id}")
 
         netmask_max = 16
         netmask_min = 32
@@ -250,14 +255,15 @@
                         Interface.acl_out,
                         Interface.is_disabled,
                         Interface.description,
                     )
                     .where(
                         IPAddress.network.in_(networks),
                         Interface.id == IPAddress.interface_id,
+                        Interface.is_disabled.in_(shutdown_status_query),
                         Device.id == Interface.device_id,
                         Device.revision_id == self.revision_id,
                     )
                     .order_by(Device.name)
                     .order_by(Interface.name)
                     .order_by(IPAddress.with_prefixlen)
                 ),
```

### Comparing `faddr-0.6.0a2/faddr/exceptions.py` & `faddr-0.6.1/faddr/exceptions.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/faddr.py` & `faddr-0.6.1/faddr/faddr.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,52 +34,108 @@
         "-D",
         "--debug",
         action="store_true",
         help="Enable debug messages",
     )
     parser.add_argument(
         "-d",
-        "--description",
+        "--no-description",
         action="store_true",
-        help="Print description column",
+        help="Print without description column",
     )
-
     parser.add_argument(
         "-o",
         "--output",
         choices=("table", "json"),
         default="table",
         help="Output format, default is 'table'",
     )
     parser.add_argument(
+        "-s",
+        "--no-shutdown",
+        action="store_true",
+        help="Do not show interfaces in disabled state",
+    )
+    parser.add_argument(
         "-t",
         "--table",
         action="store_true",
         help="Print table borders",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="store_true",
         help="Print version and exit",
     )
+    parser.add_argument(
+        "-w",
+        "--wide",
+        action="store_true",
+        help="Print results in wide format: with separated in and out acls",
+    )
 
     args = parser.parse_args()
     return vars(args)
 
 
 def parse_input(input_data):
     """Remove masks from input ip addresses."""
     query = []
     for address in input_data:
         query.append(address.split("/")[0])
     return query
 
 
-def make_table(result, row_type, include_description=True, color=True, border=False):
+def combine_acls(data, data_type="row"):
+    """Combine `ACL in` and `ACL out` columns into single `ACL in/out` column."""
+
+    combined_data = []
+
+    if data_type == "header" and "ACL in" in data:
+        for key in data:
+            if key == "ACL in":
+                key = "ACL in/out"
+            elif key == "ACL out":
+                continue
+            combined_data.append(key)
+        return combined_data
+
+    elif data_type == "keys" and "acl_in" in data:
+        for key in data:
+            if key == "acl_in":
+                key = "acl_in_out"
+            elif key == "acl_out":
+                continue
+            combined_data.append(key)
+        return combined_data
+
+    elif data_type == "row" and "acl_in" in data:
+        acl_in = data.get("acl_in")
+        if acl_in is None:
+            acl_in = "-"
+        acl_out = data.get("acl_out", "-")
+        if acl_out is None:
+            acl_out = "-"
+
+        if acl_in == "-" and acl_out == "-":
+            acl_in_out = None
+        elif acl_out == "-":
+            acl_in_out = acl_in
+        else:
+            acl_in_out = acl_in + " / " + acl_out
+
+        data["acl_in_out"] = acl_in_out
+
+    return data
+
+
+def make_table(
+    result, row_type, exclude_description=False, color=True, border=False, wide=False
+):
     """Create rich table according to search results and cli arguments."""
 
     if border:
         table_border = box.SQUARE
         padding = (0, 1, 0, 1)
     else:
         table_border = None
@@ -95,33 +151,42 @@
     )
 
     keys = []
 
     # Prepare header according to passed cli options
     header = []
     header[:] = result.schema["headers"][row_type]
-    if not include_description and row_type == "direct":
+    if row_type == "direct" and exclude_description:
         header.remove("Description")
     if len(result.data.keys()) == 1:
         header.remove("Query")
+    if not wide:
+        header = combine_acls(header, data_type="header")
     for column in header:
         table.add_column(column)
 
     # Filter keys according to passed cli options
     keys[:] = result.schema["keys"][row_type]
-    if not include_description and row_type == "direct":
+    if row_type == "direct" and exclude_description:
         keys.remove("description")
     if len(result.data.keys()) == 1:
         keys.remove("query")
+    if not wide:
+        keys = combine_acls(keys, data_type="keys")
 
     return table, keys
 
 
 def print_result(
-    result, include_description=True, output_format="table", color=True, border=False
+    result,
+    exclude_description=False,
+    output_format="table",
+    color=True,
+    border=False,
+    wide=False,
 ):
     """Print result to console."""
 
     console = Console()
     if output_format == "json":
         console.print(json.dumps(result.data, indent=2))
     elif output_format == "table":
@@ -136,22 +201,26 @@
         for query in result.data.keys():
             for row_data in result.data[query]:
                 row_type = row_data["type"]
 
                 # Create rich table if it doesn't exist
                 if row_type not in tables:
                     tables[row_type], keys[row_type] = make_table(
-                        result, row_type, include_description, color, border
+                        result, row_type, exclude_description, color, border, wide
                     )
 
                 # Add rows to table
                 row_keys = keys[row_type]
                 if "query" in row_keys:
                     row_data["query"] = query
 
+                # Combine acl cells
+                if not wide:
+                    row_data = combine_acls(row_data, data_type="row")
+
                 # Normalize cell data
                 # cells = [str(row_data.get(key)) for key in row_keys]
                 cells = []
                 for key in row_keys:
                     value = row_data.get(key)
                     if value is None or value is False:
                         cells.append("-")
@@ -187,18 +256,21 @@
         print(__version__)
         sys.exit(0)
 
     database = Database(**settings.database.dict())
 
     result = NetworkResult(
         database.find_networks(
-            cmd_args.get("ip_address"), network_types=("direct", "static")
+            cmd_args.get("ip_address"),
+            network_types=("direct", "static"),
+            no_shutdown=cmd_args.get("no_shutdown"),
         )
     )
 
     print_result(
         result,
-        include_description=cmd_args.get("description"),
+        exclude_description=cmd_args.get("no_description"),
         output_format=cmd_args.get("output"),
         color=cmd_args.get("color"),
         border=cmd_args.get("table"),
+        wide=cmd_args.get("wide"),
     )
```

### Comparing `faddr-0.6.0a2/faddr/faddr_db.py` & `faddr-0.6.1/faddr/faddr_db.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/faddr_rest.py` & `faddr-0.6.1/faddr/faddr_rest.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/models.py` & `faddr-0.6.1/faddr/models.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/parser.py` & `faddr-0.6.1/faddr/parser.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/rancid.py` & `faddr-0.6.1/faddr/rancid.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/repo.py` & `faddr-0.6.1/faddr/repo.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/results.py` & `faddr-0.6.1/faddr/results.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/schemas.py` & `faddr-0.6.1/faddr/schemas.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/settings.py` & `faddr-0.6.1/faddr/settings.py`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/static/redoc.standalone.js` & `faddr-0.6.1/faddr/static/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/static/swagger-ui-bundle.js` & `faddr-0.6.1/faddr/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/static/swagger-ui.css` & `faddr-0.6.1/faddr/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/templates/cisco-ios.ttp` & `faddr-0.6.1/faddr/templates/cisco-ios.ttp`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/templates/cisco-iosxr.ttp` & `faddr-0.6.1/faddr/templates/cisco-iosxr.ttp`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/templates/cisco-nxos.ttp` & `faddr-0.6.1/faddr/templates/cisco-nxos.ttp`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/templates/huawei-vrp.ttp` & `faddr-0.6.1/faddr/templates/huawei-vrp.ttp`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/faddr/templates/juniper-junos.ttp` & `faddr-0.6.1/faddr/templates/juniper-junos.ttp`

 * *Files identical despite different names*

### Comparing `faddr-0.6.0a2/pyproject.toml` & `faddr-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "faddr"
-version = "0.6.0a2"
+version = "0.6.1"
 description = "Tool to parse configuration of network devices such as Juniper routers and store gathered data in database"
 license = "MIT"
 authors = ["Fedor Suchkov <f.suchkov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kido5217/faddr"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `faddr-0.6.0a2/setup.py` & `faddr-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 entry_points = \
 {'console_scripts': ['faddr = faddr.faddr:main',
                      'faddr-db = faddr.faddr_db:main',
                      'faddr-rest = faddr.faddr_rest:main']}
 
 setup_kwargs = {
     'name': 'faddr',
-    'version': '0.6.0a2',
+    'version': '0.6.1',
     'description': 'Tool to parse configuration of network devices such as Juniper routers and store gathered data in database',
     'long_description': '# FAddr\n\n[![CodeFactor](https://www.codefactor.io/repository/github/kido5217/faddr/badge)](https://www.codefactor.io/repository/github/kido5217/faddr)\n[![GitHub top language](https://img.shields.io/github/languages/top/kido5217/faddr)](https://www.python.org/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/faddr)](https://pypi.org/project/faddr/)\n[![GitHub](https://img.shields.io/github/license/kido5217/faddr)](https://opensource.org/licenses/MIT)\n\nFAddr is a Python program for parsing configuration of network devices such as Juniper and Cisco routers and storing gathered data in database.\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install faddr.\n\n```bash\npip install faddr\n```\n\n## Usage\n\nGenerate database:\n\n```bash\nfaddr-db\n```\n\nFind ip address termination point:\n\n```bash\nfaddr 10.20.30.1\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Fedor Suchkov',
     'author_email': 'f.suchkov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kido5217/faddr',
```

### Comparing `faddr-0.6.0a2/PKG-INFO` & `faddr-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faddr
-Version: 0.6.0a2
+Version: 0.6.1
 Summary: Tool to parse configuration of network devices such as Juniper routers and store gathered data in database
 Home-page: https://github.com/kido5217/faddr
 License: MIT
 Author: Fedor Suchkov
 Author-email: f.suchkov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

