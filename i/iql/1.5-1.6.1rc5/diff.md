# Comparing `tmp/iql-1.5-py3-none-any.whl.zip` & `tmp/iql-1.6.1rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,29 @@
-Zip file size: 48099 bytes, number of entries: 25
--rw-r--r--  2.0 unx      391 b- defN 23-May-10 20:03 iql/__init__.py
--rw-r--r--  2.0 unx       99 b- defN 23-May-10 20:04 iql/_version.py
--rw-r--r--  2.0 unx    34989 b- defN 23-May-10 20:03 iql/iqmoql.py
--rw-r--r--  2.0 unx     1282 b- defN 23-May-10 20:03 iql/options_parser.py
--rw-r--r--  2.0 unx     3233 b- defN 23-May-10 20:03 iql/q_cache.py
--rw-r--r--  2.0 unx     2191 b- defN 23-May-10 20:03 iql/threading_experimental.py
--rw-r--r--  2.0 unx       77 b- defN 23-May-10 20:03 iql/bbg_bql/__init__.py
--rw-r--r--  2.0 unx    10069 b- defN 23-May-10 20:03 iql/bbg_bql/bql_datamodel.py
--rw-r--r--  2.0 unx     9162 b- defN 23-May-10 20:03 iql/bbg_bql/bql_extension.py
--rw-r--r--  2.0 unx    14310 b- defN 23-May-10 20:03 iql/bbg_bql/bql_wrapper.py
--rw-r--r--  2.0 unx      692 b- defN 23-May-10 20:03 iql/bbg_bql/debug_tools.py
--rw-r--r--  2.0 unx       77 b- defN 23-May-10 20:03 iql/db_connectors/__init__.py
--rw-r--r--  2.0 unx     4795 b- defN 23-May-10 20:03 iql/db_connectors/duckdb_connector.py
--rw-r--r--  2.0 unx       77 b- defN 23-May-10 20:03 iql/extensions/__init__.py
--rw-r--r--  2.0 unx     3470 b- defN 23-May-10 20:03 iql/extensions/aws_s3_extension.py
--rw-r--r--  2.0 unx     7829 b- defN 23-May-10 20:03 iql/extensions/edgar_extension.py
--rw-r--r--  2.0 unx     4279 b- defN 23-May-10 20:03 iql/extensions/fred_extension.py
--rw-r--r--  2.0 unx     4106 b- defN 23-May-10 20:03 iql/extensions/kaggle_extension.py
--rw-r--r--  2.0 unx     2495 b- defN 23-May-10 20:03 iql/extensions/pandas_extension.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-10 20:03 iql/extensions/template_extension.py
--rw-r--r--  2.0 unx      535 b- defN 23-May-10 20:04 iql-1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    27294 b- defN 23-May-10 20:04 iql-1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 20:04 iql-1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-10 20:04 iql-1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2020 b- defN 23-May-10 20:04 iql-1.5.dist-info/RECORD
-25 files, 134234 bytes uncompressed, 44853 bytes compressed:  66.6%
+Zip file size: 48598 bytes, number of entries: 27
+-rw-r--r--  2.0 unx      327 b- defN 23-Jun-03 19:08 iql/__init__.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-03 19:08 iql/_version.py
+-rw-r--r--  2.0 unx    34190 b- defN 23-Jun-03 19:08 iql/iqmoql.py
+-rw-r--r--  2.0 unx     1282 b- defN 23-Jun-03 19:08 iql/options_parser.py
+-rw-r--r--  2.0 unx      432 b- defN 23-Jun-03 19:08 iql/q_cache_base.py
+-rw-r--r--  2.0 unx     2191 b- defN 23-Jun-03 19:08 iql/threading_experimental.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-03 19:08 iql/bbg_bql/__init__.py
+-rw-r--r--  2.0 unx    10069 b- defN 23-Jun-03 19:08 iql/bbg_bql/bql_datamodel.py
+-rw-r--r--  2.0 unx     9377 b- defN 23-Jun-03 19:08 iql/bbg_bql/bql_extension.py
+-rw-r--r--  2.0 unx    14633 b- defN 23-Jun-03 19:08 iql/bbg_bql/bql_wrapper.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Jun-03 19:08 iql/bbg_bql/debug_tools.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-03 19:08 iql/db_connectors/__init__.py
+-rw-r--r--  2.0 unx     5109 b- defN 23-Jun-03 19:08 iql/db_connectors/duckdb_connector.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-03 19:08 iql/extensions/__init__.py
+-rw-r--r--  2.0 unx     3407 b- defN 23-Jun-03 19:08 iql/extensions/aws_s3_extension.py
+-rw-r--r--  2.0 unx     7829 b- defN 23-Jun-03 19:08 iql/extensions/edgar_extension.py
+-rw-r--r--  2.0 unx     4279 b- defN 23-Jun-03 19:08 iql/extensions/fred_extension.py
+-rw-r--r--  2.0 unx     4106 b- defN 23-Jun-03 19:08 iql/extensions/kaggle_extension.py
+-rw-r--r--  2.0 unx     2495 b- defN 23-Jun-03 19:08 iql/extensions/pandas_extension.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jun-03 19:08 iql/extensions/template_extension.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-03 19:08 iql/jupyter_magics/__init__.py
+-rw-r--r--  2.0 unx     4131 b- defN 23-Jun-03 19:08 iql/jupyter_magics/iql_magic.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Jun-03 19:09 iql-1.6.1rc5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    25594 b- defN 23-Jun-03 19:09 iql-1.6.1rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 19:09 iql-1.6.1rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-03 19:09 iql-1.6.1rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2223 b- defN 23-Jun-03 19:09 iql-1.6.1rc5.dist-info/RECORD
+27 files, 134075 bytes uncompressed, 45018 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -6,15 +6,15 @@
 
 Filename: iql/iqmoql.py
 Comment: 
 
 Filename: iql/options_parser.py
 Comment: 
 
