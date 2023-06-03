# Comparing `tmp/syft-0.8.1b4.tar.gz` & `tmp/syft-0.8.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b4.tar", last modified: Tue May 30 06:02:09 2023, max compression
+gzip compressed data, was "syft-0.8.1b5.tar", last modified: Sat Jun  3 12:39:18 2023, max compression
```

## Comparing `syft-0.8.1b4.tar` & `syft-0.8.1b5.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.360423 syft-0.8.1b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-30 05:59:36.000000 syft-0.8.1b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 05:59:36.000000 syft-0.8.1b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-30 06:02:09.360423 syft-0.8.1b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-30 05:59:36.000000 syft-0.8.1b4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 05:59:36.000000 syft-0.8.1b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-30 06:02:09.360423 syft-0.8.1b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 05:59:36.000000 syft-0.8.1b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.320423 syft-0.8.1b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.324422 syft-0.8.1b4/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 05:59:49.000000 syft-0.8.1b4/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-30 05:59:49.000000 syft-0.8.1b4/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.332423 syft-0.8.1b4/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.332423 syft-0.8.1b4/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.336423 syft-0.8.1b4/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.336423 syft-0.8.1b4/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.340423 syft-0.8.1b4/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.340423 syft-0.8.1b4/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.344423 syft-0.8.1b4/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42329 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.348423 syft-0.8.1b4/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.352423 syft-0.8.1b4/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.356423 syft-0.8.1b4/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    18931 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.360423 syft-0.8.1b4/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-30 05:59:36.000000 syft-0.8.1b4/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:02:09.328423 syft-0.8.1b4/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 06:02:09.000000 syft-0.8.1b4/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.619018 syft-0.8.1b5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-03 12:36:52.000000 syft-0.8.1b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 12:36:52.000000 syft-0.8.1b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-03 12:39:18.619018 syft-0.8.1b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-03 12:36:51.000000 syft-0.8.1b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 12:36:52.000000 syft-0.8.1b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-03 12:39:18.623018 syft-0.8.1b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-03 12:36:52.000000 syft-0.8.1b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.547017 syft-0.8.1b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.559017 syft-0.8.1b5/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-03 12:37:07.000000 syft-0.8.1b5/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-03 12:37:07.000000 syft-0.8.1b5/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.563017 syft-0.8.1b5/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.567017 syft-0.8.1b5/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.567017 syft-0.8.1b5/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.571017 syft-0.8.1b5/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.575017 syft-0.8.1b5/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.583017 syft-0.8.1b5/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.583017 syft-0.8.1b5/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.587017 syft-0.8.1b5/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.587017 syft-0.8.1b5/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40512 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.599018 syft-0.8.1b5/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.599018 syft-0.8.1b5/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.603018 syft-0.8.1b5/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.603018 syft-0.8.1b5/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.607018 syft-0.8.1b5/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.611018 syft-0.8.1b5/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.615018 syft-0.8.1b5/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.619018 syft-0.8.1b5/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.559017 syft-0.8.1b5/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b4/LICENSE` & `syft-0.8.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/PKG-INFO` & `syft-0.8.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b4
+Version: 0.8.1b5
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -28,15 +28,15 @@
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.9 - 3.10
+## Install syft on Python 3.9 - 3.11
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
@@ -84,17 +84,17 @@
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
+  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
 `0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
 `0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b4 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b5 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
@@ -11,15 +11,15 @@
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
 else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
+Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
 Domain ```python # from Jupyter / Python import syft as sy sy.requires
 (">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
 dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
 --name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
 8080 ``` ## Connect with our Python Client ```python import syft as sy
 sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
@@ -34,17 +34,17 @@
 to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
 a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
 `ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
 `#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
 `git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
 WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
 not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
 Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
-run this first: `pip install jaxlib==0.3.14 -f https://
+run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
 `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
 (Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
 - Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
```

### Comparing `syft-0.8.1b4/README.md` & `syft-0.8.1b5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.9 - 3.10
+## Install syft on Python 3.9 - 3.11
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
@@ -64,17 +64,17 @@
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
+  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
 `0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
 `0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
 else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
+Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
 Domain ```python # from Jupyter / Python import syft as sy sy.requires
 (">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
 dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
 --name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
 8080 ``` ## Connect with our Python Client ```python import syft as sy
 sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
@@ -25,17 +25,17 @@
 to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
 a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
 `ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
 `#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
 `git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
 WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
 not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
 Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
-run this first: `pip install jaxlib==0.3.14 -f https://
+run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
 `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
 (Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
 - Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
```

### Comparing `syft-0.8.1b4/setup.cfg` & `syft-0.8.1b5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.4"
+version = attr: "0.8.1-beta.5"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -21,20 +21,19 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 syft = 
 	astunparse==1.6.3
 	bcrypt==4.0.1
-	flax==0.5.3
 	forbiddenfruit==0.1.4
 	gevent==22.10.2
 	gipc==1.5.0
-	jax==0.3.14
-	jaxlib==0.3.14
+	jax==0.4.10
+	jaxlib==0.4.10
 	loguru==0.7.0
 	networkx==2.8
 	numpy==1.24.3
 	opendp==0.6.2
 	packaging>=21.0
 	pandas==1.5.3
 	pyarrow==11.0.0
@@ -50,14 +49,16 @@
 	tqdm==4.65.0
 	typeguard==2.13.3
 	typing_extensions==4.5.0
 	sherlock[redis,filelock]==0.4.1
 	uvicorn[standard]==0.21.1
 	fastapi==0.95.1
 	hagrid>=0.3
+	matplotlib==3.7.1
+	dm-haiku==0.0.9
 telemetry = 
 	opentelemetry-api==1.14.0
 	opentelemetry-sdk==1.14.0
 	opentelemetry-exporter-jaeger==1.14.0
 	opentelemetry-instrumentation==0.35b0
 	opentelemetry-instrumentation-requests==0.35b0
 install_requires = 
