# Comparing `tmp/optilogic-2.5.0-py3-none-any.whl.zip` & `tmp/optilogic-2.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 39706 bytes, number of entries: 17
--rw-r--r--  2.0 unx       22 b- defN 23-May-10 01:06 optilogic/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 23-May-10 01:06 optilogic/pioneer/__init__.py
--rw-r--r--  2.0 unx       20 b- defN 23-May-10 01:06 optilogic/pioneer/api/__init__.py
--rw-r--r--  2.0 unx    72496 b- defN 23-May-10 01:06 optilogic/pioneer/api/api.py
--rw-r--r--  2.0 unx    96477 b- defN 23-May-10 01:06 optilogic/pioneer/api/api_tests.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-10 01:06 optilogic/pioneer/api/quick_tests/__init__.py
--rw-r--r--  2.0 unx     5111 b- defN 23-May-10 01:06 optilogic/pioneer/api/quick_tests/airline_hub_location_cbc.py
--rw-r--r--  2.0 unx      317 b- defN 23-May-10 01:06 optilogic/pioneer/api/quick_tests/bash.py
--rw-r--r--  2.0 unx      209 b- defN 23-May-10 01:06 optilogic/pioneer/api/quick_tests/quick.py
--rw-r--r--  2.0 unx      577 b- defN 23-May-10 01:06 optilogic/pioneer/api/quick_tests/sleep.py
--rw-r--r--  2.0 unx      131 b- defN 23-May-10 01:06 optilogic/pioneer/job_utils/__init__.py
--rw-r--r--  2.0 unx     3553 b- defN 23-May-10 01:06 optilogic/pioneer/job_utils/job_utils.py
--rw-r--r--  2.0 unx     1070 b- defN 23-May-10 01:06 optilogic-2.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      759 b- defN 23-May-10 01:06 optilogic-2.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:06 optilogic-2.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-10 01:06 optilogic-2.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1523 b- defN 23-May-10 01:06 optilogic-2.5.0.dist-info/RECORD
-17 files, 182415 bytes uncompressed, 37144 bytes compressed:  79.6%
+Zip file size: 46542 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-03 19:27 optilogic/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-03 19:27 optilogic/pioneer/__init__.py
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/__init__.py
+-rw-r--r--  2.0 unx    74338 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/api.py
+-rw-r--r--  2.0 unx   126839 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/api_tests.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/__init__.py
+-rw-r--r--  2.0 unx     5111 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/airline_hub_location_cbc.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/bash.py
+-rw-r--r--  2.0 unx      209 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/quick.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/sidecar.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Jun-03 19:27 optilogic/pioneer/api/quick_tests/sleep.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-03 19:27 optilogic/pioneer/job_utils/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Jun-03 19:27 optilogic/pioneer/job_utils/job_utils.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-03 19:28 optilogic-2.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      759 b- defN 23-Jun-03 19:28 optilogic-2.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 19:28 optilogic-2.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-03 19:28 optilogic-2.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jun-03 19:28 optilogic-2.6.0.dist-info/RECORD
+18 files, 215446 bytes uncompressed, 43816 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -21,32 +21,35 @@
 
 Filename: optilogic/pioneer/api/quick_tests/bash.py
 Comment: 
 
 Filename: optilogic/pioneer/api/quick_tests/quick.py
 Comment: 
 
+Filename: optilogic/pioneer/api/quick_tests/sidecar.py
+Comment: 
+
 Filename: optilogic/pioneer/api/quick_tests/sleep.py
 Comment: 
 
 Filename: optilogic/pioneer/job_utils/__init__.py
 Comment: 
 
 Filename: optilogic/pioneer/job_utils/job_utils.py
 Comment: 
 
-Filename: optilogic-2.5.0.dist-info/LICENSE
+Filename: optilogic-2.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: optilogic-2.5.0.dist-info/METADATA
+Filename: optilogic-2.6.0.dist-info/METADATA
 Comment: 
 
-Filename: optilogic-2.5.0.dist-info/WHEEL
+Filename: optilogic-2.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: optilogic-2.5.0.dist-info/top_level.txt
+Filename: optilogic-2.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: optilogic-2.5.0.dist-info/RECORD
+Filename: optilogic-2.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optilogic/pioneer/api/api.py

