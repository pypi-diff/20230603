# Comparing `tmp/bmsdna_lakeapi-0.6.0.tar.gz` & `tmp/bmsdna_lakeapi-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.6.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.6.4.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.6.0.tar` & `bmsdna_lakeapi-0.6.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/README.md
--rw-r--r--   0        0        0      337 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      670 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6355 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9131 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6039 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11565 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    11712 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15480 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1452 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6512 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4293 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3579 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-01 10:49:26.909496 bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-06-01 10:49:26.913496 bmsdna_lakeapi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-03 09:25:26.935517 bmsdna_lakeapi-0.6.4/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-03 09:25:26.935517 bmsdna_lakeapi-0.6.4/README.md
+-rw-r--r--   0        0        0      337 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6595 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9409 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6030 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15456 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1452 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6408 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.4/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.6.0/LICENSE` & `bmsdna_lakeapi-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/README.md` & `bmsdna_lakeapi-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from bmsdna.lakeapi.context.df_base import ExecutionContext
 from bmsdna.lakeapi.core.types import Engines
-from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
-from bmsdna.lakeapi.context.df_polars import PolarsExecutionContext
 
 
-def get_context_by_engine(engine: Engines):
+def get_context_by_engine(engine: Engines) -> ExecutionContext:
     match engine.lower():
         case "duckdb":
             from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
-            ExecutionContext = DuckDbExecutionContext
+            return DuckDbExecutionContext()
         case "polars":
             from bmsdna.lakeapi.context.df_polars import PolarsExecutionContext
 
-            ExecutionContext = PolarsExecutionContext
+            return PolarsExecutionContext()
         case _:
             raise Exception(f"Unknown engine {engine}")
-    return ExecutionContext
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,22 @@
 
 
 class ExecutionContext(ABC):
     def __init__(self) -> None:
         super().__init__()
         self.modified_dates: dict[str, datetime] = {}
 
+    @abstractmethod
+    def __enter__(self) -> "ExecutionContext":
+        ...
+
+    @abstractmethod
+    def __exit__(self, *args, **kwargs):
+        ...
+
     def get_pyarrow_dataset(
         self,
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
     ) -> Optional[pa.dataset.Dataset | pa.Table]:
         if file_type in ["parquet", "ipc", "arrow", "feather", "csv", "orc"]:
@@ -200,7 +208,11 @@
         ds = self.get_pyarrow_dataset(uri, file_type, partitions)
         self.modified_dates[name] = self.get_modified_date(uri, file_type)
         self.register_arrow(name, ds)
 
     @abstractmethod
     def execute_sql(self, sql: Union[pypika.queries.QueryBuilder, str]) -> ResultData:
         ...
+
+    @abstractmethod
+    def list_tables(self) -> ResultData:
+        ...
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 import pypika.functions
 import pypika.enums
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
-ENABLE_COPY_TO = os.getenv("ENABLE_COPY_TO", "0") == "1"
 
+ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
+#ENABLE_COPY_TO = True
 
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
@@ -208,33 +209,38 @@
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='array')")
             return
         if file_type == "ndjson":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='newline_delimited')")
             return
         return super().register_dataframe(name, uri, file_type, partitions)
 
+    def list_tables(self) -> ResultData:
+        return self.execute_sql(
+            "SELECT table_name as name, table_type from information_schema.tables where table_schema='main'"
+        )
+
     def __enter__(self):
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self, *args, **kwargs):
         if self.res_con:
-            self.res_con.__exit__(*args)
+            self.res_con.__exit__(*args, **kwargs)
 
 
 class DuckDbExecutionContext(DuckDbExecutionContextBase):
     def __init__(self):
         super().__init__(duckdb.connect())
 
     def __enter__(self):
         super().__enter__()
         self.con.__enter__()
         self.con.execute("SET memory_limit='200MB'")
         self.con.execute("SET threads =2")
         self.con.execute("SET enable_object_cache=true")
         return self
 
-    def __exit__(self, *args):
-        super().__exit__(*args)
-        self.con.__exit__(*args)
+    def __exit__(self, *args, **kwargs):
+        super().__exit__(*args, **kwargs)
+        self.con.__exit__(*args, **kwargs)
 
     def close(self):
         self.con.close()
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_polars.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,18 +112,14 @@
         self.sql_context = sql_context or pl.SQLContext()
 
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         import polars as pl
 
         ds = pl.scan_pyarrow_dataset(ds) if isinstance(ds, pyarrow.dataset.Dataset) else pl.from_arrow(ds)
 
