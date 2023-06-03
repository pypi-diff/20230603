# Comparing `tmp/summa_embed-0.15.8.tar.gz` & `tmp/summa_embed-0.15.9.tar.gz`

## Comparing `summa_embed-0.15.8.tar` & `summa_embed-0.15.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10419 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24648 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    16401 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1595 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    57848 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-05-31 18:46:00.000000 summa_embed-0.15.8/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.8/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-31 18:46:00.000000 summa_embed-0.15.8/.gitignore
--rwxr-xr-x   0      501       20      347 2023-05-31 18:46:00.000000 summa_embed-0.15.8/build.sh
--rw-r--r--   0      501       20      515 2023-05-31 18:46:00.000000 summa_embed-0.15.8/pyproject.toml
--rw-r--r--   0      501       20       14 2023-05-31 18:46:00.000000 summa_embed-0.15.8/requirements.txt
--rw-r--r--   0      501       20     4398 2023-05-31 18:46:00.000000 summa_embed-0.15.8/src/lib.rs
--rw-r--r--   0      501       20     1050 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16689 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20021 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    21461 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    29410 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-05-31 18:46:00.000000 summa_embed-0.15.8/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   102226 2023-05-31 18:48:32.000000 summa_embed-0.15.8/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.8/PKG-INFO
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.9/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10419 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.9/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24648 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14323 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    16401 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1595 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    57848 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.9/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-01 08:47:09.000000 summa_embed-0.15.9/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-06-01 08:47:09.000000 summa_embed-0.15.9/build.sh
+-rw-r--r--   0      501       20      515 2023-06-01 08:47:09.000000 summa_embed-0.15.9/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-06-01 08:47:09.000000 summa_embed-0.15.9/requirements.txt
+-rw-r--r--   0      501       20     4398 2023-06-01 08:47:09.000000 summa_embed-0.15.9/src/lib.rs
+-rw-r--r--   0      501       20     1082 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16689 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20021 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    21461 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    29410 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   102226 2023-06-01 08:47:30.000000 summa_embed-0.15.9/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.9/PKG-INFO
```

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.9/local_dependencies/summa-proto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.9/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.9/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.9/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.9/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.9/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.9/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.9/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.9/local_dependencies/summa-proto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.9/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.8"
+version = "0.15.9"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.9/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     }
     pub fn index(&self) -> &Index {
         match self {
             IndexWriterImpl::SameThread(writer) => &writer.index,
             IndexWriterImpl::Threaded(writer) => writer.index(),
         }
     }
-    pub fn merge_with_attributes(&mut self, segment_ids: &[SegmentId], segment_attributes: Option<serde_json::Value>) -> SummaResult<Option<SegmentMeta>> {
+    pub fn merge_with_attributes(&self, segment_ids: &[SegmentId], segment_attributes: Option<serde_json::Value>) -> SummaResult<Option<SegmentMeta>> {
         match self {
             IndexWriterImpl::SameThread(_) => {
                 unimplemented!()
             }
             IndexWriterImpl::Threaded(writer) => {
                 let target_segment = writer.merge_with_attributes(segment_ids, segment_attributes).wait()?;
                 writer.garbage_collect_files().wait()?;
@@ -231,15 +231,15 @@
         Ok(())
     }
 
     /// Merge segments into one.
     ///
     /// Also cleans deleted documents and do recompression. Possible to pass the only segment in `segment_ids` to do recompression or clean up.
     /// It is heavy operation that also blocks on `.await` so should be spawned if non-blocking behaviour is required
-    pub fn merge(&mut self, segment_ids: &[SegmentId], segment_attributes: Option<SummaSegmentAttributes>) -> SummaResult<Option<SegmentMeta>> {
+    pub fn merge(&self, segment_ids: &[SegmentId], segment_attributes: Option<SummaSegmentAttributes>) -> SummaResult<Option<SegmentMeta>> {
         info!(action = "merge_segments", segment_ids = ?segment_ids);
         let segment_meta = self.index_writer.merge_with_attributes(
             segment_ids,
             segment_attributes.map(|segment_attributes| serde_json::to_value(segment_attributes).expect("cannot serialize")),
         )?;
         info!(action = "merged_segments", segment_ids = ?segment_ids, merged_segment_meta = ?segment_meta);
         Ok(segment_meta)
@@ -253,15 +253,15 @@
         self.index_writer.commit()
     }
 
     pub fn rollback(&mut self) -> SummaResult<()> {
         self.index_writer.rollback()
     }
 
-    pub fn vacuum(&mut self, segment_attributes: Option<SummaSegmentAttributes>, excluded_segments: Vec<String>) -> SummaResult<()> {
+    pub fn vacuum(&self, segment_attributes: Option<SummaSegmentAttributes>, excluded_segments: Vec<String>) -> SummaResult<()> {
         let mut segments = self.index().searchable_segments()?;
         segments.sort_by_key(|segment| segment.meta().num_deleted_docs());
 
         let excluded_segments: HashSet<SegmentId, RandomState> = excluded_segments
             .into_iter()
             .map(|s| SegmentId::from_uuid_string(&s))
             .collect::<Result<_, _>>()
```

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.9/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/Cargo.toml` & `summa_embed-0.15.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.8"
+version = "0.15.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.15.8", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.9", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.8/.gitignore` & `summa_embed-0.15.9/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/pyproject.toml` & `summa_embed-0.15.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/src/lib.rs` & `summa_embed-0.15.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/__init__.py` & `summa_embed-0.15.9/summa_embed/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from typing import Dict, Optional
 
 from izihawa_utils.pb_to_json import ParseDict
 