```diff
@@ -33,25 +33,61 @@
 import pickle
 import time
 from cachetools import cached, TTLCache
 from datetime import datetime
 from getpass import getpass
 from json import dumps, loads
 from os import getenv
-from re import fullmatch
+from re import fullmatch, search
 from requests import ConnectionError, delete, get, HTTPError, Response, request
 from sys import platform
 from tempfile import gettempdir
 from types import FrameType
-from typing import Any, cast, Dict, List, Literal, Tuple, TypedDict, Optional
+from typing import Any, cast, Dict, List, Literal, Set, Tuple, TypedDict, Optional
 from warnings import warn, warn_explicit
 
 if platform == 'linux':
     from inspect import currentframe
     from signal import alarm, signal, SIGALRM
+    from urllib.parse import unquote
+
+
+class DbTemplates(TypedDict):
+    id: Literal[
+        '2.1',
+        '3.1',
+        '5.1',
+        '7.5',
+        '9.6',
+        '12.3',
+        '15.2',
+        '18.3',
+        '21.2',
+        '24.3',
+        '27.2',
+        '28.2',
+        '30.2',
+        '31.1',
+    ]
+    name: Literal[
+        'Empty Database',
+        'Anura New Model v2.4',
+        'Anura New Model v2.5',
+        'Anura New Model v2.6.31.3',
+        'Global Supply Chain Strategy',
+        'Tactical Capacity Optimization',
+        'Detailed Facility Selection',
+        'United States Greenfield Facility Selection',
+        'China Exit Strategy in Asia',
+        'China Exit Risk Strategy',
+        'Multi-Year Capacity Planning',
+        'Fleet Size Optimization - EMEA Geo',
+        'Fleet Size Optimization - US Geo',
+        'Global Sustainability Analysis',
+    ]
 
 
 class Api:
     '''Optilogic API is to pilot Andromeda system
 
     EXAMPLE CONFIG
     :{'un': 'username', 'pw': 'password', 'auth_legacy': True}
@@ -61,81 +97,47 @@
     :param pw: str: password of the user to authenticate and generate api key
     :param auth_legacy: bool: true for conventional username password or false for appkey
     :param cfg: dict: addition config to unpack and setup for api use
     :param apikey: str: username password authentication with one hour time to live
     :param appkey: str: authentication key generated in product without time to live restrictions
     '''
 
-    class DbTemplates(TypedDict):
-        id: Literal[
-            '2.1',
-            '3.1',
-            '5.1',
-            '7.1',
-            '9.2',
-            '9.3',
-            '12.1',
-            '15.1',
-            '18.1',
-            '21.1',
-            '24.1',
-            '27.1',
-            '28.1',
-            '30.1',
-        ]
-        name: Literal[
-            'Empty Database',
-            'Anura New Model v2.4',
-            'Anura New Model v2.5',
-            'Anura New Model v2.6',
-            'Blast Off To Space (BOTS) - v2.4',
-            'Blast Off To Space (BOTS) - v2.5',
-            'Tactical Capacity Optimization',
-            'Detailed Facility Selection',
-            'Greenfield Facility Selection',
-            'China Exit Strategy in Asia',
-            'Out of China',
-            'Multi-Year Capacity Planning',
-            'Fleet Size Optimization - EMEA Geo',
-            'Fleet Size Optimization - US Geo',
-        ]
-
     DATABASE_TEMPLATES_NEW: Tuple[DbTemplates, ...] = (
         {'id': '2.1', 'name': 'Empty Database'},
         {'id': '3.1', 'name': 'Anura New Model v2.4'},
         {'id': '5.1', 'name': 'Anura New Model v2.5'},
-        {'id': '7.1', 'name': 'Anura New Model v2.6'},
-        {'id': '9.2', 'name': 'Blast Off To Space (BOTS) - v2.4'},
-        {'id': '9.3', 'name': 'Blast Off To Space (BOTS) - v2.5'},
-        {'id': '12.1', 'name': 'Tactical Capacity Optimization'},
-        {'id': '15.1', 'name': 'Detailed Facility Selection'},
-        {'id': '18.1', 'name': 'Greenfield Facility Selection'},
-        {'id': '21.1', 'name': 'China Exit Strategy in Asia'},
-        {'id': '24.1', 'name': 'Out of China'},
-        {'id': '27.1', 'name': 'Multi-Year Capacity Planning'},
-        {'id': '28.1', 'name': 'Fleet Size Optimization - EMEA Geo'},
-        {'id': '30.1', 'name': 'Fleet Size Optimization - US Geo'},
-    )
-
-    DATABASE_TEMPLATES: Tuple[str, ...] = (
-        'empty',
-        'anura_2_4_clean',
-        'anura_2_5_clean',
-        'anura_2_6_clean',
-        'anura_2_4_blast_off_to_space',
-        'anura_2_5_blast_off_to_space',
-        '37392edb-d582-4ce8-9f75-024651aa8592',  # Tactical Capacity Optimization
-        '67a881b3-b6ab-4e95-9452-6dae8e831a6b',  # Detailed Facility Selection
-        '71214744-f90a-4dcc-8008-bb9dab9493be',  # Greenfield Facility Selection
-        '812d6fae-9fe7-4541-bee5-3cdb78e03eeb',  # China Exit Strategy in Asia
-        'b30d9156-d00b-11ed-b72f-9fd8ea75300c',  # Fleet Size Optimization - US Geo
-        'b69f11eb-ed38-4b72-a43d-d59f7ab2cfa6',  # Out of China
-        'd3cba0d2-d00a-11ed-b72f-9fd8ea75300c',  # Fleet Size Optimization - EMEA Geo
-        'd74fd9cc-e829-4ad3-9f33-f4ef0f3ddae1',  # Multi-Year Capacity Planning
+        {'id': '7.5', 'name': 'Anura New Model v2.6.31.3'},
+        {'id': '9.6', 'name': 'Global Supply Chain Strategy'},
+        {'id': '12.3', 'name': 'Tactical Capacity Optimization'},
+        {'id': '15.2', 'name': 'Detailed Facility Selection'},
+        {'id': '18.3', 'name': 'United States Greenfield Facility Selection'},
+        {'id': '21.2', 'name': 'China Exit Strategy in Asia'},
+        {'id': '24.3', 'name': 'China Exit Risk Strategy'},
+        {'id': '27.2', 'name': 'Multi-Year Capacity Planning'},
+        {'id': '28.2', 'name': 'Fleet Size Optimization - EMEA Geo'},
+        {'id': '30.2', 'name': 'Fleet Size Optimization - US Geo'},
+        {'id': '31.1', 'name': 'Global Sustainability Analysis'},
     )
+    DATABASE_TEMPLATES_NAMEID: Dict[str, str] = {
+        'Empty Database': 'template1',
+        'Anura New Model v2.4': 'anura_2_4_clean',
+        'Anura New Model v2.5': 'anura_2_5_clean',
+        'Anura New Model v2.6.31.3': 'anura_2_6_31_3_clean',
+        'China Exit Risk Strategy': '013464d6-fc26-11ed-9e4e-a11cd8043d36',
+        'China Exit Strategy in Asia': '8540fa74-fc25-11ed-9e4e-a11cd8043d36',
+        'Detailed Facility Selection': 'b1d326f8-fc24-11ed-9e4e-a11cd8043d36',
+        'Fleet Size Optimization - EMEA Geo': 'a7f7f15c-fc26-11ed-9e4e-a11cd8043d36',
+        'Fleet Size Optimization - US Geo': '31409694-fc27-11ed-9e4e-a11cd8043d36',
+        'Global Supply Chain Strategy': '45e32716-fc12-11ed-9e4e-a11cd8043d36',
+        'Global Sustainability Analysis': '414f1a0e-014c-11ee-a300-87949ad7341e',
+        'Multi-Year Capacity Planning': '6f94b818-fc26-11ed-9e4e-a11cd8043d36',
+        'Tactical Capacity Optimization': '42c32042-fc24-11ed-9e4e-a11cd8043d36',
+        'United States Greenfield Facility Selection': '0d2017a0-fc25-11ed-9e4e-a11cd8043d36',
+    }
+    DATABASE_TEMPLATES: List[str] = [v for v in DATABASE_TEMPLATES_NAMEID.values()]
     GEO_PROVIDERS: Tuple[str, ...] = ('bing', 'google', 'mapbox', 'pcmiler', 'ptv')
     JOBSTATES: Tuple[str, ...] = (
         'submitted',
         'starting',
         'started',
         'running',
         'done',
@@ -250,14 +252,15 @@
         self._log_active: bool = False
 
         if os.path.exists(self.dir_tmp) is False:
             os.makedirs(self.dir_tmp)
         if os.path.exists(self.file_cache_auth) is False and self.auth_method_legacy:
             self.authenticate_legacy()
 
+        self.re_uuid4 = '(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)'
         self._job_start_recent_key: str = self.__job_key_recent()
 
         if cfg.get('user_info'):
             self.__account_summary_info()
 
     def __account_summary_info(self) -> None:
         '''display account information'''
@@ -384,16 +387,31 @@
         fn: str = cast(
             FrameType, cast(FrameType, cast(FrameType, currentframe()).f_back).f_back
         ).f_code.co_name
 
         secs: float = round(rsp.elapsed.total_seconds(), 4)
         verb: str = rsp.request.method.upper() if rsp.request.method else ''
         now: datetime = datetime.utcnow()
+        url: str = unquote(rsp.url)
+        url = url.replace(',', '')
+        log: str = f'{now},{secs},{fn.upper()},{rsp.status_code},{verb},{url},'
+        if rsp.request.body and isinstance(rsp.request.body, bytes):
+            body: str = rsp.request.body.decode('utf-8', 'ignore')
+            body = body.replace(',', '')
+            log += f'{body},'
+        else:
+            log += ','
+        if 500 <= rsp.status_code < 600:
+            try:
+                d: dict = rsp.json()
+                log += f"{rsp.reason} {d.get('error')} {d.get('correlationId')}"
+            except ValueError:
+                log += f'{rsp.text}'
         with open(self.file_log_http, 'a+') as f:
-            f.write(f'{now},{secs},{fn.upper()},{rsp.status_code},{verb},{rsp.url}\n')
+            f.write(f'{log}\n')
 
     def __schema_anura_versions(self) -> List[str]:
         '''list of anura schemas tha major.minor.build'''
 
         resp = self.database_schemas()
         versions: List[str] = [s['schemaVersion'] for s in resp['schemas']['anura']]
         return sorted(versions, reverse=True)
@@ -474,36 +492,42 @@
             now_time: float = datetime.now().timestamp() + 120
             mins_left: float = round((cache['expiration_time'] - now_time) / 60, 2)
             self.auth_apikey_mins_left = mins_left
             self.auth_apikey = cache['apikey']
             self.auth_apikey_expiry = cache['expiration_time']
             self.auth_req_header.update({'x-api-key': cache['apikey']})
 
+    def _database_by_name(self, name: str, wildcard=False) -> List[Dict[str, Any]]:
+        '''find all database by name
+
+        :param name: str: database name
+        :param wildcard: str: allow name to use regex case-insensitive matching, default to False
+        '''
+
+        devices: List[Dict[str, Any]] = self.__storage_type('postgres_db')
+        dbs: List[Dict[str, Any]] = []
+
+        for d in devices:
+            if wildcard is False:
+                if name == d['name']:
+                    dbs.append(d)
+                else:
+                    if search(name, d['name'].lower()):
+                        dbs.append(d)
+        return dbs
+
     def _database_templates_by_name(self, name: str, wildcard=False) -> List[str]:
         '''find all database template ids by case-insensitive template name
 
         :param name: str: template name
-        :param wildcard: str: substr matching, default to False
+        :param wildcard: str: allow name to use substr matching, default to False
         '''
 
         # template[name, id]
-        template_map: Dict[str, str] = {
-            'empty': 'Empty Database',
-            'Anura - Blast off to Space': 'anura_2_5_blast_off_to_space',
-            'Anura - New Model': 'anura_2_5_clean',
-            'Anura - New Model (2.6)': 'anura_2_6_clean',
-            'China Exit Strategy in Asia': '812d6fae-9fe7-4541-bee5-3cdb78e03eeb',
-            'Detailed Facility Selection': '67a881b3-b6ab-4e95-9452-6dae8e831a6b',
-            'Fleet Size Optimization - EMEA Geo': 'd3cba0d2-d00a-11ed-b72f-9fd8ea75300c',
-            'Fleet Size Optimization - US Geo': 'b30d9156-d00b-11ed-b72f-9fd8ea75300c',
-            'Greenfield Facility Selection': '71214744-f90a-4dcc-8008-bb9dab9493be',
-            'Multi-Year Capacity Planning': 'd74fd9cc-e829-4ad3-9f33-f4ef0f3ddae1',
-            'Out of China': 'b69f11eb-ed38-4b72-a43d-d59f7ab2cfa6',
-            'Tactical Capacity Optimization': '37392edb-d582-4ce8-9f75-024651aa8592',
-        }
+        template_map: Dict[str, str] = {t['name']: t['id'] for t in self.DATABASE_TEMPLATES_NEW}
 
         matches: List[str] = []
         name = name.lower()
 
         for t in template_map.items():
             if wildcard is False:
                 # case-insensitive
@@ -527,34 +551,18 @@
     def _database_templates_legacy_by_name(self, name: str, wildcard=False) -> List[str]:
         '''find all database template ids by case-insensitive template name
 
         :param name: str: template name
         :param wildcard: str: substr matching, default to False
         '''
 
-        # template[name, id]
-        template_map: Dict[str, str] = {
-            'empty': 'Empty Database',
-            'Anura - Blast off to Space': 'anura_2_5_blast_off_to_space',
-            'Anura - New Model': 'anura_2_5_clean',
-            'Anura - New Model (2.6)': 'anura_2_6_clean',
-            'China Exit Strategy in Asia': '812d6fae-9fe7-4541-bee5-3cdb78e03eeb',
-            'Detailed Facility Selection': '67a881b3-b6ab-4e95-9452-6dae8e831a6b',
-            'Fleet Size Optimization - EMEA Geo': 'd3cba0d2-d00a-11ed-b72f-9fd8ea75300c',
-            'Fleet Size Optimization - US Geo': 'b30d9156-d00b-11ed-b72f-9fd8ea75300c',
-            'Greenfield Facility Selection': '71214744-f90a-4dcc-8008-bb9dab9493be',
-            'Multi-Year Capacity Planning': 'd74fd9cc-e829-4ad3-9f33-f4ef0f3ddae1',
-            'Out of China': 'b69f11eb-ed38-4b72-a43d-d59f7ab2cfa6',
-            'Tactical Capacity Optimization': '37392edb-d582-4ce8-9f75-024651aa8592',
-        }
-
         matches: List[str] = []
         name = name.lower()
 
-        for t in template_map.items():
+        for t in self.DATABASE_TEMPLATES_NAMEID.items():
             if wildcard is False:
                 # case-insensitive
                 if name == t[0].lower():
                     matches.append(t[1])
             else:
                 # substring case-insensitive
                 if t[0].lower().find(name) > -1:
@@ -716,20 +724,20 @@
             elif params == 1:
                 if (n == name) or (t and t == category) or (d and desc and d.find(desc) > -1):
                     matches.append(s)
 
         return matches
 
     def _storage_attr(
-        self, name: str, attr: Literal['annotation', 'label', 'tag'] = 'tag'
+        self, name: str, attr: Literal['annotations', 'labels', 'tags'] = 'tags'
     ) -> Dict[str, Any]:
         '''GET /v0/storage/{storageName}/{attribute}
 
         :param name: str: storage device name
-        :param attr: str: specific storage device attribute, defaults to tag
+        :param attr: str: specific storage device attribute, defaults to tags
         '''
 
         url: str = f'{self.api_version}storage/{name}/{attr}'
         resp: Dict[str, Any] = self._fetch_json('get', url)
         return resp
 
     @cached(cache=TTLCache(maxsize=1, ttl=86400))
@@ -858,28 +866,39 @@
         return self.storage(name)
 
     @property
     def database_count(self) -> int:
         ''' 'quantity of a postgres databases in account'''
         return self.storagetype_count('postgres_db')
 
+    def database_clone(self, name: str, new_name: str) -> Dict[str, str]:
+        '''POST /storage/clone - duplicate a postgress database
+
+        :param name: str: postgres database name
+        :param new_name: str: change the db name that is to be duplicated to a new name
+        '''
+
+        url: str = f'{self.api_version}storage/{name}/clone?name={new_name}&description=Duplicated via OptiPy'
+        resp: Dict[str, Any] = self._fetch_json('post', url)
+        return resp
+
     def database_create(
-        self, name: str, desc: Optional[str] = None, template='anura_2_5_clean'
+        self, name: str, desc: Optional[str] = None, template='anura_2_6_31_3_clean'
     ) -> Dict[str, Any]:
         '''POST /storage/{database_name} - create a postgres database
 
         :param name: str: name of postgres database to create
         :param desc: str: describe the purpose
         :param template: str: database template id
             empty,
-            anura_2_5_clean,
-            anura_2_6_clean is for Tech Preview users only,
-            anura_2_5_blast_off_to_space
+            anura_2_6_31_3_clean
         '''
 
+        if template == 'empty':
+            template = 'template1'
         if template not in self.DATABASE_TEMPLATES:
             # try to find id by looking up by name
             template_ids: List[str] = self._database_templates_legacy_by_name(name)
             if len(template_ids) > 0:
                 raise ValueError(
                     f'invalid database template id {template}, possible matches {template_ids}'
                 )
@@ -924,14 +943,53 @@
             query += 'views' if views else ''
             query = query.rstrip(',')
             url += query
 
         resp: Dict[str, Any] = self._fetch_json('get', url)
         return resp
 
+    def database_export(
+        self,
+        name: str,
+        named: Optional[List[str]] = None,
+        group: Optional[
+            Literal['all', 'nonEmptyAll', 'nonEmptyTables', 'nonEmptyViews', 'tables', 'views']
+        ] = None,
+        query: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        '''POST /storage/{database_name}/db-data-export - initiates a system job to perform export operation
+
+        set group, named, or query param to dictate what is exported to a zip csv download
+
+        :param name: str: postgres database name
+        :param named: list[str]: table or view name(s), defaults to None
+        :param group: str: all, nonEmptyAll, tables, views, nonEmptyTables, nonEmptyViews, defaults to None
+        :param query: str: sql query to execute, defaults to None
+        '''
+
+        g: Set[str] = {'all', 'nonEmptyAll', 'nonEmptyTables', 'nonEmptyViews', 'tables', 'views'}
+        d: Dict[str, Any] = {}
+
+        if named is not None:
+            if len(named) == 0:
+                raise ValueError(f'must provide a table/view name to export from {name} database')
+            d['sourceList'] = named
+        if group is not None:
+            if group not in g:
+                raise ValueError(f'invalid export group {group}, expecting: {g}')
+            d['sourceGroup'] = group
+        if query is not None:
+            if len(query) < 5:
+                raise AssertionError('sql query too short to be valid')
+            d['sourceQuery'] = query
+
+        url: str = f'{self.api_version}storage/{name}/db-data-export'
+        resp: Dict[str, Any] = self._fetch_json('post', url, json=d)
+        return resp
+
     @cached(cache=TTLCache(maxsize=1, ttl=86400))
     def database_schemas(self) -> Dict[str, Any]:
         '''postgres database schemas and versions'''
 
         url: str = f'{self.api_version}storage/db-versions'
         resp: Dict[str, Any] = self._fetch_json('get', url)
         return resp
@@ -1281,19 +1339,16 @@
 
         fail-safe stop will occur when job is in a terminal state
         '''
 
         if stop_when not in self.JOBSTATES:
             raise ValueError(f'expecting job state in {str(self.JOBSTATES)}')
 
-        # uuid4 pattern
-        pat = '(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)'
-
         # validate uuid4 job key case-insensitive
-        valid_job_key = bool(fullmatch(pat, job_key, flags=2))
+        valid_job_key = bool(fullmatch(self.re_uuid4, job_key, flags=2))
         if valid_job_key is False:
             raise ValueError(f'job_key is invalid uuid4 {job_key}')
 
         time_start: float = time.time()
         secs: float = 2.5
         retry: bool = True
         while True:
```