-        if isinstance(ds, pl.DataFrame):
-            ds = ds.lazy()
-
-        ds = pl.scan_ds(ds)
         self.sql_context.register(name, ds)
 
     def close(self):
         pass
 
     def json_function(self, term: pypika.terms.Term, assure_string=False):
         raise NotImplementedError()
@@ -172,12 +168,15 @@
         import polars as pl
 
         df = self.sql_context.execute(get_sql(sql))
         if isinstance(df, pl.LazyFrame):
             df = df.collect()
         return PolarsResultData(df, self.sql_context)
 
+    def list_tables(self) -> ResultData:
+        return self.execute_sql("SHOW TABLES")
+
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,68 +88,35 @@
     alias: Optional[str] = None
 
     def __post_init__(self):
         self.alias = self.alias if self.alias else self.name
 
 
 @dataclass
-class GroupByExpConfig:
-    # expression: str
-    col: str = ""
-    func: Optional[PolaryTypeFunction] = None
-    alias: Optional[str] = None
-
-    @classmethod
-    def from_dict(cls, config: Dict):
-        return cls(col=config["col"], func=config.get("func"), alias=config.get("alias"))
-
-
-@dataclass
-class GroupByConfig:
-    by: List[str]
-    expressions: List[GroupByExpConfig]
-
-
-@dataclass
-class Join:
-    uri: str
-    left_on: str
-    right_on: str
-    file_type: FileTypes = "delta"
-    how: JoinStrategy = "inner"
-    suffix: str = "_right"
-
-
-@dataclass
 class DatasourceConfig:
     uri: str
     file_type: FileTypes = "delta"
     select: Optional[List[Column]] = None
     exclude: Optional[List[str]] = None
     sortby: Optional[List[SortBy]] = None
     filters: Optional[List[Filter]] = None
+    in_memory: bool = False
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
 
 
 @dataclass
-class Option:
-    ...
-
-
-@dataclass
 class Config:
     name: str
     tag: str
     datasource: DatasourceConfig
     version: Optional[int] = 1
     api_method: Union[Literal["get", "post"], List[Literal["get", "post"]]] = "get"
     params: Optional[List[Union[Param, str]]] = None
     timestamp: Optional[datetime] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
