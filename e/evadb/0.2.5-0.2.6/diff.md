# Comparing `tmp/evadb-0.2.5.tar.gz` & `tmp/evadb-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.5.tar", last modified: Sat Jun  3 02:07:23 2023, max compression
+gzip compressed data, was "evadb-0.2.6.tar", last modified: Sat Jun  3 03:19:58 2023, max compression
```

## Comparing `evadb-0.2.5.tar` & `evadb-0.2.6.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.189962 evadb-0.2.5/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2022-08-11 16:20:33.000000 evadb-0.2.5/LICENSE.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 02:07:23.185961 evadb-0.2.5/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13539 2023-06-02 21:04:24.000000 evadb-0.2.5/README.md
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      645 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7778 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15552 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    18583 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3320 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8604 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      886 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/association_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4671 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/base_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5266 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/column_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3393 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/index_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/table_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3532 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4429 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2262 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4722 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2668 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2127 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/schema_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1167 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/base_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2873 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4571 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3669 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3078 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2826 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2476 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1936 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/sql_config.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5490 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4798 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/configuration_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1005 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      882 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      852 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/eva.yml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3246 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2140 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/create_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5191 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1924 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7292 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4738 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2515 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1968 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/drop_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3537 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/exchange_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3017 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4366 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1522 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1591 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/function_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1759 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/groupby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1800 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/hash_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2255 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/join_build_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1661 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/lateral_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1583 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3086 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_csv_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1648 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6038 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1488 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4183 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8198 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1644 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1277 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/predicate_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1272 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/project_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2074 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/ray_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1186 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1413 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1812 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2533 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/storage_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1264 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/union_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3916 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/vector_index_scan_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5559 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3973 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/aggregation_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1618 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/arithmetic_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4351 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/comparison_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2542 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/constant_value_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10433 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10358 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3055 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/logical_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4685 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/interfaces/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/interfaces/relational/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10769 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/db.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7278 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/relation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4472 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      633 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1332 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/frame_info.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      857 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/properties.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/server/response.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14841 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/storage/batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3259 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2129 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3450 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2669 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/group_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4335 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    37333 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/operators.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3837 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      982 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12582 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10874 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4102 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/plan_generator.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1169 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/property.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1019 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/pattern.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    49728 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/optimizer/rules/rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7440 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7534 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13726 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.145960 evadb-0.2.5/eva/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1360 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/alias.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2740 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_index_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2872 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5341 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4882 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2048 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1767 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1793 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/drop_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19702 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/eva.lark
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1384 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2922 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/insert_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_parser.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.149960 evadb-0.2.5/eva/parser/lark_visitor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2655 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2161 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10824 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1404 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1202 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1006 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4672 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6231 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2465 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2241 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      932 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2143 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1112 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3214 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1227 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6248 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1460 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/show_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1426 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8637 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/table_ref.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1787 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1689 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3453 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1455 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1930 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2076 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3603 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1660 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1532 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2057 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/plan_nodes/exchange_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1033 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1755 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1712 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2179 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2023 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1468 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2710 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1510 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1564 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1177 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1249 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/project_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1760 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1201 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4419 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1421 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/union_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/vector_index_scan_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2320 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/abstract_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2648 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5987 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/readers/document/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1467 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/document_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1979 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/registry.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/readers/image/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/image/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1067 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/image/opencv_image_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2050 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/pdf_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      623 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3289 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3263 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2926 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6133 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2383 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1713 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/document_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1717 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/image_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/pdf_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8972 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1941 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2496 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      605 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/huggingface/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      612 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1420 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6473 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/create.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2615 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/model.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/vector_stores/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3284 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/faiss.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2960 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/qdrant.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1376 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1594 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/abstract/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2442 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3843 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3914 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/tracker_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3464 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/asl_action_recognition.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3413 2023-06-03 01:20:14.000000 evadb-0.2.5/eva/udfs/chatgpt.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2755 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3376 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2067 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5478 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2539 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/face_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5999 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1822 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1028 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/gpu_compatible.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3528 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/mnist_image_classifier.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2472 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2568 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1647 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1179 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2202 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/horizontal_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1557 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1782 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2139 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/vertical_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2750 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ocr_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/sift_feature_extractor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/trackers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/trackers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2367 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/trackers/nor_fair.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/tutorials/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/tutorials/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7934 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3859 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      611 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      909 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/errors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6966 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1956 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/kv_cache.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      985 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/logging_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1388 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/math_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1562 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/s3_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/stats.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-03 02:07:22.000000 evadb-0.2.5/eva/version.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/evadb.egg-info/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14107 2023-06-03 02:07:23.000000 evadb-0.2.5/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       88 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/entry_points.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1329 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/requires.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       21 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/top_level.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2022-06-26 17:11:46.000000 evadb-0.2.5/pyproject.toml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-03 02:07:23.189962 evadb-0.2.5/setup.cfg
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4575 2023-06-03 02:07:16.000000 evadb-0.2.5/setup.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-09-30 14:20:49.000000 evadb-0.2.5/test/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/benchmark_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:53.000000 evadb-0.2.5/test/benchmark_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1176 2023-05-09 19:58:04.000000 evadb-0.2.5/test/benchmark_tests/conftest.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6639 2023-05-12 03:48:38.000000 evadb-0.2.5/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2032 2023-01-02 23:54:53.000000 evadb-0.2.5/test/binder/test_binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13819 2023-06-01 22:37:10.000000 evadb-0.2.5/test/binder/test_statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7962 2023-05-16 03:45:18.000000 evadb-0.2.5/test/binder/test_statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7234 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/models/test_models.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-01-07 03:29:08.000000 evadb-0.2.5/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4794 2023-05-17 22:20:34.000000 evadb-0.2.5/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-04-01 16:09:26.000000 evadb-0.2.5/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3210 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3035 2023-04-02 20:13:44.000000 evadb-0.2.5/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6808 2023-05-09 19:58:04.000000 evadb-0.2.5/test/catalog/test_catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1402 2022-12-13 23:02:13.000000 evadb-0.2.5/test/catalog/test_column_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-04-01 16:09:26.000000 evadb-0.2.5/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1486 2023-05-25 14:58:01.000000 evadb-0.2.5/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1620 2023-05-25 14:58:01.000000 evadb-0.2.5/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.173961 evadb-0.2.5/test/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1106 2023-03-28 02:19:14.000000 evadb-0.2.5/test/executor/test_abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3989 2023-05-16 03:45:18.000000 evadb-0.2.5/test/executor/test_create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4227 2023-04-09 04:33:37.000000 evadb-0.2.5/test/executor/test_execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1275 2022-12-13 23:02:13.000000 evadb-0.2.5/test/executor/test_executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4650 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3890 2023-04-09 22:04:17.000000 evadb-0.2.5/test/executor/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2884 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10983 2023-05-16 03:45:18.000000 evadb-0.2.5/test/executor/test_plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1397 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/test_pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1817 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2752 2023-04-09 04:33:37.000000 evadb-0.2.5/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      847 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.173961 evadb-0.2.5/test/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3722 2023-03-28 02:19:14.000000 evadb-0.2.5/test/expression/test_abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5149 2023-03-19 05:07:03.000000 evadb-0.2.5/test/expression/test_aggregation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2975 2023-01-02 23:54:50.000000 evadb-0.2.5/test/expression/test_arithmetic.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5578 2023-01-02 23:54:53.000000 evadb-0.2.5/test/expression/test_comparison.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2867 2022-08-08 22:30:00.000000 evadb-0.2.5/test/expression/test_expression_tree.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7555 2023-04-01 16:09:26.000000 evadb-0.2.5/test/expression/test_expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2022-11-12 17:07:12.000000 evadb-0.2.5/test/expression/test_function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10242 2023-04-28 05:16:29.000000 evadb-0.2.5/test/expression/test_logical.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/integration_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/integration_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3585 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4522 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_chatgpt.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6167 2023-05-17 22:20:34.000000 evadb-0.2.5/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3886 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5158 2023-05-14 18:56:25.000000 evadb-0.2.5/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4839 2023-05-16 03:45:18.000000 evadb-0.2.5/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2358 2023-05-14 15:06:41.000000 evadb-0.2.5/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3361 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3183 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    16033 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3806 2023-05-12 03:48:38.000000 evadb-0.2.5/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2983 2023-05-14 15:06:41.000000 evadb-0.2.5/test/integration_tests/test_like.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    20932 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_load_pdf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7168 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2658 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10646 2023-05-16 03:45:18.000000 evadb-0.2.5/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14654 2023-06-02 21:04:24.000000 evadb-0.2.5/test/integration_tests/test_pytorch.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2953 2023-03-28 02:19:14.000000 evadb-0.2.5/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10469 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_reuse.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5210 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    30781 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_select_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3277 2023-05-07 22:24:29.000000 evadb-0.2.5/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14709 2023-05-17 22:20:34.000000 evadb-0.2.5/test/integration_tests/test_similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12062 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1574 2023-05-17 22:20:34.000000 evadb-0.2.5/test/markers.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2022-10-16 04:44:32.000000 evadb-0.2.5/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5919 2023-04-09 04:33:37.000000 evadb-0.2.5/test/models/storage/test_batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11653 2023-06-02 21:04:24.000000 evadb-0.2.5/test/optimizer/rules/test_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4195 2023-03-16 05:59:55.000000 evadb-0.2.5/test/optimizer/test_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2233 2023-05-25 14:58:01.000000 evadb-0.2.5/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4406 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2689 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1996 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1034 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5522 2023-05-25 14:58:01.000000 evadb-0.2.5/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2000 2023-01-07 03:29:08.000000 evadb-0.2.5/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13564 2023-05-17 22:20:34.000000 evadb-0.2.5/test/optimizer/test_statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36070 2023-05-17 22:20:34.000000 evadb-0.2.5/test/parser/test_parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7783 2023-05-17 22:20:34.000000 evadb-0.2.5/test/parser/test_parser_statements.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.2.5/test/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6292 2023-03-28 02:19:14.000000 evadb-0.2.5/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-04-01 16:09:26.000000 evadb-0.2.5/test/readers/test_csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8104 2023-05-07 22:24:29.000000 evadb-0.2.5/test/readers/test_decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-12 17:07:12.000000 evadb-0.2.5/test/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1268 2023-01-02 23:54:53.000000 evadb-0.2.5/test/server/test_command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5068 2023-06-01 22:37:10.000000 evadb-0.2.5/test/server/test_db_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2603 2023-06-01 22:37:10.000000 evadb-0.2.5/test/server/test_interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-05-23 15:21:38.000000 evadb-0.2.5/test/server/test_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4113 2023-05-07 22:24:29.000000 evadb-0.2.5/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4023 2023-03-28 02:19:14.000000 evadb-0.2.5/test/storage/test_video_storage.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3309 2023-05-16 03:45:18.000000 evadb-0.2.5/test/test_eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1294 2022-12-13 23:02:13.000000 evadb-0.2.5/test/test_eva_imports.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1841 2023-05-25 14:58:01.000000 evadb-0.2.5/test/test_eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-08-08 22:30:00.000000 evadb-0.2.5/test/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7429 2023-05-16 03:45:18.000000 evadb-0.2.5/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2137 2023-05-16 03:45:18.000000 evadb-0.2.5/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      648 2022-10-16 04:44:32.000000 evadb-0.2.5/test/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1842 2023-06-01 22:37:10.000000 evadb-0.2.5/test/udfs/ndarray/test_annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      849 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2410 2022-10-16 04:44:32.000000 evadb-0.2.5/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2012 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_flips.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1700 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2374 2023-04-28 05:16:29.000000 evadb-0.2.5/test/udfs/ndarray/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1675 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4412 2023-05-10 04:58:49.000000 evadb-0.2.5/test/udfs/test_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2154 2022-09-30 14:24:37.000000 evadb-0.2.5/test/udfs/test_emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3345 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/test_facenet_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2548 2022-10-30 19:28:39.000000 evadb-0.2.5/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2768 2023-05-09 19:58:04.000000 evadb-0.2.5/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17438 2023-05-16 03:45:18.000000 evadb-0.2.5/test/util.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4196 2023-04-28 05:16:29.000000 evadb-0.2.5/test/utils/test_generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2256 2023-03-28 02:19:14.000000 evadb-0.2.5/test/utils/test_timer.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1296 2023-05-25 14:58:01.000000 evadb-0.2.5/test/utils/test_xdist.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2022-06-26 17:11:46.000000 evadb-0.2.5/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.725496 evadb-0.2.6/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2022-08-11 16:20:33.000000 evadb-0.2.6/LICENSE.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 03:19:58.725496 evadb-0.2.6/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13539 2023-06-02 21:04:24.000000 evadb-0.2.6/README.md
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.665494 evadb-0.2.6/eva/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      645 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.665494 evadb-0.2.6/eva/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7778 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/binder/binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15552 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/binder/statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7997 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.665494 evadb-0.2.6/eva/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    18583 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3320 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/catalog_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8604 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.669494 evadb-0.2.6/eva/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      886 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/association_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4671 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/base_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5266 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3393 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2997 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3532 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4429 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2262 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4722 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2668 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2127 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/schema_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.669494 evadb-0.2.6/eva/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1167 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/base_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2873 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4571 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3669 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3078 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2826 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2476 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1936 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/catalog/sql_config.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.669494 evadb-0.2.6/eva/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5490 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4798 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/configuration/configuration_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1005 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/configuration/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      882 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      852 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/eva.yml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1997 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3246 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2140 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/executor/create_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5191 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1924 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7292 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4738 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2515 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1968 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3537 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/executor/exchange_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3017 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4366 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1522 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1591 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/function_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1759 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/groupby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1800 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/hash_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2255 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/join_build_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1661 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1583 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3086 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/load_csv_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1648 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6038 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1488 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4183 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8198 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/executor/plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1644 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1277 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/predicate_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1272 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/project_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2074 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/executor/ray_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1186 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1413 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1812 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2533 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/storage_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1264 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/union_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3916 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/executor/vector_index_scan_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5559 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3973 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/aggregation_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1618 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4351 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/comparison_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2542 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/constant_value_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10433 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10358 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3055 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/logical_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4685 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10769 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/interfaces/relational/db.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7278 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/interfaces/relational/relation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4472 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/interfaces/relational/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      633 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1332 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/catalog/frame_info.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      857 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/catalog/properties.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/models/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/server/response.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.677494 evadb-0.2.6/eva/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14841 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/models/storage/batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.681494 evadb-0.2.6/eva/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3259 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2129 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3450 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2669 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/group_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4335 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    37333 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/operators.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3837 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      982 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12582 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10874 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4102 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/plan_generator.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1169 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/property.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.681494 evadb-0.2.6/eva/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1019 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    49728 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/optimizer/rules/rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7440 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7534 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13726 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/optimizer/statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.685494 evadb-0.2.6/eva/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1360 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/alias.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2740 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/create_index_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2872 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5341 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/create_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4882 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/create_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2048 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1767 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1793 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19702 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/eva.lark
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1384 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2922 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/insert_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_parser.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.685494 evadb-0.2.6/eva/parser/lark_visitor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2655 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2161 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10824 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1404 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1202 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1006 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4672 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6231 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2465 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2241 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      932 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2143 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1112 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9469 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3214 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1227 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6248 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1460 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/show_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1426 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8637 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/table_ref.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1787 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/parser/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1689 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3453 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1455 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1930 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2469 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2076 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3603 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1660 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1532 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2057 2023-06-02 21:04:24.000000 evadb-0.2.6/eva/plan_nodes/exchange_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1033 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1755 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1712 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2179 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2023 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1468 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2710 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1510 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1564 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1177 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1249 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1469 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1760 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1201 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4419 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1421 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/union_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/plan_nodes/vector_index_scan_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2320 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/abstract_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2648 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5987 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/readers/document/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/document/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1467 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/document/document_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1979 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/document/registry.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/readers/image/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/image/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1067 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/image/opencv_image_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2050 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/readers/pdf_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      623 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3289 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/server/command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3263 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/server/interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2926 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/server/server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.693495 evadb-0.2.6/eva/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6133 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2383 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1713 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/document_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1717 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/image_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/pdf_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8972 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1941 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2496 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.697495 evadb-0.2.6/eva/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      605 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.697495 evadb-0.2.6/eva/third_party/huggingface/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      612 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1420 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6473 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/huggingface/create.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2615 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.697495 evadb-0.2.6/eva/third_party/vector_stores/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/vector_stores/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3284 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/vector_stores/faiss.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2960 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/vector_stores/qdrant.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1376 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/vector_stores/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1594 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/third_party/vector_stores/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.697495 evadb-0.2.6/eva/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/abstract/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2442 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3843 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3914 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/abstract/tracker_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3464 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/asl_action_recognition.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3413 2023-06-03 01:20:14.000000 evadb-0.2.6/eva/udfs/chatgpt.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2755 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3376 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2067 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/decorators/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5478 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2539 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/face_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5999 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1822 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1028 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3528 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/mnist_image_classifier.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2472 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2568 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1647 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1179 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2202 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/horizontal_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1557 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1782 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2139 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ndarray/vertical_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2750 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/sift_feature_extractor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/trackers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/trackers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2367 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/trackers/nor_fair.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.701495 evadb-0.2.6/eva/udfs/tutorials/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/tutorials/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7934 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3859 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/eva/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      611 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      909 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/errors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6966 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1956 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/kv_cache.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      985 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/logging_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1388 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/math_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1562 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/s3_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.6/eva/utils/stats.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-03 03:19:56.000000 evadb-0.2.6/eva/version.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/evadb.egg-info/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14107 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       88 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1329 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/requires.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       21 2023-06-03 03:19:58.000000 evadb-0.2.6/evadb.egg-info/top_level.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2022-06-26 17:11:46.000000 evadb-0.2.6/pyproject.toml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-03 03:19:58.725496 evadb-0.2.6/setup.cfg
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4575 2023-06-03 03:03:15.000000 evadb-0.2.6/setup.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/test/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-09-30 14:20:49.000000 evadb-0.2.6/test/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/test/benchmark_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:53.000000 evadb-0.2.6/test/benchmark_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1176 2023-05-09 19:58:04.000000 evadb-0.2.6/test/benchmark_tests/conftest.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6639 2023-05-12 03:48:38.000000 evadb-0.2.6/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/test/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2032 2023-01-02 23:54:53.000000 evadb-0.2.6/test/binder/test_binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13819 2023-06-01 22:37:10.000000 evadb-0.2.6/test/binder/test_statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7962 2023-05-16 03:45:18.000000 evadb-0.2.6/test/binder/test_statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/test/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/catalog/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.705495 evadb-0.2.6/test/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7234 2023-03-28 02:19:14.000000 evadb-0.2.6/test/catalog/models/test_models.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.709495 evadb-0.2.6/test/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-01-07 03:29:08.000000 evadb-0.2.6/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4794 2023-05-17 22:20:34.000000 evadb-0.2.6/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-03-28 02:19:14.000000 evadb-0.2.6/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-04-01 16:09:26.000000 evadb-0.2.6/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3210 2023-03-28 02:19:14.000000 evadb-0.2.6/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3035 2023-04-02 20:13:44.000000 evadb-0.2.6/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6808 2023-05-09 19:58:04.000000 evadb-0.2.6/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1402 2022-12-13 23:02:13.000000 evadb-0.2.6/test/catalog/test_column_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-04-01 16:09:26.000000 evadb-0.2.6/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.709495 evadb-0.2.6/test/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1486 2023-05-25 14:58:01.000000 evadb-0.2.6/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1620 2023-05-25 14:58:01.000000 evadb-0.2.6/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.709495 evadb-0.2.6/test/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1106 2023-03-28 02:19:14.000000 evadb-0.2.6/test/executor/test_abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3989 2023-05-16 03:45:18.000000 evadb-0.2.6/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4227 2023-04-09 04:33:37.000000 evadb-0.2.6/test/executor/test_execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1275 2022-12-13 23:02:13.000000 evadb-0.2.6/test/executor/test_executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4650 2023-01-02 23:54:50.000000 evadb-0.2.6/test/executor/test_limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3890 2023-04-09 22:04:17.000000 evadb-0.2.6/test/executor/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2884 2023-01-02 23:54:50.000000 evadb-0.2.6/test/executor/test_orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10983 2023-05-16 03:45:18.000000 evadb-0.2.6/test/executor/test_plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1397 2022-08-08 22:30:00.000000 evadb-0.2.6/test/executor/test_pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1817 2023-01-02 23:54:50.000000 evadb-0.2.6/test/executor/test_sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2752 2023-04-09 04:33:37.000000 evadb-0.2.6/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      847 2022-08-08 22:30:00.000000 evadb-0.2.6/test/executor/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.713495 evadb-0.2.6/test/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3722 2023-03-28 02:19:14.000000 evadb-0.2.6/test/expression/test_abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5149 2023-03-19 05:07:03.000000 evadb-0.2.6/test/expression/test_aggregation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2975 2023-01-02 23:54:50.000000 evadb-0.2.6/test/expression/test_arithmetic.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5578 2023-01-02 23:54:53.000000 evadb-0.2.6/test/expression/test_comparison.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2867 2022-08-08 22:30:00.000000 evadb-0.2.6/test/expression/test_expression_tree.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7555 2023-04-01 16:09:26.000000 evadb-0.2.6/test/expression/test_expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2022-11-12 17:07:12.000000 evadb-0.2.6/test/expression/test_function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10242 2023-04-28 05:16:29.000000 evadb-0.2.6/test/expression/test_logical.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/integration_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/integration_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3585 2023-05-09 19:58:04.000000 evadb-0.2.6/test/integration_tests/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4522 2023-05-09 19:58:04.000000 evadb-0.2.6/test/integration_tests/test_chatgpt.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6167 2023-05-17 22:20:34.000000 evadb-0.2.6/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3886 2023-06-01 22:37:10.000000 evadb-0.2.6/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5158 2023-05-14 18:56:25.000000 evadb-0.2.6/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4839 2023-05-16 03:45:18.000000 evadb-0.2.6/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2358 2023-05-14 15:06:41.000000 evadb-0.2.6/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3361 2023-05-25 14:58:01.000000 evadb-0.2.6/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3183 2023-04-09 04:33:37.000000 evadb-0.2.6/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    16033 2023-06-01 22:37:10.000000 evadb-0.2.6/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3806 2023-05-12 03:48:38.000000 evadb-0.2.6/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2983 2023-05-14 15:06:41.000000 evadb-0.2.6/test/integration_tests/test_like.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    20932 2023-05-25 14:58:01.000000 evadb-0.2.6/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-05-25 14:58:01.000000 evadb-0.2.6/test/integration_tests/test_load_pdf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7168 2023-06-01 22:37:10.000000 evadb-0.2.6/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2658 2023-05-09 19:58:04.000000 evadb-0.2.6/test/integration_tests/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10646 2023-05-16 03:45:18.000000 evadb-0.2.6/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14654 2023-06-02 21:04:24.000000 evadb-0.2.6/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2953 2023-03-28 02:19:14.000000 evadb-0.2.6/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10469 2023-05-25 14:58:01.000000 evadb-0.2.6/test/integration_tests/test_reuse.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5210 2023-04-09 04:33:37.000000 evadb-0.2.6/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    30781 2023-05-09 19:58:04.000000 evadb-0.2.6/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3277 2023-05-07 22:24:29.000000 evadb-0.2.6/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14709 2023-05-17 22:20:34.000000 evadb-0.2.6/test/integration_tests/test_similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12062 2023-04-09 04:33:37.000000 evadb-0.2.6/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1574 2023-05-17 22:20:34.000000 evadb-0.2.6/test/markers.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2022-10-16 04:44:32.000000 evadb-0.2.6/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5919 2023-04-09 04:33:37.000000 evadb-0.2.6/test/models/storage/test_batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/optimizer/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.6/test/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11653 2023-06-02 21:04:24.000000 evadb-0.2.6/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4195 2023-03-16 05:59:55.000000 evadb-0.2.6/test/optimizer/test_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2233 2023-05-25 14:58:01.000000 evadb-0.2.6/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4406 2022-08-08 22:30:00.000000 evadb-0.2.6/test/optimizer/test_cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2689 2022-08-08 22:30:00.000000 evadb-0.2.6/test/optimizer/test_group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1996 2022-08-08 22:30:00.000000 evadb-0.2.6/test/optimizer/test_memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1034 2022-08-08 22:30:00.000000 evadb-0.2.6/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5522 2023-05-25 14:58:01.000000 evadb-0.2.6/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2000 2023-01-07 03:29:08.000000 evadb-0.2.6/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13564 2023-05-17 22:20:34.000000 evadb-0.2.6/test/optimizer/test_statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36070 2023-05-17 22:20:34.000000 evadb-0.2.6/test/parser/test_parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7783 2023-05-17 22:20:34.000000 evadb-0.2.6/test/parser/test_parser_statements.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.2.6/test/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6292 2023-03-28 02:19:14.000000 evadb-0.2.6/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.717496 evadb-0.2.6/test/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-04-01 16:09:26.000000 evadb-0.2.6/test/readers/test_csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8104 2023-05-07 22:24:29.000000 evadb-0.2.6/test/readers/test_decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-12 17:07:12.000000 evadb-0.2.6/test/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1268 2023-01-02 23:54:53.000000 evadb-0.2.6/test/server/test_command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5068 2023-06-01 22:37:10.000000 evadb-0.2.6/test/server/test_db_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2603 2023-06-01 22:37:10.000000 evadb-0.2.6/test/server/test_interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-05-23 15:21:38.000000 evadb-0.2.6/test/server/test_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4113 2023-05-07 22:24:29.000000 evadb-0.2.6/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4023 2023-03-28 02:19:14.000000 evadb-0.2.6/test/storage/test_video_storage.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3309 2023-05-16 03:45:18.000000 evadb-0.2.6/test/test_eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1294 2022-12-13 23:02:13.000000 evadb-0.2.6/test/test_eva_imports.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1841 2023-05-25 14:58:01.000000 evadb-0.2.6/test/test_eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-08-08 22:30:00.000000 evadb-0.2.6/test/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.6/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.6/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7429 2023-05-16 03:45:18.000000 evadb-0.2.6/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2137 2023-05-16 03:45:18.000000 evadb-0.2.6/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.721496 evadb-0.2.6/test/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      648 2022-10-16 04:44:32.000000 evadb-0.2.6/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1842 2023-06-01 22:37:10.000000 evadb-0.2.6/test/udfs/ndarray/test_annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      849 2023-03-28 02:19:14.000000 evadb-0.2.6/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2410 2022-10-16 04:44:32.000000 evadb-0.2.6/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2012 2023-05-25 14:58:01.000000 evadb-0.2.6/test/udfs/ndarray/test_flips.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1700 2023-05-25 14:58:01.000000 evadb-0.2.6/test/udfs/ndarray/test_gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2374 2023-04-28 05:16:29.000000 evadb-0.2.6/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1675 2023-05-25 14:58:01.000000 evadb-0.2.6/test/udfs/ndarray/test_to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4412 2023-05-10 04:58:49.000000 evadb-0.2.6/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2154 2022-09-30 14:24:37.000000 evadb-0.2.6/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3345 2023-03-28 02:19:14.000000 evadb-0.2.6/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2548 2022-10-30 19:28:39.000000 evadb-0.2.6/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2768 2023-05-09 19:58:04.000000 evadb-0.2.6/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17438 2023-05-16 03:45:18.000000 evadb-0.2.6/test/util.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.725496 evadb-0.2.6/test/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.6/test/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4196 2023-04-28 05:16:29.000000 evadb-0.2.6/test/utils/test_generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2256 2023-03-28 02:19:14.000000 evadb-0.2.6/test/utils/test_timer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1296 2023-05-25 14:58:01.000000 evadb-0.2.6/test/utils/test_xdist.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 03:19:58.725496 evadb-0.2.6/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2022-06-26 17:11:46.000000 evadb-0.2.6/third_party/__init__.py
```

### Comparing `evadb-0.2.5/LICENSE.txt` & `evadb-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/PKG-INFO` & `evadb-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.5 Summary: EVA AI-Relational
+Metadata-Version: 2.1 Name: evadb Version: 0.2.6 Summary: EVA AI-Relational
 Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
 https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `evadb-0.2.5/README.md` & `evadb-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/__init__.py` & `evadb-0.2.6/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/binder/__init__.py` & `evadb-0.2.6/eva/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/binder/binder_utils.py` & `evadb-0.2.6/eva/binder/binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/binder/statement_binder.py` & `evadb-0.2.6/eva/binder/statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/binder/statement_binder_context.py` & `evadb-0.2.6/eva/binder/statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/__init__.py` & `evadb-0.2.6/eva/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/catalog_manager.py` & `evadb-0.2.6/eva/catalog/catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/catalog_type.py` & `evadb-0.2.6/eva/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/catalog_utils.py` & `evadb-0.2.6/eva/catalog/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/__init__.py` & `evadb-0.2.6/eva/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/association_models.py` & `evadb-0.2.6/eva/catalog/models/association_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/base_model.py` & `evadb-0.2.6/eva/catalog/models/base_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/column_catalog.py` & `evadb-0.2.6/eva/catalog/models/column_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/index_catalog.py` & `evadb-0.2.6/eva/catalog/models/index_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/table_catalog.py` & `evadb-0.2.6/eva/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.6/eva/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/udf_catalog.py` & `evadb-0.2.6/eva/catalog/models/udf_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.6/eva/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.6/eva/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.6/eva/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/schema_utils.py` & `evadb-0.2.6/eva/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/__init__.py` & `evadb-0.2.6/eva/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/base_service.py` & `evadb-0.2.6/eva/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.6/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/catalog/sql_config.py` & `evadb-0.2.6/eva/catalog/sql_config.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/configuration/__init__.py` & `evadb-0.2.6/eva/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/configuration/bootstrap_environment.py` & `evadb-0.2.6/eva/configuration/bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/configuration/configuration_manager.py` & `evadb-0.2.6/eva/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/configuration/constants.py` & `evadb-0.2.6/eva/configuration/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/constants.py` & `evadb-0.2.6/eva/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/eva.yml` & `evadb-0.2.6/eva/eva.yml`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/eva_cmd_client.py` & `evadb-0.2.6/eva/eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/eva_server.py` & `evadb-0.2.6/eva/eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/__init__.py` & `evadb-0.2.6/eva/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/abstract_executor.py` & `evadb-0.2.6/eva/executor/abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.6/eva/executor/apply_and_merge_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/create_executor.py` & `evadb-0.2.6/eva/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/create_index_executor.py` & `evadb-0.2.6/eva/executor/create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/create_mat_view_executor.py` & `evadb-0.2.6/eva/executor/create_mat_view_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/create_udf_executor.py` & `evadb-0.2.6/eva/executor/create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/delete_executor.py` & `evadb-0.2.6/eva/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/drop_executor.py` & `evadb-0.2.6/eva/executor/drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/drop_udf_executor.py` & `evadb-0.2.6/eva/executor/drop_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/exchange_executor.py` & `evadb-0.2.6/eva/executor/exchange_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/execution_context.py` & `evadb-0.2.6/eva/executor/execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/executor_utils.py` & `evadb-0.2.6/eva/executor/executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/explain_executor.py` & `evadb-0.2.6/eva/executor/explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/function_scan_executor.py` & `evadb-0.2.6/eva/executor/function_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/groupby_executor.py` & `evadb-0.2.6/eva/executor/groupby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/hash_join_executor.py` & `evadb-0.2.6/eva/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/insert_executor.py` & `evadb-0.2.6/eva/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/join_build_executor.py` & `evadb-0.2.6/eva/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/lateral_join_executor.py` & `evadb-0.2.6/eva/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/limit_executor.py` & `evadb-0.2.6/eva/executor/limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/load_csv_executor.py` & `evadb-0.2.6/eva/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/load_executor.py` & `evadb-0.2.6/eva/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/load_multimedia_executor.py` & `evadb-0.2.6/eva/executor/load_multimedia_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.6/eva/executor/nested_loop_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/orderby_executor.py` & `evadb-0.2.6/eva/executor/orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/plan_executor.py` & `evadb-0.2.6/eva/executor/plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/pp_executor.py` & `evadb-0.2.6/eva/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/predicate_executor.py` & `evadb-0.2.6/eva/executor/predicate_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/project_executor.py` & `evadb-0.2.6/eva/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/ray_utils.py` & `evadb-0.2.6/eva/executor/ray_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/rename_executor.py` & `evadb-0.2.6/eva/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/sample_executor.py` & `evadb-0.2.6/eva/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/seq_scan_executor.py` & `evadb-0.2.6/eva/executor/seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/show_info_executor.py` & `evadb-0.2.6/eva/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/storage_executor.py` & `evadb-0.2.6/eva/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/union_executor.py` & `evadb-0.2.6/eva/executor/union_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/executor/vector_index_scan_executor.py` & `evadb-0.2.6/eva/executor/vector_index_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/__init__.py` & `evadb-0.2.6/eva/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/abstract_expression.py` & `evadb-0.2.6/eva/expression/abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/aggregation_expression.py` & `evadb-0.2.6/eva/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/arithmetic_expression.py` & `evadb-0.2.6/eva/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/comparison_expression.py` & `evadb-0.2.6/eva/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/constant_value_expression.py` & `evadb-0.2.6/eva/expression/constant_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/expression_utils.py` & `evadb-0.2.6/eva/expression/expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/function_expression.py` & `evadb-0.2.6/eva/expression/function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/logical_expression.py` & `evadb-0.2.6/eva/expression/logical_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/expression/tuple_value_expression.py` & `evadb-0.2.6/eva/expression/tuple_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/interfaces/__init__.py` & `evadb-0.2.6/eva/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/interfaces/relational/__init__.py` & `evadb-0.2.6/eva/interfaces/relational/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/interfaces/relational/db.py` & `evadb-0.2.6/eva/interfaces/relational/db.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/interfaces/relational/relation.py` & `evadb-0.2.6/eva/interfaces/relational/relation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/interfaces/relational/utils.py` & `evadb-0.2.6/eva/interfaces/relational/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/__init__.py` & `evadb-0.2.6/eva/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/catalog/__init__.py` & `evadb-0.2.6/eva/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/catalog/frame_info.py` & `evadb-0.2.6/eva/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/catalog/properties.py` & `evadb-0.2.6/eva/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/server/__init__.py` & `evadb-0.2.6/eva/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/server/response.py` & `evadb-0.2.6/eva/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/storage/__init__.py` & `evadb-0.2.6/eva/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/models/storage/batch.py` & `evadb-0.2.6/eva/models/storage/batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/__init__.py` & `evadb-0.2.6/eva/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/binder.py` & `evadb-0.2.6/eva/optimizer/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/cost_model.py` & `evadb-0.2.6/eva/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/group.py` & `evadb-0.2.6/eva/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/group_expression.py` & `evadb-0.2.6/eva/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/memo.py` & `evadb-0.2.6/eva/optimizer/memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/operators.py` & `evadb-0.2.6/eva/optimizer/operators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/optimizer_context.py` & `evadb-0.2.6/eva/optimizer/optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.6/eva/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.6/eva/optimizer/optimizer_tasks.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/optimizer_utils.py` & `evadb-0.2.6/eva/optimizer/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/plan_generator.py` & `evadb-0.2.6/eva/optimizer/plan_generator.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/property.py` & `evadb-0.2.6/eva/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/rules/__init__.py` & `evadb-0.2.6/eva/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/rules/pattern.py` & `evadb-0.2.6/eva/optimizer/rules/pattern.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/rules/rules.py` & `evadb-0.2.6/eva/optimizer/rules/rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/rules/rules_base.py` & `evadb-0.2.6/eva/optimizer/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.6/eva/optimizer/rules/rules_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/optimizer/statement_to_opr_converter.py` & `evadb-0.2.6/eva/optimizer/statement_to_opr_converter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/__init__.py` & `evadb-0.2.6/eva/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/alias.py` & `evadb-0.2.6/eva/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/create_index_statement.py` & `evadb-0.2.6/eva/parser/create_index_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/create_mat_view_statement.py` & `evadb-0.2.6/eva/parser/create_mat_view_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/create_statement.py` & `evadb-0.2.6/eva/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/create_udf_statement.py` & `evadb-0.2.6/eva/parser/create_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/delete_statement.py` & `evadb-0.2.6/eva/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/drop_statement.py` & `evadb-0.2.6/eva/parser/drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/drop_udf_statement.py` & `evadb-0.2.6/eva/parser/drop_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/eva.lark` & `evadb-0.2.6/eva/parser/eva.lark`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/explain_statement.py` & `evadb-0.2.6/eva/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/insert_statement.py` & `evadb-0.2.6/eva/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_parser.py` & `evadb-0.2.6/eva/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.6/eva/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.6/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.6/eva/parser/lark_visitor/_create_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.6/eva/parser/lark_visitor/_expressions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.6/eva/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.6/eva/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.6/eva/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.6/eva/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.6/eva/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/load_statement.py` & `evadb-0.2.6/eva/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/parser.py` & `evadb-0.2.6/eva/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/rename_statement.py` & `evadb-0.2.6/eva/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/select_statement.py` & `evadb-0.2.6/eva/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/show_statement.py` & `evadb-0.2.6/eva/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/statement.py` & `evadb-0.2.6/eva/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/table_ref.py` & `evadb-0.2.6/eva/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/types.py` & `evadb-0.2.6/eva/parser/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/parser/utils.py` & `evadb-0.2.6/eva/parser/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/__init__.py` & `evadb-0.2.6/eva/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.6/eva/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.6/eva/plan_nodes/abstract_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.6/eva/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.6/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.6/eva/plan_nodes/create_index_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.6/eva/plan_nodes/create_mat_view_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/create_plan.py` & `evadb-0.2.6/eva/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.6/eva/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/delete_plan.py` & `evadb-0.2.6/eva/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/drop_plan.py` & `evadb-0.2.6/eva/plan_nodes/drop_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.6/eva/plan_nodes/drop_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/exchange_plan.py` & `evadb-0.2.6/eva/plan_nodes/exchange_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/explain_plan.py` & `evadb-0.2.6/eva/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.6/eva/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.6/eva/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.6/eva/plan_nodes/hash_join_build_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.6/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/insert_plan.py` & `evadb-0.2.6/eva/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.6/eva/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/limit_plan.py` & `evadb-0.2.6/eva/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.6/eva/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.6/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.6/eva/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/pp_plan.py` & `evadb-0.2.6/eva/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.6/eva/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/project_plan.py` & `evadb-0.2.6/eva/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/rename_plan.py` & `evadb-0.2.6/eva/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/sample_plan.py` & `evadb-0.2.6/eva/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.6/eva/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.6/eva/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/storage_plan.py` & `evadb-0.2.6/eva/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/types.py` & `evadb-0.2.6/eva/plan_nodes/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/union_plan.py` & `evadb-0.2.6/eva/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/plan_nodes/vector_index_scan_plan.py` & `evadb-0.2.6/eva/plan_nodes/vector_index_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/__init__.py` & `evadb-0.2.6/eva/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/abstract_reader.py` & `evadb-0.2.6/eva/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/csv_reader.py` & `evadb-0.2.6/eva/readers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/decord_reader.py` & `evadb-0.2.6/eva/readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/document/__init__.py` & `evadb-0.2.6/eva/readers/document/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/document/document_reader.py` & `evadb-0.2.6/eva/readers/document/document_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/document/registry.py` & `evadb-0.2.6/eva/readers/document/registry.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/image/__init__.py` & `evadb-0.2.6/eva/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.6/eva/readers/image/opencv_image_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/readers/pdf_reader.py` & `evadb-0.2.6/eva/readers/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/server/__init__.py` & `evadb-0.2.6/eva/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/server/command_handler.py` & `evadb-0.2.6/eva/server/command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/server/interpreter.py` & `evadb-0.2.6/eva/server/interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/server/server.py` & `evadb-0.2.6/eva/server/server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/__init__.py` & `evadb-0.2.6/eva/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.6/eva/storage/abstract_media_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/abstract_storage_engine.py` & `evadb-0.2.6/eva/storage/abstract_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/document_storage_engine.py` & `evadb-0.2.6/eva/storage/document_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/image_storage_engine.py` & `evadb-0.2.6/eva/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/pdf_storage_engine.py` & `evadb-0.2.6/eva/storage/pdf_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.6/eva/storage/sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/storage_engine.py` & `evadb-0.2.6/eva/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/storage/video_storage_engine.py` & `evadb-0.2.6/eva/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/__init__.py` & `evadb-0.2.6/eva/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/huggingface/__init__.py` & `evadb-0.2.6/eva/third_party/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/huggingface/binder.py` & `evadb-0.2.6/eva/third_party/huggingface/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/huggingface/create.py` & `evadb-0.2.6/eva/third_party/huggingface/create.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/huggingface/model.py` & `evadb-0.2.6/eva/third_party/huggingface/model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/vector_stores/__init__.py` & `evadb-0.2.6/eva/third_party/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/vector_stores/faiss.py` & `evadb-0.2.6/eva/third_party/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/vector_stores/qdrant.py` & `evadb-0.2.6/eva/third_party/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/vector_stores/types.py` & `evadb-0.2.6/eva/third_party/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/third_party/vector_stores/utils.py` & `evadb-0.2.6/eva/third_party/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/__init__.py` & `evadb-0.2.6/eva/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/abstract/__init__.py` & `evadb-0.2.6/eva/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.6/eva/udfs/abstract/abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.6/eva/udfs/abstract/hf_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.6/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/abstract/tracker_abstract_udf.py` & `evadb-0.2.6/eva/udfs/abstract/tracker_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/asl_action_recognition.py` & `evadb-0.2.6/eva/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/chatgpt.py` & `evadb-0.2.6/eva/udfs/chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/__init__.py` & `evadb-0.2.6/eva/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/decorators.py` & `evadb-0.2.6/eva/udfs/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.6/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.6/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.6/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/decorators/utils.py` & `evadb-0.2.6/eva/udfs/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/emotion_detector.py` & `evadb-0.2.6/eva/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/face_detector.py` & `evadb-0.2.6/eva/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.6/eva/udfs/fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/feature_extractor.py` & `evadb-0.2.6/eva/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/gpu_compatible.py` & `evadb-0.2.6/eva/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/mnist_image_classifier.py` & `evadb-0.2.6/eva/udfs/mnist_image_classifier.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.6/eva/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/__init__.py` & `evadb-0.2.6/eva/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/annotate.py` & `evadb-0.2.6/eva/udfs/ndarray/annotate.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/array_count.py` & `evadb-0.2.6/eva/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/crop.py` & `evadb-0.2.6/eva/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.6/eva/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/gaussian_blur.py` & `evadb-0.2.6/eva/udfs/ndarray/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/horizontal_flip.py` & `evadb-0.2.6/eva/udfs/ndarray/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/open.py` & `evadb-0.2.6/eva/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/similarity.py` & `evadb-0.2.6/eva/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/to_grayscale.py` & `evadb-0.2.6/eva/udfs/ndarray/to_grayscale.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ndarray/vertical_flip.py` & `evadb-0.2.6/eva/udfs/ndarray/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/ocr_extractor.py` & `evadb-0.2.6/eva/udfs/ocr_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/sift_feature_extractor.py` & `evadb-0.2.6/eva/udfs/sift_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/trackers/__init__.py` & `evadb-0.2.6/eva/udfs/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/trackers/nor_fair.py` & `evadb-0.2.6/eva/udfs/trackers/nor_fair.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/tutorials/__init__.py` & `evadb-0.2.6/eva/udfs/tutorials/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.6/eva/udfs/udf_bootstrap_queries.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/udfs/yolo_object_detector.py` & `evadb-0.2.6/eva/udfs/yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/__init__.py` & `evadb-0.2.6/eva/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/errors.py` & `evadb-0.2.6/eva/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/generic_utils.py` & `evadb-0.2.6/eva/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/kv_cache.py` & `evadb-0.2.6/eva/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/logging_manager.py` & `evadb-0.2.6/eva/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/math_utils.py` & `evadb-0.2.6/eva/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/s3_utils.py` & `evadb-0.2.6/eva/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/eva/utils/stats.py` & `evadb-0.2.6/eva/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/evadb.egg-info/PKG-INFO` & `evadb-0.2.6/evadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.5 Summary: EVA AI-Relational
+Metadata-Version: 2.1 Name: evadb Version: 0.2.6 Summary: EVA AI-Relational
 Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
 https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `evadb-0.2.5/evadb.egg-info/SOURCES.txt` & `evadb-0.2.6/evadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/evadb.egg-info/requires.txt` & `evadb-0.2.6/evadb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/setup.py` & `evadb-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/__init__.py` & `evadb-0.2.6/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/benchmark_tests/__init__.py` & `evadb-0.2.6/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/benchmark_tests/conftest.py` & `evadb-0.2.6/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.6/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/binder/__init__.py` & `evadb-0.2.6/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/binder/test_binder_utils.py` & `evadb-0.2.6/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/binder/test_statement_binder.py` & `evadb-0.2.6/test/binder/test_statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/binder/test_statement_binder_context.py` & `evadb-0.2.6/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/__init__.py` & `evadb-0.2.6/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/models/__init__.py` & `evadb-0.2.6/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/models/test_models.py` & `evadb-0.2.6/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/__init__.py` & `evadb-0.2.6/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.6/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/test_catalog_manager.py` & `evadb-0.2.6/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/test_column_type.py` & `evadb-0.2.6/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/catalog/test_sqlalchemy.py` & `evadb-0.2.6/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/configuration/__init__.py` & `evadb-0.2.6/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.6/test/configuration/test_bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/configuration/test_configuration_manager.py` & `evadb-0.2.6/test/configuration/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/__init__.py` & `evadb-0.2.6/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_abstract_executor.py` & `evadb-0.2.6/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_create_udf_executor.py` & `evadb-0.2.6/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_execution_context.py` & `evadb-0.2.6/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_executor_utils.py` & `evadb-0.2.6/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_limit_executor.py` & `evadb-0.2.6/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_load_executor.py` & `evadb-0.2.6/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_orderby_executor.py` & `evadb-0.2.6/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_plan_executor.py` & `evadb-0.2.6/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_pp_executor.py` & `evadb-0.2.6/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_sample_executor.py` & `evadb-0.2.6/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/test_seq_scan_executor.py` & `evadb-0.2.6/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/executor/utils.py` & `evadb-0.2.6/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/__init__.py` & `evadb-0.2.6/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_abstract_expression.py` & `evadb-0.2.6/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_aggregation.py` & `evadb-0.2.6/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_arithmetic.py` & `evadb-0.2.6/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_comparison.py` & `evadb-0.2.6/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_expression_tree.py` & `evadb-0.2.6/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_expression_utils.py` & `evadb-0.2.6/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_function_expression.py` & `evadb-0.2.6/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/expression/test_logical.py` & `evadb-0.2.6/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/__init__.py` & `evadb-0.2.6/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_array_count.py` & `evadb-0.2.6/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_chatgpt.py` & `evadb-0.2.6/test/integration_tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.6/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.6/test/integration_tests/test_create_table_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_delete_executor.py` & `evadb-0.2.6/test/integration_tests/test_delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_drop_executor.py` & `evadb-0.2.6/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.6/test/integration_tests/test_error_handling_with_ray.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_explain_executor.py` & `evadb-0.2.6/test/integration_tests/test_explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.6/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.6/test/integration_tests/test_huggingface_udfs.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_insert_executor.py` & `evadb-0.2.6/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_like.py` & `evadb-0.2.6/test/integration_tests/test_like.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_load_executor.py` & `evadb-0.2.6/test/integration_tests/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_load_pdf_executor.py` & `evadb-0.2.6/test/integration_tests/test_load_pdf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_mat_executor.py` & `evadb-0.2.6/test/integration_tests/test_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_open.py` & `evadb-0.2.6/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.6/test/integration_tests/test_optimizer_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_pytorch.py` & `evadb-0.2.6/test/integration_tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_rename_executor.py` & `evadb-0.2.6/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_reuse.py` & `evadb-0.2.6/test/integration_tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.6/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_select_executor.py` & `evadb-0.2.6/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.6/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_similarity.py` & `evadb-0.2.6/test/integration_tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/integration_tests/test_udf_executor.py` & `evadb-0.2.6/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/markers.py` & `evadb-0.2.6/test/markers.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/models/__init__.py` & `evadb-0.2.6/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/models/catalog/__init__.py` & `evadb-0.2.6/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/models/catalog/test_frame_info.py` & `evadb-0.2.6/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/models/storage/__init__.py` & `evadb-0.2.6/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/models/storage/test_batch.py` & `evadb-0.2.6/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/__init__.py` & `evadb-0.2.6/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/rules/__init__.py` & `evadb-0.2.6/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/rules/test_rules.py` & `evadb-0.2.6/test/optimizer/rules/test_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_binder.py` & `evadb-0.2.6/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.6/test/optimizer/test_cascade_optimizer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_cost_model.py` & `evadb-0.2.6/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_group.py` & `evadb-0.2.6/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_memo.py` & `evadb-0.2.6/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_optimizer_context.py` & `evadb-0.2.6/test/optimizer/test_optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_optimizer_task.py` & `evadb-0.2.6/test/optimizer/test_optimizer_task.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.6/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/optimizer/test_statement_to_opr_converter.py` & `evadb-0.2.6/test/optimizer/test_statement_to_opr_converter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/parser/__init__.py` & `evadb-0.2.6/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/parser/test_parser.py` & `evadb-0.2.6/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/parser/test_parser_statements.py` & `evadb-0.2.6/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/plan_nodes/__init__.py` & `evadb-0.2.6/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/plan_nodes/test_plan.py` & `evadb-0.2.6/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/readers/__init__.py` & `evadb-0.2.6/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/readers/test_csv_reader.py` & `evadb-0.2.6/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/readers/test_decord_reader.py` & `evadb-0.2.6/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/server/__init__.py` & `evadb-0.2.6/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/server/test_command_handler.py` & `evadb-0.2.6/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/server/test_db_api.py` & `evadb-0.2.6/test/server/test_db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/server/test_interpreter.py` & `evadb-0.2.6/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/server/test_server.py` & `evadb-0.2.6/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/storage/__init__.py` & `evadb-0.2.6/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.6/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/storage/test_video_storage.py` & `evadb-0.2.6/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/test_eva_cmd_client.py` & `evadb-0.2.6/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/test_eva_imports.py` & `evadb-0.2.6/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/test_eva_server.py` & `evadb-0.2.6/test/test_eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/__init__.py` & `evadb-0.2.6/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/decorators/__init__.py` & `evadb-0.2.6/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.6/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.6/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/decorators/test_decorators.py` & `evadb-0.2.6/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/__init__.py` & `evadb-0.2.6/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_annotate.py` & `evadb-0.2.6/test/udfs/ndarray/test_annotate.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.6/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_crop.py` & `evadb-0.2.6/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_flips.py` & `evadb-0.2.6/test/udfs/ndarray/test_flips.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_gaussian_blur.py` & `evadb-0.2.6/test/udfs/ndarray/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_open.py` & `evadb-0.2.6/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/ndarray/test_to_grayscale.py` & `evadb-0.2.6/test/udfs/ndarray/test_to_grayscale.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/test_abstract_udf.py` & `evadb-0.2.6/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/test_emotion_detector.py` & `evadb-0.2.6/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/test_facenet_udf.py` & `evadb-0.2.6/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.6/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.6/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/util.py` & `evadb-0.2.6/test/util.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/utils/__init__.py` & `evadb-0.2.6/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/utils/test_generic_utils.py` & `evadb-0.2.6/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/utils/test_timer.py` & `evadb-0.2.6/test/utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.5/test/utils/test_xdist.py` & `evadb-0.2.6/test/utils/test_xdist.py`

 * *Files identical despite different names*