-Filename: iql/q_cache.py
+Filename: iql/q_cache_base.py
 Comment: 
 
 Filename: iql/threading_experimental.py
 Comment: 
 
 Filename: iql/bbg_bql/__init__.py
 Comment: 
@@ -54,23 +54,29 @@
 
 Filename: iql/extensions/pandas_extension.py
 Comment: 
 
 Filename: iql/extensions/template_extension.py
 Comment: 
 
-Filename: iql-1.5.dist-info/LICENSE
+Filename: iql/jupyter_magics/__init__.py
 Comment: 
 
-Filename: iql-1.5.dist-info/METADATA
+Filename: iql/jupyter_magics/iql_magic.py
 Comment: 
 
-Filename: iql-1.5.dist-info/WHEEL
+Filename: iql-1.6.1rc5.dist-info/LICENSE
 Comment: 
 
-Filename: iql-1.5.dist-info/top_level.txt
+Filename: iql-1.6.1rc5.dist-info/METADATA
 Comment: 
 
-Filename: iql-1.5.dist-info/RECORD
+Filename: iql-1.6.1rc5.dist-info/WHEEL
+Comment: 
+
+Filename: iql-1.6.1rc5.dist-info/top_level.txt
+Comment: 
+
+Filename: iql-1.6.1rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iql/__init__.py

```diff
@@ -1,19 +1,15 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
-from multiprocessing import Process, log_to_stderr
 
+from iql._version import __version__
 from iql.iqmoql import (
+    configure,
     execute,
     execute_debug,
-    configure,
     get_extension,
     list_extensions,
     register_extension,
+    get_cache,
+    set_cache,
 )
-from iql.q_cache import clear_caches
-
-from iql._version import __version__
-
-# import logging
-
-# log_to_stderr(logging.INFO)
+from iql.q_cache_base import QueryCacheBase
```

## iql/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__="1.5"
-__commit__="fec839f1f96aaf863b7269a2781f792e528afe6a"
-__commit_short__="fec839f"
+__version__="1.6.1rc5"
+__commit__="9da217d9424abae4800939d18b5da6a420e49c14"
+__commit_short__="9da217d"
```

## iql/iqmoql.py

```diff
@@ -1,57 +1,59 @@
 # Copyright (C) 2023, IQMO Corporation [info@iqmo.com]
 # All Rights Reserved
 
 import logging
 import sqlparse
 import importlib
-import os
 import re
 from dataclasses import dataclass, field
 from typing import List, Dict, Optional, Union, Tuple, Callable
 from pandas import DataFrame
 import pandas as pd
 from abc import abstractmethod
-from iql import q_cache as qc
+from iql.q_cache_base import QueryCacheBase
 from iql import options_parser
 from iql import threading_experimental as te
 
 
 # Cache Settings
 # Use iqmoql.activate_cache() before first execute() to
 # ensure settings propogate to individual extensions.
 # Infinite in memory cache by default
-_CACHE_PERIOD = -1
-_USE_FILE_CACHE = False
+
 DEFAULT_EXT_DIRECTORY = None
 
 # DB_MODULE is loaded on first call to get_dbmodule()
 # Replace this string with another connector prior to first use,
 # or set _DBCONNECTOR to None after changing.
 DB_MODULE: str = "iql.db_connectors.duckdb_connector"
 
 _EXTENSIONS: Dict[Tuple[str, str], "IqlExtension"] = {}
 _DBCONNECTOR: Optional["IqlDatabaseConnector"] = None
 
 # Used internally to name the dataframes
 _DFPREFIX: str = "iqldf"
 
+CACHE = QueryCacheBase()
+
 # Add extensions via register_extension()
 # Extensions are loaded on first access, to avoid requiring
 # unused dependencies
 _KNOWN_EXTENSIONS: Dict[str, str] = {
     "bql": "iql.bbg_bql.bql_extension",
     "s3": "iql.extensions.aws_s3_extension",
     "fred": "iql.extensions.fred_extension",
     "kaggle": "iql.extensions.kaggle_extension",
     "edgar": "iql.extensions.edgar_extension",
     "pandas": "iql.extensions.pandas_extension",
 }
 