## optilogic/pioneer/api/api_tests.py

```diff
@@ -28,19 +28,37 @@
 from docopt import docopt
 from io import StringIO
 from json import dumps, loads
 from numbers import Number
 from random import randint
 from re import fullmatch, search
 from sys import platform
-from typing import Any, Dict, List, Literal, Tuple, Optional
+from typing import Any, Dict, Final, List, Literal, Tuple, TypedDict, Optional
 from warnings import warn
 from uuid import uuid4
 
 
+class Templates(TypedDict):
+    '''Typing database templates data structure'''
+
+    baseId: int
+    baselineSchemaVersion: str
+    id: float
+    isDefault: bool
+    longDescription: str
+    media: list
+    name: str
+    pgTemplateName: str
+    schema: str
+    shortDescription: str
+    tags: list
+    templateType: str
+    templateVersion: str
+
+
 class TestApi(unittest.TestCase):
     '''A series of Pioneer REST API unit tests
 
     OVERRIDE
     docopt configuration passed into the module will override the default static members
 
     STATIC MEMBERS
@@ -52,44 +70,45 @@
     '''
 
     USERNAME: Optional[str] = None
     USERPASS: Optional[str] = None
     WKSP: str = 'Studio'
     APPKEY: Optional[str] = None
     AUTH_LEGACY: bool = False
-
-    # method execution order - unittest.TestLoader.sortTestMethodsUsing
-    # default string sort of class method names startswith test_{method-name}, ie dir(self)
+    TEST_SYSTEM: bool = False
 
     @classmethod
     def setUpClass(cls) -> None:
         '''called before test methods are ran
         ensure cache directories and test data inputs are available in target wksp
         '''
 
         cls.API = api.Api(
             auth_legacy=cls.AUTH_LEGACY,
             appkey=cls.APPKEY,
             un=cls.USERNAME,
             pw=cls.USERPASS,
+            test_system=cls.TEST_SYSTEM,
         )
+        print(cls.API._domain)
         cls.__jobkey_quick: str = ''
         cls.API._log_active = True
 
         # directory references
         cls.dir_local_current: str = os.path.dirname(__file__)
         cls.dir_testdata_local: str = os.path.join(cls.dir_local_current, 'quick_tests')
         assert os.path.exists(cls.dir_testdata_local)
         assert len(os.listdir(cls.dir_testdata_local)) >= 1
         cls.dir_testdata_remote: str = 'quick_tests'
         cls.files_testdata_local: list[str] = []
         cls.files_testdata_remote: list[str] = []
-        cls.py_run_me: str = ''
-        cls.py_run_me_bash: str = ''
-        cls.py_run_me_quick: str = ''
+        cls.py_sleep: str = ''
+        cls.py_bash: str = ''
+        cls.py_quick: str = ''
+        cls.py_sidecar: str = ''
 
         # get all directories from wksp
         resp = cls.API.wksp_files(cls.WKSP, '/quick_tests/')
         files_remote: list[str] = [f['filePath'] for f in resp['files']]
 
         # comb over local test data and map to destination file structure
         for f in os.listdir(cls.dir_testdata_local):
@@ -98,30 +117,41 @@
                 continue
             elif os.path.getsize(local) == 0:
                 continue
             dest: str = os.path.join(cls.dir_testdata_remote, f)
             cls.files_testdata_local.append(local)
             cls.files_testdata_remote.append(dest)
             if dest.endswith('sleep.py'):
-                cls.py_run_me = dest
+                cls.py_sleep = dest
             elif dest.endswith('quick.py'):
-                cls.py_run_me_quick = dest
+                cls.py_quick = dest
             elif dest.endswith('bash.py'):
-                cls.py_run_me_bash = dest
+                cls.py_bash = dest
+            elif dest.endswith('sidecar.py'):
+                cls.py_sidecar = dest
 
             # upload local test data to destination
             for idx, local in enumerate(cls.files_testdata_local):
                 dest = cls.files_testdata_remote[idx]
             res: list[str] = [f for f in files_remote if dest in f]
             if len(res) == 0:
                 print(f'uploading {dest}')
                 resp = cls.API.wksp_file_upload(
                     cls.WKSP, file_path_dest=dest, file_path_local=local
                 )
 
+    @classmethod
+    def tearDownClass(cls) -> None:
+        '''called after all tests have ran'''
+
+        dbs: List[Dict[str, Any]] = cls.API._database_by_name(r'unittest_\d')
+        for d in dbs:
+            print(f"Deleting database dust bunny {d['name']}")
+            cls.API.database_delete(d['name'])
+
     def database_ensure_exist(self, name: str = 'pg_unittest') -> None:
         '''database must exist for db unit tests'''
 
         # cache is for 10 seconds
         exists: bool = self.API.storagename_database_exists(name)
         if exists:
             resp: Dict[str, Any] = self.API.storage(name)
@@ -139,15 +169,15 @@
         except ValueError:
             return False
 
     def job_prereq(self) -> None:
         '''for running test methods in isolation'''
 
         resp = self.API.wksp_job_start(
-            self.WKSP, self.py_run_me_quick, tags='unittest_prereq', resourceConfig='mini'
+            self.WKSP, self.py_quick, tags='unittest_prereq', resourceConfig='mini'
         )
         self.assertEqual(resp['result'], 'success')
         self.__jobkey_quick = resp['jobKey']
         # BUG ledger and metrics should be immediately available when job is running
         res: bool = self.API.util_job_monitor(self.WKSP, resp['jobKey'], stop_when='done')
         self.assertTrue(res)
 
@@ -192,21 +222,27 @@
         self.assertIsInstance(d['bytesUsedLastUpdated'], int)
         self.assertIsInstance(d['dbname'], str)
         self.assertIsInstance(d['defaultSchema'], str)
         self.assertIsInstance(d['host'], str)
         self.assertIsInstance(d['port'], int)
         self.assertIsInstance(d['schemaStatus'], str)
         self.assertTrue(d['schemaStatus'] in ('error', 'invalid', 'valid'))
-        # self.assertIsInstance(d['schemaStatusLastUpdated'], float)  # BUG OE-7561
+        self.assertIsInstance(d['schemaStatusLastUpdated'], Number)
         self.assertIsInstance(d['schemaVersion'], str)
         self.assertIsInstance(d['user'], str)
+
         # empty pg datase vs anura schema
         if d['defaultSchema'].startswith('anura_2_'):
             self.assertRegex(d['schemaVersion'], r'2\.[4-9]\.\d+')
-            # self.assertIsInstance(d['schemaStatusLastValidated'], float)  # BUG OE-7561
+            self.assertIsInstance(d['schemaReleaseStatus'], str)
+            release_status: bool = d['schemaReleaseStatus'].startswith('stable') or d[
+                'schemaReleaseStatus'
+            ].startswith('preview')
+            self.assertTrue(release_status)
+            self.assertIsInstance(d['schemaStatusLastValidated'], Number)
         else:
             # self.assertTrue(len(d['defaultSchema']) == 0)  # TODO OE-7561
             self.assertTrue(len(d['schemaVersion']) == 0)
 
     def storage_onedrive(self, d: dict) -> None:
         '''common onedrive storage response for get device and devices'''
 
@@ -249,15 +285,15 @@
 
         self.assertEqual(output.find('REQUIRED API User Password'), -1)
 
     def test_000_prereqs(self) -> None:
         '''ensure job data is available to test against'''
 
         resp = self.API.wksp_job_start(
-            self.WKSP, self.py_run_me_quick, tags='unittest_preseed', resourceConfig='mini'
+            self.WKSP, self.py_quick, tags='unittest_preseed', resourceConfig='mini'
         )
         self.assertEqual(resp['result'], 'success')
         self.__jobkey_quick = resp['jobKey']
         stime: float = time.time()
         print('Pre-seeding by running a new job')
         res: bool = self.API.util_job_monitor(
             self.WKSP, resp['jobKey'], stop_when='done', secs_max=300
@@ -358,47 +394,47 @@
             if job['jobInfo']['command'] != 'run_custom':
                 self.assertIsInstance(job['jobInfo']['directoryPath'], str)
                 self.assertIsInstance(job['jobInfo']['filename'], str)
             self.assertIsInstance(job['jobInfo']['resourceConfig'], dict)
             self.assertIsInstance(job['jobInfo']['resourceConfig']['cpu'], str)
             self.assertIsInstance(job['jobInfo']['resourceConfig']['name'], str)
             self.assertIsInstance(job['jobInfo']['resourceConfig']['ram'], str)
-            self.assertIsInstance(
-                float(job['jobInfo']['resourceConfig']['run_rate']), float
-            )  # BUG OE-6710 float or int
+            self.assertIsInstance(job['jobInfo']['resourceConfig']['run_rate'], Number)
             self.assertIsInstance(job['jobInfo']['tags'], str)
             self.assertIsInstance(int(job['jobInfo']['timeout']), int)  # BUG OE-6710 str or int
             self.assertIsInstance(job['jobInfo']['workspace'], str)
             self.assertIsInstance(job['jobKey'], str)
-            self.assertIsInstance(float(job['runRate']), float)  # BUG OE-6710 float or int
+            self.assertIsInstance(job['runRate'], Number)
             self.assertIsInstance(job['status'], str)
             self.assertIsInstance(job['submittedDatetime'], str)
             self.assertIsInstance(job['submittedTimeStamp'], int)
 
-            if job['status'] in ('done', 'cancelled', 'error'):
+            if job['status'] in self.API.JOBSTATES_TERMINAL_RUNTIME:
                 self.assertTrue(job['canHaveResult'])
                 self.assertIsInstance(job['billedTime'], str)
-                self.assertIsInstance(float(job['billedTimeMs']), float)  # BUG OE-6710 float or int
+                self.assertIsInstance(job['billedTimeMs'], Number)
                 self.assertIsInstance(job['endDatetime'], str)
                 self.assertIsInstance(job['endTimeStamp'], int)
                 self.assertIsInstance(job['runTime'], str)
                 self.assertIsInstance(job['runTimeMs'], int)
                 self.assertIsInstance(job['startDatetime'], str)
                 self.assertIsInstance(job['startTimeStamp'], int)
             else:
-                # self.assertFalse(job['canHaveResult']) # BUG OE-6710 stopped cant have a result
-                pass
+                with self.subTest():
+                    self.assertIsNone(job['startDatetime'])
+                    self.assertIsNone(job['endDatetime'])
+                    self.assertFalse(job['canHaveResult'])
 
     def test_account_jobs_active(self) -> None:
         '''compare active account jobs count to all active wksp jobs'''
 
         start_new_job: bool = bool(randint(0, 1))
         if start_new_job:
             self.API.wksp_job_start(
-                self.WKSP, self.py_run_me, tags='unittest_jobs_active', resourceConfig='mini'
+                self.WKSP, self.py_sleep, tags='unittest_jobs_active', resourceConfig='mini'
             )
 
         active_account: int = 0
         resp = self.API._account_jobs(
             max_jobs=200
         )  # BUG submitted counts as active therefore must account for excessive submitted jobs
         for job in resp['jobs']:
@@ -427,15 +463,15 @@
                 if d['type'] == 'azure_workspace':
                     self.assertEqual(len(d), 16)
                     self.storage_azure_workspace(d)
                 elif d['type'] == 'onedrive':
                     self.assertEqual(len(d), 22)
                     self.storage_onedrive(d)
                 elif d['type'] == 'postgres_db':
-                    self.assertEqual(len(d), 22)
+                    self.assertEqual(len(d), 23)
                     self.storage_database(d)
 
     def test_account_usage(self) -> None:
         '''atlas and andromeda information'''
 
         resp = self.API._account_usage()
         self.assertEqual(resp['result'], 'success')
@@ -453,35 +489,32 @@
         self.assertEqual(len(str(resp['andromeda']['jobsMostRecent'])), 13)
         dt: datetime = datetime.fromtimestamp(resp['andromeda']['jobsMostRecent'] / 1000)
         now: datetime = datetime.utcnow()
         self.assertEqual(dt.year, now.year)
         self.assertEqual(dt.month, now.month)
 
         self.assertIsInstance(resp['atlas'], dict)
-        self.assertIsInstance(resp['atlas']['lastLogin'], int)
-        if resp['atlas']['periodHours'] == 0:
-            self.assertIsInstance(resp['atlas']['periodHours'], int)
+        if (
+            self.API._domain != 'https://api.optilogic.app'
+            and resp['atlas'].get('lastLogin') is None
+        ):
+            # BUG OE-7432
+            self.assertEqual(len(resp['atlas']), 3)
         else:
-            self.assertIsInstance(resp['atlas']['periodHours'], float)
+            self.assertEqual(len(resp['atlas']), 4)
+            self.assertIsInstance(resp['atlas']['lastLogin'], int)
+            self.assertEqual(len(str(resp['atlas']['lastLogin'])), 13)
+            dt: datetime = datetime.fromtimestamp(resp['atlas']['lastLogin'] / 1000)
+            self.assertIsInstance(dt, datetime)
+        self.assertIsInstance(resp['atlas']['periodHours'], Number)
         self.assertIsInstance(resp['atlas']['task'], dict)
         self.assertIsInstance(resp['atlas']['workspaceCount'], int)
-        self.assertEqual(len(resp['atlas']), 4)
-        self.assertEqual(len(str(resp['atlas']['lastLogin'])), 13)
-        dt: datetime = datetime.fromtimestamp(resp['atlas']['lastLogin'] / 1000)
-        self.assertIsInstance(dt, datetime)
-
         self.assertIsInstance(resp['atlas']['task'], dict)
-        if resp['atlas']['task']['durationCurrentWeek'] == 0:
-            self.assertIsInstance(resp['atlas']['task']['durationCurrentWeek'], int)
-        else:
-            self.assertIsInstance(resp['atlas']['task']['durationCurrentWeek'], float)
-        if resp['atlas']['task']['durationLastThirty'] == 0:
-            self.assertIsInstance(resp['atlas']['task']['durationLastThirty'], int)
-        else:
-            self.assertIsInstance(resp['atlas']['task']['durationLastThirty'], float)
+        self.assertIsInstance(resp['atlas']['task']['durationCurrentWeek'], Number)
+        self.assertIsInstance(resp['atlas']['task']['durationLastThirty'], Number)
         self.assertIsInstance(resp['atlas']['task']['durationTotal'], float)
         self.assertIsInstance(resp['atlas']['task']['lastDuration'], float)
         self.assertIsInstance(resp['atlas']['task']['lastRunStart'], int)
         self.assertIsInstance(resp['atlas']['task']['runCurrentWeek'], int)
         self.assertIsInstance(resp['atlas']['task']['runlastThirty'], int)
         self.assertIsInstance(resp['atlas']['task']['runTotal'], int)
         self.assertEqual(len(resp['atlas']['task']), 8)
@@ -548,18 +581,66 @@
         self.assertTrue(self.API.api_server_online)
 
     def test_api_version(self) -> None:
         '''only version zero is supported'''
 
         self.assertTrue(self.API.api_version.endswith('v0/'))
 
+    def test_database_clone(self) -> None:
+        '''duplicate a postgress database'''
+
+        self.database_ensure_exist()
+        name_new: str = f'pg_unittest_{time.perf_counter_ns()}'
+        name: str = f'pg_unittest'
+        resp: Dict[str, str] = self.API.database_clone(name, name_new)
+        self.assertIsInstance(resp['result'], str)
+        self.assertEqual(resp['result'], 'success')
+        self.assertEqual(len(resp.keys()), 3)
+        self.assertIsInstance(resp['jobKey'], str)
+        self.assertIsInstance(resp['storageId'], str)
+        self.assertTrue(bool(fullmatch(self.API.re_uuid4, resp['jobKey'], flags=2)))
+        self.assertTrue(bool(fullmatch(self.API.re_uuid4, resp['storageId'], flags=2)))
+
+        # TODO verify database was actually created and time to complete system jobs
+        # 1) db_clone
+        # 2) db_analyze
+        db_src = self.API.database(name)
+        ready: bool = False
+        while ready is False:
+            db_clone = self.API.database(name_new)
+            if db_clone.get('lockoutReason') is None:
+                ready = True
+                break
+            time.sleep(10)
+
+        # 3) db now exists
+        # self.assertEqual(db_clone['annotations']['sharedByUserName'], self.API.auth_username)
+        self.assertEqual(db_clone['description'], 'Duplicated via OptiPy')
+        self.assertTrue(db_clone['annotations']['shared'])
+
+        self.assertEqual(
+            db_src['annotations']['sourceBaseTemplateId'],
+            db_clone['annotations']['sourceBaseTemplateId'],
+        )
+        self.assertEqual(
+            db_src['annotations']['sourceBaseTemplateName'],
+            db_clone['annotations']['sourceBaseTemplateName'],
+        )
+        # self.assertEqual(db_src['bytesUsed'], db_clone['bytesUsed']) # BUG OE-8195
+        self.assertEqual(db_src['defaultSchema'], db_clone['defaultSchema'])
+        self.assertEqual(db_src['notes'], db_clone['notes'])
+        self.assertEqual(db_src['schemaReleaseStatus'], db_clone['schemaReleaseStatus'])
+        self.assertEqual(db_src['schemaStatus'], db_clone['schemaStatus'])
+        self.assertEqual(db_src['schemaVersion'], db_clone['schemaVersion'])
+        self.assertEqual(db_src['tags'], db_clone['tags'])
+
     def test_database_create_delete(self) -> None:
         '''create a postgres database then delete'''
 
-        bots: List[str] = self.API._database_templates_legacy_by_name('blast', wildcard=True)
+        bots: List[str] = self.API._database_templates_legacy_by_name('Global', wildcard=True)
         self.assertGreaterEqual(len(bots), 1)
         dbname: str = f'pg_unittest_{time.perf_counter_ns()}'
 
         # create database
         resp: dict = self.API.database_create(dbname, desc=f'unittest {dbname}', template=bots[0])
         self.assertIsInstance(resp['result'], str)
         self.assertEqual(resp['result'], 'success')
@@ -586,26 +667,64 @@
             warn(f'failed to create db within {wait_until} seconds)', UserWarning, stacklevel=2)
 
         # delete database
         resp = self.API.storage_delete(dbname)
         self.assertIsInstance(resp['result'], str)
         self.assertEqual(resp['result'], 'success')
 
+    @unittest.skip('run sparingly to minimize excessive db tombstoning')
+    def test_database_create_delete_all(self) -> None:
+        '''for each database template create a database, verify then delete it'''
+
+        for tname, tid in self.API.DATABASE_TEMPLATES_NAMEID.items():
+            # create database
+            db_name: str = f'pg_unittest_t_{time.perf_counter_ns()}'
+            db_desc: str = f'unittest {db_name}'
+            resp: dict = self.API.database_create(db_name, desc=db_desc, template=tid)
+            self.assertIsInstance(resp['result'], str)
+            self.assertEqual(resp['result'], 'success')
+            self.assertIsInstance(resp['storageId'], str)
+            self.assertEqual(len(resp['storageId']), 36)
+
+            # verify
+            db = self.API.database(db_name)
+            self.storage_database(db)
+            self.assertEqual(db['id'], resp['storageId'])
+            self.assertEqual(db['name'], db_name)
+            self.assertEqual(db['description'], db_desc)
+            self.assertEqual(db['schemaStatus'], 'valid')
+            print(f'\n\n{tid}, {tname},')
+            print(f"  tags: {len(db['tags'])},\n  {db['annotations']}")
+            if tid == 'template1':
+                self.assertTrue(db['annotations']['sourcedAsEmptyDatabase'])
+            elif tid.startswith('anura_2_'):
+                self.assertIsInstance(db['annotations']['sourceBaseTemplateId'], Number)
+                self.assertEqual(db['annotations']['sourceBaseTemplateName'], tname)
+            else:
+                self.assertIsInstance(db['annotations']['sourceTemplateSetId'], Number)
+                self.assertEqual(db['annotations']['sourceTemplateSetName'], tname)
+                self.assertEqual(len(db['tags']), 0)
+
+            # delete database
+            resp = self.API.storage_delete(db_name)
+            self.assertIsInstance(resp['result'], str)
+            self.assertEqual(resp['result'], 'success')
+
     def test_database_create_delete_wrong_id(self) -> None:
         '''create a postgres database with a template name instead of id'''
 
-        tname: str = 'Out of China'
+        tname: str = 'China Exit Risk Strategy'
         self.assertFalse(tname in self.API.DATABASE_TEMPLATES)
         with self.assertRaises(ValueError):
             self.API.database_create(name='cant', template=tname)
 
         # get template id
         tids: List[str] = self.API._database_templates_legacy_by_name(tname)
         self.assertEqual(len(tids), 1)
-        self.assertEqual(tids[0], 'b69f11eb-ed38-4b72-a43d-d59f7ab2cfa6')
+        self.assertEqual(tids[0], self.API.DATABASE_TEMPLATES_NAMEID[tname])
         dbname: str = f'pg_unittest_{time.perf_counter_ns()}'
 
         # create database with matching template id
         resp = self.API.database_create(dbname, desc=f'unittest {dbname} {tname}', template=tids[0])
         self.assertIsInstance(resp['result'], str)
         self.assertEqual(resp['result'], 'success')
         self.assertIsInstance(resp['storageId'], str)
@@ -632,14 +751,60 @@
 
     def test_database_create_failure_template_swap(self) -> None:
         '''attempt creating a postgres database with template name instead of id'''
 
         with self.assertRaises(ValueError):
             self.API.database_create(name='cant', template='Out of China')
 
+    def test_database_export(self) -> None:
+        '''initiate job to export database named empty table, nonEmptyTables, and custom sql query'''
+
+        DB: Final[str] = 'pg_unittest'
+        G: Final[str] = 'nonEmptyTables'
+        Q: Final[str] = 'SELECT datname FROM pg_database'  # BUG OE-8117
+        TBL: Final[List[str]] = ['advancedqueueingdetails']
+
+        with self.assertRaises(ValueError):
+            self.API.database_export(DB, named=[])
+
+        with self.assertRaises(ValueError):
+            self.API.database_export(DB, group='does_not_exist')  # type: ignore
+
+        with self.assertRaises(AssertionError):
+            self.API.database_export(DB, query='ha')
+
+        resp: Dict[str, Any] = self.API.database_export(DB, named=TBL, group=G, query=Q)
+        self.assertEqual(resp['result'], 'success')
+        self.assertEqual(len(resp.keys()), 9)
+        self.assertIsInstance(resp['jobKey'], str)
+        self.assertIsInstance(resp['message'], str)
+        self.assertIsInstance(resp['sourceGroup'], str)
+        self.assertIsInstance(resp['sourceList'], list)
+        self.assertIsInstance(resp['sourceQuery'], str)
+        self.assertIsInstance(resp['sourceSchema'], str)
+        self.assertIsInstance(resp['storageId'], str)
+        self.assertIsInstance(resp['storageName'], str)
+        self.assertTrue(bool(fullmatch(self.API.re_uuid4, resp['jobKey'])))
+        self.assertEqual(
+            resp['message'], 'DB Data Export job submitted. Poll job info for current job status.'
+        )
+        self.assertIsNone(resp.get('multipleFiles'))
+        self.assertEqual(resp['sourceGroup'], G)
+        self.assertEqual(resp['sourceList'], TBL)
+        self.assertEqual(resp['sourceQuery'], Q)
+        self.assertTrue(bool(fullmatch(self.API.re_uuid4, resp['storageId'])))
+        self.assertEqual(resp['storageName'], DB)
+
+        # TODO
+        # 1) poll job key status
+        # 2) download zip
+        # 3) unpack zip
+        # 4) verify meta file
+        # 5) verify content
+
     def test_database_objects(self) -> None:
         '''tables and views with stats'''
 
         self.database_ensure_exist()
         resp: Dict[str, Any] = self.API.database_objects('pg_unittest')
         self.assertEqual(resp['result'], 'success')
         self.assertIsInstance(resp['schemas'], list)
@@ -670,15 +835,22 @@
         self.assertEqual(resp['result'], 'success')
         for schema in resp['schemas']:
             self.assertIsNone(schema.get('tables'))
 
     def test_database_schemas(self) -> None:
         '''currently only anura schemas'''
 
-        ANURA_STATUS: Tuple[str, ...] = ('current', 'deprecated', 'preview', 'retired')
+        ANURA_STATUS: Tuple[str, ...] = (
+            'current',
+            'deprecated',
+            'preview',
+            'release candidate',
+            'retired',
+            'stable',
+        )
         resp = self.API.database_schemas()
         self.assertIsInstance(resp['result'], str)
         self.assertEqual(resp['result'], 'success')
         self.assertIsInstance(resp['schemas'], dict)
         self.assertEqual(len(resp), 2)
         self.assertEqual(len(resp['schemas']), 1)
         self.assertTrue(resp['schemas'].get('anura', False))
@@ -786,73 +958,409 @@
         resp = self.API.sql_query(db, QUERY_ROWS)
         rows_cleared: int = int(resp['queryResults'][0]['count'])
         self.assertEqual(rows_cleared, 0)
 
     def test_database_templates(self) -> None:
         '''empty db or anura schemas'''
 
+        # 2023-06-02
+        templates: Dict[float, Templates] = {
+            2.1: {
+                'id': 2.1,
+                'name': 'Empty Database',
+                'templateType': 'baseline',
+                'pgTemplateName': 'template1',
+                'schema': 'none',
+                'baselineSchemaVersion': '1.0',
+                'baseId': 2,
+                'templateVersion': '1.0',
+                'shortDescription': 'Database with no tables or schemas other than public.',
+                'longDescription': 'Database with no tables or schemas other than public.',
+                'isDefault': True,
+                'tags': ['Cosmic Frog'],
+                'media': [],
+            },
+            3.1: {
+                'id': 3.1,
+                'name': 'Anura New Model v2.4',
+                'templateType': 'baseline',
+                'pgTemplateName': 'anura_2_4_clean',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.4.1',
+                'baseId': 3,
+                'templateVersion': '2.4.1',
+                'shortDescription': 'Optilogic standard supply chain schema.',
+                'longDescription': 'Optilogic standard supply chain schema.',
+                'isDefault': True,
+                'tags': ['Cosmic Frog'],
+                'media': [],
+            },
+            5.1: {
+                'id': 5.1,
+                'name': 'Anura New Model v2.5',
+                'templateType': 'baseline',
+                'pgTemplateName': 'anura_2_5_clean',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.5.18',
+                'baseId': 5,
+                'templateVersion': '2.5.18',
+                'shortDescription': 'Optilogic standard supply chain schema.',
+                'longDescription': 'Optilogic standard supply chain schema.',
+                'isDefault': True,
+                'tags': ['Cosmic Frog'],
+                'media': [],
+            },
+            7.5: {
+                'id': 7.5,
+                'name': 'Anura New Model v2.6.31.3',
+                'templateType': 'baseline',
+                'pgTemplateName': 'anura_2_6_31_3_clean',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 7,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Optilogic standard supply chain schema.',
+                'longDescription': 'Optilogic standard supply chain schema.',
+                'isDefault': True,
+                'tags': ['Cosmic Frog'],
+                'media': [],
+            },
+            9.6: {
+                'id': 9.6,
+                'name': 'Global Supply Chain Strategy',
+                'templateType': 'templateSet',
+                'pgTemplateName': '45e32716-fc12-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 9,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Global network strategy that includes inbound raw material sourcing and outbound finished goods distribution.',
+                'longDescription': 'Use this database to answer global network strategy questions. Database Structure: Raw material suppliers located in Asia and Europe, production plants located in Mexico and USA, and outbound distribution to 1000+ customers in USA. Questions answered: What is our baseline as-is network? What if we increase production volume in Mexico? What if we close the Detroit DC? What if demand increases 10%? What are the financial tradeoffs between production cost, transportation cost, and fixed operating cost? What are tradeoffs between financials, service level, and risk?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Risk',
+                    'Cosmic Frog',
+                    'Network Strategy',
+                    'Sourcing Optimization',
+                    'Distribution',
+                    'Product Flow',
+                    'Risk & Resiliency',
+                ],  # OE-8191
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/IGDxhMO1zeA'}],
+            },
+            12.3: {
+                'id': 12.3,
+                'name': 'Tactical Capacity Optimization',
+                'templateType': 'templateSet',
+                'pgTemplateName': '42c32042-fc24-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 12,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Pharmaceutical manufacturer uses strategic network databaseing to support tactical daily capacity planning. Tactical capacity planning for a pharmaceutical manufacturer. Optimizing the daily storage and manufacturing plan to support vaccine production.',
+                'longDescription': 'Optimizing daily storage and manufacturing plan to support vaccine production. Pharmaceutical raw materials have unique temperature requirements and finite capacities for onsite storage. If the plant runs out of storage capacity, then offsite 3rd party storage is needed. Questions answered: If, when, and how much 3PL space will be required? How do we balance the transportation costs and external storage costs? What is the detailed storage and shipment plan? What is the optimized plan at the daily level for 180 days? What happens if a supplier fails? Can we use an alternate supplier?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Risk',
+                    'Cosmic Frog',
+                    'Network Strategy',
+                    'Capacity Planning',
+                    'Production Planning',
+                    'Risk & Resiliency',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/G0LZnkfyYlI'}],
+            },
+            15.2: {
+                'id': 15.2,
+                'name': 'Detailed Facility Selection',
+                'templateType': 'templateSet',
+                'pgTemplateName': 'b1d326f8-fc24-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 15,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Use this database for facility selection, where detailed cost and capacities are important.',
+                'longDescription': 'Detailed Facility Selection uses network optimization to determine which facilities to open and close as well as how products should flow from those facilities to the customers.  Feed the database with pre-identified candidate sites, which could be generated by Triad (Intelligent Greenfield engine) and the solver will select optimal locations from this pool of candidates.  This database is appropriate where detailed cost and capacities are important beyond what is supported in Triad.  Questions answered (used in conjunction with Triad): What is the optimal DC footprint to serve our existing customer demand? We want to open X# of short listed DCs. What are the optimal locations? I have a list of possible candidate facility locations. How many facilities should I choose? Where should they be located? Can I create a sensitivity analysis by running dozens of scenarios? What are the cost, service level, and risk tradeoffs? What is the break point where the incremental benefits of adding a new DC are outweighed by the costs?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Cosmic Frog',
+                    'Risk',
+                    'Network Strategy',
+                    'Capacity Planning',
+                    'Product Flow',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/S1XCLtmTqeY'}],
+            },
+            18.3: {
+                'id': 18.3,
+                'name': 'United States Greenfield Facility Selection',
+                'templateType': 'templateSet',
+                'pgTemplateName': '0d2017a0-fc25-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 18,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Use this database for facility selection from many automatically generated candidates, considering basic capacities, costs and service levels.',
+                'longDescription': 'The database uses the Intelligent Greenfield engine. Simply provide the database with Customers and Demand to be able to find the optimum facilities from many automatically generated candidates. You are also able to include existing facilities, basic fixed and variables costs, capacities as well as service level bands. This database is appropriate where considering high-level greenfield networks to narrow down facility selection for more detailed analysis in Neo (network optimization). Questions answered: “# cost optimized Facilities that meet a defined service level”, “# of Facilities that meet a defined service level, minimizing weighting.',
+                'isDefault': True,
+                'tags': [
+                    'Intelligent Greenfield',
+                    'Triad',
+                    'Cosmic Frog',
+                    'Greenfield',
+                    'Network Strategy',
+                    'Facility Selection',
+                    'CAPEX Planning',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/IC2cmYYHR8s'}],
+            },
+            21.2: {
+                'id': 21.2,
+                'name': 'China Exit Strategy in Asia',
+                'templateType': 'templateSet',
+                'pgTemplateName': '8540fa74-fc25-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 21,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Japan network strategy that includes inbound raw material sourcing and outbound finished goods distribution. This database focuses on overseas suppliers and potentially shifting the supply base from China to Thailand, Vietnam and local Japanese suppliers.',
+                'longDescription': 'Use this database to answer Japanese network strategy questions related to supply base. How do we adjust and respond to a supplier bottleneck? What if capacity drops at our Chinese suppliers due to COVID restrictions, port congestion, factory shutdown, or other factors? What if our Chinese suppliers go offline entirely? How does the supply base shift if we bring Thailand and Vietnam suppliers online? What are the financial, service and risk tradeoffs? Risk is a very important consideration because as we migrate from China to other countries in Asia, we reduce cost but increase risk due to political and economic stability in the other countries. Should we Exit China?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Cosmic Frog',
+                    'Risk',
+                    'Network Strategy',
+                    'Risk & Resiliency',
+                    'Sourcing Optimization',
+                    'Distribution',
+                    'Product Flow',
+                    'Japan',
+                    'Asia',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/P8oHfujEx2Y'}],
+            },
+            24.3: {
+                'id': 24.3,
+                'name': 'China Exit Risk Strategy',
+                'templateType': 'templateSet',
+                'pgTemplateName': '013464d6-fc26-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 24,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Global network strategy that includes inbound raw material sourcing and outbound finished goods distribution. This database focuses on overseas suppliers and potentially shifting the supply base from APAC to LATAM and EMEA.',
+                'longDescription': 'Use this database to answer global network strategy questions related to supply base. How do we adjust and respond to a supplier bottleneck? What if capacity drops at our Chinese suppliers due to COVID restrictions, port congestion, factory shutdown, or other factors? What if our Chinese suppliers go offline entirely? How does the supply base shift if we bring EMEA and LATAM suppliers online? What are the financial, service and risk tradeoffs? Risk is a very important consideration because as we migrate from China to LATAM, we reduce cost but increase risk due to political and economic stability in the LATAM region. Should we Exit China?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Risk',
+                    'Cosmic Frog',
+                    'Network Strategy',
+                    'Risk & Resiliency',
+                    'Sourcing Optimization',
+                    'Distribution',
+                    'Product Flow',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/EpplSGcHbEE'}],
+            },
+            27.2: {
+                'id': 27.2,
+                'name': 'Multi-Year Capacity Planning',
+                'templateType': 'templateSet',
+                'pgTemplateName': '6f94b818-fc26-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 27,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Designing the network to expand over the next 5 years in support of future demand growth. Determining the timing and location of capital expenditure (CAPEX) investments in production and distribution capacity.',
+                'longDescription': 'Use this database to answer questions about where and when to invest in additional production and distribution capacity. A European cheese manufacturer has enough capacity to serve the mature market in Western Europe today. However, the next 5 years show growth in the Eastern Europe market and inadequate capacity to support this. Questions answered: Is our current network sufficient to meet demand in the next 5 years? When and where will we run out of capacity? Where should we invest in additional Production Capacity? When should we time these investments? Where should we invest in additional Distribution Capacity? When should we bring the new DCs online? Should we close existing DC(s)? Where should we open additional DC(s)?',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Cosmic Frog',
+                    'Network Strategy',
+                    'Capacity Planning',
+                    'CAPEX Planning',
+                    'Distribution',
+                    'Product Flow',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/SESKKVbcoGk'}],
+            },
+            28.2: {
+                'id': 28.2,
+                'name': 'Fleet Size Optimization - EMEA Geo',
+                'templateType': 'templateSet',
+                'pgTemplateName': 'a7f7f15c-fc26-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 28,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Use this database to answer fleet sizing questions. This database leverages network optimization to solve the fleet size problem – how many and what type of assets are needed. Include factors such as fixed & variable transportation cost, transit time, service level, and asset capacity.',
+                'longDescription': "Use this database to solve fleet size and asset mix questions. Find out if your current fleet is optimal. Define your own asset types like 24'' truck, 48'' truck, 53'' truck, and 3PL. What is the optimal number and mix of assets needed to fulfill demand across multiple echelons in your network? Do you need to add capacity by investing in new assets for your private fleet or use a 3rd party carrier? What is the ROI of investing in additional assets for your private fleet? If your network footprint changes - like a DC closure or addition - what is the impact to your fleet? How does seasonal demand affect fleet and costs?",
+                'isDefault': True,
+                'tags': [
+                    'Fleet Sizing',
+                    'Mode Selection',
+                    'Network Strategy',
+                    'MIP',
+                    'Cosmic Frog',
+                ],
+                'media': [],
+            },
+            30.2: {
+                'id': 30.2,
+                'name': 'Fleet Size Optimization - US Geo',
+                'templateType': 'templateSet',
+                'pgTemplateName': '31409694-fc27-11ed-9e4e-a11cd8043d36',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 30,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'Use this database to answer fleet sizing questions. This database leverages network optimization to solve the fleet size problem – how many and what type of assets are needed. Include factors such as fixed & variable transportation cost, transit time, service level, and asset capacity.',
+                'longDescription': "Use this USA-centric database to solve fleet size and asset mix questions. Find out if your current fleet is optimal. Define your own asset types like 24'' truck, 48'' truck, 53'' truck, and 3PL. What is the optimal number and mix of assets needed to fulfill demand across multiple echelons in your network? Do you need to add capacity by investing in new assets for your private fleet or use a 3rd party carrier? What is the ROI of investing in additional assets for your private fleet? If your network footprint changes - like a DC closure or addition - what is the impact to your fleet? How does seasonal demand affect fleet and costs?",
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Cosmic Frog',
+                    'Fleet Sizing',
+                    'Mode Selection',
+                    'Network Strategy',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/BrUJQjhcVTQ'}],
+            },
+            31.1: {
+                'id': 31.1,
+                'name': 'Global Sustainability Analysis',
+                'templateType': 'templateSet',
+                'pgTemplateName': '414f1a0e-014c-11ee-a300-87949ad7341e',
+                'schema': 'anura',
+                'baselineSchemaVersion': '2.6.31.3',
+                'baseId': 31,
+                'templateVersion': '2.6.31.3',
+                'shortDescription': 'This sustainability model optimizes a global supply chain for a manufacturer operating production plants in China, Vietnam, and Brazil, with distribution in the USA. It focuses on achieving sustainability while considering financials, service, and risk. The model also includes recycling and landfill flows to simulate a circular supply chain.',
+                'longDescription': 'This global sustainability model features a manufacturer’s supply chain with a network of production plants in China, Vietnam, and Brazil, and outbound distribution in USA. The manufactured products could be textiles (retail) or consumer goods (CPG). In addition to balancing financials, service, and risk, the goal for this analysis is to find the most sustainable supply chain. As a next step, add recycling flows and landfill flows to model the circular supply chain.',
+                'isDefault': True,
+                'tags': [
+                    'MIP',
+                    'Cosmic Frog',
+                    'Network Strategy',
+                    'Sustainability',
+                    'Sourcing Optimization',
+                    'Risk',
+                ],
+                'media': [{'type': 'yt', 'url': 'https://youtu.be/Ivr1j1u_xuU'}],
+            },
+        }
+
         resp: Dict[str, Any] = self.API.database_templates()
         self.assertEqual(resp['result'], 'success')
         self.assertEqual(len(resp.keys()), 3)
         self.assertIsInstance(resp['count'], int)
         self.assertEqual(resp['count'], 14)
         self.assertIsInstance(resp['templates'], list)
         tcount: int = len(resp['templates'])
         self.assertEqual(tcount, 14)
         self.assertEqual(tcount, resp['count'])
         for t in resp['templates']:
             self.assertIsInstance(t, dict)
-            for k in t.keys():
-                self.assertIsInstance(k, str)
+            self.assertTrue(issubclass(type(templates[t['id']]['baseId']), type(t['baseId'])))
+            self.assertTrue(
+                issubclass(
+                    type(templates[t['id']]['baselineSchemaVersion']),
+                    type(t['baselineSchemaVersion']),
+                )
+            )
+            self.assertTrue(issubclass(type(templates[t['id']]['id']), type(t['id'])))
+            self.assertTrue(issubclass(type(templates[t['id']]['isDefault']), type(t['isDefault'])))
+            self.assertTrue(
+                issubclass(type(templates[t['id']]['longDescription']), type(t['longDescription']))
+            )
+            self.assertTrue(issubclass(type(templates[t['id']]['media']), type(t['media'])))
+            self.assertTrue(issubclass(type(templates[t['id']]['name']), type(t['name'])))
+            self.assertTrue(
+                issubclass(type(templates[t['id']]['pgTemplateName']), type(t['pgTemplateName']))
+            )
+            self.assertTrue(issubclass(type(templates[t['id']]['schema']), type(t['schema'])))
+            self.assertTrue(
+                issubclass(
+                    type(templates[t['id']]['shortDescription']), type(t['shortDescription'])
+                )
+            )
+            self.assertTrue(issubclass(type(templates[t['id']]['tags']), type(t['tags'])))
+            self.assertTrue(
+                issubclass(type(templates[t['id']]['templateType']), type(t['templateType']))
+            )
+            self.assertTrue(issubclass(type(templates[t['id']]['baseId']), type(t['baseId'])))
+            self.assertEqual(templates[t['id']]['baseId'], t['baseId'])
+            self.assertEqual(
+                templates[t['id']]['baselineSchemaVersion'], t['baselineSchemaVersion']
+            )
+            self.assertEqual(templates[t['id']]['id'], t['id'])
+            self.assertEqual(templates[t['id']]['isDefault'], t['isDefault'])
+            self.assertEqual(templates[t['id']]['longDescription'], t['longDescription'])
+            self.assertEqual(templates[t['id']]['media'], t['media'])
+            self.assertEqual(templates[t['id']]['name'], t['name'])
+            self.assertEqual(templates[t['id']]['pgTemplateName'], t['pgTemplateName'])
+            self.assertEqual(templates[t['id']]['schema'], t['schema'])
+            self.assertEqual(templates[t['id']]['shortDescription'], t['shortDescription'])
+            if t['id'] != 9.6:
+                # OE-8191 db # 9.6 tags are missing
+                self.assertEqual(templates[t['id']]['tags'], t['tags'])
+            self.assertEqual(templates[t['id']]['templateType'], t['templateType'])
+            self.assertEqual(templates[t['id']]['baseId'], t['baseId'])
+
+    def test_database_templates_by_name(self) -> None:
+        '''look up the database template id by case-insensitive template name'''
+
+        template_names: List[str] = [t['name'] for t in self.API.DATABASE_TEMPLATES_NEW]
+
+        for name in template_names:
+            tids: List[str] = self.API._database_templates_by_name(name)
+            self.assertEqual(len(tids), 1)
+            tids = self.API._database_templates_by_name(name[5:], wildcard=True)
+            self.assertEqual(len(tids), 1)
 
     def test_database_templates_legacy(self) -> None:
         '''legacy empty db or anura schemas'''
 
         resp: Dict[str, Any] = self.API._database_templates_legacy()
         self.assertEqual(resp['result'], 'success')
         self.assertIsInstance(resp['count'], int)
-        self.assertEqual(resp['count'], 15)  # TODO OE-7816
+        self.assertEqual(resp['count'], 14)
         self.assertIsInstance(resp['templates'], list)
         tcount: int = len(resp['templates'])
-        self.assertEqual(tcount, 15)
+        self.assertEqual(tcount, 14)
         self.assertEqual(tcount, resp['count'])
-        self.assertEqual(tcount, len(self.API.DATABASE_TEMPLATES) + 1)  # TODO OE-7816
+        self.assertEqual(tcount, len(self.API.DATABASE_TEMPLATES))
 
         TEMPLATE_KEYS: Tuple[str, ...] = ('id', 'is_default', 'name', 'role', 'schema')
         for t in resp['templates']:
             self.assertIsInstance(t, dict)
             for k in t.keys():
                 self.assertIsInstance(k, str)
-            keys = tuple(sorted(t.keys()))
-            # self.assertEqual(keys, TEMPLATE_KEYS) # TODO OE-7816
-            # if t['name'] in ('Empty Database', 'Blast Off To Space (BOTS)', 'Global Risk Analysis'):
-            #    continue  # OE-7918 legacy call changed
-            # self.assertTrue(t['id'] in self.API.DATABASE_TEMPLATES)
+                self.assertIn(t['id'], self.API.DATABASE_TEMPLATES)
 
     def test_database_templates_legacy_by_name(self) -> None:
         '''look up the database template id by case-insensitive template name'''
 
-        template_names: List[str] = [
-            'empty',
-            'Anura - Blast off to Space',
-            'Anura - New Model',
-            'Anura - New Model (2.6)',
-            'China Exit Strategy in Asia',
-            'Detailed Facility Selection',
-            'Fleet Size Optimization - EMEA Geo',
-            'Fleet Size Optimization - US Geo',
-            'Greenfield Facility Selection',
-            'Multi-Year Capacity Planning',
-            'Out of China',
-            'Tactical Capacity Optimization',
-        ]
+        template_names: List[str] = [k for k in self.API.DATABASE_TEMPLATES_NAMEID.keys()]
 
         for name in template_names:
             tids: List[str] = self.API._database_templates_legacy_by_name(name)
             self.assertEqual(len(tids), 1)
+            self.assertEqual(tids[0], self.API.DATABASE_TEMPLATES_NAMEID[name])
+            tids = self.API._database_templates_legacy_by_name(name[5:], wildcard=True)
+            if name == 'Anura New Model v2.6':
+                self.assertEqual(len(tids), 2)
+            else:
+                self.assertEqual(len(tids), 1)
 
     def test_ip_address_allow(self) -> None:
         '''whitelist ip address'''
 
         self.database_ensure_exist()
         db: Dict[str, Any] = self.API.account_storage_device(type='postgres_db')
         resp: Dict[str, str] = self.API.ip_address_allow(database_name=db['name'], ip='127.0.0.0')
@@ -1136,46 +1644,45 @@
         devices = self.API.account_storage_devices()
         self.assertEqual(devices['result'], 'success')
         with self.subTest():
             for device in devices['storages']:
                 d: Dict[str, Any] = self.API.storage(device['name'])
                 self.assertEqual(d['result'], 'success')
                 if d['type'] == 'azure_afs':
-                    self.assertEqual(len(d), 12)
+                    self.assertEqual(len(d), 16)
                     self.storage_azure_afs(d)
                 if d['type'] == 'azure_workspace':
                     self.assertEqual(len(d), 17)
                     self.storage_azure_workspace(d)
                 elif d['type'] == 'onedrive':
                     self.assertEqual(len(d), 24)
                     self.storage_onedrive(d)
                     # connect is not in get devices call due to real time performance
                     self.assertIsInstance(d['connected'], bool)
                 elif d['type'] == 'postgres_db':
                     # storage item contains an additional result key
-                    self.assertEqual(len(d), 23)
+                    self.assertEqual(len(d), 24)
                     self.storage_database(d)
 
     def test_storage_attr(self) -> None:
         '''device attributes: annotations, label, and tag'''
 
-        attrs: Tuple[Literal['annotation'], Literal['label'], Literal['tag']] = (
-            'annotation',
-            'label',
-            'tag',
+        attrs: Tuple[Literal['annotations'], Literal['labels'], Literal['tags']] = (
+            'annotations',
+            'labels',
+            'tags',
         )
         devices: Dict[str, Any] = self.API.account_storage_devices()
         self.assertEqual(devices['result'], 'success')
         with self.subTest():
             for d in devices['storages']:
                 for a in attrs:
                     resp: Dict[str, Any] = self.API._storage_attr(d['name'], a)
                     self.assertEqual(resp['result'], 'success')
                     self.assertEqual(len(resp.keys()), 2)
-                    a += 's'  #  BUG PR-924 route vs attribute is not the same
                     self.assertTrue(a in resp.keys())
                     if a == 'tags':
                         self.assertIsInstance(resp[a], str)
                     else:
                         self.assertIsInstance(resp[a], dict)
 
     @unittest.skip('api has not implemented')
@@ -1237,15 +1744,15 @@
         # valid but job key does not exist
         resp: bool = self.API.util_job_monitor(self.WKSP, '00000000-0000-0000-0000-000000000000')
         self.assertFalse(resp)
 
     def test_wksp_file_copy(self) -> None:
         '''make a copy of a file within a workspace'''
 
-        src: str = self.py_run_me
+        src: str = self.py_sleep
         dest: str = f'{self.dir_testdata_remote}/cp_test.txt'
         resp = self.API.wksp_file_copy(
             self.WKSP, file_path_src=src, file_path_dest=dest, overwrite=True
         )
         self.assertEqual(resp['result'], 'success')
         self.assertEqual(resp['copyStatus'], 'success')
         self.assertEqual(resp['message'], 'Copy complete')
@@ -1267,15 +1774,15 @@
         self.assertEqual(resp['message'], 'File deleted')
         file_result = f"{resp['fileInfo']['directoryPath']}/{resp['fileInfo']['filename']}"
         self.assertEqual(f, file_result)
 
     def test_wksp_file_download(self) -> None:
         '''download a file from a given workspace'''
 
-        download = self.API.wksp_file_download(self.WKSP, file_path=self.py_run_me)
+        download = self.API.wksp_file_download(self.WKSP, file_path=self.py_sleep)
         self.assertGreaterEqual(len(download), 1)
         self.assertIsInstance(download, str)
 
     def test_wksp_file_download_crash(self) -> None:
         '''download a file from a given workspace'''
 
         resp: str = self.API.wksp_file_download(self.WKSP, file_path='does_not_exist')
@@ -1284,15 +1791,15 @@
         self.assertEqual(r['result'], 'error')
         self.assertIsInstance(r['error'], str)
         self.assertEqual(len(r['correlationId']), 36)
 
     def test_wksp_file_download_meta(self) -> None:
         '''file metadata'''
 
-        resp = self.API.wksp_file_download_status(self.WKSP, file_path=self.py_run_me)
+        resp = self.API.wksp_file_download_status(self.WKSP, file_path=self.py_sleep)
         self.assertEqual(resp['result'], 'success')
         keys: Tuple[str, ...] = (
             'result',
             'workspace',
             'filename',
             'directoryPath',
             'filePath',
@@ -1301,15 +1808,15 @@
             'date',
             'fileCreatedOn',
             'fileLastWriteOn',
             'fileChangeOn',
         )
         for key in resp.keys():
             self.assertIn(key, keys)
-        self.assertEqual(resp['filePath'], self.py_run_me)
+        self.assertEqual(resp['filePath'], self.py_sleep)
         self.assertEqual(resp['workspace'], self.WKSP)
         self.assertIsInstance(resp['contentLength'], int)
         dt: datetime = parse(resp['lastModified'])
         self.assertEqual(dt.tzname(), 'UTC')
 
     def test_wksp_file_upload(self) -> None:
         '''upload a file to a workspace'''
@@ -1534,32 +2041,41 @@
             self.assertEqual(len(err['correlationId']), 36)
         else:
             self.assertGreater(len(resp), 0)
 
     def test_wksp_job_ledger(self) -> None:
         '''get job ledger that has realtime messages'''
 
-        if len(self.__jobkey_quick) == 0:
-            self.job_prereq()
-        resp = self.API.wksp_job_ledger(self.WKSP, self.__jobkey_quick)
+        job = self.API.wksp_job_start(
+            self.WKSP, self.py_sidecar, resourceConfig='mini', tags='unittest'
+        )
+        res: bool = self.API.util_job_monitor(self.WKSP, job['jobKey'], stop_when='done')
+        self.assertTrue(res)
+        resp = self.API.wksp_job_ledger(self.WKSP, job['jobKey'])
         self.assertEqual(resp['result'], 'success')
         self.assertIsInstance(resp['count'], int)
         self.assertGreaterEqual(resp['count'], 1)
         self.assertIsInstance(resp['records'], list)
         self.assertGreaterEqual(len(resp['records']), 1)
-        self.assertIsInstance(resp['records'][0]['timestamp'], int)
-        self.assertIsInstance(resp['records'][0]['datetime'], str)
-        # job was created during init, assert same day
-        self.assertTrue(resp['records'][0]['datetime'].endswith('Z'))
-        dt: datetime = parse(resp['records'][0]['datetime'])
-        self.assertTrue(dt.tzname(), 'UTC')
-        now: datetime = datetime.utcnow()
-        self.assertEqual(dt.year, now.year)
-        self.assertEqual(dt.month, now.month)
-        self.assertEqual(dt.day, now.day)
+        for r in resp['records']:
+            self.assertIsInstance(r['timestamp'], int)
+            self.assertIsInstance(r['datetime'], str)
+            # job was created during init, assert same day
+            self.assertTrue(r['datetime'].endswith('Z'))
+            dt: datetime = parse(r['datetime'])
+            self.assertTrue(dt.tzname(), 'UTC')
+            now: datetime = datetime.utcnow()
+            self.assertEqual(dt.year, now.year)
+            self.assertEqual(dt.month, now.month)
+            self.assertEqual(dt.day, now.day)
+            self.assertIsInstance(r['key'], str)
+            self.assertIsInstance(r['message'], str)
+            self.assertIn(r['key'], ('eta', 'type', '96k'))
+            if r['key'] == '96k':
+                self.assertEqual(len(r['message']), 32_000)  # OE-8083 truncate
 
     def test_wksp_job_metrics(self) -> None:
         '''get one second cpu and memory sampling of a job'''
 
         if len(self.__jobkey_quick) == 0:
             self.job_prereq()
         resp = self.API.wksp_job_metrics(self.WKSP, self.__jobkey_quick)
@@ -1622,20 +2138,20 @@
         jobs_max: int = 9
         tag_time: float = time.time()
         tag: str = f'metrics_{tag_time}'
         secs: int = 20
         d: dict = {}  # store job key and elapsed time without metrics
         for job in range(jobs_max):
             resp = self.API.wksp_job_start(
-                self.WKSP, self.py_run_me, tags=tag, timeout=secs, resourceConfig='mini'
+                self.WKSP, self.py_sleep, tags=tag, timeout=secs, resourceConfig='mini'
             )
             if resp.get('crash'):
                 print(resp)
                 jobs_max -= 1
-                continue  
+                continue
             d[resp['jobKey']] = {'seen_first': None, 'missing_last': None}
 
         # check the jobs that are about to run
         metrics_missing = False
         check: bool = True
         while check:
             # stop if all jobs finished
@@ -1681,15 +2197,15 @@
             for item in d.items():
                 print(item)
 
     def test_wksp_job_start(self) -> None:
         '''creating a job'''
 
         resp = self.API.wksp_job_start(
-            self.WKSP, file_path=self.py_run_me, tags='unittest_start', resourceConfig='mini'
+            self.WKSP, file_path=self.py_sleep, tags='unittest_start', resourceConfig='mini'
         )
         self.assertEqual(resp['result'], 'success')
         self.assertEqual(len(resp['jobKey']), 36)
         job_info_keys: Tuple[str, ...] = (
             'workspace',
             'directoryPath',
             'filename',
@@ -1702,25 +2218,25 @@
             self.assertIn(key, job_info_keys)
 
     def test_wksp_job_start_preview(self) -> None:
         '''create a job using andromeda preview image and compare to stable'''
 
         job_beta: Dict[str, Any] = self.API.wksp_job_start(
             self.WKSP,
-            file_path=self.py_run_me_bash,
+            file_path=self.py_bash,
             commandArgs="'pip list -v'",
             resourceConfig='mini',
             tags='unittest',
             preview_image=True,
         )
         self.assertEqual(job_beta['result'], 'success')
 
         job: Dict[str, Any] = self.API.wksp_job_start(
             self.WKSP,
-            file_path=self.py_run_me_bash,
+            file_path=self.py_bash,
             commandArgs="'pip list -v'",
             resourceConfig='mini',
             tags='unittest',
             preview_image=False,
         )
         self.assertEqual(job['result'], 'success')
 
@@ -1736,32 +2252,30 @@
         done = self.API.util_job_monitor(self.WKSP, job_key=job['jobKey'], stop_when='done')
         self.assertTrue(done)
         std_out: str = self.API.wksp_job_file_result(self.WKSP, job['jobKey'])
         self.assertIsInstance(std_out, str)
         self.assertGreater(len(std_out), 100)
         m = search(r'(?P<pkg>neo)\s+(?P<ver>[\w\.]+)', std_out)
         version: str = m.groupdict()['ver'] if m else ''
-        self.assertRegex(version, r'2\.5\.\d+')
-
-        self.assertNotEqual(version, version_preview)
+        self.assertRegex(version, r'2\.[6-9]\.\d+')
 
     def test_wksp_job_start_sample(self) -> None:
         '''create job api call reponse time is the slowest and fails often withg 504s'''
 
         max: int = int(self.API.account_info()['limits']['concurrentJobs'] * 0.5)
         min: int = 10
         job_count: int = max if max > min else min
         jobs: List[str] = []
         tag: str = 'unittest_job_speed'
 
         # start jobs
         for j in range(job_count):
             with self.subTest():
                 resp = self.API.wksp_job_start(
-                    self.WKSP, self.py_run_me_quick, tags=tag, resourceConfig='mini'
+                    self.WKSP, self.py_quick, tags=tag, resourceConfig='mini'
                 )
                 self.assertEqual(resp['result'], 'success')
             # d = {}
             # d['key'] = resp['jobKey']
             # jobs.append(d)
             # spin up a few jobs to create load and evaluate all
 
@@ -1772,15 +2286,15 @@
         max: int = jobs_max - jobs_active if jobs_max > jobs_active else 0
 
         jobs_max: int = 9
         tag_time: float = time.time()
         tag: str = f'unittest_job_sample_{tag_time}'
 
         for job in range(jobs_max):
-            self.API.wksp_job_start(self.WKSP, self.py_run_me, tags=tag)
+            self.API.wksp_job_start(self.WKSP, self.py_sleep, tags=tag)
 
         # check the jobs that are about to run
         d: dict = {}
         check: bool = True
         while check:
             jobs = self.API.wksp_jobs(self.WKSP, tags=tag)
 
@@ -1868,15 +2382,15 @@
 
     def test_wksp_job_stop(self) -> None:
         '''stop a most recently created job'''
 
         # guarantee a job is currently running
         resp = self.API.wksp_job_status(self.WKSP, self.API._job_start_recent_key)
         if resp['status'] in self.API.JOBSTATES_TERMINAL:
-            resp = self.API.wksp_job_start(self.WKSP, self.py_run_me, resourceConfig='mini')
+            resp = self.API.wksp_job_start(self.WKSP, self.py_sleep, resourceConfig='mini')
             success: bool = self.API.util_job_monitor(self.WKSP, resp['jobKey'])
             if success is False:
                 self.skipTest('failed to start job within two minutes')
 
         # stop running job
         resp = self.API.wksp_job_stop(self.WKSP, self.API._job_start_recent_key)
         self.assertEqual(resp['result'], 'success')
@@ -2013,15 +2527,15 @@
     def test_wksp_share_file(self) -> None:
         '''share a file from a workspace to all other workspaces of a user/self'''
 
         if self.API.auth_username is None:
             self.skipTest('test_wksp_share_folder requires a username')
 
         resp = self.API.wksp_share_file(
-            self.WKSP, file_path=self.py_run_me, targetUsers=self.API.auth_username
+            self.WKSP, file_path=self.py_sleep, targetUsers=self.API.auth_username
         )
         self.assertEqual(resp['result'], 'success')
         self.assertEqual(len(resp.keys()), 8)
         self.assertIsInstance(resp['errored'], list)
         self.assertEqual(len(resp['errored']), 0)
         self.assertIsInstance(resp['erroredCount'], int)
         self.assertIsInstance(resp['jobs'], list)
@@ -2032,17 +2546,17 @@
             self.assertEqual(j['result'], 'success')
         self.assertEqual(resp['jobsCount'], self.API.account_workspace_count - 1)
         self.assertIsInstance(resp['message'], str)
         self.assertEqual(resp['message'], 'Share Accepted')
         self.assertIsInstance(resp['sourceFileInfo'], dict)
         self.assertEqual(len(resp['sourceFileInfo'].keys()), 2)
         self.assertIsInstance(resp['sourceFileInfo']['directoryPath'], str)
-        self.assertEqual(resp['sourceFileInfo']['directoryPath'], os.path.split(self.py_run_me)[0])
+        self.assertEqual(resp['sourceFileInfo']['directoryPath'], os.path.split(self.py_sleep)[0])
         self.assertIsInstance(resp['sourceFileInfo']['filename'], str)
-        self.assertEqual(resp['sourceFileInfo']['filename'], os.path.split(self.py_run_me)[1])
+        self.assertEqual(resp['sourceFileInfo']['filename'], os.path.split(self.py_sleep)[1])
         self.assertEqual(resp['targetUsers'], self.API.auth_username)
 
     def test_wksp_share_file_sample(self) -> None:
         '''OE-5840 API Share File/Folder Results in 500 Internal Server Error'''
 
         if self.API.auth_username is None:
             self.skipTest('test_wksp_share_folder requires a username')
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `optilogic-2.5.0.dist-info/LICENSE` & `optilogic-2.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `optilogic-2.5.0.dist-info/METADATA` & `optilogic-2.6.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optilogic
-Version: 2.5.0
+Version: 2.6.0
 Summary: Tools for interfacing with Optilogic Jobs and APIs
 Home-page: https://optilogic.com
 Author: Optilogic
 Author-email: support@optilogic.com
 License: MIT
 Project-URL: Documentation, https://api-docs.optilogic.app/documentation
 Keywords: mip,mixed integer programming,network optimization,optimization,risk,simulation,supply chain design
```