-from .proto import search_service_pb2 as search_service_pb
-from .summa_embed_bin import IndexRegistry
+from .proto import index_service_pb2, search_service_pb2
+from .summa_embed_bin import IndexRegistry as IndexRegistryBin
 
 
-class SummaEmbed:
+class IndexRegistry:
     def __init__(self):
-        self.index_registry = IndexRegistry()
+        self.index_registry = IndexRegistryBin()
 
     def add(self, index_config, index_name: Optional[str] = None):
-        parsed_index_config = search_service_pb.IndexQuery()
+        parsed_index_config = index_service_pb2.IndexEngineConfig()
         ParseDict(index_config, parsed_index_config)
         return self.index_registry.add(parsed_index_config.SerializeToString(), index_name=index_name)
 
     def search(self, index_queries):
-        search_request = search_service_pb.SearchRequest()
+        search_request = search_service_pb2.SearchRequest()
         for index_query in index_queries:
             if isinstance(index_query, Dict):
                 dict_index_query = index_query
-                index_query = search_service_pb.IndexQuery()
+                index_query = search_service_pb2.IndexQuery()
                 ParseDict(dict_index_query, index_query)
             search_request.index_queries.append(index_query)
         return self.index_registry.search(search_request.SerializeToString())
-
```

### Comparing `summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/index_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/query_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/query_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/summa_embed/proto/utils_pb2.py` & `summa_embed-0.15.9/summa_embed/proto/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.8/Cargo.lock` & `summa_embed-0.15.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1220,15 +1220,15 @@
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipfs-hamt-directory"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "bincode",
  "bitvec",
  "cid 0.10.1",
  "fastmurmur3",
  "format-bytes",
@@ -1241,15 +1241,15 @@
  "sled",
  "summa-proto 0.26.0 (registry+https://github.com/rust-lang/crates.io-index)",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "ipfs-hamt-directory-py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "cid 0.10.1",
  "ipfs-hamt-directory",
  "multihash 0.18.1",
  "pyo3",
 ]
 
@@ -1888,15 +1888,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -2912,15 +2912,15 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.8"
+version = "0.15.9"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -2958,15 +2958,15 @@
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.15.8"
+version = "0.15.9"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
@@ -3131,15 +3131,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3187,38 +3187,38 @@
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.3.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -3233,44 +3233,44 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#0567a4b0fad647c6ffe4451f9be053e8b596a87b"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
```

