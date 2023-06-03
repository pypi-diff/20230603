# Comparing `tmp/bqemulatormanager-0.1.8.tar.gz` & `tmp/bqemulatormanager-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqemulatormanager-0.1.8.tar", max compression
+gzip compressed data, was "bqemulatormanager-0.1.9.tar", max compression
```

## Comparing `bqemulatormanager-0.1.8.tar` & `bqemulatormanager-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1217 2022-10-26 02:36:44.755121 bqemulatormanager-0.1.8/README.md
--rw-r--r--   0        0        0      144 2022-10-24 05:40:24.974381 bqemulatormanager-0.1.8/bqemulatormanager/__init__.py
--rw-r--r--   0        0        0      927 2022-10-28 02:59:13.500747 bqemulatormanager-0.1.8/bqemulatormanager/emulator.py
--rw-r--r--   0        0        0     2877 2022-10-27 08:07:55.623906 bqemulatormanager-0.1.8/bqemulatormanager/manager.py
--rw-r--r--   0        0        0     1884 2022-10-26 06:19:58.626701 bqemulatormanager-0.1.8/bqemulatormanager/schema.py
--rw-r--r--   0        0        0      538 2022-10-28 03:01:30.909946 bqemulatormanager-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 bqemulatormanager-0.1.8/setup.py
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 bqemulatormanager-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1321 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/README.md
+-rw-r--r--   0        0        0      145 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/__init__.py
+-rw-r--r--   0        0        0      915 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/emulator.py
+-rw-r--r--   0        0        0     3000 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/manager.py
+-rw-r--r--   0        0        0     1883 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/schema.py
+-rw-r--r--   0        0        0     1176 2023-06-01 08:47:11.107981 bqemulatormanager-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 bqemulatormanager-0.1.9/PKG-INFO
```

### Comparing `bqemulatormanager-0.1.8/README.md` & `bqemulatormanager-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,11 +33,13 @@
 
     sql = 'SELECT id, name FROM `dataset1.table_a`'
 
     df = manager.query(sql)
 print(df)
 ```
 
+unit test example is [here](https://github.com/gyuta/bqemulatormanager/blob/main/examples/testing.py).
+
 ### automatically detect schema
 When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `master_schema.yaml`).
 
 If schema definition canot be found, `SchemaManager` request it from BigQuery in production environmant and update master schema file.
```

### Comparing `bqemulatormanager-0.1.8/bqemulatormanager/manager.py` & `bqemulatormanager-0.1.9/bqemulatormanager/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from typing import List
+from typing import Dict, List
 
 import pandas as pd
 from google.api_core.client_options import ClientOptions
 from google.auth.credentials import AnonymousCredentials
 from google.cloud import bigquery
 
 from bqemulatormanager.emulator import Emulator, PortOccupiedError
 from bqemulatormanager.schema import SchemaManager
 
 
 class Manager:
-
-    def __init__(self, project: str = 'test', port: int = 9050, schema_path: str = 'master_schema.yaml',
-    launch_emulator:bool=True, debug_mode:bool=False, max_pool:int=20):
-
+    def __init__(
+        self,
+        project: str = "test",
+        port: int = 9050,
+        schema_path: str = "master_schema.yaml",
+        launch_emulator: bool = True,
+        debug_mode: bool = False,
+        max_pool: int = 20,
+    ):
         original_port = port
         for i in range(max_pool):
             port = original_port + i
             try:
                 self.emulator = Emulator(project, port, launch_emulator=launch_emulator, debug_mode=debug_mode)
             except PortOccupiedError as e:
                 print(e)
             else:
                 break
         else:
-            raise RuntimeError(f'there is no empty port from {original_port} to {port}')
+            raise RuntimeError(f"there is no empty port from {original_port} to {port}")
 
         self.client = self._make_client(project, port)
 
         prod_client = bigquery.Client(project)
 
         self.schema_manager = SchemaManager(client=prod_client, master_path=schema_path)