## Comparing `optilogic-2.5.0.dist-info/RECORD` & `optilogic-2.6.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 optilogic/__init__.py,sha256=t3hXtM_MyajzEyk-V1xxM1ZzFZCZtADNjJvvShxdl4A,22
 optilogic/pioneer/__init__.py,sha256=ELVJEdWM5Ia28-LjwVes2qvd7nGkORgVOw0g21vsGPU,48
 optilogic/pioneer/api/__init__.py,sha256=kaCK0y1h6dN5NhQnehgpJCEwyihVDPuuQ7xgtexVric,20
-optilogic/pioneer/api/api.py,sha256=LWCVnQP_lsPR_i5MiIPtYiqDrIcy-Ez3BJ9H8BwIlEA,72496
-optilogic/pioneer/api/api_tests.py,sha256=cl_GE9gAgv8Yg2UgWMgxZEHfNCGiZHuHYiMA_lDIfxI,96477
+optilogic/pioneer/api/api.py,sha256=DHKOUGE0eQ24qGCGmHRL_CkZy9ud9WTO80oDo9vMZDA,74338
+optilogic/pioneer/api/api_tests.py,sha256=wJZAJ07B7dTWg03KgCYxRyoIz7ab-dKQAlugWItCIcc,126839
 optilogic/pioneer/api/quick_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 optilogic/pioneer/api/quick_tests/airline_hub_location_cbc.py,sha256=S6nxwIvWFqBo1tsFRi0D9VBD8ohBDhb42aBzXkKNgw4,5111
 optilogic/pioneer/api/quick_tests/bash.py,sha256=WPnbdoPVGxOwdMlsk-IyxVWeqXae5DbdN2bpMzNgVCQ,317
 optilogic/pioneer/api/quick_tests/quick.py,sha256=Yf_jhZbx5Nx5W3Dc_iJz8t70KvMDBn7xVTMmNvBn5gM,209
