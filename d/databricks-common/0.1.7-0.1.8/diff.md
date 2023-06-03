# Comparing `tmp/databricks_common-0.1.7.tar.gz` & `tmp/databricks_common-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.7.tar", max compression
+gzip compressed data, was "databricks_common-0.1.8.tar", max compression
```

## Comparing `databricks_common-0.1.7.tar` & `databricks_common-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-05-22 19:24:47.486951 databricks_common-0.1.7/databricks_common/__init__.py
--rw-r--r--   0        0        0     9354 2023-05-22 19:24:27.859793 databricks_common-0.1.7/databricks_common/common.py
--rw-r--r--   0        0        0      258 2023-05-22 15:12:32.530513 databricks_common-0.1.7/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.7/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.7/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.7/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      740 2023-05-22 19:24:39.005870 databricks_common-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.8/README.md
+-rw-r--r--   0        0        0       22 2023-06-03 04:47:21.965190 databricks_common-0.1.8/databricks_common/__init__.py
+-rw-r--r--   0        0        0     9567 2023-06-03 04:44:38.820065 databricks_common-0.1.8/databricks_common/common.py
+-rw-r--r--   0        0        0      258 2023-05-22 15:12:32.530513 databricks_common-0.1.8/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.8/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.8/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.8/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-06-03 04:47:32.987358 databricks_common-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.8/PKG-INFO
```

### Comparing `databricks_common-0.1.7/databricks_common/common.py` & `databricks_common-0.1.8/databricks_common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,32 @@
         self.schema_ref = self._get_schema_ref()
 
     def __repr__(self) -> str:
         cls = self.__class__.__name__
         return f"{cls}({self.ref})"
 
     @classmethod
-    def from_string(cls, ref: str) -> "MetastoreTable":
+    def from_string(cls, table_ref: str) -> "MetastoreTable":
         """
         Alternative constructor to initialise a TableReference object from a string.
         """
-        cat, schema, table = ref.split(".")
-        return cls(cat, schema, table)
+        cat, schema, name = table_ref.split(".")
+        return cls(name=name, catalog=cat, schema=schema)
 
-    def check_exists(self) -> bool:
+    def check_exists_depr(self) -> bool:
         MetastoreCatalog(self.catalog).set()
         return spark.catalog.tableExists(self.short_ref)
 
+    def check_exists(self) -> bool:
+        try:
+            spark.sql(f"DESC TABLE {self.ref}")
+            return True
+        except Exception as e:
+            return False
+
     def drop(self) -> None:
         spark.sql(f"DROP TABLE {self.ref}")
 
     def drop_if_exists(self) -> None:
         if self.check_exists():
             self.drop()
```

### Comparing `databricks_common-0.1.7/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.8/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_common-0.1.7/pyproject.toml` & `databricks_common-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-common"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Xavier Armitage <xtarmitage@gmail.com>"]
 readme = "README.md"
 packages = [{include = "databricks_common"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

