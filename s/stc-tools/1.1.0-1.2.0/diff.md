# Comparing `tmp/stc-tools-1.1.0.tar.gz` & `tmp/stc-tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-tools-1.1.0.tar", last modified: Sat Jun  3 15:54:48 2023, max compression
+gzip compressed data, was "stc-tools-1.2.0.tar", last modified: Sat Jun  3 17:51:05 2023, max compression
```

## Comparing `stc-tools-1.1.0.tar` & `stc-tools-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 15:54:48.031400 stc-tools-1.1.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.1.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 15:54:48.031025 stc-tools-1.1.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.1.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      560 2023-05-30 19:50:14.000000 stc-tools-1.1.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       42 2023-06-01 07:12:13.000000 stc-tools-1.1.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-03 15:54:48.031530 stc-tools-1.1.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 15:54:48.027051 stc-tools-1.1.0/stc_tools/
--rw-r--r--   0 pasha      (501) staff       (20)     4481 2023-06-03 15:54:29.000000 stc-tools-1.1.0/stc_tools/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     2770 2023-06-03 11:42:04.000000 stc-tools-1.1.0/stc_tools/client.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 15:54:48.030482 stc-tools-1.1.0/stc_tools.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-03 15:54:48.000000 stc-tools-1.1.0/stc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.026045 stc-tools-1.2.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-tools-1.2.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 17:51:05.025719 stc-tools-1.2.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-tools-1.2.0/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      560 2023-06-03 17:50:38.000000 stc-tools-1.2.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-03 17:46:10.000000 stc-tools-1.2.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-03 17:51:05.026168 stc-tools-1.2.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.020744 stc-tools-1.2.0/stc_tools/
+-rw-r--r--   0 pasha      (501) staff       (20)     4499 2023-06-03 16:05:24.000000 stc-tools-1.2.0/stc_tools/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2770 2023-06-03 11:42:04.000000 stc-tools-1.2.0/stc_tools/client.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-03 17:51:05.025058 stc-tools-1.2.0/stc_tools.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      298 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      290 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       49 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       44 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-03 17:51:05.000000 stc-tools-1.2.0/stc_tools.egg-info/top_level.txt
```

### Comparing `stc-tools-1.1.0/pyproject.toml` & `stc-tools-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-tools"
-version = "1.1.0"
+version = "1.2.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Standard Template Construct Client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-tools-1.1.0/stc_tools/cli.py` & `stc-tools-1.2.0/stc_tools/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
     def __str__(self):
         return f'CidNotFound(query="{self.query}")'
 
 
 class StcCliTools(StcTools):
     default_default_fields = {
-        'nexus_science': ('title', 'abstract',),
-        'nexus_books': ('title',),
+        'nexus_science': ['title', 'abstract', ],
+        'nexus_books': ['title', ],
     }
 
     def __init__(
-        self,
-        ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
-        index_name: str = 'nexus_science',
-        timeout: int = 600,
+            self,
+            ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
+            index_name: str = 'nexus_science',
+            timeout: int = 600,
     ):
         super().__init__(ipfs_http_endpoint=ipfs_http_endpoint,
                          paths=(f'/ipns/standard-template-construct.org/data/{index_name}/',))
         self.index_name = index_name
         self.timeout = timeout
 
     async def search(self, query: str, limit: int = 1):
@@ -52,22 +52,22 @@
         :return: metadata records
         """
         print(f"{colored('INFO', 'green')}: Setting up indices: {', '.join(self.paths)}...")
         await self.start()
         print(f"{colored('INFO', 'green')}: Searching {query}...")
         response = await super().search([{
             "index_alias": self.index_name,
-            "query": {"query": {
+            "query": {
                 "match": {"value": query, "default_fields": self.default_default_fields[self.index_name],
-                          'field_boosts': {}}}},
-            "collectors": [{"collector": {"top_docs": {"limit": limit}}}],
+                          'field_boosts': {}}},
+            "collectors": [{"top_docs": {"limit": limit}}],
             "is_fieldnorms_scoring_enabled": False,
         }])
         return list(
-            map(lambda x: json.loads(x['document']), response[0]['collector_output']['documents']['scored_documents']))
+            map(lambda x: json.loads(x.document), response.collector_outputs[0].documents.scored_documents))
 
     async def download(self, query: str, output_path: str):
         """
         Download file from STC using default Summa match queries.
         Examples: `doi:10.1234/abc, isbns:9781234567890`
 
         :param query: query in Summa match format
@@ -79,32 +79,33 @@
         output_path, output_path_ext = os.path.splitext(output_path)
         output_path_ext = output_path_ext.lstrip('.')
         if results:
             print(f"{colored('INFO', 'green')}: Found {query}")
             if 'cid' in results[0]:
                 print(f"{colored('INFO', 'green')}: Receiving file {query}...")
                 if (real_extension := results[0].get('extension', 'pdf')) != output_path_ext:
-                    print(f"{colored('WARN', 'yellow')}: Receiving file extension `{real_extension}` is not matching with your output path extension `{output_path_ext}`. Changed to correct one.")
+                    print(
+                        f"{colored('WARN', 'yellow')}: Receiving file extension `{real_extension}` is not matching with your output path extension `{output_path_ext}`. Changed to correct one.")
                     output_path_ext = real_extension
                 data = await super().download(results[0]["cid"], self.timeout)
                 final_file_name = output_path + '.' + output_path_ext
                 with open(final_file_name, 'wb') as f:
                     f.write(data)
                     f.close()
                     print(f"{colored('INFO', 'green')}: File {final_file_name} is written")
             else:
                 print(f"{colored('ERROR', 'red')}: Not found CID for {query}", file=sys.stderr)
         else:
             print(f"{colored('ERROR', 'red')}: Not found {query}", file=sys.stderr)
 
 
 async def stc_tools_cli(
-    ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
-    index_name: str = 'nexus_science',
-    timeout: int = 600
+        ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
+        index_name: str = 'nexus_science',
+        timeout: int = 600
 ):
     """
 
     :param ipfs_http_endpoint: IPFS HTTP API Endpoint
     :param index_name: `nexus_books` (similar to LibGen) or `nexus_science` (similar to Crossref)
     :param timeout: timeout for requests to IPFS
     :return:
```

### Comparing `stc-tools-1.1.0/stc_tools/client.py` & `stc-tools-1.2.0/stc_tools/client.py`

 * *Files identical despite different names*