-        self.structure = {}
+        self.structure: Dict[str, Dict[str, bool]] = {}
         self.project_name = project
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_value, traceback):
         del self.emulator
@@ -48,32 +53,32 @@
             project_name,
             client_options=client_options,
             credentials=AnonymousCredentials(),
         )
         return client
 
     def load(self, data, path):
-        dataset, table = path.split('.')
+        dataset, table = path.split(".")
         if dataset not in self.structure:
             self.create_dataset(dataset)
 
         if table not in self.structure[dataset]:
             self.create_table(dataset, table, [])
 
-        table = self.client.get_table(f'{self.project_name}.{path}')
+        table = self.client.get_table(f"{self.project_name}.{path}")
         self.client.insert_rows_from_dataframe(table, data)
 
     def create_dataset(self, dataset_name: str, exists_ok=True):
-        dataset = bigquery.Dataset(f'{self.project_name}.{dataset_name}')
-        self.client.create_dataset(dataset)
+        dataset = bigquery.Dataset(f"{self.project_name}.{dataset_name}")
+        self.client.create_dataset(dataset, exists_ok=exists_ok)
         self.structure[dataset_name] = {}
 
     def create_table(self, dataset_name: str, table_name: str, schema: List[bigquery.SchemaField]):
         if schema == []:
-            schema = self.schema_manager.get_schema(f'{self.project_name}.{dataset_name}.{table_name}')
+            schema = self.schema_manager.get_schema(f"{self.project_name}.{dataset_name}.{table_name}")
 
-        table = bigquery.Table(f'{self.project_name}.{dataset_name}.{table_name}', schema=schema)
+        table = bigquery.Table(f"{self.project_name}.{dataset_name}.{table_name}", schema=schema)
         self.client.create_table(table)
-        self.structure[dataset_name][table_name] = {}
+        self.structure[dataset_name][table_name] = True
 
     def query(self, sql: str) -> pd.DataFrame:
         return self.client.query(sql).to_dataframe(create_bqstorage_client=False)
```

### Comparing `bqemulatormanager-0.1.8/bqemulatormanager/schema.py` & `bqemulatormanager-0.1.9/bqemulatormanager/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,52 +2,51 @@
 from typing import List
 
 import yaml
 from google.cloud import bigquery
 
 
 class SchemaManager:
-
-    def __init__(self, master_path: str = 'master_schema.yaml', client=None):
+    def __init__(self, master_path: str = "master_schema.yaml", client=None):
         self.client = client
         self.master_path = master_path
         self.change_flg = False
         if os.path.isfile(master_path):
             with open(master_path) as f:
                 master_schema = yaml.safe_load(f)
         else:
             master_schema = {}
         self.master_schema = master_schema
 
     def get_schema(self, table_id: str) -> List[bigquery.SchemaField]:
-        project, dataset, table = table_id.split('.')
+        project, dataset, table = table_id.split(".")
 
         schema = self.master_schema.get(project, {}).get(dataset, {}).get(table, {})
 
         if schema == {}:
             schema = self._get_schema_from_production(table_id)
             deepupdate(self.master_schema, {project: {dataset: {table: [s._properties for s in schema]}}})
             self.change_flg = True
             return schema
         else:
             return [bigquery.SchemaField.from_api_repr(s) for s in schema]
 
     def _get_schema_from_production(self, table_id: str) -> List[bigquery.SchemaField]:
         if not self.client:
-            raise Exception('set client')
+            raise Exception("set client")
         table = self.client.get_table(table_id)
         return table.schema
 
     def save(self):
         if self.change_flg:
-            with open(self.master_path, 'w') as f:
+            with open(self.master_path, "w") as f:
                 head_msg = '# This code is generated from BigQuery table metadata by "bqemulatormanager"; DO NOT EDIT.\n'
                 f.write(head_msg)
 
-                yaml.dump(self.master_schema, f, encoding='utf8', allow_unicode=True)
+                yaml.dump(self.master_schema, f, encoding="utf8", allow_unicode=True)
 
     def __del__(self):
         self.save()
 
 
 def deepupdate(dict_base, other):
     for k, v in other.items():