-    options: Optional[Union[Option, None]] = None
     allow_get_all_pages: Optional[bool] = False
     search: Optional[List[SearchConfig]] = None
     engine: Optional[Engines] = None
 
     def __post_init__(self):
         self.version_str = (
             str(self.version) if str(self.version or 1).startswith("v") else "v" + str(self.version or 1)
@@ -214,62 +181,64 @@
             else:
                 ls = []
                 for it in os.scandir(root_folder):
                     res_name = (version, tag, it.name)
                     if res_name not in table_names and (
                         (it.is_dir() and file_type == "delta") or (it.is_file() and file_type != "delta")
                     ):
-                        datasource = DatasourceConfig(
+                        datasource_obj = DatasourceConfig(
                             uri=folder + "/" + it.name,
                             file_type=file_type,
                             select=select,
                             exclude=exclude,
+                            in_memory=datasource.get("in_memory", False),
                             sortby=sortby,
                             filters=None,
                             cache_expiration_time_seconds=cache_expiration_time_seconds,
                         )
-                        new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource.uri)
+                        new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
                         ls.append(
                             cls(
                                 name=it.name,
                                 tag=tag,
                                 version=version,
                                 engine=config.get("engine", None),
                                 api_method=api_method,
                                 search=search_config,
                                 params=new_params,  # type: ignore
                                 allow_get_all_pages=config.get("allow_get_all_pages", False),
-                                datasource=datasource,
+                                datasource=datasource_obj,
                                 cache_expiration_time_seconds=cache_expiration_time_seconds,
                             )
                         )
             return ls
         else:
-            datasource = DatasourceConfig(
+            datasource_obj = DatasourceConfig(
                 uri=uri,
                 file_type=file_type,
                 select=select,
                 exclude=exclude,
+                in_memory=datasource.get("in_memory", False),
                 sortby=sortby,
                 filters=None,
                 cache_expiration_time_seconds=cache_expiration_time_seconds,
             )
-            new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource.uri)
+            new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
 
             return [
                 cls(
                     name=name,
                     tag=tag,
                     version=version,
                     search=search_config,
                     api_method=api_method,
                     engine=config.get("engine", None),
                     params=new_params,  # type: ignore
                     allow_get_all_pages=config.get("allow_get_all_pages", False),
-                    datasource=datasource,
+                    datasource=datasource_obj,
                     cache_expiration_time_seconds=cache_expiration_time_seconds,
                 )
             ]
 
     async def to_dict(self) -> dict:
         return self.__dict__
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pyarrow.parquet
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 
-from bmsdna.lakeapi.core.config import BasicConfig, DatasourceConfig, GroupByConfig, GroupByExpConfig, Param
+from bmsdna.lakeapi.core.config import BasicConfig, DatasourceConfig, Param
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.model import get_param_def
 from bmsdna.lakeapi.core.types import DeltaOperatorTypes, FileTypes
 from bmsdna.lakeapi.context.df_base import ResultData, ExecutionContext
 import pypika
 from pypika.queries import QueryBuilder
 import pypika.queries as fn
-import duckdb
+from datetime import datetime
 
 logger = get_logger(__name__)
 
 endpoints = Literal["query", "meta", "request", "sql"]
 
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
+df_cache: dict[str, tuple[datetime, pyarrow.Table]] = {}
+
 
 class Dataframe:
     def __init__(
         self,
         version: str,
         tag: str,
         name: str,
@@ -96,36 +98,49 @@
             pass
         else:
             df = self.select_df(df)
         return df
 
     @property
     def tablename(self):
-        if self.version  in ["1", "v1"]:
+        if self.version in ["1", "v1"]:
             return self.tag + "_" + self.name
         return self.tag + "_" + self.name + "_" + self.version
 
     def get_df(
         self,
         partitions: Optional[List[Tuple[str, str, Any]]],
         endpoint: endpoints = "request",
     ) -> ResultData:
         if self.df is None:
-            path = self.uri
-
-            tname = self.tablename
-            df = self.sql_context.register_dataframe(
-                tname,
-                path,
-                self.config.file_type,
-                partitions=partitions,
-            )
-            query = pypika.Query.from_(tname)
+            query = pypika.Query.from_(self.tablename)
             self.query = self._prep_df(query, endpoint=endpoint)
-            self.df = self.sql_context.execute_sql(self.query)
+            global df_cache
+            mod_date: datetime | None = None
+            if self.config.in_memory:
+                mod_date = self.sql_context.get_modified_date(self.uri, self.config.file_type)
+                if self.config.in_memory and self.tablename in df_cache:
+                    cache_date, df_t = df_cache[self.tablename]
+                    if mod_date <= cache_date:
+                        self.sql_context.register_arrow(self.tablename, df_t)
+                        self.df = self.sql_context.execute_sql(self.query)
+                    else:
+                        df_cache.pop(self.tablename)
+
+            if self.df is None:
+                self.sql_context.register_dataframe(
+                    self.tablename,
+                    self.uri,
+                    self.config.file_type,
+                    partitions=partitions,
+                )
+                self.df = self.sql_context.execute_sql(self.query)
+            if self.config.in_memory and not self.tablename in df_cache:
+                assert mod_date is not None
+                df_cache[self.tablename] = mod_date, self.df.to_arrow_table()
 
         return self.df  # type: ignore
 
 
 @cache
 async def get_partition_filter(param, deltaMeta, param_def):
     operators = ("<=", ">=", "=", "==", "in", "not in")
@@ -148,30 +163,30 @@
             col_for_partitioning = partcol
             value_for_partitioning = value
 
         elif partcol.startswith(colname + "_md5_prefix_"):
             col_for_partitioning = partcol
             prefix_len = int(partcol[len(colname + "_md5_prefix_") :])
             if isinstance(value, (List, Tuple)):
-                hashvl = [hashlib.md5(v.encode("utf8")).hexdigest() for v in value]
+                hashvl = [hashlib.md5(str(v).encode("utf8")).hexdigest() for v in value]
                 value_for_partitioning = [hvl[:prefix_len] for hvl in hashvl]
             else:
-                hashvl = hashlib.md5(value.encode("utf8")).hexdigest()
+                hashvl = hashlib.md5(str(value).encode("utf8")).hexdigest()
                 value_for_partitioning = hashvl[:prefix_len]
             if op not in operators:
                 col_for_partitioning = None
                 continue
         elif partcol.startswith(colname + "_md5_mod_"):
             col_for_partitioning = partcol
             modulo_len = int(partcol[len(colname + "_md5_mod_") :])
             if isinstance(value, (List, Tuple)):
-                hashvl = [int(hashlib.md5(v.encode("utf8")).hexdigest(), 16) for v in value]
+                hashvl = [int(hashlib.md5(str(v).encode("utf8")).hexdigest(), 16) for v in value]
                 value_for_partitioning = [hvl % modulo_len for hvl in hashvl]
             else:
-                hashvl = int(hashlib.md5(value.encode("utf8")).hexdigest(), 16)
+                hashvl = int(hashlib.md5(str(value).encode("utf8")).hexdigest(), 16)
                 value_for_partitioning = hashvl % modulo_len
             if op not in operators:
                 col_for_partitioning = None
                 continue
         elif partcol.startswith(colname + "_prefix_"):
             col_for_partitioning = partcol
             prefix_len = int(partcol[len(colname + "_prefix_") :])
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,16 @@
     ):  # type: ignore
         logger.info(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
         logger.info(f"Engine: {engine}")
 
-        ExecutionContext = get_context_by_engine(engine)
 
-        with ExecutionContext() as context:
+        with  get_context_by_engine(engine) as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
@@ -338,14 +337,15 @@
                 assert len(columns) <= 3  # reduce complexity here
                 new_query = new_query.distinct()
 
             if not (limit == -1 and config.allow_get_all_pages):
                 limit = 1000 if limit == -1 else limit
                 new_query = new_query.offset(offset or 0).limit(limit)
 
+
             if len(searches) > 0 and config.search is not None:
                 import pypika.queries
                 import pypika.terms
 
                 source_view = realdataframe.tablename
                 context.init_search(source_view, config.search)
                 score_sum = None
@@ -363,12 +363,12 @@
 
             logger.info(f"Query: {get_sql(new_query)}")
 
             df2 = context.execute_sql(new_query)
 
             try:
                 return await create_response(
-                    request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config
+                    request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config, close_context=True
                 )
             except Exception as err:
                 logger.error("Error in creating response", exc_info=err)
                 raise HTTPException(status_code=500)
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import io
-import json
 import mimetypes
 import os
 from enum import Enum
 from typing import Union
-from uuid import uuid4
+import tempfile
 
-import anyio
 import pyarrow as pa
-from fastapi import BackgroundTasks
 from starlette.background import BackgroundTask
 from starlette.datastructures import URL
 from starlette.responses import FileResponse
 
 from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
 from bmsdna.lakeapi.core.config import BasicConfig
 from bmsdna.lakeapi.core.log import get_logger
@@ -131,20 +127,22 @@
 class FileResponseWCharset(FileResponse):
     def __init__(self, *args, **kwargs):
         if "charset" in kwargs:
             self.charset = kwargs.pop("charset")
         super().__init__(*args, **kwargs)
 
 
+
 async def create_response(
     url: URL,
     accept: str,
     content: ResultData,
     context: ExecutionContext,
     basic_config: BasicConfig,
+    close_context=False,
 ):
     headers = {}
 
     format = parse_format(accept)
 
     format, extension = parse_format(accept)
     content_dispositiont_type = "attachment"
@@ -154,34 +152,29 @@
         OutputFormats.ND_JSON,
         OutputFormats.CSV,
         OutputFormats.SEMI_CSV,
         OutputFormats.CSV4EXCEL,
     ]:
         content_dispositiont_type = "inline"
         filename = None
-    path = os.path.join(basic_config.temp_folder_path, str(uuid4()) + extension)
-    media_type = "text/csv" if extension == ".csv" else mimetypes.guess_type("file" + extension)[0]
-    additional_files = write_frame(url=url, content=content, format=format, out=path, basic_config=basic_config)
-
-    tasks = BackgroundTasks()
-    import asyncio
 
-    async def remove():
-        context.close()
-        await anyio.sleep(3)
+    temp_file = tempfile.NamedTemporaryFile(delete=False, suffix=extension)
+    media_type = "text/csv" if extension == ".csv" else mimetypes.guess_type("file" + extension)[0]
+    additional_files = write_frame(url=url, content=content, format=format, out=temp_file.name, basic_config=basic_config)
 
-        os.remove(path)
+    def clean_up():
+        if close_context:
+            context.close()
+        temp_file.close()
         for f in additional_files:
             os.remove(f)
 
-    tasks.add_task(remove)
-
     fr = FileResponseWCharset(
-        path=path,
+        path=temp_file.name,
         headers=headers,
         media_type=media_type,
         content_disposition_type=content_dispositiont_type,
         filename=filename,
-        background=tasks,
+        background=BackgroundTask(clean_up),
         charset="utf-16le" if format == OutputFormats.CSV4EXCEL else "utf-8",
     )
     return fr
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,11 +102,11 @@
                 if config.search:
                     from bmsdna.lakeapi.core.dataframe import Dataframe
 
                     realdataframe = Dataframe(
                         config.version_str, config.tag, config.name, config.datasource, context, basic_config
                     )
                     if realdataframe.file_exists():
-                        with get_context_by_engine(basic_config.default_engine)() as ctx:
+                        with get_context_by_engine(basic_config.default_engine) as ctx:
                             ctx.init_search(realdataframe.tablename, config.search)
 
         return router
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,95 @@
 from typing import Any, Optional, Callable, Union
 import duckdb
-from fastapi import APIRouter, BackgroundTasks, Header, Request
+from fastapi import APIRouter, BackgroundTasks, Header, Query, Request
 from bmsdna.lakeapi.context.df_base import ExecutionContext
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
-from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
 from bmsdna.lakeapi.core.dataframe import Dataframe
 from bmsdna.lakeapi.core.types import OutputFileType
 from bmsdna.lakeapi.core.response import create_response
+from bmsdna.lakeapi.context import get_context_by_engine, Engines
 
-duckcon: Optional[duckdb.DuckDBPyConnection] = None
+sql_contexts: dict[str, ExecutionContext] = {}
 
 
-def init_duck_con(con: DuckDbExecutionContextBase, basic_config: BasicConfig, configs: Configs):
+def init_duck_con(con: ExecutionContext, basic_config: BasicConfig, configs: Configs):
     for cfg in configs:
         df = Dataframe(cfg.version_str, cfg.tag, cfg.name, cfg.datasource, con, basic_config)
         if df.file_exists():
             con.register_dataframe(df.tablename, df.uri, df.config.file_type, None)
 
 
-def get_duckdb_con(basic_config: BasicConfig, configs: Configs):
-    global duckcon
-    if duckcon is None:
-        duckcon = duckdb.connect()
-        context = DuckDbExecutionContextBase(duckcon)
-        init_duck_con(context, basic_config, configs)
+def get_sql_context(engine: Engines, basic_config: BasicConfig, configs: Configs):
+    global sql_contexts
+    if not engine in sql_contexts:
+        sql_contexts[engine] = get_context_by_engine(engine)
+        init_duck_con(sql_contexts[engine], basic_config, configs)
         if basic_config.prepare_sql_db_hook is not None:
-            basic_config.prepare_sql_db_hook(context)
+            basic_config.prepare_sql_db_hook(sql_contexts[engine])
 
-    else:
-        context = DuckDbExecutionContextBase(duckcon)
-    return context
+    return sql_contexts[engine]
 
 
 def create_sql_endpoint(
     router: APIRouter,
     basic_config: BasicConfig,
     configs: Configs,
 ):
     @router.on_event("shutdown")
     async def shutdown_event():
-        global duckcon
-        if duckcon is not None:
-            duckcon.close()
+        global sql_contexts
+        for item in sql_contexts.values():
+            item.__exit__()
+        sql_contexts = {}
 
     @router.get("/api/sql/tables", tags=["sql"], operation_id="get_sql_tables")
     async def get_sql_tables(
         request: Request,
         background_tasks: BackgroundTasks,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
+        engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
     ):
-        con = get_duckdb_con(basic_config, configs)
-        return (
-            con.execute_sql("SELECT table_name, table_type from information_schema.tables where table_schema='main'")
-            .to_arrow_table()
-            .to_pylist()
-        )
+        con = get_sql_context(engine, basic_config, configs)
+        return con.list_tables().to_arrow_table().to_pylist()
 
     @router.post(
         "/api/sql",
         tags=["sql"],
         operation_id="post_sql_endpoint",
     )
     async def get_sql_post(
         request: Request,
         background_tasks: BackgroundTasks,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
+        engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
     ):
         body = await request.body()
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
 
-        con = get_duckdb_con(basic_config, configs)
+        con = get_sql_context(engine, basic_config, configs)
         df = con.execute_sql(body.decode("utf-8"))
 
         return await create_response(
-            request.url, format or request.headers["Accept"], df, con, basic_config=basic_config
+            request.url, format or request.headers["Accept"], df, con, basic_config=basic_config, close_context=False
         )
 
     @router.get(
         "/api/sql",
         tags=["sql"],
         operation_id="get_sql_endpoint",
     )
     async def get_sql_get(
         request: Request,
         background_tasks: BackgroundTasks,
         sql: str,
         Accept: Union[str, None] = Header(default=None),
         format: Optional[OutputFileType] = "json",
+        engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
     ):
-        from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContextBase
-
-        con = get_duckdb_con(basic_config, configs)
+        con = get_sql_context(engine, basic_config, configs)
 
         df = con.execute_sql(sql)
         return await create_response(
-            request.url, format or request.headers["Accept"], df, con, basic_config=basic_config
+            request.url, format or request.headers["Accept"], df, con, basic_config=basic_config, close_context=False
         )
```

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.0/pyproject.toml` & `bmsdna_lakeapi-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.6.0"
+version = "0.6.4"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.6.0/PKG-INFO` & `bmsdna_lakeapi-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.6.0
+Version: 0.6.4
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