@@ -188,13 +189,13 @@
 [files]
 packages = 
 	syft
 data_files = 
 	img = img/*
 
 [mypy]
-python_version = 3.10
+python_version = 3.11
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `syft-0.8.1b4/src/syft/VERSION` & `syft-0.8.1b5/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.4"
+__version__ = "0.8.1-beta.5"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b4/src/syft/__init__.py` & `syft-0.8.1b5/src/syft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.4"
+__version__ = "0.8.1-beta.5"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.1b4/src/syft/abstract_node.py` & `syft-0.8.1b5/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/api.py` & `syft-0.8.1b5/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/client.py` & `syft-0.8.1b5/src/syft/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,16 +503,14 @@
                 institution=institution,
                 website=website,
             )
         except Exception as e:
             return SyftError(message=str(e))
         response = self.connection.register(new_user=new_user)
         if isinstance(response, tuple):
-            self.credentials = response[1].signing_key
-            self._fetch_api(self.credentials)
             response = response[0]
         return response
 
     @property
     def peer(self) -> Any:
         # relative
         from ..service.network.network_service import NodePeer
```

### Comparing `syft-0.8.1b4/src/syft/client/connection.py` & `syft-0.8.1b5/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/deploy.py` & `syft-0.8.1b5/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/registry.py` & `syft-0.8.1b5/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/search.py` & `syft-0.8.1b5/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/client/user_settings.py` & `syft-0.8.1b5/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/__init__.py` & `syft-0.8.1b5/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/__init__.py` & `syft-0.8.1b5/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/deployment.py` & `syft-0.8.1b5/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b5/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b5/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b5/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b5/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b5/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/gevent_patch.py` & `syft-0.8.1b5/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/node/credentials.py` & `syft-0.8.1b5/src/syft/node/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             return False
         return self.verify_key == other.verify_key
 
     def __repr__(self) -> str:
         return str(self)
 
     def __hash__(self) -> int:
-        return self.verify_key.__hash__()
+        return hash(self.verify_key)
 
 
 @serializable()
 class SyftSigningKey(SyftBaseModel):
     signing_key: SigningKey
 
     def __init__(self, signing_key: Union[str, SigningKey]) -> None:
@@ -77,15 +77,15 @@
         return f"<{SIGNING_KEY_FOR}: {self.verify}>"
 
     @property
     def verify(self) -> str:
         return str(self.verify_key)
 
     def __hash__(self) -> int:
-        return self.signing_key.__hash__()
+        return hash(self.signing_key)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, SyftSigningKey):
             return False
         return self.signing_key == other.signing_key
```

### Comparing `syft-0.8.1b4/src/syft/node/gateway.py` & `syft-0.8.1b5/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/node/node.py` & `syft-0.8.1b5/src/syft/node/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/node/routes.py` & `syft-0.8.1b5/src/syft/node/routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # stdlib
-from typing import Any
 from typing import Dict
 
 # third party
 from fastapi import APIRouter
 from fastapi import Body
 from fastapi import Depends
 from fastapi import Request
 from fastapi import Response
 from fastapi.responses import JSONResponse
 from loguru import logger
 from pydantic import ValidationError
+from typing_extensions import Annotated
 
 # relative
 from ..abstract_node import AbstractNode
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.serialize import _serialize as serialize
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
@@ -95,27 +95,27 @@
             serialize(result, to_bytes=True),
             media_type="application/octet-stream",
         )
 
     # make a request to the SyftAPI
     @router.post("/api_call")
     def syft_new_api_call(
-        request: Request, data: bytes = Depends(get_body)  # noqa: B008
+        request: Request, data: Annotated[bytes, Depends(get_body)]
     ) -> Response:
         if TRACE_MODE:
             with trace.get_tracer(syft_new_api_call.__module__).start_as_current_span(
                 syft_new_api_call.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
                 return handle_new_api_call(data)
         else:
             return handle_new_api_call(data)
 
-    def handle_login(email: str, password: str, node: AbstractNode) -> Any:
+    def handle_login(email: str, password: str, node: AbstractNode) -> Response:
         try:
             login_credentials = UserLoginCredentials(email=email, password=password)
         except ValidationError as e:
             return {"Error": e.json()}
 
         method = node.get_service_method(UserService.exchange_credentials)
         context = UnauthedServiceContext(node=node, login_credentials=login_credentials)
@@ -131,15 +131,15 @@
             response = user_private_key
 
         return Response(
             serialize(response, to_bytes=True),
             media_type="application/octet-stream",
         )
 
-    def handle_register(data: bytes, node: AbstractNode) -> Any:
+    def handle_register(data: bytes, node: AbstractNode) -> Response:
         user_create = deserialize(data, from_bytes=True)
 
         if not isinstance(user_create, UserCreate):
             raise Exception(f"Incorrect type received: {user_create}")
 
         context = NodeServiceContext(node=node)
         method = node.get_method_with_context(UserService.register, context)
@@ -157,31 +157,31 @@
             media_type="application/octet-stream",
         )
 
     # exchange email and password for a SyftSigningKey
     @router.post("/login", name="login", status_code=200)
     def login(
         request: Request,
-        email: str = Body(..., example="info@openmined.org"),  # noqa: B008
-        password: str = Body(..., example="changethis"),  # noqa: B008
-    ) -> Any:
+        email: Annotated[str, Body(example="info@openmined.org")],
+        password: Annotated[str, Body(example="changethis")],
+    ) -> Response:
         if TRACE_MODE:
             with trace.get_tracer(login.__module__).start_as_current_span(
                 login.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
                 return handle_login(email, password, worker)
         else:
             return handle_login(email, password, worker)
 
     @router.post("/register", name="register", status_code=200)
     def register(
-        request: Request, data: bytes = Depends(get_body)  # noqa: B008
-    ) -> Any:
+        request: Request, data: Annotated[bytes, Depends(get_body)]
+    ) -> Response:
         if TRACE_MODE:
             with trace.get_tracer(register.__module__).start_as_current_span(
                 register.__qualname__,
                 context=extract(request.headers),
                 kind=trace.SpanKind.SERVER,
             ):
                 return handle_register(data, worker)
```

### Comparing `syft-0.8.1b4/src/syft/node/run.py` & `syft-0.8.1b5/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/node/server.py` & `syft-0.8.1b5/src/syft/node/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,25 +124,28 @@
                     time.sleep(1)
             except KeyboardInterrupt:
                 try:
                     stop()
                 except SystemExit:
                     os._exit(130)
         else:
-            for _ in range(WAIT_TIME_SECONDS):
+            for i in range(WAIT_TIME_SECONDS):
                 try:
                     req = requests.get(
                         f"http://{host}:{port}{API_PATH}/metadata", timeout=0.5
                     )
                     if req.status_code == 200:
-                        print("Server Started")
+                        print(" Done.")
                         break
                 except Exception:
                     time.sleep(1)
-                    print("Waiting for server to start")
+                    if i == 0:
+                        print("Waiting for server to start", end="")
+                    else:
+                        print(".", end="")
 
     return start, stop
 
 
 def find_python_processes_on_port(port: int) -> List[int]:
     system = platform.system()
```

### Comparing `syft-0.8.1b4/src/syft/serde/array.py` & `syft-0.8.1b5/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/arrow.py` & `syft-0.8.1b5/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/deserialize.py` & `syft-0.8.1b5/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/lib_permissions.py` & `syft-0.8.1b5/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b5/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/mock.py` & `syft-0.8.1b5/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/recursive.py` & `syft-0.8.1b5/src/syft/serde/recursive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from enum import Enum
+from enum import EnumMeta
 import sys
 import types
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Set
@@ -38,40 +39,72 @@
             _type = annotations[key]
         else:
             for parent_cls in cls.mro():
                 sub_annotations = getattr(parent_cls, "__annotations__", None)
                 if sub_annotations and key in sub_annotations:
                     _type = sub_annotations[key]
         if _type is None:
-            print(f"Failed to find type for key: {key} in {cls}")
             return None
         types.append(_type)
     return types
 
 
+def check_fqn_alias(cls: Union[object, type]) -> Optional[tuple]:
+    """Currently, typing.Any has different metaclasses in different versions of Python 🤦‍♂️.
+    For Python <=3.10
+    Any is an instance of typing._SpecialForm
+
+    For Python >=3.11
+    Any is an instance of typing._AnyMeta
+    Hence adding both the aliases to the type bank.
+
+    This would cause issues, when the server and client
+    have different python versions.
+
+    As their serde is same, we can use the same serde for both of them.
+    with aliases for  fully qualified names in type bank
+
+    In a similar manner for Enum.
+
+    For Python<=3.10:
+    Enum is metaclass of enum.EnumMeta
+
+    For Python>=3.11:
+    Enum is metaclass of enum.EnumType
+    """
+    if cls == Any:
+        return ("typing._AnyMeta", "typing._SpecialForm")
+    if cls == EnumMeta:
+        return ("enum.EnumMeta", "enum.EnumType")
+
+    return None
+
+
 def recursive_serde_register(
     cls: Union[object, type],
     serialize: Optional[Callable] = None,
     deserialize: Optional[Callable] = None,
     serialize_attrs: Optional[List] = None,
     exclude_attrs: Optional[List] = None,
     inherit_attrs: Optional[bool] = True,
     inheritable_attrs: Optional[bool] = True,
 ) -> None:
     pydantic_fields = None
     base_attrs = None
     attribute_list: Set[str] = set()
 
+    alias_fqn = check_fqn_alias(cls)
     cls = type(cls) if not isinstance(cls, type) else cls
     fqn = f"{cls.__module__}.{cls.__name__}"
 
     nonrecursive = bool(serialize and deserialize)
     _serialize = serialize if nonrecursive else rs_object2proto
     _deserialize = deserialize if nonrecursive else rs_proto2object
     is_pydantic = issubclass(cls, BaseModel)
+    hash_exclude_attrs = getattr(cls, "__hash_exclude_attrs__", [])
 
     if inherit_attrs and not is_pydantic:
         # get attrs from base class
         base_attrs = getattr(cls, "__syft_serializable__", [])
         attribute_list.update(base_attrs)
 
     if is_pydantic and not serialize_attrs:
@@ -100,25 +133,32 @@
         cls.__syft_serializable__ = attribute_list
 
     attributes = set(list(attribute_list)) if attribute_list else None
     attribute_types = get_types(cls, attributes)
     serde_overrides = getattr(cls, "__serde_overrides__", {})
 
     # without fqn duplicate class names overwrite
-    TYPE_BANK[fqn] = (
+    serde_attributes = (
         nonrecursive,
         _serialize,
         _deserialize,
         attributes,
         exclude_attrs,
         serde_overrides,
+        hash_exclude_attrs,
         cls,
         attribute_types,
     )
 
+    TYPE_BANK[fqn] = serde_attributes
+
+    if isinstance(alias_fqn, tuple):
+        for alias in alias_fqn:
+            TYPE_BANK[alias] = serde_attributes
+
 
 def chunk_bytes(
     data: bytes, field_name: Union[str, int], builder: _DynamicStructBuilder
 ) -> None:
     CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
     list_size = len(data) // CHUNK_SIZE + 1
     data_lst = builder.init(field_name, list_size)
@@ -134,15 +174,15 @@
     # and move the bytes into it as we go
     bytes_value = b""
     for value in capnp_list:
         bytes_value += value
     return bytes_value
 
 
-def rs_object2proto(self: Any) -> _DynamicStructBuilder:
+def rs_object2proto(self: Any, for_hashing: bool = False) -> _DynamicStructBuilder:
     is_type = False
     if isinstance(self, type):
         is_type = True
 
     msg = recursive_scheme.new_message()
     fqn = get_fully_qualified_name(self)
     if fqn not in TYPE_BANK:
@@ -153,14 +193,15 @@
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         exclude_attrs_list,
         serde_overrides,
+        hash_exclude_attrs,
         cls,
         attribute_types,
     ) = TYPE_BANK[fqn]
 
     if nonrecursive or is_type:
         if serialize is None:
             raise Exception(
@@ -168,15 +209,18 @@
             )
         chunk_bytes(serialize(self), "nonrecursiveBlob", msg)
         return msg
 
     if attribute_list is None:
         attribute_list = self.__dict__.keys()
 
-    attribute_list = set(attribute_list) - set(exclude_attrs_list)
+    hash_exclude_attrs = hash_exclude_attrs if for_hashing else []
+    attribute_list = (
+        set(attribute_list) - set(exclude_attrs_list) - set(hash_exclude_attrs)
+    )
 
     msg.init("fieldsName", len(attribute_list))
     msg.init("fieldsData", len(attribute_list))
 
     for idx, attr_name in enumerate(sorted(attribute_list)):
         if not hasattr(self, attr_name):
             raise ValueError(
@@ -188,15 +232,15 @@
 
         if transforms is not None:
             field_obj = transforms[0](field_obj)
 
         if isinstance(field_obj, types.FunctionType):
             continue
 
-        serialized = sy.serialize(field_obj, to_bytes=True)
+        serialized = sy.serialize(field_obj, to_bytes=True, for_hashing=for_hashing)
         msg.fieldsName[idx] = attr_name
         chunk_bytes(serialized, idx, msg.fieldsData)
 
     return msg
 
 
 def rs_bytes2object(blob: bytes) -> Any:
@@ -246,14 +290,15 @@
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         exclude_attrs_list,
         serde_overrides,
+        hash_exclude_attrs,
         cls,
         attribute_types,
     ) = TYPE_BANK[proto.fullyQualifiedName]
 
     if class_type == type(None):
         # yes this looks stupid but it works and the opposite breaks
         class_type = cls
```

### Comparing `syft-0.8.1b4/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b5/src/syft/serde/recursive_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,8 +357,9 @@
             "__args__",
             "__module__",
             "__origin__",
         ],
     )
     recursive_serde_register_type(_SpecialGenericAlias)
 
+recursive_serde_register_type(Any)
 recursive_serde_register_type(EnumMeta)
```

### Comparing `syft-0.8.1b4/src/syft/serde/serializable.py` & `syft-0.8.1b5/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/signature.py` & `syft-0.8.1b5/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/serde/third_party.py` & `syft-0.8.1b5/src/syft/serde/third_party.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 from datetime import date
 from datetime import datetime
 from datetime import time
 from io import BytesIO
 
 # third party
 from dateutil import parser
-import flax
-from flax.core.frozen_dict import FrozenDict
 from jax import numpy as jnp
-from jaxlib.xla_extension import DeviceArray
+from jaxlib.xla_extension import ArrayImpl
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import networkx as nx
 from networkx import DiGraph
 import numpy as np
 from pandas import DataFrame
 from pandas import Series
@@ -145,28 +143,20 @@
     recursive_serde_register(Image)
 
 except Exception:  # nosec
     pass
 
 # jax
 recursive_serde_register(
-    DeviceArray,
+    ArrayImpl,
     serialize=lambda x: serialize(np.array(x), to_bytes=True),
     deserialize=lambda x: jnp.array(deserialize(x, from_bytes=True)),
 )
 
 
-recursive_serde_register(
-    FrozenDict,
-    serialize=lambda x: serialize(flax.serialization.to_state_dict(x), to_bytes=True),
-    deserialize=lambda x: FrozenDict(
-        flax.serialization.from_state_dict(FrozenDict, deserialize(x, from_bytes=True))
-    ),
-)
-
 # unsure why we have to register the object not the type but this works
 recursive_serde_register(np.core._ufunc_config._unspecified())
 
 recursive_serde_register(
     pydantic.networks.EmailStr,
     serialize=lambda x: x.encode(),
     deserialize=lambda x: pydantic.networks.EmailStr(x.decode()),
```

### Comparing `syft-0.8.1b4/src/syft/service/action/action_data_empty.py` & `syft-0.8.1b5/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_graph.py` & `syft-0.8.1b5/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_graph_service.py` & `syft-0.8.1b5/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_object.py` & `syft-0.8.1b5/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_permissions.py` & `syft-0.8.1b5/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_service.py` & `syft-0.8.1b5/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_store.py` & `syft-0.8.1b5/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/action_types.py` & `syft-0.8.1b5/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/numpy.py` & `syft-0.8.1b5/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/pandas.py` & `syft-0.8.1b5/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/plan.py` & `syft-0.8.1b5/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/action/verification.py` & `syft-0.8.1b5/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/code/unparse.py` & `syft-0.8.1b5/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/code/user_code.py` & `syft-0.8.1b5/src/syft/service/code/user_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ...client.api import NodeView
 from ...node.credentials import SyftVerifyKey
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.document_store import PartitionKey
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SyftHashableObject
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 from ..context import AuthedServiceContext
@@ -91,29 +92,23 @@
         return hash(self.value)
 
 
 # User Code status context for multiple approvals
 # To make nested dicts hashable for mongodb
 # as status is in attr_searchable
 @serializable(attrs=["base_dict"])
-class UserCodeStatusContext:
+class UserCodeStatusContext(SyftHashableObject):
     base_dict: Dict = {}
 
     def __init__(self, base_dict: Dict):
         self.base_dict = base_dict
 
     def __repr__(self):
         return str(self.base_dict)
 
-    def __hash__(self) -> int:
-        hash_sum = 0
-        for k, v in self.base_dict.items():
-            hash_sum = hash(k) + hash(v)
-        return hash_sum
-
     @property
     def approved(self) -> bool:
         # approved for this node only
         statuses = set(self.base_dict.values())
         return len(statuses) == 1 and UserCodeStatus.EXECUTE in statuses
 
     def for_context(self, context: AuthedServiceContext) -> UserCodeStatus:
```

### Comparing `syft-0.8.1b4/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b5/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/code/user_code_service.py` & `syft-0.8.1b5/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b5/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/context.py` & `syft-0.8.1b5/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b5/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b5/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b5/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b5/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/dataset/dataset.py` & `syft-0.8.1b5/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b5/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b5/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/message/message_service.py` & `syft-0.8.1b5/src/syft/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/message/message_stash.py` & `syft-0.8.1b5/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/message/messages.py` & `syft-0.8.1b5/src/syft/service/message/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b5/src/syft/service/metadata/node_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from ...types.syft_object import StorableObjectType
 from ...types.syft_object import SyftObject
 from ...types.transforms import convert_types
 from ...types.transforms import drop
 from ...types.transforms import rename
 from ...types.transforms import transform
 from ...types.uid import UID
-from ...util.util import recursive_hash
 
 
 def check_version(
     client_version: str, server_version: str, server_name: str, silent: bool = False
 ) -> bool:
     client_syft_version = version.parse(client_version)
     node_syft_version = version.parse(server_version)
@@ -78,28 +77,14 @@
     def check_version(self, client_version: str) -> None:
         return check_version(
             client_version=client_version,
             server_version=self.syft_version,
             server_name=self.name,
         )
 
-    def __hash__(self) -> int:
-        hashes = 0
-        hashes += recursive_hash(self.id)
-        hashes += recursive_hash(self.name)
-        hashes += recursive_hash(self.verify_key)
-        hashes += recursive_hash(self.highest_object_version)
-        hashes += recursive_hash(self.lowest_object_version)
-        hashes += recursive_hash(self.node_type)
-        hashes += recursive_hash(self.deployed_on)
-        hashes += recursive_hash(self.organization)
-        hashes += recursive_hash(self.on_board)
-        hashes += recursive_hash(self.description)
-        return hashes
-
 
 @serializable()
 class NodeMetadataJSON(BaseModel, StorableObjectType):
     metadata_version: int
     name: str
     id: str
     verify_key: str
```

### Comparing `syft-0.8.1b4/src/syft/service/network/network_service.py` & `syft-0.8.1b5/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/network/node_peer.py` & `syft-0.8.1b5/src/syft/service/network/node_peer.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ...client.client import SyftClient
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
-from ...util.util import recursive_hash
 from ..context import NodeServiceContext
 from ..metadata.node_metadata import NodeMetadata
 from .routes import NodeRoute
 from .routes import connection_to_route
 from .routes import route_to_connection
 
 
@@ -34,22 +33,14 @@
     vpn_auth_key: Optional[str] = None
     node_routes: List[NodeRoute] = []
 
     __attr_searchable__ = ["name"]
     __attr_unique__ = ["verify_key"]
     __attr_repr_cols__ = ["name"]
 
-    def __hash__(self) -> int:
-        hashes = 0
-        hashes += recursive_hash(self.id)
-        hashes += recursive_hash(self.name)
-        hashes += recursive_hash(self.verify_key)
-        hashes += recursive_hash(self.node_routes)
-        return hashes
-
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
         existing_routes = set(self.node_routes)
         for new_route in new_routes:
             if new_route not in existing_routes:
                 add_routes.append(new_route)
         self.node_routes += add_routes
```

### Comparing `syft-0.8.1b4/src/syft/service/network/routes.py` & `syft-0.8.1b5/src/syft/service/network/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,22 +71,14 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     host_or_ip: str
     private: bool = False
     protocol: str = "http"
     port: int = 80
 
-    def __hash__(self) -> int:
-        return (
-            hash(self.host_or_ip)
-            + hash(self.private)
-            + hash(self.protocol)
-            + hash(self.port)
-        )
-
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, HTTPNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
 
 @serializable()
@@ -112,21 +104,14 @@
         return node
 
     @staticmethod
     def with_node(self, node: AbstractNode) -> Self:
         worker_settings = WorkerSettings.from_node(node)
         return PythonNodeRoute(id=worker_settings.id, worker_settings=worker_settings)
 
-    def __hash__(self) -> int:
-        return (
-            hash(self.worker_settings.id)
-            + hash(self.worker_settings.name)
-            + hash(self.worker_settings.signing_key)
-        )
-
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, PythonNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
 
 def route_to_connection(
```

### Comparing `syft-0.8.1b4/src/syft/service/policy/policy.py` & `syft-0.8.1b5/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/policy/policy_service.py` & `syft-0.8.1b5/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b5/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/project/project.py` & `syft-0.8.1b5/src/syft/service/project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 # relative
 from ...client.client import SyftClient
 from ...client.client import SyftClientSessionCache
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
-from ...serde.serialize import _serialize
 from ...service.metadata.node_metadata import NodeMetadata
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
 from ...types.transforms import transform
@@ -55,17 +54,14 @@
 class Identity(SyftObject):
     __canonical_name__ = "Identity"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     verify_key: SyftVerifyKey
 
-    def __hash__(self) -> int:
-        return hash(str(self.id) + str(self.verify_key))
-
     __attr_repr_cols__ = ["id", "verify_key"]
 
     def __repr__(self) -> str:
         verify_key_str = f"{self.verify_key}"
         id_str = f"{self.id}"
         return f"<🔑 {verify_key_str[0:8]} @ 🟢 {id_str[0:8]}>"
 
@@ -96,70 +92,71 @@
     return [keep(["id", "verify_key"])]
 
 
 class ProjectEvent(SyftObject):
     __canonical_name__ = "ProjectEvent"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    __hash_exclude_attrs__ = [
+        "event_hash",
+        "signature",
+    ]
+
     # 1. Creation attrs
     id: UID
     timestamp: DateTime
     allowed_sub_types: Optional[List] = []
     # 2. Rebase attrs
     project_id: Optional[UID]
     seq_no: Optional[int]
     prev_event_uid: Optional[UID]
-    prev_event_hash: Optional[int]
-    event_hash: Optional[int]
+    prev_event_hash: Optional[str]
+    event_hash: Optional[str]
     # 3. Signature attrs
     creator_verify_key: Optional[SyftVerifyKey]
-    signature: Optional[bytes]  # dont use in signature
+    signature: Optional[bytes]  # dont use in signing
 
     @pydantic.root_validator(pre=True)
     def make_timestamp(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "timestamp" not in values or values["timestamp"] is None:
             values["timestamp"] = DateTime.now()
         return values
 
     def _pre_add_update(self, project: Project) -> None:
         pass
 
-    def __hash__(self) -> int:
-        return type(self).calculate_hash(self, self.__hash_keys__)
-
     def rebase(self, project: Project) -> Self:
         prev_event = project.events[-1] if project.events else None
         self.project_id = project.id
 
         if prev_event:
             self.prev_event_uid = prev_event.id
             self.prev_event_hash = prev_event.event_hash
             self.seq_no = prev_event.seq_no + 1
         else:
             self.prev_event_uid = project.id
             self.prev_event_hash = project.start_hash
             self.seq_no = 1
 
-        # make sure these are reset
-        self.event_hash = None
-        self.signature = None
-
-        self.event_hash = hash(self)  # recalculate it
         return self
 
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.signature is None:
             return SyftError(message="Sign event first")
         try:
-            signature = self.signature
-            self.signature = None
-            signed_bytes = _serialize(self, to_bytes=True)
-            self.creator_verify_key.verify_key.verify(signed_bytes, signature)
-            self.signature = signature
+            # Recompute hash
+            event_hash_bytes = self.__sha256__()
+            current_hash = event_hash_bytes.hex()
+            if current_hash != self.event_hash:
+                raise Exception(
+                    f"Event hash {current_hash} does not match {self.event_hash}"
+                )
+
+            self.creator_verify_key.verify_key.verify(event_hash_bytes, self.signature)
             return SyftSuccess(message="Event signature is valid")
         except Exception as e:
             return SyftError(message=f"Failed to validate message. {e}")
 
     def valid_descendant(
         self, project: Project, prev_event: Optional[Self]
     ) -> Union[SyftSuccess, SyftError]:
@@ -210,17 +207,20 @@
 
     def sign(self, signing_key: SyftSigningKey) -> None:
         if self.creator_verify_key != signing_key.verify_key:
             raise Exception(
                 f"creator_verify_key has changed from: {self.creator_verify_key} to "
                 f"{signing_key.verify_key}"
             )
-        self.signature = None
-        signed_bytes = _serialize(self, to_bytes=True)
-        signed_obj = signing_key.signing_key.sign(signed_bytes)
+        # Calculate Hash
+        event_hash_bytes = self.__sha256__()
+        self.event_hash = event_hash_bytes.hex()
+
+        # Sign Hash
+        signed_obj = signing_key.signing_key.sign(event_hash_bytes)
         self.signature = signed_obj._signature
 
     def publish(self, project: Project) -> Union[SyftSuccess, SyftError]:
         try:
             result = project.add_event(self)
             return result
         except EventAlreadyAddedException:  # nosec
@@ -256,81 +256,43 @@
 @serializable()
 class ProjectThreadMessage(ProjectSubEvent):
     __canonical_name__ = "ProjectThreadMessage"
     __version__ = SYFT_OBJECT_VERSION_1
 
     message: str
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "parent_event_id",
-        "prev_event_uid",
-        "prev_event_hash",
-        "message",
-    ]
-
 
 @serializable()
 class ProjectMessage(ProjectEventAddObject):
     __canonical_name__ = "ProjectMessage"
     __version__ = SYFT_OBJECT_VERSION_1
 
     message: str
     allowed_sub_types: List[Type] = [ProjectThreadMessage]
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "prev_event_uid",
-        "prev_event_hash",
-        "message",
-    ]
-
     def reply(self, message: str) -> ProjectMessage:
         return ProjectThreadMessage(message=message, parent_event_id=self.id)
 
 
 @serializable()
 class ProjectRequestResponse(ProjectSubEvent):
     __canonical_name__ = "ProjectRequestResponse"
     __version__ = SYFT_OBJECT_VERSION_1
 
     response: bool
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "parent_event_id",
-        "prev_event_uid",
-        "prev_event_hash",
-        "response",
-    ]
-
 
 @serializable()
 class ProjectRequest(ProjectEventAddObject):
     __canonical_name__ = "ProjectRequest"
     __version__ = SYFT_OBJECT_VERSION_1
 
     request: Request
     allowed_sub_types: List[Type] = [ProjectRequestResponse]
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "prev_event_uid",
-        "prev_event_hash",
-        "request",
-    ]
-
     def approve(self) -> ProjectRequestResponse:
         result = self.request.approve()
         if isinstance(result, SyftError):
             return result
         return ProjectRequestResponse(response=True, parent_event_id=self.id)
 
     # TODO: To add deny requests, when deny functionality is added
@@ -551,24 +513,14 @@
 @serializable()
 class AnswerProjectPoll(ProjectSubEvent):
     __canonical_name__ = "AnswerProjectPoll"
     __version__ = SYFT_OBJECT_VERSION_1
 
     answer: int
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "parent_event_id",
-        "prev_event_uid",
-        "prev_event_hash",
-        "answer",
-    ]
-
 
 @serializable()
 class ProjectMultipleChoicePoll(ProjectEventAddObject):
     __canonical_name__ = "ProjectPoll"
     __version__ = SYFT_OBJECT_VERSION_1
 
     question: str
@@ -577,24 +529,14 @@
 
     @validator("choices")
     def choices_min_length(cls, v):
         if len(v) < 1:
             raise ValueError("choices must have at least one item")
         return v
 
-    __hash_keys__ = [
-        "id",
-        "timestamp",
-        "creator_verify_key",
-        "prev_event_uid",
-        "prev_event_hash",
-        "question",
-        "choices",
-    ]
-
     def answer(self, answer: int) -> ProjectMessage:
         return AnswerProjectPoll(answer=answer, parent_event_id=self.id)
 
     def status(
         self, project: Project, pretty_print: bool = True
     ) -> Union[Dict, SyftError]:
         """Returns the status of the poll
@@ -664,36 +606,22 @@
     state_sync_leader: NodeIdentity
     leader_node_peer: Optional[NodePeer]
     consensus_model: ConsensusModel
     store: Dict[UID, Dict[UID, SyftObject]] = {}
     permissions: Dict[UID, Dict[UID, Set[str]]] = {}
     events: List[ProjectEvent] = []
     event_id_hashmap: Dict[UID, ProjectEvent] = {}
-    start_hash: int
+    start_hash: Optional[str]
     # WARNING:  Do not add it to hash keys , or print directly
     user_signing_key: Optional[SyftSigningKey] = None
     user_email_address: Optional[str] = None
     users: List[UserIdentity] = []
 
     __attr_repr_cols__ = ["name", "shareholders", "state_sync_leader"]
-    __hash_keys__ = [
-        "id",
-        "name",
-        "description",
-        "shareholders",
-        "project_permissions",
-        "state_sync_leader",
-        "consensus_model",
-        "store",
-        "permissions",
-        "events",
-    ]
-
-    def __hash__(self) -> int:
-        return type(self).calculate_hash(self, self.__hash_keys__)
+    __hash_exclude_attrs__ = ["user_signing_key", "start_hash"]
 
     def _broadcast_event(
         self, project_event: ProjectEvent
     ) -> Union[SyftSuccess, SyftError]:
         leader_client = self.get_leader_client(self.user_signing_key)
 
         return leader_client.api.services.project.broadcast_event(project_event)
@@ -1242,20 +1170,10 @@
             add_shareholders_as_owners(context.output["shareholders"])
         )
         context.output["project_permissions"] = project_permissions
 
     return context
 
 
-def calculate_final_hash(context: TransformContext) -> TransformContext:
-    context.output["store"] = {}
-    context.output["permissions"] = {}
-    context.output["events"] = []
-
-    start_hash = Project.calculate_hash(context.output, Project.__hash_keys__)
-    context.output["start_hash"] = start_hash
-    return context
-
-
 @transform(ProjectSubmit, Project)
 def new_projectsubmit_to_project() -> List[Callable]:
-    return [elect_leader, check_permissions, calculate_final_hash]
+    return [elect_leader, check_permissions]
```

### Comparing `syft-0.8.1b4/src/syft/service/project/project_service.py` & `syft-0.8.1b5/src/syft/service/project/project_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,17 @@
                 # the route is then validated by the leader
                 leader_node_peer = project.leader_node_route.validate_with_context(
                     context=context
                 )
 
             project_obj.leader_node_peer = leader_node_peer
 
+            # This should always be the last call before flushing to DB
+            project_obj.start_hash = project_obj.hash()
+
             result = self.stash.set(context.credentials, project_obj)
             if result.is_err():
                 return SyftError(message=str(result.err()))
 
             project_obj_store = result.ok()
             project_obj_store = add_signing_key_to_project(context, project_obj_store)
```

### Comparing `syft-0.8.1b4/src/syft/service/project/project_stash.py` & `syft-0.8.1b5/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/queue/base_queue.py` & `syft-0.8.1b5/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/queue/queue.py` & `syft-0.8.1b5/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b5/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/queue/zmq_queue.py` & `syft-0.8.1b5/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/request/request.py` & `syft-0.8.1b5/src/syft/service/request/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/request/request_service.py` & `syft-0.8.1b5/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/request/request_stash.py` & `syft-0.8.1b5/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/response.py` & `syft-0.8.1b5/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/service.py` & `syft-0.8.1b5/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/settings/settings.py` & `syft-0.8.1b5/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/settings/settings_service.py` & `syft-0.8.1b5/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/settings/settings_stash.py` & `syft-0.8.1b5/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/user/user.py` & `syft-0.8.1b5/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/user/user_roles.py` & `syft-0.8.1b5/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/user/user_service.py` & `syft-0.8.1b5/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/user/user_stash.py` & `syft-0.8.1b5/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/vpn/headscale_client.py` & `syft-0.8.1b5/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.1b5/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/service/vpn/vpn.py` & `syft-0.8.1b5/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/dict_document_store.py` & `syft-0.8.1b5/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/document_store.py` & `syft-0.8.1b5/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/kv_document_store.py` & `syft-0.8.1b5/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/linked_obj.py` & `syft-0.8.1b5/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/locks.py` & `syft-0.8.1b5/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/mongo_client.py` & `syft-0.8.1b5/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/mongo_codecs.py` & `syft-0.8.1b5/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/mongo_document_store.py` & `syft-0.8.1b5/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b5/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/datetime.py` & `syft-0.8.1b5/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/grid_url.py` & `syft-0.8.1b5/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/syft_metaclass.py` & `syft-0.8.1b5/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/syft_object.py` & `syft-0.8.1b5/src/syft/types/syft_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from collections import defaultdict
+from hashlib import sha256
 import inspect
 from inspect import Signature
 import types
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
@@ -27,15 +28,14 @@
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.recursive_primitives import recursive_serde_register_type
 from ..serde.serialize import _serialize as serialize
 from ..util.autoreload import autoreload_enabled
 from ..util.util import aggressive_set_attr
 from ..util.util import full_name_with_qualname
 from ..util.util import get_qualname_for
-from ..util.util import recursive_hash
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 
@@ -136,15 +136,29 @@
             f"the registry: {cls.__object_transform_registry__.keys()}"
         )
 
 
 print_type_cache = defaultdict(list)
 
 
-class SyftObject(SyftBaseObject, SyftObjectRegistry):
+class SyftHashableObject:
+    __hash_exclude_attrs__ = []
+
+    def __hash__(self) -> int:
+        return int.from_bytes(self.__sha256__(), byteorder="big")
+
+    def __sha256__(self) -> bytes:
+        _bytes = serialize(self, to_bytes=True, for_hashing=True)
+        return sha256(_bytes).digest()
+
+    def hash(self) -> str:
+        return self.__sha256__().hex()
+
+
+class SyftObject(SyftBaseObject, SyftObjectRegistry, SyftHashableObject):
     __canonical_name__ = "SyftObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     class Config:
         arbitrary_types_allowed = True
 
     # all objects have a UID
@@ -349,14 +363,18 @@
                     )
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self._syft_set_validate_private_attrs_(**kwargs)
         self.__post_init__()
 
+    # TODO: Check why Pydantic is removing the __hash__ method during inheritance
+    def __hash__(self) -> int:
+        return int.from_bytes(self.__sha256__(), byteorder="big")
+
     @classmethod
     def _syft_keys_types_dict(cls, attr_name: str) -> Dict[str, type]:
         kt_dict = {}
         for key in getattr(cls, attr_name, []):
             if key in cls.__fields__:
                 type_ = cls.__fields__[key].type_
             else:
@@ -381,25 +399,14 @@
     def _syft_unique_keys_dict(cls) -> Dict[str, type]:
         return cls._syft_keys_types_dict("__attr_unique__")
 
     @classmethod
     def _syft_searchable_keys_dict(cls) -> Dict[str, type]:
         return cls._syft_keys_types_dict("__attr_searchable__")
 
-    @staticmethod
-    def calculate_hash(obj: Any, keys: List[str]) -> int:
-        hashes = 0
-        for key in keys:
-            if isinstance(obj, dict):
-                value = obj[key]
-            else:
-                value = getattr(obj, key)
-            hashes += recursive_hash(value)
-        return hashes
-
 
 def list_dict_repr_html(self) -> str:
     try:
         max_check = 1
         items_checked = 0
         has_syft = False
         extra_fields = []
```

### Comparing `syft-0.8.1b4/src/syft/types/transforms.py` & `syft-0.8.1b5/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/twin_object.py` & `syft-0.8.1b5/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/types/uid.py` & `syft-0.8.1b5/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/autoreload.py` & `syft-0.8.1b5/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/decorators.py` & `syft-0.8.1b5/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/experimental_flags.py` & `syft-0.8.1b5/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/filterwarnings.py` & `syft-0.8.1b5/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/logger.py` & `syft-0.8.1b5/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/schema.py` & `syft-0.8.1b5/src/syft/util/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             _type = cls.__annotations__[key]
         else:
             for parent_cls in cls.mro():
                 annotations = getattr(parent_cls, "__annotations__", None)
                 if annotations and key in annotations:
                     _type = annotations[key]
         if _type is None:
-            print(f"Failed to find type for key: {key} in {cls}")
+            # print(f"Failed to find type for key: {key} in {cls}")
             return None
         types.append(_type)
     return dict(zip(keys, types))
 
 
 def convert_attribute_types(cls, attribute_list, attribute_types):
     jsonschema = {}
```

### Comparing `syft-0.8.1b4/src/syft/util/telemetry.py` & `syft-0.8.1b5/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/trace_decorator.py` & `syft-0.8.1b5/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft/util/util.py` & `syft-0.8.1b5/src/syft/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 # third party
 from forbiddenfruit import curse
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
 import requests
 
 # relative
-from ..serde.serialize import _serialize
 from .logger import critical
 from .logger import debug
 from .logger import error
 from .logger import traceback_and_raise
 
 DATASETS_URL = "https://raw.githubusercontent.com/OpenMined/datasets/main"
 PANDAS_DATA = f"{DATASETS_URL}/pandas_cookbook"
@@ -830,36 +829,14 @@
     try:
         shell = get_ipython().__class__.__module__
         return shell
     except NameError:
         return "StandardInterpreter"  # not sure
 
 
-def recursive_hash(obj: Any) -> int:
-    hashes = 0
-    if isinstance(obj, (list, dict, set)):
-        if isinstance(obj, (list, set)):
-            for item in obj:
-                hashes += recursive_hash(item)
-        elif isinstance(obj, dict):
-            for item_key, item in obj:
-                hashes += recursive_hash(item_key)
-                hashes += recursive_hash(item)
-    else:
-        # TODO: remove the generic python hash from other checks and use a more secure one
-        # As the python hash does not produce unique hashes for different runs
-        # and also for different python versions
-        # to be modified in the hashing PR
-        # Adding a temp fix for now
-        serde_bytes = _serialize(obj, to_bytes=True)
-        hash_bytes = hashlib.sha256(serde_bytes).digest()
-        hashes += int.from_bytes(hash_bytes, byteorder="big")
-    return hashes
-
-
 if os_name() == "macOS":
     # needed on MacOS to prevent [__NSCFConstantString initialize] may have been in
     # progress in another thread when fork() was called.
     multiprocessing.set_start_method("spawn", True)
 
 
 def thread_ident() -> int:
```

### Comparing `syft-0.8.1b4/src/syft/util/version_compare.py` & `syft-0.8.1b5/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b5/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b4
+Version: 0.8.1b5
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -28,15 +28,15 @@
 
 Perform `numpy`-like analysis on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
 
-## Install syft on Python 3.9 - 3.10
+## Install syft on Python 3.9 - 3.11
 
 ```bash
 $ pip install -U syft -f https://whls.blob.core.windows.net/unstable/index.html
 ```
 
 ## Launch a python dev Domain
 
@@ -84,17 +84,17 @@
 - `#support` on <a href="https://slack.openmined.org/">Slack</a>
 
 # Install Notes
 
 - HAGrid 0.3 Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
   †`Windows` does not support `ansible`, preventing some remote deployment targets
-- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.10` - Run: `pip install -U syft`  
+- PySyft 0.8 Requires: 🐍 `python 3.9 - 3.11` - Run: `pip install -U syft`  
   \*`macOS` Apple Silicon users might need cmake: `brew install cmake`  
-  ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
+  ‡`Windows` users must run this first: `pip install jaxlib==0.4.10 -f https://whls.blob.core.windows.net/unstable/index.html`
 - PyGrid Requires: 🐳 `docker` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`
 
 # Versions
 
 `0.8.1` (Beta) - `dev` branch 👈🏽 <a href="/notebooks/api/0.8">API</a>  
 `0.8.0` (Stable) - <a href="/notebooks/api/0.8">API</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b4 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b5 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
@@ -11,15 +11,15 @@
 img.shields.io/badge/docker-images-blue?logo=docker] [https://github.com/
 OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev] [https:/
 /img.shields.io/badge/chat-on%20slack-purple?logo=slack] [https://
 img.shields.io/badge/read-docs-yellow?logo=mdbook]
 
   [Syft Logo]  Perform `numpy`-like analysis on `data` that remains in `someone
 else's` server # Quickstart â `Linux` â `macOS`\* â `Windows`â â¡ ##
-Install syft on Python 3.9 - 3.10 ```bash $ pip install -U syft -f https://
+Install syft on Python 3.9 - 3.11 ```bash $ pip install -U syft -f https://
 whls.blob.core.windows.net/unstable/index.html ``` ## Launch a python dev
 Domain ```python # from Jupyter / Python import syft as sy sy.requires
 (">=0.8,<0.8.1") node = sy.orchestra.launch(name="my-domain", port=8080,
 dev_mode=True, reset=True) ``` ```bash # or from the command line $ syft launch
 --name=my-domain --port=8080 --reset=True Starting syft-node server on 0.0.0.0:
 8080 ``` ## Connect with our Python Client ```python import syft as sy
 sy.requires(">=0.8,<0.8.1") domain_client = sy.login(port=8080,
@@ -34,17 +34,17 @@
 to localhost with ð³ `docker`, however ðµ HAGrid can deploy to `podman` or
 a ð§ `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using ð¨
 `ansible`â  ## Docs and Support - ð API_Example_Notebooks - ð Docs -
 `#support` on Slack # Install Notes - HAGrid 0.3 Requires: ð `python` ð
 `git` - Run: `pip install -U hagrid` - Interactive Install ð§ð½ââï¸
 WizardBETA Requires ðµ `hagrid`: - Run: `hagrid quickstart` â `Windows` does
 not support `ansible`, preventing some remote deployment targets - PySyft 0.8
-Requires: ð `python 3.9 - 3.10` - Run: `pip install -U syft` \*`macOS` Apple
+Requires: ð `python 3.9 - 3.11` - Run: `pip install -U syft` \*`macOS` Apple
 Silicon users might need cmake: `brew install cmake` â¡`Windows` users must
-run this first: `pip install jaxlib==0.3.14 -f https://
+run this first: `pip install jaxlib==0.4.10 -f https://
 whls.blob.core.windows.net/unstable/index.html` - PyGrid Requires: ð³
 `docker` or ð§ `ubuntu` VM - Run: `hagrid launch ...` # Versions `0.8.1`
 (Beta) - `dev` branch ðð½ API `0.8.0` (Stable) - API Deprecated: - `0.7.0`
 - Course_3_Updated - `0.6.0` - Course_3 - `0.5.1` - Course_2 + M1 Hotfix -
 `0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
 match them up where possible. We release weekly betas which can be used in each
 context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
```

### Comparing `syft-0.8.1b4/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b5/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b4/src/syft.egg-info/requires.txt` & `syft-0.8.1b5/src/syft.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 astunparse==1.6.3
 bcrypt==4.0.1
-flax==0.5.3
 forbiddenfruit==0.1.4
 gevent==22.10.2
 gipc==1.5.0
-jax==0.3.14
-jaxlib==0.3.14
+jax==0.4.10
+jaxlib==0.4.10
 loguru==0.7.0
 networkx==2.8
 numpy==1.24.3
 opendp==0.6.2
 packaging>=21.0
 pandas==1.5.3
 pyarrow==11.0.0
@@ -25,14 +24,16 @@
 tqdm==4.65.0
 typeguard==2.13.3
 typing_extensions==4.5.0
 sherlock[filelock,redis]==0.4.1
 uvicorn[standard]==0.21.1
 fastapi==0.95.1
 hagrid>=0.3
+matplotlib==3.7.1
+dm-haiku==0.0.9
 opentelemetry-api==1.14.0
 opentelemetry-sdk==1.14.0
 opentelemetry-exporter-jaeger==1.14.0
 opentelemetry-instrumentation==0.35b0
 opentelemetry-instrumentation-requests==0.35b0
 
 [dev]
```