+optilogic/pioneer/api/quick_tests/sidecar.py,sha256=qPCpK-tD0rIs_UBfhrieya9BIaZRB_6HZG8b1qQxTR0,726
 optilogic/pioneer/api/quick_tests/sleep.py,sha256=CSb8T0inq6NAlDqW321vFCBmldPIiiGWfAU98OwUmV4,577
 optilogic/pioneer/job_utils/__init__.py,sha256=ewS513f69vgJB7L8QZIYtwl6umBFDtOqM52Ms0pAzy4,131
 optilogic/pioneer/job_utils/job_utils.py,sha256=nBeFlkmqXjiNQub-i962qk64c-M2QCMjQvLLv5fuv6U,3553
-optilogic-2.5.0.dist-info/LICENSE,sha256=BfGwbupGKO-1uV11X7aBMgE3LCjo5N7OxqZpMFhP7ls,1070
-optilogic-2.5.0.dist-info/METADATA,sha256=0-vMNZbFP8ryF_r9x7fDKMtO5tlhB0mT9lAXjBs7m7U,759
-optilogic-2.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-optilogic-2.5.0.dist-info/top_level.txt,sha256=A59vwR2Gu9fxXluO4gG-COTlfSKCJW910611UXOwnuo,10
-optilogic-2.5.0.dist-info/RECORD,,
+optilogic-2.6.0.dist-info/LICENSE,sha256=BfGwbupGKO-1uV11X7aBMgE3LCjo5N7OxqZpMFhP7ls,1070
+optilogic-2.6.0.dist-info/METADATA,sha256=JxYcAE8OtURukYUFg141OWPoIvfhiQekpHtoyGN-QVM,759
+optilogic-2.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+optilogic-2.6.0.dist-info/top_level.txt,sha256=A59vwR2Gu9fxXluO4gG-COTlfSKCJW910611UXOwnuo,10
+optilogic-2.6.0.dist-info/RECORD,,
```