```

### Comparing `bqemulatormanager-0.1.8/setup.py` & `bqemulatormanager-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,64 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bqemulatormanager
+Version: 0.1.9
+Summary: bqemulatormanager is a wrapper of bigquery-emulator which provides us BigQuery mock working in local machine.
+Author: gyuta
+Author-email: kuroshiba0408@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: db-dtypes (>=1.0.0,<2.0.0)
+Requires-Dist: google-auth (>=2.17.2,<3.0.0)
+Requires-Dist: google-cloud-bigquery (>=3.0.0,<4.0.0)
+Requires-Dist: psutil (>=5.0.0,<6.0.0)
+Requires-Dist: pyyaml
+Description-Content-Type: text/markdown
+
+# BiqQueryEmulator Manager
+
+
+this package is wrapper of [bigquery-emulator](https://github.com/goccy/bigquery-emulator) which provides us BigQuery mock working in local machine.
+
+using this package, you can
+
+- do unit test of your sql
+- download the schema of big query, and use it to make test data
+
+## usage
+1. following [instruction](https://github.com/goccy/bigquery-emulator#install),  download `bigquery-emulator` command.
+
+2. install this package. 
+```
+pip install bqemulatormanager
+```
+
+3. test your sql.
+```python
+import bqemulatormanager as bqem
+import pandas as pd
+
+manager = bqem.Manager(project='test', schema_path='resources/schema_example.yaml')
+
+with manager:
+    data = pd.DataFrame([
+        {'id': 1, 'name': 'sato'},
+        {'id': 2, 'name': 'yamada'}
+    ])
+
+    manager.load(data, 'dataset1.table_a')
+
+    sql = 'SELECT id, name FROM `dataset1.table_a`'
+
+    df = manager.query(sql)
+print(df)
+```
 
-packages = \
-['bqemulatormanager']
+unit test example is [here](https://github.com/gyuta/bqemulatormanager/blob/main/examples/testing.py).
 
-package_data = \
-{'': ['*']}
+### automatically detect schema
+When called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `master_schema.yaml`).
 
-install_requires = \
-['db-dtypes>=1.0.4,<2.0.0',
- 'google-cloud-bigquery==2.34.4',
- 'psutil>=5.9.3,<6.0.0',
- 'pyyaml>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'bqemulatormanager',
-    'version': '0.1.8',
-    'description': '',
-    'long_description': "# BiqQueryEmulator Manager\n\n\nthis package is wrapper of [bigquery-emulator](https://github.com/goccy/bigquery-emulator) which provides us BigQuery mock working in local machine.\n\nusing this package, you can\n\n- do unit test of your sql\n- download the schema of big query, and use it to make test data\n\n## usage\n1. following [instruction](https://github.com/goccy/bigquery-emulator#install),  download `bigquery-emulator` command.\n\n2. install this package. \n```\npip install bqemulatormanager\n```\n\n3. test your sql.\n```python\nimport bqemulatormanager as bqem\nimport pandas as pd\n\nmanager = bqem.Manager(project='test', schema_path='resources/schema_example.yaml')\n\nwith manager:\n    data = pd.DataFrame([\n        {'id': 1, 'name': 'sato'},\n        {'id': 2, 'name': 'yamada'}\n    ])\n\n    manager.load(data, 'dataset1.table_a')\n\n    sql = 'SELECT id, name FROM `dataset1.table_a`'\n\n    df = manager.query(sql)\nprint(df)\n```\n\n### automatically detect schema\nWhen called `Manager.load`, `SchemaManager` search correspond table schema from `schema_path` (default is `master_schema.yaml`).\n\nIf schema definition canot be found, `SchemaManager` request it from BigQuery in production environmant and update master schema file.",
-    'author': 'gyuta',
-    'author_email': 'kuroshiba0408@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
+If schema definition canot be found, `SchemaManager` request it from BigQuery in production environmant and update master schema file.
```