-_ALIASES: Dict[str, str] = {}
+_ALIASES: Dict[
+    str, Callable[[], str]
+] = {}  # Callable, so we can either use text or external files
 
 logger = logging.getLogger(__name__)
 
 
 def _find_closing_paren(text: str, start: int) -> int:
     # TODO: Handle escaping
     paren_depth = 1
@@ -196,51 +198,34 @@
     # implement their own execute_batch.
     # Can only contain pickleable elements
     # etc
 
     # Determines whether the local cache settings should be used
     # vs  CACHE_PERIOD and
     # USE_FILE_CACHE
-    use_default_caching: bool = field(default=True, init=False)
-    _cache_period: Optional[int] = field(default=None, init=False)
-    _use_file_cache: bool = field(default=False, init=False)
     temp_file_directory: Optional[str] = field(default=None, init=False)
 
     def get_output_dir(self) -> str:
         tempdir = (
             self.temp_file_directory if self.temp_file_directory is not None else "./"
         )
         return tempdir
 
     def allow_cache_read(self, sq: "SubQuery") -> bool:
         """Dont use cached values"""
         if sq.options.get("nocache") is True:
             return False
         elif sq.options.get("cache") is not None:
             return True
-        elif self.get_cache_period() is None:
-            return False
         else:
             return True
 
     def allow_cache_save(self, sq: "SubQuery") -> bool:
         return self.allow_cache_read(sq)
 
