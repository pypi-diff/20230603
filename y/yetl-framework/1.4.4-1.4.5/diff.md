# Comparing `tmp/yetl-framework-1.4.4.tar.gz` & `tmp/yetl-framework-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.4.4.tar", last modified: Fri Jun  2 08:04:32 2023, max compression
+gzip compressed data, was "yetl-framework-1.4.5.tar", last modified: Sat Jun  3 16:03:16 2023, max compression
```

## Comparing `yetl-framework-1.4.4.tar` & `yetl-framework-1.4.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16017 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.449226 yetl-framework-1.4.5/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.449226 yetl-framework-1.4.5/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.449226 yetl-framework-1.4.5/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-03 16:02:20.000000 yetl-framework-1.4.5/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 16:03:16.453226 yetl-framework-1.4.5/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-03 16:03:16.000000 yetl-framework-1.4.5/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.4.4/PKG-INFO` & `yetl-framework-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.4
+Version: 1.4.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.4/README.md` & `yetl-framework-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/setup.py` & `yetl-framework-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.4.4",
+    version="1.4.5",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.4.4/yetl/__main__.py` & `yetl-framework-1.4.5/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/cli/_init.py` & `yetl-framework-1.4.5/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.4.5/yetl/cli/metadata_provider/_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class ColumnNames(str, Enum):
     stage = "stage"
     table_type = "table_type"
     database = "database"
     table = "table"
     sql = "sql"
-    ids = "ids"
+    id = "id"
     depends_on = "depends_on"
     deltalake = "deltalake"
     identity = "identity"
     partition_by = "partition_by"
     delta_constraints = "delta_constraints"
     z_order_by = "z_order_by"
     delta_properties = "delta_properties"
@@ -41,15 +41,15 @@
 class Metadata(BaseModel):
     SCHEMA = {
         ColumnNames.stage: str,
         ColumnNames.table_type: str,
         ColumnNames.database: str,
         ColumnNames.table: str,
         ColumnNames.sql: str,
-        ColumnNames.ids: str,
+        ColumnNames.id: str,
         ColumnNames.depends_on: str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": int,
@@ -70,15 +70,15 @@
         super().__init__(**data)
 
     stage: StageType = Field(...)
     table_type: TableType = Field(...)
     database: str = Field(...)
     table: str = Field(...)
     sql: str = Field(default=None)
-    ids: str = Field(default=None)
+    id: str = Field(default=None)
     depends_on: str = Field(default=None)
     deltalake_delta_properties: str = Field(default=None)
     custom_properties: Dict[str, Any] = Field(default=None)
     deltalake_identity: str = Field(default=None)
     deltalake_partition_by: str = Field(default=None)
     deltalake_delta_constraints: str = Field(default=None)
     deltalake_z_order_by: str = Field(default=None)
@@ -142,15 +142,15 @@
             ]
         )
 
     def _has_properties(self):
         return any(
             [
                 self.sql is not None,
-                self.ids is not None,
+                self.id is not None,
                 self.depends_on is not None,
                 self.deltalake_delta_properties is not None,
                 self.deltalake_identity is not None,
                 self.deltalake_partition_by is not None,
                 self.deltalake_delta_constraints is not None,
                 self.deltalake_z_order_by is not None,
                 self._has_warning_thresholds(),
@@ -214,16 +214,16 @@
         table = None
         if self._has_properties():
             table = {}
             if self.depends_on is not None:
                 table[ColumnNames.depends_on.name] = self._get_list(
                     self.depends_on, default_singluar_to_str=False
                 )
-            if self.ids is not None:
-                table[ColumnNames.ids.name] = self._get_list(self.ids)
+            if self.id is not None:
+                table[ColumnNames.id.name] = self._get_list(self.id)
             if self.sql is not None and self.sql.lower() == "y":
                 table["sql"] = "../sql/{{database}}/{{table}}.sql"
             if self.deltalake_partition_by is not None:
                 table[ColumnNames.partition_by.name] = self._get_list(
                     self.deltalake_partition_by
                 )
             if self.deltalake_z_order_by is not None:
@@ -255,15 +255,15 @@
 class XlsMetadata(BaseModel):
     SCHEMA = {
         ColumnNames.stage: str,
         ColumnNames.table_type: str,
         ColumnNames.database: str,
         ColumnNames.table: str,
         ColumnNames.sql: str,
-        ColumnNames.ids: str,
+        ColumnNames.id: str,
         ColumnNames.depends_on: str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
         f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": str,
@@ -286,15 +286,14 @@
         df = self.validate_schema(df)
         self.data = self._deserialize(df)
 
     source: str = Field(...)
     data: dict = Field(default=None)
 
     def _auto_convert(self, data: Any):
-
         if isinstance(data, float):
             if data.is_integer():
                 return int(data)
         if isinstance(data, str):
             try:
                 data = float(data)
             except ValueError:
```

### Comparing `yetl-framework-1.4.4/yetl/config/__init__.py` & `yetl-framework-1.4.5/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_config.py` & `yetl-framework-1.4.5/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_decorators.py` & `yetl-framework-1.4.5/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_logging_config.py` & `yetl-framework-1.4.5/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_project.py` & `yetl-framework-1.4.5/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_spark_context.py` & `yetl-framework-1.4.5/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_tables.py` & `yetl-framework-1.4.5/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_timeslice.py` & `yetl-framework-1.4.5/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/_utils.py` & `yetl-framework-1.4.5/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/deltalake.py` & `yetl-framework-1.4.5/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/table/_deltalake.py` & `yetl-framework-1.4.5/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/table/_factory.py` & `yetl-framework-1.4.5/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/table/_read.py` & `yetl-framework-1.4.5/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/config/table/_table.py` & `yetl-framework-1.4.5/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.4.5/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.4/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.4.5/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.4
+Version: 1.4.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.4/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.4.5/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