-    def get_cache_period(self) -> Optional[int]:
-        if self.use_default_caching:
-            return _CACHE_PERIOD
-        else:
-            return self._cache_period
-
-    def use_file_cache(self) -> bool:
-        if self.use_default_caching:
-            return _USE_FILE_CACHE
-        else:
-            return self._use_file_cache
-
     def use_path_replacement(self) -> bool:
         """Some extensions just return a filestring to use instead of the SubQuery, such as the
         S3 Extension. If execute() returns None, then use_path_replacement must be used.
         """
         return False
 
     def get_path_replacement(
@@ -408,15 +393,15 @@
 
             if not parameter_name.startswith("$"):
                 logger.debug("Parameter name doesn't start with $, inserting one")
                 # This is helpful to avoid replacing the paramquery when substituting
                 parameter_name = f"${parameter_name}"
 
             for v in parameter_values:
-                v_query = query.replace(parameter_name, v)
+                v_query = query.replace(parameter_name, str(v))
 
                 sq = create_function(  # type: ignore
                     subquery=v_query, name=f"{name}_{count}", iqc=iqc
                 )
 
                 sqs.append(sq)
                 count += 1
@@ -663,49 +648,31 @@
         """Returns cached value if it's available"""
         cache_val = self.subquery
 
         logger.debug(f"Checking cache for {cache_val}, {type(self)}")
         if not self.extension.allow_cache_read(self):
             return False
 
-        df = qc.get(key=cache_val, use_file_cache=self.extension.use_file_cache())
+        df = CACHE.get(key=cache_val)
         if df is not None:
             logger.debug("Using cached SubQuery")
             self.dataframe = df  # type: ignore
             return True
         else:
             logger.debug("Not found in cache")
             return False
 
     def save_to_cache(self):
         if not self.extension.allow_cache_save(self):
             return
 
-        cache_period = self.extension.get_cache_period()
-
-        cache_override = self.options.get("cache")
-        if cache_override is not None:
-            if isinstance(cache_override, int):
-                cache_period = cache_override
-            else:
-                raise ValueError(f"Invalid cache value passed: {cache_override}")
-
         cache_val = self.subquery
 
-        logger.debug(
-            f"Saving to cache {cache_val} {self.extension.get_cache_period()} override {cache_override}"
-        )
-
         if self.dataframe is not None:
-            qc.save(
-                key=cache_val,
-                o=self.dataframe,
-                duration_seconds=cache_period,
-                use_file_cache=self.extension.use_file_cache(),
-            )
+            CACHE.save(key=cache_val, data=self.dataframe)
 
 
 @dataclass
 class SubQueryGroup(SubQuery):
     """SubQueryGroups represent a set of queries whose outputs will be combined.
     SubQueries are executed in parallel (via get_subqueries_flat),
     so this step is needed to gather the results.
@@ -861,105 +828,117 @@
         result = self.db.execute_query(query=self.query, completed_results=completed_results)  # type: ignore
 
         if result is None:
             df = None
         else:
             df = result.df_numpy()
 
+        # add the final result to the completions
+        final_result = IqlResultData(name="final", query=self.query, _data=df)  # type: ignore
+
+        completed_results.append(final_result)
+
         return (df, completed_results)  # type: ignore
 
 
 class IqlPlan:
     pass
 
 
 def _parameterize_sql_alias(subword, query) -> str:
     if subword not in _ALIASES.keys():
         raise ValueError(f"Unknown alias {subword}")
 
-    base_query = _ALIASES[subword]
+    base_query_gen = _ALIASES[subword]
+    base_query = base_query_gen()
 
     for k, v in options_parser.options_to_list(query).items():
         # convert the parameter to $uppercase, so security => $SECURITY
         newk = f"${k.upper()}"
-        if newk not in base_query:
-            raise ValueError(f"Parameter {k} / {newk} not in alias SQL")
-        else:
-            base_query = base_query.replace(newk, str(v))
+        base_query = base_query.replace(newk, str(v))
 
     return base_query
 
 
 def replace_sql_aliases(query) -> str:
     newquery = query
     for keyword, subword, outer, inner in _extract_subquery_strings(query, ["alias"]):
         sql = _parameterize_sql_alias(subword, outer)
 
+        # aliases might recurse
+        sql = replace_sql_aliases(sql)
         logger.debug(f"Found SQL alias, replacing and parameterizing: {outer}")
 
         newquery = newquery.replace(outer, sql)
         # logger.info(f"After alias replacement {query}")
 
     return newquery
 
 
 def execute_debug(
-    query: str, con: Optional[object] = None
+    query: str, con: Optional[object] = None, params: Dict[str, object] = None
 ) -> Tuple[bool, Optional[DataFrame], Optional[Dict[str, List[IqlResult]]]]:
     """Returns the success (True or False), final query result, and the debug results: all the intermediate queries and subqueries."""
     # Connection to database
+
+    # TODO: Get rid of this special case for BQL only.
+    if query.strip().startswith("get") or query.strip().startswith("let"):
+        query = query.replace('"', '"')
+        query = f"""select * from bql("{query}")"""
+
+    # Initialize or Reuse DB Connector
     get_dbconnector()
     if _DBCONNECTOR is None:
         raise ValueError("DBConnector Not Set")
     if con is None:
         db = _DBCONNECTOR.create_database()
     else:
         db = _DBCONNECTOR.create_database_from_con(con=con)
 
+    if params is not None:
+        logger.info(f"Parameterizing with {params}")
+        for k, v in params.items():
+            query = query.replace(f"${k.upper()}", str(v))
+
     # Aliases
     query = replace_sql_aliases(query)
 
     try:
         # A single query might contain multiple SQL statements. Parse them out and iterate:
-
         df = None
         completed_result_map = {}
         if ";" not in query:
             # Performance optimization for simple queries
             iqc = IqlQueryContainer(query=query, db=db)
 
-            df, completed_dfs = iqc.execute()
+            df, completed_results = iqc.execute()
+            return (True, df, {query: completed_results})
         else:
             for statement in sqlparse.parse(query):
                 singlequery = statement.value.strip(";")
                 iqc = IqlQueryContainer(query=singlequery, db=db)
 
                 # Run each statement, but only keep the results from the last one
                 df, completed_results = iqc.execute()
 
-                # add the final result to the completions
-                final_result = IqlResultData(name="final", query=statement, _data=df)
-
-                completed_results.append(final_result)
                 completed_result_map[statement] = completed_results
 
         return (True, df, completed_result_map)
 
     finally:
         if con is None:  # DB was created here, so close it
             db.close_db()
 
 
-def execute(query: str, con: Optional[object] = None) -> Optional[DataFrame]:
+def execute(
+    query: str, con: Optional[object] = None, params: Dict[str, object] = None
+) -> Optional[DataFrame]:
     """Executes the given SQL query. Keyword is only used to run a single subquery without SQL."""
 
-    if query.strip().startswith("get") or query.strip().startswith("let"):
-        query = query.replace('"', '"')
-        query = f"""select * from bql("{query}")"""
-    success, df, completed_dfs = execute_debug(query, con)
+    success, df, completed_results = execute_debug(query, con, params=params)
 
     return df
 
 
 def get_dbconnector() -> IqlDatabaseConnector:
     global _DBCONNECTOR
     if _DBCONNECTOR is None:
@@ -977,22 +956,31 @@
     if e.keyword not in _KNOWN_EXTENSIONS.keys():
         _KNOWN_EXTENSIONS[e.keyword] = e.keyword
 
     if e.temp_file_directory is None:
         e.temp_file_directory = DEFAULT_EXT_DIRECTORY
 
 
-def register_alias(subword: str, sql: str):
+def register_alias(subword: str, sql: str, file: str):
     """
     Aliases are called via
     alias.aliasname(param1=abc, param2.abc)
-    When run, the alias will be replaced, and "$PARAM1" will be replaced with abc
+    When run, the alias will be replaced, and "$PARAM1" will be replaced with abc.
+    You can either register the entire SQL or a path to a file containing the SQL.
+    If both are passed, the SQL is used/cached
     """
+
     logger.debug(f"Registering alias: {subword}")
-    _ALIASES[subword] = sql
+
+    if sql is not None:
+        _ALIASES[subword] = lambda: sql
+    elif file is not None:
+        _ALIASES[subword] = lambda: open(file).read()
+    else:
+        raise ValueError("register_alias: sql or file is None. One must be passed")
 
 
 def list_extensions() -> List[str]:
     return list(_KNOWN_EXTENSIONS.keys())
 
 
 def get_extension(keyword: str, subword: str) -> "IqlExtension":
@@ -1012,36 +1000,30 @@
         module.register(keyword)
 
         if words not in _EXTENSIONS:
             raise ValueError(f"{keyword}.{subword} is not registered")
         return _EXTENSIONS[words]
 
 
+def get_cache():
+    return CACHE
+
+
+def set_cache(cache: QueryCacheBase):
+    global CACHE
+    CACHE = cache
+
+
 def configure(
-    duration_seconds: Optional[int] = -1,
-    cache_directory: Optional[str] = None,
     temp_dir: Optional[str] = None,
     max_processes: Optional[int] = None,
 ):
     """
     Must be called before extensions are initialized (on first use)
     duration_seconds: None (Disabled), -1 (Infinite), int (Seconds)
     file_directory: None (no file cache), string (output directory)
     """
-    global _CACHE_PERIOD
-    global _USE_FILE_CACHE
     global DEFAULT_EXT_DIRECTORY
-
-    _CACHE_PERIOD = duration_seconds
-    if cache_directory is None:
-        _USE_FILE_CACHE = False
-    else:
-        _USE_FILE_CACHE = True
-        if not os.path.exists(cache_directory):
-            raise ValueError(f"cache_directory {cache_directory} does not exist")
-
-        qc.activate_file_cache(cache_directory)
-
     DEFAULT_EXT_DIRECTORY = temp_dir
 
     if max_processes is not None:
         te.MAX_PROCESSES = max_processes
```

## iql/bbg_bql/bql_extension.py

```diff
@@ -3,23 +3,24 @@
 
 import logging
 import re
 from pandas import DataFrame
 from typing import List, Optional, Dict
 from dataclasses import dataclass, field
 
-from iql import q_cache
+from iql import get_cache
 from iql.bbg_bql.bql_wrapper import BaseBqlQuery, execute_bql_str_list_async_q
 from iql.bbg_bql.bql_datamodel import RawBqlQuery
 from iql.iqmoql import (
     IqlExtension,
     register_extension,
     SubQuery,
     get_subqueries_flat,
     IqlQueryContainer,
+    IqlResultData,
 )
 
 
 logger = logging.getLogger(__name__)
 
 _KEYWORD = "bql"
 
@@ -80,14 +81,17 @@
     def execute(self) -> bool:
         # populate_from_cache is called from execute_batch, doesn't need to be run again here
         if self.dataframe is not None:
             return True
 
         success = self.execute_internal()
 
+        if not success:
+            logger.warning(self.bqlquery.exception_msg)
+
         if success:
             df = self.bqlquery.to_df()
 
             df = self.extension.apply_pandas_operations_prepivot(df, self.options)
 
             df = self.extension.pivot(df, self.options.get("pivot"))  # type: ignore
             df = self.extension.apply_pandas_operations_postpivot(df, self.options)
@@ -169,15 +173,15 @@
         iqc: IqlQueryContainer,
         create_function: object = None,
     ) -> List["SubQuery"]:
         return super().create_subqueries(
             query=query, name=name, iqc=iqc, create_function=self.create_subquery
         )
 
-    def execute_batch(self, subqueries: List[_IqmoBqlQuery]) -> Dict[str, DataFrame]:
+    def execute_batch(self, subqueries: List[_IqmoBqlQuery]) -> List[IqlResultData]:
         # Caching operates at two levels here:
         # The SubQuery result, and within the bql_wrapper
         # To force a refresh, we'll clear both the subquery and bql raw query
         # cache
 
         subqueries_flat: List[_IqmoBqlQuery] = get_subqueries_flat(subqueries)  # type: ignore
 
@@ -186,15 +190,15 @@
 
         clear_inner_caches = False
 
         needs_to_be_cleared = [q for q in subqueries_flat if clear_inner_caches]
         logger.debug(f"Clearing {len(needs_to_be_cleared)}")
         # clear lower-level cache entries
         for q in needs_to_be_cleared:
-            q_cache.clear(q.bqlquery.to_bql_query())
+            get_cache().clear(prefix="bql", key=q.bqlquery.to_bql_query())
 
         to_run: List[_IqmoBqlQuery] = [
             sq for sq in subqueries_flat if sq.dataframe is None
         ]
 
         queries = [q.bqlquery for q in to_run]
 
@@ -212,22 +216,25 @@
             try:
                 q.execute()
             except Exception as e:
                 raise ValueError(
                     f"Error on q.bqlquery: {q.bqlquery.to_bql_query()}"
                 ) from e
 
-        completed_dfs = {}
+        completed_results = []
         # Final step to merge any grouped subqueries.
         for q in subqueries:
             q.merge()
             df = q.dataframe
-            completed_dfs[q.name] = df
 
-        return completed_dfs
+            result = IqlResultData(name=q.name, query=q.subquery, _data=df)
+
+            completed_results.append(result)
+
+        return completed_results
 
 
 def execute_bql(query: str, pivot: Optional[str] = None) -> DataFrame:
     """Convenience function for testing, or executing single queries"""
 
     if _KEYWORD in query:
         raise ValueError(f"Pass raw BQL queries only, don't wrap with {_KEYWORD}(...)")
```

## iql/bbg_bql/bql_wrapper.py

```diff
@@ -8,18 +8,17 @@
 import logging
 from threading import Lock
 from datetime import datetime
 from functools import partial
 from typing import List, Optional, Union, Dict
 from pandas import DataFrame
 from abc import abstractmethod
-
+import os
 import bql  # pyright: ignore pylint: disable=C0413 # noqa: E402
-from iql import q_cache
-from iql import iqmoql
+from iql import get_cache
 
 
 _MAX_CONCURRENT = 128
 _SHIFT_DUPLICATES = True
 
 logger = logging.getLogger(__name__)
 
@@ -79,19 +78,37 @@
 
     def _populate_data(self):
         execute_bql_str_list_async_q([self])
 
 
 def get_bqservice(retries: int = 3):
     global bqService
-    logger.debug("Creating new bqService")
 
     try:
         if bqService is None:  # type: ignore
-            bqService = bql.Service()  # (bqlmetadata.ShippedMetadataReader())
+            logger.debug("Creating new bqService")
+
+            start_time = time.time()
+
+            if is_bquant():
+                try:
+                    from bqlmetadata import ShippedMetadataReader
+
+                    bqService = bql.Service(ShippedMetadataReader())
+                except Exception:
+                    logger.exception("Unable to initialize with ShippedMetadataReader")
+                    bqService = bql.Service()
+
+            else:
+                bqService = bql.Service()
+
+            end_time = time.time()
+            duration = end_time - start_time
+            logger.info(f"Creating new bqService took {round(duration)} seconds")
+
     except Exception as e:
         logger.exception("Unable to create bq service")
         if retries <= 0:
             raise e
 
     if bqService is None:
         if retries > 0:
@@ -192,34 +209,34 @@
 
     if "preferences" not in request_str:
         request_str += "\npreferences (addcols=all)"
 
     return request_str
 
 
-def error_callback(o, errorlist=None):
-    if errorlist is None:
-        logger.info(o)
-        return
-
+def bql_exception_to_str(e) -> object:
     try:
-        e = o[1]
+        e = e[1]
         long_error = {
             "message": e.exception_messages,
             "request_id": e._request_id,
             "details": e.internal_messages,
         }
-        errorlist.append(long_error)
+        return long_error
+    except Exception:
+        return str(e)
 
-    except Exception as e:
-        logger.exception("Couldn't expand error callback")
-        errorlist.append(o)
-    logger.warning("Error executing" + str(o))
-    if errorlist is not None:
-        errorlist.append(o)
+
+def error_callback(o, errorlist=None):
+    if errorlist is None:
+        logger.warning(o)
+        return
+
+    msg = bql_exception_to_str(o)
+    errorlist.append(msg)
 
 
 def execute_bql_str_list_async_q(
     queries_input: List[BaseBqlQuery],
     suppress_warning_log: bool = False,
     max_queries: int = _MAX_CONCURRENT,
 ):
@@ -230,15 +247,15 @@
     Either batch requests through a single requester thread, or
     distribute workload across requesters.
     """
     logger.debug("Checking to see if any are already cached")
 
     for q in queries_input:
         qstr = q.to_bql_query()
-        data = q_cache.get(qstr)  # type: ignore
+        data = get_cache().get(key=qstr, prefix="bql")  # type: ignore
         if data is not None:
             logger.debug(f"Found in cache: {qstr}")
 
             if isinstance(data, DataFrame):
                 q._df = data
             else:
                 q._data = data  # type: ignore
@@ -250,15 +267,15 @@
     into smaller groups of max_queries size and execute each serially"""
 
     if len(queries_not_cached) == 0:
         logger.debug("No queries to run")
         return
 
     query_groups = [
-        queries_input[i * max_queries : (i + 1) * max_queries]
+        queries_not_cached[i * max_queries : (i + 1) * max_queries]
         for i in range((len(queries_not_cached) + max_queries - 1) // max_queries)
     ]
 
     start = time.time()
 
     count = 1
     for query_group in query_groups:
@@ -271,68 +288,56 @@
         # t1.start()
         # t1.join
 
         logger.debug("Done async with callbacks")
         _execute_bql_str_list_async_orig(query_group, suppress_warning_log)
 
     end = time.time()
-    logger.info(f"Elapsed time running queries: {end-start} seconds")
+    logger.info(f"Elapsed time running queries: {round(end-start)} seconds")
 
     for q in queries_not_cached:
         logger.debug("Saving to cache")
         if q._data is not None:
-            q_cache.save(
-                q.to_bql_query(),
-                q._data,
-                type=__name__,
-                duration_seconds=iqmoql._CACHE_PERIOD,
-            )
+            get_cache().save(key=q.to_bql_query(), data=q._data, prefix="bql")
 
     return
 
 
-def submit_fetch_many_available():
-    # Force execute_many for now.
-    # return os.environ.get("BQUANT_USERNAME") is not None
-
-    return False
+def is_bquant():
+    return os.environ.get("BQUANT_USERNAME") is not None
 
 
 def _execute_bql_str_list_async_orig(
     queries: List[BaseBqlQuery], suppress_warning_log: bool = False
 ):
     with bqllock:
-        query_strings = []
-        for query in queries:
-            qstr = query.to_bql_query()
-
-            if "iqmo" in qstr:
-                raise ValueError("IQMO parameters passed to BQL layer, cannot run")
-
-            logger.debug(f"Executing {qstr}")
-            query_strings.append(qstr)
+        query_strings = [query.to_bql_query() for query in queries]
 
         bqService = get_bqservice()
 
         # TODO: Out of order errors are not handled here. Not an issue in many cases
         # but is still very likely.
         errorlist: List[str] = []
 
-        if submit_fetch_many_available():
-            logger.debug("Using submit fetch many")
+        try:
+            if is_bquant():
+                logger.debug("Using submit fetch many")
 
-            gen = bqService.submit_fetch_many(
-                query_strings,
-                on_request_error=partial(error_callback, errorlist=errorlist),
-            )
-        else:
-            gen = bqService.execute_many(
-                query_strings,
-                partial(error_callback, errorlist=errorlist),
-            )
+                gen = bqService.submit_fetch_many(
+                    query_strings,
+                    on_request_error=partial(error_callback, errorlist=errorlist),
+                )
+            else:
+                gen = bqService.execute_many(
+                    query_strings,
+                    on_request_error=partial(error_callback, errorlist=errorlist),
+                )
+        except Exception as e:
+            logger.exception(bql_exception_to_str(e))
+            raise ValueError(f"Error submitting {query_strings}") from e
 
         error_index = 0
 
         logger.info("Waiting for and processing BQL results")
         for r, q in zip(gen, queries):
             try:
                 if r is None:
@@ -345,15 +350,15 @@
                     q._data = data
                     q.execution_status = q.STATUS_COMPLETED
 
             except Exception as e:
                 logger.exception("Query error")
                 q._data = None
                 q.execution_status = q.STATUS_FAILURE
-                q.exception_msg = str(e)
+                q.exception_msg = bql_exception_to_str(e)  # type: ignore
         logger.info("Done executing")
 
 
 def flatten_list_str(value: Union[str, List[str]]) -> List[str]:
     """Converts input to a List, if not already a List"""
     if isinstance(value, str):
         value_str = str(value)
```

## iql/db_connectors/duckdb_connector.py

```diff
@@ -101,21 +101,28 @@
                         con.register(result.name, data)  # type: ignore
 
                 d = con.execute(query)  # type: ignore
                 # Don't use con.sql, as it adds a small but
                 # measurable overhead of creating a duckdb relation, that we don't need
                 if d is not None:
                     # logger.debug("Using Pandas format")
-                    table = d.arrow()
-                    return DuckDbResult(name=query, query=query, _table=table)
+                    try:
+                        table = d.arrow()
+
+                        table = rename_dupe_arrow_columns(table)
+                        return DuckDbResult(name=query, query=query, _table=table)
+                    except Exception as e:
+                        # TODO: Detect this more gracefully
+                        logger.debug(f"Didn't have a result set {str(e)}")
+                        return None
                 else:
                     return None
             except Exception as e:
                 logger.exception(f"Error executing SQL DFs: {query}")
-                raise ValueError("Error executing {query}") from e
+                raise ValueError(f"Error executing {query}") from e
 
     def get_connection(self):
         return self._connection.cursor()  # type: ignore
 
     def close_db(self):
         try:
             if self._connection is None:
```

## iql/extensions/aws_s3_extension.py

```diff
@@ -6,15 +6,15 @@
 from pandas import DataFrame
 from typing import Tuple, Optional, Dict
 from iql.iqmoql import IqlExtension, register_extension, SubQuery
 import boto3
 import re
 import os
 from pathlib import Path
-from iql import q_cache
+from iql import get_cache
 
 logger = logging.getLogger(__name__)
 
 _PATTERN = re.compile(r"s3://(.*?)/(.*)")
 
 BOTO3_S3_RESOURCES: Dict[str, object] = {}
 BOTO3_S3_RESOURCE_DEFAULT = None
@@ -71,36 +71,34 @@
 
         return (bucket, key, local_path)
 
     def execute(self, sq: SubQuery) -> Optional[DataFrame]:
         url = sq.get_query()
         bucket, key, local_path = self.options_to_tuple(url)
 
-        # For path replacement cases, the q_cache just stores a reference to the path.
-        # when the file is expired, q_cache returns None
-        obj = q_cache.get(local_path)
+        # For path replacement cases, the cache just stores a reference to the path.
+        # when the file is expired, cache returns None
+        obj = get_cache().get(local_path)
         expired = obj is None  # if obj is None, then the file is expired
 
         if Path(local_path).exists() and not expired and self.allow_cache_read(sq):
             logger.info(f"{local_path} exists, not downloading again")
             return None
         else:
             logger.debug(f"Downloading {key} to {local_path} from bucket {bucket}")
 
             s3_resource = get_boto3_resource_for_request(url)
             s3_bucket = s3_resource.Bucket(bucket)  # type: ignore
             s3_bucket.download_file(key, local_path)  # type: ignore
 
             # Just save the path name as the object
-            q_cache.save(
-                local_path,
-                local_path,
-                self.get_cache_period(),
-                self.use_file_cache(),
-                type="awss3",
+            get_cache().save(
+                key=local_path,
+                data=local_path,
+                prefix="awss3",
             )
             return None
 
 
 def register(keyword: str):
     extension = AwsS3Extension(keyword=keyword)
     register_extension(extension)
```

## Comparing `iql-1.5.dist-info/LICENSE` & `iql-1.6.1rc5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iql-1.5.dist-info/METADATA` & `iql-1.6.1rc5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: iql
-Version: 1.5
+Version: 1.6.1rc5
 Summary: SQL Overlay Language with support for Bloomberg BQL, FRED, Edgar, Kaggle and other financial data sources within SQL
 Home-page: https://github.com/iqmo-org/iql_dev
 Author: Paul Timmins
 Author-email: paul@iqmo.com
 Keywords: IQMO Query Language IQMOQL BQL BQUANT FRED EDGAR KAGGLE
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: duckdb (>=0.7.1)
-Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: duckdb (>=0.8.0)
+Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: sqlparse (>=0.4.3)
 Requires-Dist: pyarrow
 
 # Intermediate Query Language (IQL)
 
 IQL is a framework and a collection of Python-based extensions for financial data acquisition.
 
@@ -456,78 +456,15 @@
 ### Prophet
 
 pip install prophet
 pip install backports.zoneinfo (?)
 
 # Caching
 
-SubQueries are often expensive and often reused while developing and refining queries. If enabled, IQL will cache the SubQuery results in memory and/or in a persistent file cache.
-
-Caching can be controlled via iql.configure:
-
-```
-def configure(
-    duration_seconds: Optional[int] = -1, cache_directory: Optional[str] = None, temp_dir: Optional[str] = None, max_processes: int = 2
-):
-```
-
-duration_seconds:
-
-```
--1 (Default): Infinite (for life of kernel)
-None: Disabled
-int: Maximum life of the cached value from the time of creation.
-```
-
-cache_directory:
-
-```
-None (Default): Don't use a persistent file cache
-path: Location for the external file cache
-```
-
-## Caching Waterfall
-
-- nocache directive
-- cache directive
-- extension cache period
-- global \_CACHE_PERIOD
-
-## Caching Limitations
-
-Cached values are not pruned on expiration. The in memory dictionary is cleared on kernel restart. The file cache will grow unbounded until cleared:
-
-```
-from iql import q_cache # clear the in memory and file cache
-xq_cache.clear_caches()
-```
-
-## Caching Hints
-
-### cache=seconds
-
-Overrides the caching period. -1 is infinite caching.
-
-```
-iql.execute("""SELECT * FROM keyword("...", cache=60) as q1""")
-```
-
-### nocache=True
-
-Does not use any cached results
-
-```
-iql.execute("""SELECT * FROM keyword("...", nocache=True) as q1""")
-```
-
-## Caching Best Practices
-
-Caching is important to get right but depend on the data and use cache. Caching can significantly improve performance during design and development which frequently reuse unchanging data. For live data that changes frequently, an appropriate cache interval should be used to avoid reuse of stale data.
-
-If your kernels are short-lived, this is largely a non-issue, since the cache is reset automatically, unless a file cache is activated.
+A custom cacher may be implemented by implementing iql.q_cache_base, set via `iql.set_cache`.
 
 # Database
 
 ## Valid Queries
 
 In DuckDB, IQL was developed against DuckDB's statements, including SELECTs with CTE's (WITH clauses). IQL is seamless: it only modifies the extension SubQueries, and otherwise passes the results to the database.
```

