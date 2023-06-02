# Comparing `tmp/prodvana-0.1.5.tar.gz` & `tmp/prodvana-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.5.tar", max compression
+gzip compressed data, was "prodvana-0.1.6.tar", max compression
```

## Comparing `prodvana-0.1.5.tar` & `prodvana-0.1.6.tar`

### file list

```diff
@@ -1,332 +1,332 @@
--rw-r--r--   0        0        0       81 2023-05-19 19:00:48.877495 prodvana-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.877495 prodvana-0.1.5/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-05-19 23:43:46.670463 prodvana-0.1.5/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.883145 prodvana-0.1.5/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.883145 prodvana-0.1.5/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-05-26 21:53:53.515147 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-05-26 21:53:53.747146 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-05-26 21:53:53.515147 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-05-26 21:53:53.751146 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-05-26 21:53:53.555147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-05-26 21:53:53.803146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.799146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-05-26 21:53:53.791146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-05-26 21:53:53.795146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-05-26 21:53:53.799146 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.555147 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.791146 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-05-26 21:53:53.563147 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.803146 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-05-26 21:53:53.547147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-05-26 21:53:53.783146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.547147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.783146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-05-26 21:53:53.511147 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-05-26 21:53:53.743146 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.511147 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.747146 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-05-26 21:53:53.839145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     5636 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.615146 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.855145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3658 2023-05-26 21:53:53.595147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4110 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.603147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.591147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-05-26 21:53:53.615146 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.583147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    12624 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-05-26 21:53:53.855145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.619147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-05-26 21:53:53.619147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-05-26 21:53:53.839145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.591147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-05-26 21:53:53.595147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2192 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     1490 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.603147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3597 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4171 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.687146 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-26 21:53:53.631147 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.631147 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     7053 2023-05-26 21:53:53.639146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     6102 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11893 2023-05-26 21:53:53.639146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     7309 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    11002 2023-05-26 21:53:53.643146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3288 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    33432 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28076 2023-05-26 21:53:53.759146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    18226 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5259 2023-05-26 21:53:53.759146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    38158 2023-05-26 21:53:53.527147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    64686 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3895 2023-05-26 21:53:53.527147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7903 2023-05-26 21:53:53.763146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.763146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    18876 2023-05-26 21:55:24.562636 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    24612 2023-05-26 21:55:24.562636 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.519147 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.755146 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-05-26 21:53:53.755146 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-05-26 21:53:53.519147 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-05-26 21:53:53.751146 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-05-26 21:53:53.707146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-05-26 21:53:53.703146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.707146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-05-26 21:53:53.703146 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.475147 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-05-26 21:53:53.775146 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-05-26 21:53:53.579147 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-05-26 21:53:53.823145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-05-26 21:53:53.583147 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.743146 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-05-26 21:53:53.715146 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.715146 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-05-26 21:53:53.535147 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-05-26 21:53:53.775146 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-05-26 21:53:53.535147 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-05-26 21:53:53.771146 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.771146 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2598 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.723146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-05-26 21:53:53.727146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.727146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-26 21:53:53.431148 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.391148 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1907 2023-05-26 21:53:53.399148 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-05-26 21:53:53.663146 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.651147 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8407 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8891 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.427148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.663146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-05-26 21:53:53.655146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6409 2023-05-26 21:53:53.431148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.427148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.655146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-05-26 21:53:53.503147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-05-26 21:53:53.735146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.499147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12153 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12710 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.495147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.735146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-05-26 21:53:53.503147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-05-26 21:53:53.495147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1559 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.py
--rw-r--r--   0        0        0     1360 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.439148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-05-26 21:53:53.439148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-05-26 21:53:53.671146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.671146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-05-26 21:53:53.695146 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.463147 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.695146 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-05-26 21:53:53.447147 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.807145 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-05-26 21:53:53.819146 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.579147 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.823145 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    31313 2023-05-26 21:53:53.571147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    44213 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.571147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    47994 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-05-26 21:53:53.811146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-05-26 21:53:53.811146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-05-26 21:53:53.807145 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.563147 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.819146 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-05-26 21:53:53.455148 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-05-26 21:53:53.687146 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-05-26 21:53:53.455148 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-05-26 21:53:53.463147 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-26 21:53:53.627147 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.627147 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-26 21:53:53.391148 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-05-26 21:53:53.647146 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.387148 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.651147 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2142 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2646 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.475147 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-05-26 21:53:53.679146 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.447147 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.679146 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-05-26 21:53:53.483147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.483147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-05-26 21:53:53.723146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-26 21:53:53.923145 prodvana-0.1.5/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-05-26 21:53:53.647146 prodvana-0.1.5/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-05-26 21:53:53.879145 prodvana-0.1.5/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-26 21:53:53.643146 prodvana-0.1.5/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-26 21:53:53.879145 prodvana-0.1.5/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4079 2023-05-20 03:23:03.669262 prodvana-0.1.5/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-05-20 03:23:03.669262 prodvana-0.1.5/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-05-26 22:29:46.734902 prodvana-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-30 13:39:12.483857 prodvana-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.483857 prodvana-0.1.6/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-30 13:39:12.483857 prodvana-0.1.6/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.029790 prodvana-0.1.6/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.029790 prodvana-0.1.6/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-06-02 21:20:33.769790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-06-02 21:20:33.977790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-06-02 21:20:33.665790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.869790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-06-02 21:20:33.665790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-06-02 21:20:33.869790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-06-02 21:20:33.797790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-06-02 21:20:34.005790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-06-02 21:20:33.797790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-06-02 21:20:34.005790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-02 21:20:33.713790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.713790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-06-02 21:20:33.833790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5636 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3658 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4110 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.645790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12624 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.645790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-06-02 21:20:33.833790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2192 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     1490 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3597 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4171 2023-06-02 21:20:33.909790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.909790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-02 21:20:33.749790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.749790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     7053 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     6102 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11893 2023-06-02 21:20:33.769790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     7309 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    11002 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3288 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    35437 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28895 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    20037 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5752 2023-06-02 21:20:33.925790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    41784 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    68647 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3895 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7903 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.925790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    20651 2023-06-02 22:04:33.405790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    27158 2023-06-02 22:04:33.405790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.953790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-06-02 21:20:33.953790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-06-02 21:20:33.949790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-06-02 21:20:34.021790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-06-02 21:20:33.813790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.813790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.021790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-02 21:20:33.753790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.753790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-06-02 21:20:33.725790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.725790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2598 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-06-02 21:20:33.697790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.681790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1907 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-06-02 21:20:33.889790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8407 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8891 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-06-02 21:20:33.681790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6409 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.889790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-06-02 21:20:33.897790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12100 2023-06-02 22:16:08.617790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12611 2023-06-02 22:16:08.617790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.897790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-06-02 21:20:33.689790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-06-02 21:20:33.689790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1551 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-06-02 21:20:33.785790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.785790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.993790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    31345 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    44279 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    47994 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-06-02 21:20:33.993790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-06-02 21:20:33.697790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.617790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-06-02 21:20:33.741790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.741790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.949790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.977790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2142 2023-06-02 21:20:33.617790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2646 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.613790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-06-02 21:20:33.733790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-06-02 21:20:33.941790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:33.941790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-06-02 21:20:33.733790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-02 21:20:34.065790 prodvana-0.1.6/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-06-02 21:20:33.821790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-02 21:20:33.821790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4079 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-06-02 22:28:07.557790 prodvana-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.6/PKG-INFO
```

### Comparing `prodvana-0.1.5/prodvana/client.py` & `prodvana-0.1.6/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.prodvana.desired_state.model import desired_state_pb2 as prodvana_dot_desired__state_dot_model_dot_desired__state__pb2
 from prodvana.proto.prodvana.desired_state.model import entity_pb2 as prodvana_dot_desired__state_dot_model_dot_entity__pb2
 from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/desired_state/manager.proto\x12\x16prodvana.desired_state\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a)prodvana/desired_state/model/entity.proto\x1a%prodvana/service/service_config.proto\x1a\x17validate/validate.proto\"l\n\x12SetDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\"\xc4\x01\n\x17ValidateDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\x12Q\n\x18service_instance_configs\x18\x03 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"/\n\x13SetDesiredStateResp\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\"e\n+GetServiceDesiredStateConvergenceSummaryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"b\n\x12StatusExplanations\x12L\n\x13status_explanations\x18\x01 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\"G\n\tDebugLogs\x12:\n\ndebug_logs\x18\x01 \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\"\xaf\x0f\n\x13\x44\x65siredStateSummary\x12?\n\x0c\x65ntity_graph\x18\x0f \x01(\x0b\x32).prodvana.desired_state.model.EntityGraph\x12;\n\x0estarting_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x03 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x08statuses\x18\x04 \x03(\x0b\x32\x39.prodvana.desired_state.DesiredStateSummary.StatusesEntry\x12\x36\n\x12\x63reation_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12replaced_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x64\n\x15precondition_statuses\x18\x08 \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.PreconditionStatusesEntry\x12`\n\x13status_explanations\x18\t \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.StatusExplanationsEntry\x12N\n\ndebug_logs\x18\n \x03(\x0b\x32:.prodvana.desired_state.DesiredStateSummary.DebugLogsEntry\x12`\n\x13\x61\x63tion_explanations\x18\x0b \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.ActionExplanationsEntry\x12\x65\n\x16last_update_timestamps\x18\x0c \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.LastUpdateTimestampsEntry\x12g\n\x17last_fetched_timestamps\x18\r \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastFetchedTimestampsEntry\x12g\n\x17last_applied_timestamps\x18\x0e \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastAppliedTimestampsEntry\x1aU\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0e\x32$.prodvana.desired_state.model.Status:\x02\x38\x01\x1ai\n\x19PreconditionStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.prodvana.desired_state.model.ConditionState:\x02\x38\x01\x1a\x65\n\x17StatusExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32*.prodvana.desired_state.StatusExplanations:\x02\x38\x01\x1aS\n\x0e\x44\x65\x62ugLogsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.prodvana.desired_state.DebugLogs:\x02\x38\x01\x1aj\n\x17\x41\x63tionExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12>\n\x05value\x18\x02 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation:\x02\x38\x01\x1aW\n\x19LastUpdateTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastFetchedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastAppliedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\"B\n\x1dGetDesiredStateConvergenceReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"e\n%GetDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"l\n,GetServiceDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"Y\n\x1fGetServiceLastConvergedStateReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"w\n GetServiceLastConvergedStateResp\x12S\n\x17service_instance_states\x18\x01 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\"\x81\x01\n GetServiceDesiredStateHistoryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\x81\x01\n!GetServiceDesiredStateHistoryResp\x12\x43\n\x0e\x64\x65sired_states\x18\x01 \x03(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x12GetDesiredStateReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x96\x01\n\x13GetDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"\x9b\x01\n\x18ValidateDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"a\n\x14SetManualApprovalReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x05topic\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0e\n\x06reject\x18\x03 \x01(\x08\"\x17\n\x15SetManualApprovalResp\"m\n\x12PromoteDeliveryReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\r\n\x05stage\x18\x02 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x03 \x01(\x08\x12\x17\n\x06source\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x15\n\x13PromoteDeliveryResp2\xd4\r\n\x13\x44\x65siredStateManager\x12\x89\x01\n\x0fSetDesiredState\x12*.prodvana.desired_state.SetDesiredStateReq\x1a+.prodvana.desired_state.SetDesiredStateResp\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/desired_states:\x01*\x12\x89\x02\n(GetServiceDesiredStateConvergenceSummary\x12\x43.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryReq\x1a\x44.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryResp\"R\x82\xd3\xe4\x93\x02L\x12J/v1/applications/{application=*}/services/{service=*}/latest_desired_state\x12\xe0\x01\n\x1dGetServiceLastConvergedStates\x12\x37.prodvana.desired_state.GetServiceLastConvergedStateReq\x1a\x38.prodvana.desired_state.GetServiceLastConvergedStateResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/last_converged\x12\xe2\x01\n\x1dGetServiceDesiredStateHistory\x12\x38.prodvana.desired_state.GetServiceDesiredStateHistoryReq\x1a\x39.prodvana.desired_state.GetServiceDesiredStateHistoryResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/desired_states\x12\x9b\x01\n\x0fGetDesiredState\x12*.prodvana.desired_state.GetDesiredStateReq\x1a+.prodvana.desired_state.GetDesiredStateResp\"/\x82\xd3\xe4\x93\x02)\x12\'/v1/desired_states/{desired_state_id=*}\x12\xd2\x01\n!GetDesiredStateConvergenceSummary\x12\x35.prodvana.desired_state.GetDesiredStateConvergenceReq\x1a=.prodvana.desired_state.GetDesiredStateConvergenceSummaryResp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/desired_states/{desired_state_id=*}/summary\x12\xa1\x01\n\x14ValidateDesiredState\x12/.prodvana.desired_state.ValidateDesiredStateReq\x1a\x30.prodvana.desired_state.ValidateDesiredStateResp\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/desired_states/validate:\x01*\x12\xa8\x01\n\x11SetManualApproval\x12,.prodvana.desired_state.SetManualApprovalReq\x1a-.prodvana.desired_state.SetManualApprovalResp\"6\x82\xd3\xe4\x93\x02\x30\"+/v1/desired_states/approve_manual_condition:\x01*\x12\x9a\x01\n\x0fPromoteDelivery\x12*.prodvana.desired_state.PromoteDeliveryReq\x1a+.prodvana.desired_state.PromoteDeliveryResp\".\x82\xd3\xe4\x93\x02(\"#/v1/desired_states/promote_delivery:\x01*BRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_stateb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/desired_state/manager.proto\x12\x16prodvana.desired_state\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a)prodvana/desired_state/model/entity.proto\x1a%prodvana/service/service_config.proto\x1a\x17validate/validate.proto\"l\n\x12SetDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\"\xc4\x01\n\x17ValidateDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\x12Q\n\x18service_instance_configs\x18\x03 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"/\n\x13SetDesiredStateResp\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\"e\n+GetServiceDesiredStateConvergenceSummaryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"b\n\x12StatusExplanations\x12L\n\x13status_explanations\x18\x01 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\"G\n\tDebugLogs\x12:\n\ndebug_logs\x18\x01 \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\"\xaf\x0f\n\x13\x44\x65siredStateSummary\x12?\n\x0c\x65ntity_graph\x18\x0f \x01(\x0b\x32).prodvana.desired_state.model.EntityGraph\x12;\n\x0estarting_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x03 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x08statuses\x18\x04 \x03(\x0b\x32\x39.prodvana.desired_state.DesiredStateSummary.StatusesEntry\x12\x36\n\x12\x63reation_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12replaced_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x64\n\x15precondition_statuses\x18\x08 \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.PreconditionStatusesEntry\x12`\n\x13status_explanations\x18\t \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.StatusExplanationsEntry\x12N\n\ndebug_logs\x18\n \x03(\x0b\x32:.prodvana.desired_state.DesiredStateSummary.DebugLogsEntry\x12`\n\x13\x61\x63tion_explanations\x18\x0b \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.ActionExplanationsEntry\x12\x65\n\x16last_update_timestamps\x18\x0c \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.LastUpdateTimestampsEntry\x12g\n\x17last_fetched_timestamps\x18\r \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastFetchedTimestampsEntry\x12g\n\x17last_applied_timestamps\x18\x0e \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastAppliedTimestampsEntry\x1aU\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0e\x32$.prodvana.desired_state.model.Status:\x02\x38\x01\x1ai\n\x19PreconditionStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.prodvana.desired_state.model.ConditionState:\x02\x38\x01\x1a\x65\n\x17StatusExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32*.prodvana.desired_state.StatusExplanations:\x02\x38\x01\x1aS\n\x0e\x44\x65\x62ugLogsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.prodvana.desired_state.DebugLogs:\x02\x38\x01\x1aj\n\x17\x41\x63tionExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12>\n\x05value\x18\x02 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation:\x02\x38\x01\x1aW\n\x19LastUpdateTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastFetchedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastAppliedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\"B\n\x1dGetDesiredStateConvergenceReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"e\n%GetDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"l\n,GetServiceDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"Y\n\x1fGetServiceLastConvergedStateReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"w\n GetServiceLastConvergedStateResp\x12S\n\x17service_instance_states\x18\x01 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\"\x81\x01\n GetServiceDesiredStateHistoryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\x81\x01\n!GetServiceDesiredStateHistoryResp\x12\x43\n\x0e\x64\x65sired_states\x18\x01 \x03(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x12GetDesiredStateReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x96\x01\n\x13GetDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"\x9b\x01\n\x18ValidateDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"a\n\x14SetManualApprovalReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x05topic\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0e\n\x06reject\x18\x03 \x01(\x08\"\x17\n\x15SetManualApprovalResp\"m\n\x12PromoteDeliveryReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\r\n\x05stage\x18\x02 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x03 \x01(\x08\x12\x17\n\x06source\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x15\n\x13PromoteDeliveryResp\"Q\n\x13\x42ypassProtectionReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x17\n\x06source\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x16\n\x14\x42ypassProtectionResp2\xf5\x0e\n\x13\x44\x65siredStateManager\x12\x89\x01\n\x0fSetDesiredState\x12*.prodvana.desired_state.SetDesiredStateReq\x1a+.prodvana.desired_state.SetDesiredStateResp\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/desired_states:\x01*\x12\x89\x02\n(GetServiceDesiredStateConvergenceSummary\x12\x43.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryReq\x1a\x44.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryResp\"R\x82\xd3\xe4\x93\x02L\x12J/v1/applications/{application=*}/services/{service=*}/latest_desired_state\x12\xe0\x01\n\x1dGetServiceLastConvergedStates\x12\x37.prodvana.desired_state.GetServiceLastConvergedStateReq\x1a\x38.prodvana.desired_state.GetServiceLastConvergedStateResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/last_converged\x12\xe2\x01\n\x1dGetServiceDesiredStateHistory\x12\x38.prodvana.desired_state.GetServiceDesiredStateHistoryReq\x1a\x39.prodvana.desired_state.GetServiceDesiredStateHistoryResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/desired_states\x12\x9b\x01\n\x0fGetDesiredState\x12*.prodvana.desired_state.GetDesiredStateReq\x1a+.prodvana.desired_state.GetDesiredStateResp\"/\x82\xd3\xe4\x93\x02)\x12\'/v1/desired_states/{desired_state_id=*}\x12\xd2\x01\n!GetDesiredStateConvergenceSummary\x12\x35.prodvana.desired_state.GetDesiredStateConvergenceReq\x1a=.prodvana.desired_state.GetDesiredStateConvergenceSummaryResp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/desired_states/{desired_state_id=*}/summary\x12\xa1\x01\n\x14ValidateDesiredState\x12/.prodvana.desired_state.ValidateDesiredStateReq\x1a\x30.prodvana.desired_state.ValidateDesiredStateResp\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/desired_states/validate:\x01*\x12\xa8\x01\n\x11SetManualApproval\x12,.prodvana.desired_state.SetManualApprovalReq\x1a-.prodvana.desired_state.SetManualApprovalResp\"6\x82\xd3\xe4\x93\x02\x30\"+/v1/desired_states/approve_manual_condition:\x01*\x12\x9a\x01\n\x0fPromoteDelivery\x12*.prodvana.desired_state.PromoteDeliveryReq\x1a+.prodvana.desired_state.PromoteDeliveryResp\".\x82\xd3\xe4\x93\x02(\"#/v1/desired_states/promote_delivery:\x01*\x12\x9e\x01\n\x10\x42ypassProtection\x12+.prodvana.desired_state.BypassProtectionReq\x1a,.prodvana.desired_state.BypassProtectionResp\"/\x82\xd3\xe4\x93\x02)\"$/v1/desired_states/bypass_protection:\x01*BRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_stateb\x06proto3')
 
 
 
 _SETDESIREDSTATEREQ = DESCRIPTOR.message_types_by_name['SetDesiredStateReq']
 _VALIDATEDESIREDSTATEREQ = DESCRIPTOR.message_types_by_name['ValidateDesiredStateReq']
 _SETDESIREDSTATERESP = DESCRIPTOR.message_types_by_name['SetDesiredStateResp']
 _GETSERVICEDESIREDSTATECONVERGENCESUMMARYREQ = DESCRIPTOR.message_types_by_name['GetServiceDesiredStateConvergenceSummaryReq']
@@ -49,14 +49,16 @@
 _GETDESIREDSTATEREQ = DESCRIPTOR.message_types_by_name['GetDesiredStateReq']
 _GETDESIREDSTATERESP = DESCRIPTOR.message_types_by_name['GetDesiredStateResp']
 _VALIDATEDESIREDSTATERESP = DESCRIPTOR.message_types_by_name['ValidateDesiredStateResp']
 _SETMANUALAPPROVALREQ = DESCRIPTOR.message_types_by_name['SetManualApprovalReq']
 _SETMANUALAPPROVALRESP = DESCRIPTOR.message_types_by_name['SetManualApprovalResp']
 _PROMOTEDELIVERYREQ = DESCRIPTOR.message_types_by_name['PromoteDeliveryReq']
 _PROMOTEDELIVERYRESP = DESCRIPTOR.message_types_by_name['PromoteDeliveryResp']
+_BYPASSPROTECTIONREQ = DESCRIPTOR.message_types_by_name['BypassProtectionReq']
+_BYPASSPROTECTIONRESP = DESCRIPTOR.message_types_by_name['BypassProtectionResp']
 SetDesiredStateReq = _reflection.GeneratedProtocolMessageType('SetDesiredStateReq', (_message.Message,), {
   'DESCRIPTOR' : _SETDESIREDSTATEREQ,
   '__module__' : 'prodvana.desired_state.manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.SetDesiredStateReq)
   })
 _sym_db.RegisterMessage(SetDesiredStateReq)
 
@@ -260,14 +262,28 @@
 PromoteDeliveryResp = _reflection.GeneratedProtocolMessageType('PromoteDeliveryResp', (_message.Message,), {
   'DESCRIPTOR' : _PROMOTEDELIVERYRESP,
   '__module__' : 'prodvana.desired_state.manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.PromoteDeliveryResp)
   })
 _sym_db.RegisterMessage(PromoteDeliveryResp)
 
+BypassProtectionReq = _reflection.GeneratedProtocolMessageType('BypassProtectionReq', (_message.Message,), {
+  'DESCRIPTOR' : _BYPASSPROTECTIONREQ,
+  '__module__' : 'prodvana.desired_state.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.desired_state.BypassProtectionReq)
+  })
+_sym_db.RegisterMessage(BypassProtectionReq)
+
+BypassProtectionResp = _reflection.GeneratedProtocolMessageType('BypassProtectionResp', (_message.Message,), {
+  'DESCRIPTOR' : _BYPASSPROTECTIONRESP,
+  '__module__' : 'prodvana.desired_state.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.desired_state.BypassProtectionResp)
+  })
+_sym_db.RegisterMessage(BypassProtectionResp)
+
 _DESIREDSTATEMANAGER = DESCRIPTOR.services_by_name['DesiredStateManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state'
   _SETDESIREDSTATEREQ.fields_by_name['desired_state']._options = None
   _SETDESIREDSTATEREQ.fields_by_name['desired_state']._serialized_options = b'\372B\005\212\001\002\020\001'
@@ -309,14 +325,18 @@
   _SETMANUALAPPROVALREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
   _SETMANUALAPPROVALREQ.fields_by_name['topic']._options = None
   _SETMANUALAPPROVALREQ.fields_by_name['topic']._serialized_options = b'\372B\004r\002\020\001'
   _PROMOTEDELIVERYREQ.fields_by_name['desired_state_id']._options = None
   _PROMOTEDELIVERYREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
   _PROMOTEDELIVERYREQ.fields_by_name['source']._options = None
   _PROMOTEDELIVERYREQ.fields_by_name['source']._serialized_options = b'\372B\004r\002\020\001'
+  _BYPASSPROTECTIONREQ.fields_by_name['desired_state_id']._options = None
+  _BYPASSPROTECTIONREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
+  _BYPASSPROTECTIONREQ.fields_by_name['source']._options = None
+  _BYPASSPROTECTIONREQ.fields_by_name['source']._serialized_options = b'\372B\004r\002\020\001'
   _DESIREDSTATEMANAGER.methods_by_name['SetDesiredState']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['SetDesiredState']._serialized_options = b'\202\323\344\223\002\027\"\022/v1/desired_states:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateConvergenceSummary']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateConvergenceSummary']._serialized_options = b'\202\323\344\223\002L\022J/v1/applications/{application=*}/services/{service=*}/latest_desired_state'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceLastConvergedStates']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceLastConvergedStates']._serialized_options = b'\202\323\344\223\002F\022D/v1/applications/{application=*}/services/{service=*}/last_converged'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateHistory']._options = None
@@ -327,14 +347,16 @@
   _DESIREDSTATEMANAGER.methods_by_name['GetDesiredStateConvergenceSummary']._serialized_options = b'\202\323\344\223\0021\022//v1/desired_states/{desired_state_id=*}/summary'
   _DESIREDSTATEMANAGER.methods_by_name['ValidateDesiredState']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['ValidateDesiredState']._serialized_options = b'\202\323\344\223\002 \"\033/v1/desired_states/validate:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['SetManualApproval']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['SetManualApproval']._serialized_options = b'\202\323\344\223\0020\"+/v1/desired_states/approve_manual_condition:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['PromoteDelivery']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['PromoteDelivery']._serialized_options = b'\202\323\344\223\002(\"#/v1/desired_states/promote_delivery:\001*'
+  _DESIREDSTATEMANAGER.methods_by_name['BypassProtection']._options = None
+  _DESIREDSTATEMANAGER.methods_by_name['BypassProtection']._serialized_options = b'\202\323\344\223\002)\"$/v1/desired_states/bypass_protection:\001*'
   _SETDESIREDSTATEREQ._serialized_start=284
   _SETDESIREDSTATEREQ._serialized_end=392
   _VALIDATEDESIREDSTATEREQ._serialized_start=395
   _VALIDATEDESIREDSTATEREQ._serialized_end=591
   _SETDESIREDSTATERESP._serialized_start=593
   _SETDESIREDSTATERESP._serialized_end=640
   _GETSERVICEDESIREDSTATECONVERGENCESUMMARYREQ._serialized_start=642
@@ -385,10 +407,14 @@
   _SETMANUALAPPROVALREQ._serialized_end=4110
   _SETMANUALAPPROVALRESP._serialized_start=4112
   _SETMANUALAPPROVALRESP._serialized_end=4135
   _PROMOTEDELIVERYREQ._serialized_start=4137
   _PROMOTEDELIVERYREQ._serialized_end=4246
   _PROMOTEDELIVERYRESP._serialized_start=4248
   _PROMOTEDELIVERYRESP._serialized_end=4269
-  _DESIREDSTATEMANAGER._serialized_start=4272
-  _DESIREDSTATEMANAGER._serialized_end=6020
+  _BYPASSPROTECTIONREQ._serialized_start=4271
+  _BYPASSPROTECTIONREQ._serialized_end=4352
+  _BYPASSPROTECTIONRESP._serialized_start=4354
+  _BYPASSPROTECTIONRESP._serialized_end=4376
+  _DESIREDSTATEMANAGER._serialized_start=4379
+  _DESIREDSTATEMANAGER._serialized_end=6288
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -573,7 +573,33 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___PromoteDeliveryResp = PromoteDeliveryResp
+
+class BypassProtectionReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    desired_state_id: builtins.str
+    source: builtins.str
+    def __init__(
+        self,
+        *,
+        desired_state_id: builtins.str = ...,
+        source: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "source", b"source"]) -> None: ...
+
+global___BypassProtectionReq = BypassProtectionReq
+
+class BypassProtectionResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___BypassProtectionResp = BypassProtectionResp
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,14 +55,19 @@
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.SetManualApprovalResp.FromString,
                 )
         self.PromoteDelivery = channel.unary_unary(
                 '/prodvana.desired_state.DesiredStateManager/PromoteDelivery',
                 request_serializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryReq.SerializeToString,
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.FromString,
                 )
+        self.BypassProtection = channel.unary_unary(
+                '/prodvana.desired_state.DesiredStateManager/BypassProtection',
+                request_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
+                response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
+                )
 
 
 class DesiredStateManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SetDesiredState(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -114,14 +119,20 @@
 
     def PromoteDelivery(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def BypassProtection(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DesiredStateManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SetDesiredState': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDesiredState,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateResp.SerializeToString,
@@ -162,14 +173,19 @@
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.SetManualApprovalResp.SerializeToString,
             ),
             'PromoteDelivery': grpc.unary_unary_rpc_method_handler(
                     servicer.PromoteDelivery,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.SerializeToString,
             ),
+            'BypassProtection': grpc.unary_unary_rpc_method_handler(
+                    servicer.BypassProtection,
+                    request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.FromString,
+                    response_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prodvana.desired_state.DesiredStateManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -324,7 +340,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/PromoteDelivery',
             prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryReq.SerializeToString,
             prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def BypassProtection(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/BypassProtection',
+            prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
+            prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         prodvana.proto.prodvana.desired_state.manager_pb2.SetManualApprovalReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.SetManualApprovalResp,
     ]
     PromoteDelivery: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp,
     ]
+    BypassProtection: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
+        prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp,
+    ]
 
 class DesiredStateManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def SetDesiredState(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.SetDesiredStateReq,
         context: grpc.ServicerContext,
@@ -96,9 +100,15 @@
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.SetManualApprovalResp: ...
     @abc.abstractmethod
     def PromoteDelivery(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp: ...
+    @abc.abstractmethod
+    def BypassProtection(
+        self,
+        request: prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
+        context: grpc.ServicerContext,
+    ) -> prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp: ...
 
 def add_DesiredStateManagerServicer_to_server(servicer: DesiredStateManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
+from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLinkJ\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"\xff\x03\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x12\n\nstate_hash\x18\x0b \x01(\x0c\x12\x0f\n\x07message\x18\x0c \x01(\t\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nR\x0eunhealthy_pods\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xd4\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xa8\x04\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12@\n\x07program\x18\x04 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x05 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\"\xde\x01\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x83\x01\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x0e\n\nDEPLOYMENT\x10\x04\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x05*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*8\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLinkJ\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"V\n\x1bRuntimeExtensionFetchOutput\x12\x37\n\x08versions\x18\x01 \x03(\x0b\x32%.prodvana.desired_state.model.Version\"\xa5\x07\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12W\n\x0foutput_blob_ids\x18\x0e \x03(\x0b\x32>.prodvana.desired_state.model.RuntimeObject.OutputBlobIdsEntry\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x65\n\x10RuntimeExtension\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x12\n\nservice_id\x18\x02 \x01(\t\x1a\x34\n\x12OutputBlobIdsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cR\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xa8\x04\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12@\n\x07program\x18\x04 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x05 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\"\xc6\x02\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypassB\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x83\x01\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x0e\n\nDEPLOYMENT\x10\x04\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x05*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*O\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 _LIFECYCLE = DESCRIPTOR.enum_types_by_name['Lifecycle']
 Lifecycle = enum_type_wrapper.EnumTypeWrapper(_LIFECYCLE)
 _CUSTOMTASKTYPE = DESCRIPTOR.enum_types_by_name['CustomTaskType']
 CustomTaskType = enum_type_wrapper.EnumTypeWrapper(_CUSTOMTASKTYPE)
@@ -108,14 +109,15 @@
 REJECTED = 2
 CUSTOM_TASK_PENDING = 0
 CUSTOM_TASK_SUCCESSFUL = 1
 CUSTOM_TASK_RETRIES_EXHAUSTED = 2
 CUSTOM_TASK_TIMED_OUT = 3
 SIGNAL_UNKNOWN = 0
 DELIVERY_PROMOTION = 1
+PROTECTION_BYPASS = 2
 
 
 _PROTECTIONLINK = DESCRIPTOR.message_types_by_name['ProtectionLink']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _CONDITION_RELEASECHANNELSTABLECONDITION = _CONDITION.nested_types_by_name['ReleaseChannelStableCondition']
 _CONDITION_MANUALAPPROVAL = _CONDITION.nested_types_by_name['ManualApproval']
 _CONDITION_CUSTOMTASKSUCCESSFULCONDITION = _CONDITION.nested_types_by_name['CustomTaskSuccessfulCondition']
@@ -126,28 +128,32 @@
 _ACTIONEXPLANATION = DESCRIPTOR.message_types_by_name['ActionExplanation']
 _VERSION = DESCRIPTOR.message_types_by_name['Version']
 _SERVICEINSTANCESTATE = DESCRIPTOR.message_types_by_name['ServiceInstanceState']
 _SERVICESTATE = DESCRIPTOR.message_types_by_name['ServiceState']
 _SERVICEGROUPSTATE = DESCRIPTOR.message_types_by_name['ServiceGroupState']
 _CANARYPROGRESSSTATE = DESCRIPTOR.message_types_by_name['CanaryProgressState']
 _DELIVERYSTATE = DESCRIPTOR.message_types_by_name['DeliveryState']
+_RUNTIMEEXTENSIONFETCHOUTPUT = DESCRIPTOR.message_types_by_name['RuntimeExtensionFetchOutput']
 _RUNTIMEOBJECT = DESCRIPTOR.message_types_by_name['RuntimeObject']
+_RUNTIMEOBJECT_RUNTIMEEXTENSION = _RUNTIMEOBJECT.nested_types_by_name['RuntimeExtension']
+_RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY = _RUNTIMEOBJECT.nested_types_by_name['OutputBlobIdsEntry']
 _CONDITIONSTATE = DESCRIPTOR.message_types_by_name['ConditionState']
 _CONTROLSTATE = DESCRIPTOR.message_types_by_name['ControlState']
 _MANUALAPPROVALSTATE = DESCRIPTOR.message_types_by_name['ManualApprovalState']
 _STATE = DESCRIPTOR.message_types_by_name['State']
 _ANNOTATIONS = DESCRIPTOR.message_types_by_name['Annotations']
 _ANNOTATIONS_ANNOTATION = _ANNOTATIONS.nested_types_by_name['Annotation']
 _CUSTOMTASKEXECUTIONSTATE = DESCRIPTOR.message_types_by_name['CustomTaskExecutionState']
 _CUSTOMTASKSTATE = DESCRIPTOR.message_types_by_name['CustomTaskState']
 _PROTECTIONLINKSTATE = DESCRIPTOR.message_types_by_name['ProtectionLinkState']
 _PROTECTIONATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionAttachment']
 _DELIVERYEXTENSIONSTATE = DESCRIPTOR.message_types_by_name['DeliveryExtensionState']
 _SIGNAL = DESCRIPTOR.message_types_by_name['Signal']
 _SIGNAL_DELIVERYPROMOTIONCONFIG = _SIGNAL.nested_types_by_name['DeliveryPromotionConfig']
+_SIGNAL_PROTECTIONBYPASS = _SIGNAL.nested_types_by_name['ProtectionBypass']
 _DEBUGLOG = DESCRIPTOR.message_types_by_name['DebugLog']
 _CANARYPROGRESSSTATE_STATUS = _CANARYPROGRESSSTATE.enum_types_by_name['Status']
 _DELIVERYSTATE_STATUS = _DELIVERYSTATE.enum_types_by_name['Status']
 _RUNTIMEOBJECT_STATUS = _RUNTIMEOBJECT.enum_types_by_name['Status']
 _PROTECTIONLINKSTATE_STOPREASON = _PROTECTIONLINKSTATE.enum_types_by_name['StopReason']
 ProtectionLink = _reflection.GeneratedProtocolMessageType('ProtectionLink', (_message.Message,), {
   'DESCRIPTOR' : _PROTECTIONLINK,
@@ -261,20 +267,43 @@
 DeliveryState = _reflection.GeneratedProtocolMessageType('DeliveryState', (_message.Message,), {
   'DESCRIPTOR' : _DELIVERYSTATE,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.DeliveryState)
   })
 _sym_db.RegisterMessage(DeliveryState)
 
+RuntimeExtensionFetchOutput = _reflection.GeneratedProtocolMessageType('RuntimeExtensionFetchOutput', (_message.Message,), {
+  'DESCRIPTOR' : _RUNTIMEEXTENSIONFETCHOUTPUT,
+  '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.RuntimeExtensionFetchOutput)
+  })
+_sym_db.RegisterMessage(RuntimeExtensionFetchOutput)
+
 RuntimeObject = _reflection.GeneratedProtocolMessageType('RuntimeObject', (_message.Message,), {
+
+  'RuntimeExtension' : _reflection.GeneratedProtocolMessageType('RuntimeExtension', (_message.Message,), {
+    'DESCRIPTOR' : _RUNTIMEOBJECT_RUNTIMEEXTENSION,
+    '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.RuntimeObject.RuntimeExtension)
+    })
+  ,
+
+  'OutputBlobIdsEntry' : _reflection.GeneratedProtocolMessageType('OutputBlobIdsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY,
+    '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.RuntimeObject.OutputBlobIdsEntry)
+    })
+  ,
   'DESCRIPTOR' : _RUNTIMEOBJECT,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.RuntimeObject)
   })
 _sym_db.RegisterMessage(RuntimeObject)
+_sym_db.RegisterMessage(RuntimeObject.RuntimeExtension)
+_sym_db.RegisterMessage(RuntimeObject.OutputBlobIdsEntry)
 
 ConditionState = _reflection.GeneratedProtocolMessageType('ConditionState', (_message.Message,), {
   'DESCRIPTOR' : _CONDITIONSTATE,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.ConditionState)
   })
 _sym_db.RegisterMessage(ConditionState)
@@ -354,128 +383,146 @@
 
   'DeliveryPromotionConfig' : _reflection.GeneratedProtocolMessageType('DeliveryPromotionConfig', (_message.Message,), {
     'DESCRIPTOR' : _SIGNAL_DELIVERYPROMOTIONCONFIG,
     '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Signal.DeliveryPromotionConfig)
     })
   ,
+
+  'ProtectionBypass' : _reflection.GeneratedProtocolMessageType('ProtectionBypass', (_message.Message,), {
+    'DESCRIPTOR' : _SIGNAL_PROTECTIONBYPASS,
+    '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Signal.ProtectionBypass)
+    })
+  ,
   'DESCRIPTOR' : _SIGNAL,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Signal)
   })
 _sym_db.RegisterMessage(Signal)
 _sym_db.RegisterMessage(Signal.DeliveryPromotionConfig)
+_sym_db.RegisterMessage(Signal.ProtectionBypass)
 
 DebugLog = _reflection.GeneratedProtocolMessageType('DebugLog', (_message.Message,), {
   'DESCRIPTOR' : _DEBUGLOG,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.DebugLog)
   })
 _sym_db.RegisterMessage(DebugLog)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/model'
   _CANARYPROGRESSSTATE.fields_by_name['canary_weight']._options = None
   _CANARYPROGRESSSTATE.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._options = None
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_options = b'8\001'
   _CUSTOMTASKSTATE.fields_by_name['name']._options = None
   _CUSTOMTASKSTATE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['description']._options = None
   _CUSTOMTASKSTATE.fields_by_name['description']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['program']._options = None
   _CUSTOMTASKSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
   _DELIVERYEXTENSIONSTATE.fields_by_name['program']._options = None
   _DELIVERYEXTENSIONSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TYPE._serialized_start=8307
-  _TYPE._serialized_end=8510
-  _LIFECYCLE._serialized_start=8513
-  _LIFECYCLE._serialized_end=8644
-  _CUSTOMTASKTYPE._serialized_start=8647
-  _CUSTOMTASKTYPE._serialized_end=8801
-  _STATUS._serialized_start=8804
-  _STATUS._serialized_end=9044
-  _SIMPLESTATUS._serialized_start=9046
-  _SIMPLESTATUS._serialized_end=9128
-  _STATUSREASON._serialized_start=9131
-  _STATUSREASON._serialized_end=9367
-  _ACTIONTYPE._serialized_start=9369
-  _ACTIONTYPE._serialized_end=9483
-  _CONDITIONSTATUS._serialized_start=9486
-  _CONDITIONSTATUS._serialized_end=9636
-  _MANUALAPPROVALSTATUS._serialized_start=9638
-  _MANUALAPPROVALSTATUS._serialized_end=9701
-  _CUSTOMTASKSTATUS._serialized_start=9704
-  _CUSTOMTASKSTATUS._serialized_end=9837
-  _SIGNALTYPE._serialized_start=9839
-  _SIGNALTYPE._serialized_end=9895
-  _PROTECTIONLINK._serialized_start=294
-  _PROTECTIONLINK._serialized_end=406
-  _CONDITION._serialized_start=409
-  _CONDITION._serialized_end=1196
-  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=716
-  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=883
-  _CONDITION_MANUALAPPROVAL._serialized_start=885
-  _CONDITION_MANUALAPPROVAL._serialized_end=916
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_start=919
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_end=1183
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_start=1082
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_end=1173
-  _IDENTIFIER._serialized_start=1198
-  _IDENTIFIER._serialized_end=1274
-  _METADATA._serialized_start=1277
-  _METADATA._serialized_end=1616
-  _STATUSEXPLANATION._serialized_start=1619
-  _STATUSEXPLANATION._serialized_end=1792
-  _ACTIONEXPLANATION._serialized_start=1795
-  _ACTIONEXPLANATION._serialized_end=1934
-  _VERSION._serialized_start=1937
-  _VERSION._serialized_end=2144
-  _SERVICEINSTANCESTATE._serialized_start=2147
-  _SERVICEINSTANCESTATE._serialized_end=2537
-  _SERVICESTATE._serialized_start=2540
-  _SERVICESTATE._serialized_end=2825
-  _SERVICEGROUPSTATE._serialized_start=2828
-  _SERVICEGROUPSTATE._serialized_end=3038
-  _CANARYPROGRESSSTATE._serialized_start=3041
-  _CANARYPROGRESSSTATE._serialized_end=3337
-  _CANARYPROGRESSSTATE_STATUS._serialized_start=3276
-  _CANARYPROGRESSSTATE_STATUS._serialized_end=3337
-  _DELIVERYSTATE._serialized_start=3340
-  _DELIVERYSTATE._serialized_end=3744
-  _DELIVERYSTATE_STATUS._serialized_start=3583
-  _DELIVERYSTATE_STATUS._serialized_end=3696
-  _RUNTIMEOBJECT._serialized_start=3747
-  _RUNTIMEOBJECT._serialized_end=4258
-  _RUNTIMEOBJECT_STATUS._serialized_start=4188
-  _RUNTIMEOBJECT_STATUS._serialized_end=4236
-  _CONDITIONSTATE._serialized_start=4260
-  _CONDITIONSTATE._serialized_end=4339
-  _CONTROLSTATE._serialized_start=4342
-  _CONTROLSTATE._serialized_end=4692
-  _MANUALAPPROVALSTATE._serialized_start=4695
-  _MANUALAPPROVALSTATE._serialized_end=4853
-  _STATE._serialized_start=4856
-  _STATE._serialized_end=5561
-  _ANNOTATIONS._serialized_start=5564
-  _ANNOTATIONS._serialized_end=5694
-  _ANNOTATIONS_ANNOTATION._serialized_start=5654
-  _ANNOTATIONS_ANNOTATION._serialized_end=5694
-  _CUSTOMTASKEXECUTIONSTATE._serialized_start=5697
-  _CUSTOMTASKEXECUTIONSTATE._serialized_end=5871
-  _CUSTOMTASKSTATE._serialized_start=5874
-  _CUSTOMTASKSTATE._serialized_end=6336
-  _PROTECTIONLINKSTATE._serialized_start=6339
-  _PROTECTIONLINKSTATE._serialized_end=6935
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=6797
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=6935
-  _PROTECTIONATTACHMENT._serialized_start=6938
-  _PROTECTIONATTACHMENT._serialized_end=7459
-  _DELIVERYEXTENSIONSTATE._serialized_start=7462
-  _DELIVERYEXTENSIONSTATE._serialized_end=8014
-  _SIGNAL._serialized_start=8017
-  _SIGNAL._serialized_end=8239
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=8175
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=8229
-  _DEBUGLOG._serialized_start=8241
-  _DEBUGLOG._serialized_end=8304
+  _TYPE._serialized_start=8981
+  _TYPE._serialized_end=9184
+  _LIFECYCLE._serialized_start=9187
+  _LIFECYCLE._serialized_end=9318
+  _CUSTOMTASKTYPE._serialized_start=9321
+  _CUSTOMTASKTYPE._serialized_end=9475
+  _STATUS._serialized_start=9478
+  _STATUS._serialized_end=9718
+  _SIMPLESTATUS._serialized_start=9720
+  _SIMPLESTATUS._serialized_end=9802
+  _STATUSREASON._serialized_start=9805
+  _STATUSREASON._serialized_end=10041
+  _ACTIONTYPE._serialized_start=10043
+  _ACTIONTYPE._serialized_end=10157
+  _CONDITIONSTATUS._serialized_start=10160
+  _CONDITIONSTATUS._serialized_end=10310
+  _MANUALAPPROVALSTATUS._serialized_start=10312
+  _MANUALAPPROVALSTATUS._serialized_end=10375
+  _CUSTOMTASKSTATUS._serialized_start=10378
+  _CUSTOMTASKSTATUS._serialized_end=10511
+  _SIGNALTYPE._serialized_start=10513
+  _SIGNALTYPE._serialized_end=10592
+  _PROTECTIONLINK._serialized_start=331
+  _PROTECTIONLINK._serialized_end=443
+  _CONDITION._serialized_start=446
+  _CONDITION._serialized_end=1233
+  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=753
+  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=920
+  _CONDITION_MANUALAPPROVAL._serialized_start=922
+  _CONDITION_MANUALAPPROVAL._serialized_end=953
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_start=956
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_end=1220
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_start=1119
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_end=1210
+  _IDENTIFIER._serialized_start=1235
+  _IDENTIFIER._serialized_end=1311
+  _METADATA._serialized_start=1314
+  _METADATA._serialized_end=1653
+  _STATUSEXPLANATION._serialized_start=1656
+  _STATUSEXPLANATION._serialized_end=1829
+  _ACTIONEXPLANATION._serialized_start=1832
+  _ACTIONEXPLANATION._serialized_end=1971
+  _VERSION._serialized_start=1974
+  _VERSION._serialized_end=2181
+  _SERVICEINSTANCESTATE._serialized_start=2184
+  _SERVICEINSTANCESTATE._serialized_end=2574
+  _SERVICESTATE._serialized_start=2577
+  _SERVICESTATE._serialized_end=2862
+  _SERVICEGROUPSTATE._serialized_start=2865
+  _SERVICEGROUPSTATE._serialized_end=3075
+  _CANARYPROGRESSSTATE._serialized_start=3078
+  _CANARYPROGRESSSTATE._serialized_end=3374
+  _CANARYPROGRESSSTATE_STATUS._serialized_start=3313
+  _CANARYPROGRESSSTATE_STATUS._serialized_end=3374
+  _DELIVERYSTATE._serialized_start=3377
+  _DELIVERYSTATE._serialized_end=3781
+  _DELIVERYSTATE_STATUS._serialized_start=3620
+  _DELIVERYSTATE_STATUS._serialized_end=3733
+  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_start=3783
+  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_end=3869
+  _RUNTIMEOBJECT._serialized_start=3872
+  _RUNTIMEOBJECT._serialized_end=4805
+  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_start=4560
+  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_end=4661
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_start=4663
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_end=4715
+  _RUNTIMEOBJECT_STATUS._serialized_start=4717
+  _RUNTIMEOBJECT_STATUS._serialized_end=4765
+  _CONDITIONSTATE._serialized_start=4807
+  _CONDITIONSTATE._serialized_end=4886
+  _CONTROLSTATE._serialized_start=4889
+  _CONTROLSTATE._serialized_end=5239
+  _MANUALAPPROVALSTATE._serialized_start=5242
+  _MANUALAPPROVALSTATE._serialized_end=5400
+  _STATE._serialized_start=5403
+  _STATE._serialized_end=6108
+  _ANNOTATIONS._serialized_start=6111
+  _ANNOTATIONS._serialized_end=6241
+  _ANNOTATIONS_ANNOTATION._serialized_start=6201
+  _ANNOTATIONS_ANNOTATION._serialized_end=6241
+  _CUSTOMTASKEXECUTIONSTATE._serialized_start=6244
+  _CUSTOMTASKEXECUTIONSTATE._serialized_end=6418
+  _CUSTOMTASKSTATE._serialized_start=6421
+  _CUSTOMTASKSTATE._serialized_end=6883
+  _PROTECTIONLINKSTATE._serialized_start=6886
+  _PROTECTIONLINKSTATE._serialized_end=7505
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=7344
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=7505
+  _PROTECTIONATTACHMENT._serialized_start=7508
+  _PROTECTIONATTACHMENT._serialized_end=8029
+  _DELIVERYEXTENSIONSTATE._serialized_start=8032
+  _DELIVERYEXTENSIONSTATE._serialized_end=8584
+  _SIGNAL._serialized_start=8587
+  _SIGNAL._serialized_end=8913
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=8829
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=8883
+  _SIGNAL_PROTECTIONBYPASS._serialized_start=8885
+  _SIGNAL_PROTECTIONBYPASS._serialized_end=8903
+  _DEBUGLOG._serialized_start=8915
+  _DEBUGLOG._serialized_end=8978
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
+import prodvana.proto.prodvana.environment.clusters_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
@@ -307,19 +308,21 @@
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _SignalTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignalType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SIGNAL_UNKNOWN: _SignalType.ValueType  # 0
     DELIVERY_PROMOTION: _SignalType.ValueType  # 1
+    PROTECTION_BYPASS: _SignalType.ValueType  # 2
 
 class SignalType(_SignalType, metaclass=_SignalTypeEnumTypeWrapper): ...
 
 SIGNAL_UNKNOWN: SignalType.ValueType  # 0
 DELIVERY_PROMOTION: SignalType.ValueType  # 1
+PROTECTION_BYPASS: SignalType.ValueType  # 2
 global___SignalType = SignalType
 
 class ProtectionLink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIFECYCLE_FIELD_NUMBER: builtins.int
     ATTACHMENT_ID_FIELD_NUMBER: builtins.int
@@ -795,14 +798,29 @@
         first_run: builtins.bool = ...,
         generation: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["canary_progress", b"canary_progress", "desired_state_id", b"desired_state_id", "first_run", b"first_run", "generation", b"generation", "message", b"message", "status", b"status"]) -> None: ...
 
 global___DeliveryState = DeliveryState
 
+class RuntimeExtensionFetchOutput(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VERSIONS_FIELD_NUMBER: builtins.int
+    @property
+    def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
+    def __init__(
+        self,
+        *,
+        versions: collections.abc.Iterable[global___Version] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["versions", b"versions"]) -> None: ...
+
+global___RuntimeExtensionFetchOutput = RuntimeExtensionFetchOutput
+
 class RuntimeObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Status:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -813,60 +831,108 @@
         FAILED: RuntimeObject._Status.ValueType  # 2
 
     class Status(_Status, metaclass=_StatusEnumTypeWrapper): ...
     PENDING: RuntimeObject.Status.ValueType  # 0
     SUCCEEDED: RuntimeObject.Status.ValueType  # 1
     FAILED: RuntimeObject.Status.ValueType  # 2
 
+    class RuntimeExtension(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        FETCH_FIELD_NUMBER: builtins.int
+        SERVICE_ID_FIELD_NUMBER: builtins.int
+        @property
+        def fetch(self) -> prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand: ...
+        service_id: builtins.str
+        def __init__(
+            self,
+            *,
+            fetch: prodvana.proto.prodvana.environment.clusters_pb2.CompiledExtensionCommand | None = ...,
+            service_id: builtins.str = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["fetch", b"fetch"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fetch", b"fetch", "service_id", b"service_id"]) -> None: ...
+
+    class OutputBlobIdsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     META_FIELD_NUMBER: builtins.int
     OBJECT_TYPE_FIELD_NUMBER: builtins.int
     NAMESPACE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     VERSIONS_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     ROLLBACK_VERSION_FIELD_NUMBER: builtins.int
     DELIVERY_FIELD_NUMBER: builtins.int
     VERSION_AGNOSTIC_FIELD_NUMBER: builtins.int
-    STATE_HASH_FIELD_NUMBER: builtins.int
     MESSAGE_FIELD_NUMBER: builtins.int
+    RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
+    OUTPUT_BLOB_IDS_FIELD_NUMBER: builtins.int
+    INTERVAL_FIELD_NUMBER: builtins.int
+    TIMEOUT_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     object_type: builtins.str
     namespace: builtins.str
     name: builtins.str
     @property
     def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
     status: global___RuntimeObject.Status.ValueType
     @property
     def rollback_version(self) -> global___Version: ...
     @property
     def delivery(self) -> global___DeliveryState: ...
     version_agnostic: builtins.bool
     """This object just needs to exist - it doesn't change from version to version"""
-    state_hash: builtins.bytes
-    """Some deterministic summary which can be used to detect if state has changed (to determine if LogDebugInfo should be called)"""
     message: builtins.str
     """Human readable message (typically for errors)."""
+    @property
+    def runtime_extension(self) -> global___RuntimeObject.RuntimeExtension:
+        """additional config if this runtime object belongs to a runtime extension"""
+    @property
+    def output_blob_ids(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
+        """if output is saved, this is the ID of the blob to retrieve it, by container name"""
+    @property
+    def interval(self) -> google.protobuf.duration_pb2.Duration:
+        """if set, runtime object is continuously applied instead of being done once when there is a version mismatch"""
+    @property
+    def timeout(self) -> google.protobuf.duration_pb2.Duration:
+        """if set, runtime object is recreated when this timeout is hit if it has not converged by then."""
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         object_type: builtins.str = ...,
         namespace: builtins.str = ...,
         name: builtins.str = ...,
         versions: collections.abc.Iterable[global___Version] | None = ...,
         status: global___RuntimeObject.Status.ValueType = ...,
         rollback_version: global___Version | None = ...,
         delivery: global___DeliveryState | None = ...,
         version_agnostic: builtins.bool = ...,
-        state_hash: builtins.bytes = ...,
         message: builtins.str = ...,
+        runtime_extension: global___RuntimeObject.RuntimeExtension | None = ...,
+        output_blob_ids: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        interval: google.protobuf.duration_pb2.Duration | None = ...,
+        timeout: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "meta", b"meta", "rollback_version", b"rollback_version"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "rollback_version", b"rollback_version", "state_hash", b"state_hash", "status", b"status", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
 
 global___RuntimeObject = RuntimeObject
 
 class ConditionState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
@@ -1107,23 +1173,25 @@
         UNKNOWN: ProtectionLinkState._StopReason.ValueType  # 0
         LIFECYCLE_COMPLETED: ProtectionLinkState._StopReason.ValueType  # 1
         SUCCEEDED_ONCE: ProtectionLinkState._StopReason.ValueType  # 2
         SUCCEEDED_FOR_DURATION: ProtectionLinkState._StopReason.ValueType  # 3
         TIMED_OUT: ProtectionLinkState._StopReason.ValueType  # 4
         FAILED: ProtectionLinkState._StopReason.ValueType  # 5
         DELETED: ProtectionLinkState._StopReason.ValueType  # 6
+        MANUALLY_BYPASSED: ProtectionLinkState._StopReason.ValueType  # 7
 
     class StopReason(_StopReason, metaclass=_StopReasonEnumTypeWrapper): ...
     UNKNOWN: ProtectionLinkState.StopReason.ValueType  # 0
     LIFECYCLE_COMPLETED: ProtectionLinkState.StopReason.ValueType  # 1
     SUCCEEDED_ONCE: ProtectionLinkState.StopReason.ValueType  # 2
     SUCCEEDED_FOR_DURATION: ProtectionLinkState.StopReason.ValueType  # 3
     TIMED_OUT: ProtectionLinkState.StopReason.ValueType  # 4
     FAILED: ProtectionLinkState.StopReason.ValueType  # 5
     DELETED: ProtectionLinkState.StopReason.ValueType  # 6
+    MANUALLY_BYPASSED: ProtectionLinkState.StopReason.ValueType  # 7
 
     META_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     LINK_FIELD_NUMBER: builtins.int
     STARTED_TIMESTAMP_FIELD_NUMBER: builtins.int
     STOPPED_TIMESTAMP_FIELD_NUMBER: builtins.int
     STOPPED_REASON_FIELD_NUMBER: builtins.int
@@ -1268,28 +1336,39 @@
             self,
             *,
             stage: builtins.int = ...,
             full: builtins.bool = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["full", b"full", "stage", b"stage"]) -> None: ...
 
+    class ProtectionBypass(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        def __init__(
+            self,
+        ) -> None: ...
+
     TYPE_FIELD_NUMBER: builtins.int
     DELIVERY_PROMOTION_FIELD_NUMBER: builtins.int
+    PROTECTION_BYPASS_FIELD_NUMBER: builtins.int
     type: global___SignalType.ValueType
     @property
     def delivery_promotion(self) -> global___Signal.DeliveryPromotionConfig: ...
+    @property
+    def protection_bypass(self) -> global___Signal.ProtectionBypass: ...
     def __init__(
         self,
         *,
         type: global___SignalType.ValueType = ...,
         delivery_promotion: global___Signal.DeliveryPromotionConfig | None = ...,
+        protection_bypass: global___Signal.ProtectionBypass | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "type", b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config", b"config"]) -> typing_extensions.Literal["delivery_promotion"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "delivery_promotion", b"delivery_promotion", "protection_bypass", b"protection_bypass", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config", b"config"]) -> typing_extensions.Literal["delivery_promotion", "protection_bypass"] | None: ...
 
 global___Signal = Signal
 
 class DebugLog(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TS_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,42 +9,46 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
+from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
+from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#prodvana/environment/clusters.proto\x12\x14prodvana.environment\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\"\xe7\x04\n\x0b\x43lusterAuth\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61_cert\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x17\n\x0fservice_account\x18\x04 \x01(\t\x12\x38\n\x03\x65\x63s\x18\x05 \x01(\x0b\x32).prodvana.environment.ClusterAuth.ECSAuthH\x00\x12M\n\x0egeneric_docker\x18\x07 \x01(\x0b\x32\x33.prodvana.environment.ClusterAuth.GenericDockerAuthH\x00\x12\x38\n\x03k8s\x18\x08 \x01(\x0b\x32).prodvana.environment.ClusterAuth.K8sAuthH\x00\x12\x16\n\x0ek8s_agent_auth\x18\x06 \x01(\x08\x1ao\n\x07\x45\x43SAuth\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x12\n\nsecret_key\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x17\n\x0f\x61ssume_role_arn\x18\x04 \x01(\t\x12\x13\n\x0b\x63luster_arn\x18\x05 \x01(\t\x1a*\n\x11GenericDockerAuth\x12\x15\n\rproxy_runtime\x18\x01 \x01(\t\x1a\x86\x01\n\x07K8sAuth\x12J\n\tagent_env\x18\x01 \x03(\x0b\x32\x37.prodvana.environment.ClusterAuth.K8sAuth.AgentEnvEntry\x1a/\n\rAgentEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0c\n\nauth_oneof\"\xe9\x02\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12\x34\n\x06origin\x18\x03 \x01(\x0e\x32$.prodvana.environment.Cluster.Origin\x12/\n\x04\x61uth\x18\x04 \x01(\x0b\x32!.prodvana.environment.ClusterAuth\x12/\n\x04type\x18\x05 \x01(\x0e\x32!.prodvana.environment.ClusterType\x12\x33\n\x06\x63onfig\x18\x06 \x01(\x0b\x32#.prodvana.environment.ClusterConfig\x12<\n\x18last_heartbeat_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x06Origin\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PRODVANA\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\"\xc6\x01\n\x11\x46\x61keClusterConfig\x12Z\n\x11\x63rashing_programs\x18\x01 \x03(\x0b\x32?.prodvana.environment.FakeClusterConfig.CrashingProgramPatterns\x1aU\n\x17\x43rashingProgramPatterns\x12\x13\n\x0bimage_regex\x18\x01 \x01(\t\x12\x11\n\tcmd_regex\x18\x02 \x01(\t\x12\x12\n\nlog_output\x18\x03 \x01(\t\"\xac\x01\n\x14GenericDockerCommand\x12\x39\n\x0btask_config\x18\x01 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x02 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\xf8\x01\n\x1aGenericDockerClusterConfig\x12\x43\n\x05\x61pply\x18\x01 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommandB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x45\n\x11get_current_state\x18\x02 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommand\x12N\n\nparameters\x18\x03 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\"\xc9\x0c\n\rClusterConfig\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x17\n\x0f\x64isable_flagger\x18\x01 \x01(\x08\x12\x15\n\rdisable_istio\x18\x02 \x01(\x08\x12>\n\x08kubecost\x18\x03 \x01(\x0b\x32,.prodvana.environment.ClusterConfig.Kubecost\x12<\n\x07\x64\x61tadog\x18\x04 \x01(\x0b\x32+.prodvana.environment.ClusterConfig.Datadog\x12\x43\n\x0b\x61lb_ingress\x18\x06 \x01(\x0b\x32..prodvana.environment.ClusterConfig.ALBIngress\x12G\n\rargo_rollouts\x18\x07 \x01(\x0b\x32\x30.prodvana.environment.ClusterConfig.ArgoRollouts\x12\x43\n\x0bgke_ingress\x18\x08 \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12P\n\x18self_managed_gke_ingress\x18\x0b \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12I\n\x0e\x63loud_provider\x18\t \x01(\x0e\x32\x31.prodvana.environment.ClusterConfig.CloudProvider\x12\x37\n\x04\x66\x61ke\x18\n \x01(\x0b\x32\'.prodvana.environment.FakeClusterConfigH\x00\x12J\n\x0egeneric_docker\x18\x0c \x01(\x0b\x32\x30.prodvana.environment.GenericDockerClusterConfigH\x00\x1aH\n\x08Kubecost\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x1a\n\x12kubecost_namespace\x18\x03 \x01(\t\x1a\x65\n\x07\x44\x61tadog\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x61tadog_namespace\x18\x03 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x04 \x01(\t\x12\x0c\n\x04site\x18\x05 \x01(\t\x1a\x62\n\nALBIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\ringress_class\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12#\n\x1b\x64\x65\x66\x61ult_balancer_attributes\x18\x03 \x03(\t\x1a\xba\x03\n\x0c\x41rgoRollouts\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\ttemplates\x18\x02 \x03(\x0b\x32\x41.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate\x1a\xc2\x02\n\x10\x41nalysisTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x66\n\x0b\x61rg_mapping\x18\x02 \x03(\x0b\x32Q.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgMappingEntry\x1a}\n\x0f\x41rgMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0e\x32J.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgValue:\x02\x38\x01\"9\n\x08\x41rgValue\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x13\n\x0fRELEASE_CHANNEL\x10\x02\x1a\x37\n\nGKEIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10\x63ontainer_native\x18\x02 \x01(\x08\"T\n\rCloudProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x45KS\x10\x01\x12\x07\n\x03GKE\x10\x02\x12\x07\n\x03\x41KS\x10\x03\x12\n\n\x06ONPREM\x10\x04\x12\x0f\n\x0bOTHER_CLOUD\x10\x05\x42\x0f\n\rcluster_oneofJ\x04\x08\x05\x10\x06R\x0f\x61ws_alb_ingress*J\n\x0b\x43lusterType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03K8S\x10\x01\x12\x07\n\x03\x45\x43S\x10\x02\x12\x08\n\x04\x46\x41KE\x10\x03\x12\x12\n\x0eGENERIC_DOCKER\x10\x04\x42PZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environmentb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#prodvana/environment/clusters.proto\x12\x14prodvana.environment\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a prodvana/common_config/env.proto\x1a!prodvana/common_config/task.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xfd\x03\n\x0b\x43lusterAuth\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61_cert\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x17\n\x0fservice_account\x18\x04 \x01(\t\x12\x38\n\x03\x65\x63s\x18\x05 \x01(\x0b\x32).prodvana.environment.ClusterAuth.ECSAuthH\x00\x12\x38\n\x03k8s\x18\x08 \x01(\x0b\x32).prodvana.environment.ClusterAuth.K8sAuthH\x00\x12\x16\n\x0ek8s_agent_auth\x18\x06 \x01(\x08\x1ao\n\x07\x45\x43SAuth\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x12\n\nsecret_key\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x17\n\x0f\x61ssume_role_arn\x18\x04 \x01(\t\x12\x13\n\x0b\x63luster_arn\x18\x05 \x01(\t\x1a\x86\x01\n\x07K8sAuth\x12J\n\tagent_env\x18\x01 \x03(\x0b\x32\x37.prodvana.environment.ClusterAuth.K8sAuth.AgentEnvEntry\x1a/\n\rAgentEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0c\n\nauth_oneofJ\x04\x08\x07\x10\x08R\textension\"\xe9\x02\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12\x34\n\x06origin\x18\x03 \x01(\x0e\x32$.prodvana.environment.Cluster.Origin\x12/\n\x04\x61uth\x18\x04 \x01(\x0b\x32!.prodvana.environment.ClusterAuth\x12/\n\x04type\x18\x05 \x01(\x0e\x32!.prodvana.environment.ClusterType\x12\x33\n\x06\x63onfig\x18\x06 \x01(\x0b\x32#.prodvana.environment.ClusterConfig\x12<\n\x18last_heartbeat_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x06Origin\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PRODVANA\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\"\xc6\x01\n\x11\x46\x61keClusterConfig\x12Z\n\x11\x63rashing_programs\x18\x01 \x03(\x0b\x32?.prodvana.environment.FakeClusterConfig.CrashingProgramPatterns\x1aU\n\x17\x43rashingProgramPatterns\x12\x13\n\x0bimage_regex\x18\x01 \x01(\t\x12\x11\n\tcmd_regex\x18\x02 \x01(\t\x12\x12\n\nlog_output\x18\x03 \x01(\t\"\x86\x02\n\x10\x45xtensionCommand\x12\x39\n\x0btask_config\x18\x01 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x02 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x30\n\rpoll_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\xac\x02\n\x16\x45xtensionClusterConfig\x12?\n\x05\x61pply\x18\x01 \x01(\x0b\x32&.prodvana.environment.ExtensionCommandB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x35\n\x05\x66\x65tch\x18\x02 \x01(\x0b\x32&.prodvana.environment.ExtensionCommand\x12N\n\nparameters\x18\x03 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\rproxy_runtime\x18\x04 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"\xc2\x02\n\x18\x43ompiledExtensionCommand\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x37\n\x07\x63ommand\x18\x02 \x01(\x0b\x32&.prodvana.environment.ExtensionCommand\x12\x44\n\x11runtime_execution\x18\x03 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x44\n\x03\x65nv\x18\x04 \x03(\x0b\x32\x37.prodvana.environment.CompiledExtensionCommand.EnvEntry\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xc0\x0c\n\rClusterConfig\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x17\n\x0f\x64isable_flagger\x18\x01 \x01(\x08\x12\x15\n\rdisable_istio\x18\x02 \x01(\x08\x12>\n\x08kubecost\x18\x03 \x01(\x0b\x32,.prodvana.environment.ClusterConfig.Kubecost\x12<\n\x07\x64\x61tadog\x18\x04 \x01(\x0b\x32+.prodvana.environment.ClusterConfig.Datadog\x12\x43\n\x0b\x61lb_ingress\x18\x06 \x01(\x0b\x32..prodvana.environment.ClusterConfig.ALBIngress\x12G\n\rargo_rollouts\x18\x07 \x01(\x0b\x32\x30.prodvana.environment.ClusterConfig.ArgoRollouts\x12\x43\n\x0bgke_ingress\x18\x08 \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12P\n\x18self_managed_gke_ingress\x18\x0b \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12I\n\x0e\x63loud_provider\x18\t \x01(\x0e\x32\x31.prodvana.environment.ClusterConfig.CloudProvider\x12\x37\n\x04\x66\x61ke\x18\n \x01(\x0b\x32\'.prodvana.environment.FakeClusterConfigH\x00\x12\x41\n\textension\x18\x0c \x01(\x0b\x32,.prodvana.environment.ExtensionClusterConfigH\x00\x1aH\n\x08Kubecost\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x1a\n\x12kubecost_namespace\x18\x03 \x01(\t\x1a\x65\n\x07\x44\x61tadog\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x61tadog_namespace\x18\x03 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x04 \x01(\t\x12\x0c\n\x04site\x18\x05 \x01(\t\x1a\x62\n\nALBIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\ringress_class\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12#\n\x1b\x64\x65\x66\x61ult_balancer_attributes\x18\x03 \x03(\t\x1a\xba\x03\n\x0c\x41rgoRollouts\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\ttemplates\x18\x02 \x03(\x0b\x32\x41.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate\x1a\xc2\x02\n\x10\x41nalysisTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x66\n\x0b\x61rg_mapping\x18\x02 \x03(\x0b\x32Q.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgMappingEntry\x1a}\n\x0f\x41rgMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0e\x32J.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgValue:\x02\x38\x01\"9\n\x08\x41rgValue\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x13\n\x0fRELEASE_CHANNEL\x10\x02\x1a\x37\n\nGKEIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10\x63ontainer_native\x18\x02 \x01(\x08\"T\n\rCloudProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x45KS\x10\x01\x12\x07\n\x03GKE\x10\x02\x12\x07\n\x03\x41KS\x10\x03\x12\n\n\x06ONPREM\x10\x04\x12\x0f\n\x0bOTHER_CLOUD\x10\x05\x42\x0f\n\rcluster_oneofJ\x04\x08\x05\x10\x06R\x0f\x61ws_alb_ingress*E\n\x0b\x43lusterType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03K8S\x10\x01\x12\x07\n\x03\x45\x43S\x10\x02\x12\x08\n\x04\x46\x41KE\x10\x03\x12\r\n\tEXTENSION\x10\x04\x42PZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environmentb\x06proto3')
 
 _CLUSTERTYPE = DESCRIPTOR.enum_types_by_name['ClusterType']
 ClusterType = enum_type_wrapper.EnumTypeWrapper(_CLUSTERTYPE)
 UNKNOWN = 0
 K8S = 1
 ECS = 2
 FAKE = 3
-GENERIC_DOCKER = 4
+EXTENSION = 4
 
 
 _CLUSTERAUTH = DESCRIPTOR.message_types_by_name['ClusterAuth']
 _CLUSTERAUTH_ECSAUTH = _CLUSTERAUTH.nested_types_by_name['ECSAuth']
-_CLUSTERAUTH_GENERICDOCKERAUTH = _CLUSTERAUTH.nested_types_by_name['GenericDockerAuth']
 _CLUSTERAUTH_K8SAUTH = _CLUSTERAUTH.nested_types_by_name['K8sAuth']
 _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY = _CLUSTERAUTH_K8SAUTH.nested_types_by_name['AgentEnvEntry']
 _CLUSTER = DESCRIPTOR.message_types_by_name['Cluster']
 _FAKECLUSTERCONFIG = DESCRIPTOR.message_types_by_name['FakeClusterConfig']
 _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS = _FAKECLUSTERCONFIG.nested_types_by_name['CrashingProgramPatterns']
-_GENERICDOCKERCOMMAND = DESCRIPTOR.message_types_by_name['GenericDockerCommand']
-_GENERICDOCKERCLUSTERCONFIG = DESCRIPTOR.message_types_by_name['GenericDockerClusterConfig']
+_EXTENSIONCOMMAND = DESCRIPTOR.message_types_by_name['ExtensionCommand']
+_EXTENSIONCLUSTERCONFIG = DESCRIPTOR.message_types_by_name['ExtensionClusterConfig']
+_COMPILEDEXTENSIONCOMMAND = DESCRIPTOR.message_types_by_name['CompiledExtensionCommand']
+_COMPILEDEXTENSIONCOMMAND_ENVENTRY = _COMPILEDEXTENSIONCOMMAND.nested_types_by_name['EnvEntry']
 _CLUSTERCONFIG = DESCRIPTOR.message_types_by_name['ClusterConfig']
 _CLUSTERCONFIG_KUBECOST = _CLUSTERCONFIG.nested_types_by_name['Kubecost']
 _CLUSTERCONFIG_DATADOG = _CLUSTERCONFIG.nested_types_by_name['Datadog']
 _CLUSTERCONFIG_ALBINGRESS = _CLUSTERCONFIG.nested_types_by_name['ALBIngress']
 _CLUSTERCONFIG_ARGOROLLOUTS = _CLUSTERCONFIG.nested_types_by_name['ArgoRollouts']
 _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE = _CLUSTERCONFIG_ARGOROLLOUTS.nested_types_by_name['AnalysisTemplate']
 _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY = _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE.nested_types_by_name['ArgMappingEntry']
@@ -57,21 +61,14 @@
   'ECSAuth' : _reflection.GeneratedProtocolMessageType('ECSAuth', (_message.Message,), {
     'DESCRIPTOR' : _CLUSTERAUTH_ECSAUTH,
     '__module__' : 'prodvana.environment.clusters_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.environment.ClusterAuth.ECSAuth)
     })
   ,
 
-  'GenericDockerAuth' : _reflection.GeneratedProtocolMessageType('GenericDockerAuth', (_message.Message,), {
-    'DESCRIPTOR' : _CLUSTERAUTH_GENERICDOCKERAUTH,
-    '__module__' : 'prodvana.environment.clusters_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.environment.ClusterAuth.GenericDockerAuth)
-    })
-  ,
-
   'K8sAuth' : _reflection.GeneratedProtocolMessageType('K8sAuth', (_message.Message,), {
 
     'AgentEnvEntry' : _reflection.GeneratedProtocolMessageType('AgentEnvEntry', (_message.Message,), {
       'DESCRIPTOR' : _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY,
       '__module__' : 'prodvana.environment.clusters_pb2'
       # @@protoc_insertion_point(class_scope:prodvana.environment.ClusterAuth.K8sAuth.AgentEnvEntry)
       })
@@ -83,15 +80,14 @@
   ,
   'DESCRIPTOR' : _CLUSTERAUTH,
   '__module__' : 'prodvana.environment.clusters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.environment.ClusterAuth)
   })
 _sym_db.RegisterMessage(ClusterAuth)
 _sym_db.RegisterMessage(ClusterAuth.ECSAuth)
-_sym_db.RegisterMessage(ClusterAuth.GenericDockerAuth)
 _sym_db.RegisterMessage(ClusterAuth.K8sAuth)
 _sym_db.RegisterMessage(ClusterAuth.K8sAuth.AgentEnvEntry)
 
 Cluster = _reflection.GeneratedProtocolMessageType('Cluster', (_message.Message,), {
   'DESCRIPTOR' : _CLUSTER,
   '__module__' : 'prodvana.environment.clusters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.environment.Cluster)
@@ -109,27 +105,42 @@
   'DESCRIPTOR' : _FAKECLUSTERCONFIG,
   '__module__' : 'prodvana.environment.clusters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.environment.FakeClusterConfig)
   })
 _sym_db.RegisterMessage(FakeClusterConfig)
 _sym_db.RegisterMessage(FakeClusterConfig.CrashingProgramPatterns)
 
-GenericDockerCommand = _reflection.GeneratedProtocolMessageType('GenericDockerCommand', (_message.Message,), {
-  'DESCRIPTOR' : _GENERICDOCKERCOMMAND,
+ExtensionCommand = _reflection.GeneratedProtocolMessageType('ExtensionCommand', (_message.Message,), {
+  'DESCRIPTOR' : _EXTENSIONCOMMAND,
   '__module__' : 'prodvana.environment.clusters_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.environment.GenericDockerCommand)
+  # @@protoc_insertion_point(class_scope:prodvana.environment.ExtensionCommand)
   })
-_sym_db.RegisterMessage(GenericDockerCommand)
+_sym_db.RegisterMessage(ExtensionCommand)
 
-GenericDockerClusterConfig = _reflection.GeneratedProtocolMessageType('GenericDockerClusterConfig', (_message.Message,), {
-  'DESCRIPTOR' : _GENERICDOCKERCLUSTERCONFIG,
+ExtensionClusterConfig = _reflection.GeneratedProtocolMessageType('ExtensionClusterConfig', (_message.Message,), {
+  'DESCRIPTOR' : _EXTENSIONCLUSTERCONFIG,
+  '__module__' : 'prodvana.environment.clusters_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.environment.ExtensionClusterConfig)
+  })
+_sym_db.RegisterMessage(ExtensionClusterConfig)
+
+CompiledExtensionCommand = _reflection.GeneratedProtocolMessageType('CompiledExtensionCommand', (_message.Message,), {
+
+  'EnvEntry' : _reflection.GeneratedProtocolMessageType('EnvEntry', (_message.Message,), {
+    'DESCRIPTOR' : _COMPILEDEXTENSIONCOMMAND_ENVENTRY,
+    '__module__' : 'prodvana.environment.clusters_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.environment.CompiledExtensionCommand.EnvEntry)
+    })
+  ,
+  'DESCRIPTOR' : _COMPILEDEXTENSIONCOMMAND,
   '__module__' : 'prodvana.environment.clusters_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.environment.GenericDockerClusterConfig)
+  # @@protoc_insertion_point(class_scope:prodvana.environment.CompiledExtensionCommand)
   })
-_sym_db.RegisterMessage(GenericDockerClusterConfig)
+_sym_db.RegisterMessage(CompiledExtensionCommand)
+_sym_db.RegisterMessage(CompiledExtensionCommand.EnvEntry)
 
 ClusterConfig = _reflection.GeneratedProtocolMessageType('ClusterConfig', (_message.Message,), {
 
   'Kubecost' : _reflection.GeneratedProtocolMessageType('Kubecost', (_message.Message,), {
     'DESCRIPTOR' : _CLUSTERCONFIG_KUBECOST,
     '__module__' : 'prodvana.environment.clusters_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.environment.ClusterConfig.Kubecost)
@@ -192,62 +203,68 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environment'
   _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._options = None
   _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_options = b'8\001'
-  _GENERICDOCKERCOMMAND.oneofs_by_name['exec_config']._options = None
-  _GENERICDOCKERCOMMAND.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
-  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['apply']._options = None
-  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['apply']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['parameters']._options = None
-  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _EXTENSIONCOMMAND.oneofs_by_name['exec_config']._options = None
+  _EXTENSIONCOMMAND.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['apply']._options = None
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['apply']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['parameters']._options = None
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['proxy_runtime']._options = None
+  _EXTENSIONCLUSTERCONFIG.fields_by_name['proxy_runtime']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _COMPILEDEXTENSIONCOMMAND_ENVENTRY._options = None
+  _COMPILEDEXTENSIONCOMMAND_ENVENTRY._serialized_options = b'8\001'
   _CLUSTERCONFIG_ALBINGRESS.fields_by_name['ingress_class']._options = None
   _CLUSTERCONFIG_ALBINGRESS.fields_by_name['ingress_class']._serialized_options = b'\372B\004r\002\020\001'
   _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._options = None
   _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_options = b'8\001'
-  _CLUSTERTYPE._serialized_start=3464
-  _CLUSTERTYPE._serialized_end=3538
-  _CLUSTERAUTH._serialized_start=244
-  _CLUSTERAUTH._serialized_end=859
-  _CLUSTERAUTH_ECSAUTH._serialized_start=553
-  _CLUSTERAUTH_ECSAUTH._serialized_end=664
-  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_start=666
-  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_end=708
-  _CLUSTERAUTH_K8SAUTH._serialized_start=711
-  _CLUSTERAUTH_K8SAUTH._serialized_end=845
-  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_start=798
-  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_end=845
-  _CLUSTER._serialized_start=862
-  _CLUSTER._serialized_end=1223
-  _CLUSTER_ORIGIN._serialized_start=1174
-  _CLUSTER_ORIGIN._serialized_end=1223
-  _FAKECLUSTERCONFIG._serialized_start=1226
-  _FAKECLUSTERCONFIG._serialized_end=1424
-  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_start=1339
-  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_end=1424
-  _GENERICDOCKERCOMMAND._serialized_start=1427
-  _GENERICDOCKERCOMMAND._serialized_end=1599
-  _GENERICDOCKERCLUSTERCONFIG._serialized_start=1602
-  _GENERICDOCKERCLUSTERCONFIG._serialized_end=1850
-  _CLUSTERCONFIG._serialized_start=1853
-  _CLUSTERCONFIG._serialized_end=3462
-  _CLUSTERCONFIG_KUBECOST._serialized_start=2559
-  _CLUSTERCONFIG_KUBECOST._serialized_end=2631
-  _CLUSTERCONFIG_DATADOG._serialized_start=2633
-  _CLUSTERCONFIG_DATADOG._serialized_end=2734
-  _CLUSTERCONFIG_ALBINGRESS._serialized_start=2736
-  _CLUSTERCONFIG_ALBINGRESS._serialized_end=2834
-  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_start=2837
-  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_end=3279
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_start=2957
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_end=3279
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_start=3095
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_end=3220
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_start=3222
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_end=3279
-  _CLUSTERCONFIG_GKEINGRESS._serialized_start=3281
-  _CLUSTERCONFIG_GKEINGRESS._serialized_end=3336
-  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_start=3338
-  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_end=3422
+  _CLUSTERTYPE._serialized_start=3923
+  _CLUSTERTYPE._serialized_end=3992
+  _CLUSTERAUTH._serialized_start=351
+  _CLUSTERAUTH._serialized_end=860
+  _CLUSTERAUTH_ECSAUTH._serialized_start=581
+  _CLUSTERAUTH_ECSAUTH._serialized_end=692
+  _CLUSTERAUTH_K8SAUTH._serialized_start=695
+  _CLUSTERAUTH_K8SAUTH._serialized_end=829
+  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_start=782
+  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_end=829
+  _CLUSTER._serialized_start=863
+  _CLUSTER._serialized_end=1224
+  _CLUSTER_ORIGIN._serialized_start=1175
+  _CLUSTER_ORIGIN._serialized_end=1224
+  _FAKECLUSTERCONFIG._serialized_start=1227
+  _FAKECLUSTERCONFIG._serialized_end=1425
+  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_start=1340
+  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_end=1425
+  _EXTENSIONCOMMAND._serialized_start=1428
+  _EXTENSIONCOMMAND._serialized_end=1690
+  _EXTENSIONCLUSTERCONFIG._serialized_start=1693
+  _EXTENSIONCLUSTERCONFIG._serialized_end=1993
+  _COMPILEDEXTENSIONCOMMAND._serialized_start=1996
+  _COMPILEDEXTENSIONCOMMAND._serialized_end=2318
+  _COMPILEDEXTENSIONCOMMAND_ENVENTRY._serialized_start=2242
+  _COMPILEDEXTENSIONCOMMAND_ENVENTRY._serialized_end=2318
+  _CLUSTERCONFIG._serialized_start=2321
+  _CLUSTERCONFIG._serialized_end=3921
+  _CLUSTERCONFIG_KUBECOST._serialized_start=3018
+  _CLUSTERCONFIG_KUBECOST._serialized_end=3090
+  _CLUSTERCONFIG_DATADOG._serialized_start=3092
+  _CLUSTERCONFIG_DATADOG._serialized_end=3193
+  _CLUSTERCONFIG_ALBINGRESS._serialized_start=3195
+  _CLUSTERCONFIG_ALBINGRESS._serialized_end=3293
+  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_start=3296
+  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_end=3738
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_start=3416
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_end=3738
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_start=3554
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_end=3679
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_start=3681
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_end=3738
+  _CLUSTERCONFIG_GKEINGRESS._serialized_start=3740
+  _CLUSTERCONFIG_GKEINGRESS._serialized_end=3795
+  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_start=3797
+  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_end=3881
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.common_config.env_pb2
 import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
+import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -28,23 +31,23 @@
 
 class _ClusterTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ClusterType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _ClusterType.ValueType  # 0
     K8S: _ClusterType.ValueType  # 1
     ECS: _ClusterType.ValueType  # 2
     FAKE: _ClusterType.ValueType  # 3
-    GENERIC_DOCKER: _ClusterType.ValueType  # 4
+    EXTENSION: _ClusterType.ValueType  # 4
 
 class ClusterType(_ClusterType, metaclass=_ClusterTypeEnumTypeWrapper): ...
 
 UNKNOWN: ClusterType.ValueType  # 0
 K8S: ClusterType.ValueType  # 1
 ECS: ClusterType.ValueType  # 2
 FAKE: ClusterType.ValueType  # 3
-GENERIC_DOCKER: ClusterType.ValueType  # 4
+EXTENSION: ClusterType.ValueType  # 4
 global___ClusterType = ClusterType
 
 class ClusterAuth(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class ECSAuth(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -66,26 +69,14 @@
             secret_key: builtins.str = ...,
             region: builtins.str = ...,
             assume_role_arn: builtins.str = ...,
             cluster_arn: builtins.str = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["access_key", b"access_key", "assume_role_arn", b"assume_role_arn", "cluster_arn", b"cluster_arn", "region", b"region", "secret_key", b"secret_key"]) -> None: ...
 
-    class GenericDockerAuth(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        PROXY_RUNTIME_FIELD_NUMBER: builtins.int
-        proxy_runtime: builtins.str
-        def __init__(
-            self,
-            *,
-            proxy_runtime: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["proxy_runtime", b"proxy_runtime"]) -> None: ...
-
     class K8sAuth(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         class AgentEnvEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             KEY_FIELD_NUMBER: builtins.int
@@ -111,43 +102,39 @@
         def ClearField(self, field_name: typing_extensions.Literal["agent_env", b"agent_env"]) -> None: ...
 
     ENDPOINT_FIELD_NUMBER: builtins.int
     CA_CERT_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     SERVICE_ACCOUNT_FIELD_NUMBER: builtins.int
     ECS_FIELD_NUMBER: builtins.int
-    GENERIC_DOCKER_FIELD_NUMBER: builtins.int
     K8S_FIELD_NUMBER: builtins.int
     K8S_AGENT_AUTH_FIELD_NUMBER: builtins.int
     endpoint: builtins.str
     ca_cert: builtins.str
     token: builtins.str
     service_account: builtins.str
     @property
     def ecs(self) -> global___ClusterAuth.ECSAuth: ...
     @property
-    def generic_docker(self) -> global___ClusterAuth.GenericDockerAuth: ...
-    @property
     def k8s(self) -> global___ClusterAuth.K8sAuth: ...
     k8s_agent_auth: builtins.bool
     def __init__(
         self,
         *,
         endpoint: builtins.str = ...,
         ca_cert: builtins.str = ...,
         token: builtins.str = ...,
         service_account: builtins.str = ...,
         ecs: global___ClusterAuth.ECSAuth | None = ...,
-        generic_docker: global___ClusterAuth.GenericDockerAuth | None = ...,
         k8s: global___ClusterAuth.K8sAuth | None = ...,
         k8s_agent_auth: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auth_oneof", b"auth_oneof", "ecs", b"ecs", "generic_docker", b"generic_docker", "k8s", b"k8s"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["auth_oneof", b"auth_oneof", "ca_cert", b"ca_cert", "ecs", b"ecs", "endpoint", b"endpoint", "generic_docker", b"generic_docker", "k8s", b"k8s", "k8s_agent_auth", b"k8s_agent_auth", "service_account", b"service_account", "token", b"token"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["auth_oneof", b"auth_oneof"]) -> typing_extensions.Literal["ecs", "generic_docker", "k8s"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auth_oneof", b"auth_oneof", "ecs", b"ecs", "k8s", b"k8s"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["auth_oneof", b"auth_oneof", "ca_cert", b"ca_cert", "ecs", b"ecs", "endpoint", b"endpoint", "k8s", b"k8s", "k8s_agent_auth", b"k8s_agent_auth", "service_account", b"service_account", "token", b"token"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["auth_oneof", b"auth_oneof"]) -> typing_extensions.Literal["ecs", "k8s"] | None: ...
 
 global___ClusterAuth = ClusterAuth
 
 class Cluster(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Origin:
@@ -233,58 +220,119 @@
         *,
         crashing_programs: collections.abc.Iterable[global___FakeClusterConfig.CrashingProgramPatterns] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["crashing_programs", b"crashing_programs"]) -> None: ...
 
 global___FakeClusterConfig = FakeClusterConfig
 
-class GenericDockerCommand(google.protobuf.message.Message):
+class ExtensionCommand(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TASK_CONFIG_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
+    POLL_INTERVAL_FIELD_NUMBER: builtins.int
+    TIMEOUT_FIELD_NUMBER: builtins.int
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
+    @property
+    def poll_interval(self) -> google.protobuf.duration_pb2.Duration:
+        """customize intervals instead of using Prodvana default
+        only used for fetch
+        how often to run command after it succeeds
+        """
+    @property
+    def timeout(self) -> google.protobuf.duration_pb2.Duration:
+        """how long after a run has started to try another run if it has not completed yet"""
     def __init__(
         self,
         *,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
+        poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
+        timeout: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
-global___GenericDockerCommand = GenericDockerCommand
+global___ExtensionCommand = ExtensionCommand
 
-class GenericDockerClusterConfig(google.protobuf.message.Message):
+class ExtensionClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLY_FIELD_NUMBER: builtins.int
-    GET_CURRENT_STATE_FIELD_NUMBER: builtins.int
+    FETCH_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
+    PROXY_RUNTIME_FIELD_NUMBER: builtins.int
     @property
-    def apply(self) -> global___GenericDockerCommand: ...
+    def apply(self) -> global___ExtensionCommand: ...
     @property
-    def get_current_state(self) -> global___GenericDockerCommand: ...
+    def fetch(self) -> global___ExtensionCommand: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
+    @property
+    def proxy_runtime(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
     def __init__(
         self,
         *,
-        apply: global___GenericDockerCommand | None = ...,
-        get_current_state: global___GenericDockerCommand | None = ...,
+        apply: global___ExtensionCommand | None = ...,
+        fetch: global___ExtensionCommand | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
+        proxy_runtime: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "proxy_runtime", b"proxy_runtime"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "fetch", b"fetch", "parameters", b"parameters", "proxy_runtime", b"proxy_runtime"]) -> None: ...
+
+global___ExtensionClusterConfig = ExtensionClusterConfig
+
+class CompiledExtensionCommand(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class EnvEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        @property
+        def value(self) -> prodvana.proto.prodvana.common_config.env_pb2.EnvValue: ...
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: prodvana.proto.prodvana.common_config.env_pb2.EnvValue | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    NAME_PREFIX_FIELD_NUMBER: builtins.int
+    COMMAND_FIELD_NUMBER: builtins.int
+    RUNTIME_EXECUTION_FIELD_NUMBER: builtins.int
+    ENV_FIELD_NUMBER: builtins.int
+    name_prefix: builtins.str
+    @property
+    def command(self) -> global___ExtensionCommand: ...
+    @property
+    def runtime_execution(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
+    @property
+    def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]: ...
+    def __init__(
+        self,
+        *,
+        name_prefix: builtins.str = ...,
+        command: global___ExtensionCommand | None = ...,
+        runtime_execution: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
+        env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["apply", b"apply", "get_current_state", b"get_current_state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "get_current_state", b"get_current_state", "parameters", b"parameters"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["command", b"command", "runtime_execution", b"runtime_execution"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["command", b"command", "env", b"env", "name_prefix", b"name_prefix", "runtime_execution", b"runtime_execution"]) -> None: ...
 
-global___GenericDockerClusterConfig = GenericDockerClusterConfig
+global___CompiledExtensionCommand = CompiledExtensionCommand
 
 class ClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CloudProvider:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
@@ -458,15 +506,15 @@
     DATADOG_FIELD_NUMBER: builtins.int
     ALB_INGRESS_FIELD_NUMBER: builtins.int
     ARGO_ROLLOUTS_FIELD_NUMBER: builtins.int
     GKE_INGRESS_FIELD_NUMBER: builtins.int
     SELF_MANAGED_GKE_INGRESS_FIELD_NUMBER: builtins.int
     CLOUD_PROVIDER_FIELD_NUMBER: builtins.int
     FAKE_FIELD_NUMBER: builtins.int
-    GENERIC_DOCKER_FIELD_NUMBER: builtins.int
+    EXTENSION_FIELD_NUMBER: builtins.int
     name: builtins.str
     disable_flagger: builtins.bool
     disable_istio: builtins.bool
     @property
     def kubecost(self) -> global___ClusterConfig.Kubecost: ...
     @property
     def datadog(self) -> global___ClusterConfig.Datadog: ...
@@ -482,29 +530,29 @@
         but does not create an ingress object for you
         """
     cloud_provider: global___ClusterConfig.CloudProvider.ValueType
     @property
     def fake(self) -> global___FakeClusterConfig:
         """only used for fake runtimes"""
     @property
-    def generic_docker(self) -> global___GenericDockerClusterConfig: ...
+    def extension(self) -> global___ExtensionClusterConfig: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         disable_flagger: builtins.bool = ...,
         disable_istio: builtins.bool = ...,
         kubecost: global___ClusterConfig.Kubecost | None = ...,
         datadog: global___ClusterConfig.Datadog | None = ...,
         alb_ingress: global___ClusterConfig.ALBIngress | None = ...,
         argo_rollouts: global___ClusterConfig.ArgoRollouts | None = ...,
         gke_ingress: global___ClusterConfig.GKEIngress | None = ...,
         self_managed_gke_ingress: global___ClusterConfig.GKEIngress | None = ...,
         cloud_provider: global___ClusterConfig.CloudProvider.ValueType = ...,
         fake: global___FakeClusterConfig | None = ...,
-        generic_docker: global___GenericDockerClusterConfig | None = ...,
+        extension: global___ExtensionClusterConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "fake", b"fake", "generic_docker", b"generic_docker", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cloud_provider", b"cloud_provider", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "disable_flagger", b"disable_flagger", "disable_istio", b"disable_istio", "fake", b"fake", "generic_docker", b"generic_docker", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "name", b"name", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["cluster_oneof", b"cluster_oneof"]) -> typing_extensions.Literal["fake", "generic_docker"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["alb_ingress", b"alb_ingress", "argo_rollouts", b"argo_rollouts", "cloud_provider", b"cloud_provider", "cluster_oneof", b"cluster_oneof", "datadog", b"datadog", "disable_flagger", b"disable_flagger", "disable_istio", b"disable_istio", "extension", b"extension", "fake", b"fake", "gke_ingress", b"gke_ingress", "kubecost", b"kubecost", "name", b"name", "self_managed_gke_ingress", b"self_managed_gke_ingress"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["cluster_oneof", b"cluster_oneof"]) -> typing_extensions.Literal["fake", "extension"] | None: ...
 
 global___ClusterConfig = ClusterConfig
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 from prodvana.proto.prodvana.protection import attachments_pb2 as prodvana_dot_protection_dot_attachments__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a\x1egoogle/protobuf/duration.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xba\x04\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12Q\n\x0bprotections\x18\x08 \x03(\x0b\x32<.prodvana.release_channel.ProtectionReleaseChannelAttachment\x12U\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32\x34.prodvana.protection.ProtectionConvergenceAttachment\"\xed\x01\n\"ProtectionReleaseChannelAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\"\xf1\x03\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x1a\\\n\x14ReleaseChannelStable\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x10\n\x0eManualApproval\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTaskB\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xcf\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x45\n\x0f\x63onnection_name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12H\n\x0f\x63onnection_type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability*T\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\x0b\n\x07GENERIC\x10\x02\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a\x1egoogle/protobuf/duration.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xba\x04\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12Q\n\x0bprotections\x18\x08 \x03(\x0b\x32<.prodvana.release_channel.ProtectionReleaseChannelAttachment\x12U\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32\x34.prodvana.protection.ProtectionConvergenceAttachment\"\xed\x01\n\"ProtectionReleaseChannelAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\"\xf1\x03\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x1a\\\n\x14ReleaseChannelStable\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x10\n\x0eManualApproval\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTaskB\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xb9\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\x04name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12=\n\x04type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability*V\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\r\n\tEXTENSION\x10\x02\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
 
 _RUNTIMECONNECTIONTYPE = DESCRIPTOR.enum_types_by_name['RuntimeConnectionType']
 RuntimeConnectionType = enum_type_wrapper.EnumTypeWrapper(_RUNTIMECONNECTIONTYPE)
 UNKNOWN_CONNECTION = 0
 LONG_LIVED_COMPUTE = 1
-GENERIC = 2
+EXTENSION = 2
 
 
 _POLICY = DESCRIPTOR.message_types_by_name['Policy']
 _POLICY_DEFAULTENVENTRY = _POLICY.nested_types_by_name['DefaultEnvEntry']
 _RELEASECHANNELCONFIG = DESCRIPTOR.message_types_by_name['ReleaseChannelConfig']
 _PROTECTIONRELEASECHANNELATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionReleaseChannelAttachment']
 _PRECONDITION = DESCRIPTOR.message_types_by_name['Precondition']
@@ -123,18 +123,18 @@
   _PROTECTIONRELEASECHANNELATTACHMENT.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _PROTECTIONRELEASECHANNELATTACHMENT.fields_by_name['ref']._options = None
   _PROTECTIONRELEASECHANNELATTACHMENT.fields_by_name['ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _PROTECTIONRELEASECHANNELATTACHMENT.fields_by_name['lifecycle']._options = None
   _PROTECTIONRELEASECHANNELATTACHMENT.fields_by_name['lifecycle']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['runtime']._options = None
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['runtime']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
-  _RELEASECHANNELRUNTIMECONFIG.fields_by_name['connection_name']._options = None
-  _RELEASECHANNELRUNTIMECONFIG.fields_by_name['connection_name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
-  _RUNTIMECONNECTIONTYPE._serialized_start=2280
-  _RUNTIMECONNECTIONTYPE._serialized_end=2364
+  _RELEASECHANNELRUNTIMECONFIG.fields_by_name['name']._options = None
+  _RELEASECHANNELRUNTIMECONFIG.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
+  _RUNTIMECONNECTIONTYPE._serialized_start=2258
+  _RUNTIMECONNECTIONTYPE._serialized_end=2344
   _POLICY._serialized_start=422
   _POLICY._serialized_end=627
   _POLICY_DEFAULTENVENTRY._serialized_start=544
   _POLICY_DEFAULTENVENTRY._serialized_end=627
   _RELEASECHANNELCONFIG._serialized_start=630
   _RELEASECHANNELCONFIG._serialized_end=1200
   _PROTECTIONRELEASECHANNELATTACHMENT._serialized_start=1203
@@ -144,9 +144,9 @@
   _PRECONDITION_RELEASECHANNELSTABLE._serialized_start=1710
   _PRECONDITION_RELEASECHANNELSTABLE._serialized_end=1802
   _PRECONDITION_MANUALAPPROVAL._serialized_start=1804
   _PRECONDITION_MANUALAPPROVAL._serialized_end=1820
   _PRECONDITION_CUSTOMTASK._serialized_start=1822
   _PRECONDITION_CUSTOMTASK._serialized_end=1906
   _RELEASECHANNELRUNTIMECONFIG._serialized_start=1943
-  _RELEASECHANNELRUNTIMECONFIG._serialized_end=2278
+  _RELEASECHANNELRUNTIMECONFIG._serialized_end=2256
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _RuntimeConnectionTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_RuntimeConnectionType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN_CONNECTION: _RuntimeConnectionType.ValueType  # 0
     LONG_LIVED_COMPUTE: _RuntimeConnectionType.ValueType  # 1
-    GENERIC: _RuntimeConnectionType.ValueType  # 2
+    EXTENSION: _RuntimeConnectionType.ValueType  # 2
 
 class RuntimeConnectionType(_RuntimeConnectionType, metaclass=_RuntimeConnectionTypeEnumTypeWrapper): ...
 
 UNKNOWN_CONNECTION: RuntimeConnectionType.ValueType  # 0
 LONG_LIVED_COMPUTE: RuntimeConnectionType.ValueType  # 1
-GENERIC: RuntimeConnectionType.ValueType  # 2
+EXTENSION: RuntimeConnectionType.ValueType  # 2
 global___RuntimeConnectionType = RuntimeConnectionType
 
 class Policy(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class DefaultEnvEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -213,32 +213,32 @@
 
 global___Precondition = Precondition
 
 class ReleaseChannelRuntimeConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RUNTIME_FIELD_NUMBER: builtins.int
-    CONNECTION_NAME_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
     CONTAINER_ORCHESTRATION_FIELD_NUMBER: builtins.int
-    CONNECTION_TYPE_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
     runtime: builtins.str
-    connection_name: builtins.str
+    name: builtins.str
     """Optional identifier for this runtime connection within this release channel,
-    useful if the same runtime is used multiple times in a single release channel.
-    Defaults to runtime.
+    useful if the release channel has multiple runtimes of the same type.
+    Defaults to the value of `runtime``.
     """
     @property
     def container_orchestration(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.ContainerOrchestrationRuntime: ...
-    connection_type: global___RuntimeConnectionType.ValueType
+    type: global___RuntimeConnectionType.ValueType
     def __init__(
         self,
         *,
         runtime: builtins.str = ...,
-        connection_name: builtins.str = ...,
+        name: builtins.str = ...,
         container_orchestration: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.ContainerOrchestrationRuntime | None = ...,
-        connection_type: global___RuntimeConnectionType.ValueType = ...,
+        type: global___RuntimeConnectionType.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["capability", b"capability", "container_orchestration", b"container_orchestration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["capability", b"capability", "connection_name", b"connection_name", "connection_type", b"connection_type", "container_orchestration", b"container_orchestration", "runtime", b"runtime"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["capability", b"capability", "container_orchestration", b"container_orchestration", "name", b"name", "runtime", b"runtime", "type", b"type"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["capability", b"capability"]) -> typing_extensions.Literal["container_orchestration"] | None: ...
 
 global___ReleaseChannelRuntimeConfig = ReleaseChannelRuntimeConfig
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/runtimes/extensions.proto
+# source: prodvana/runtimes/features.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"prodvana/runtimes/extensions.proto\x12\x11prodvana.runtimes*u\n\rExtensionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0f\x45XPOSED_SERVICE\x10\x01\x12\x0f\n\x0bTLS_SERVICE\x10\x02\x12\x11\n\rCOST_ANALYSIS\x10\x03\x12\x0b\n\x07\x44\x41TADOG\x10\x04\x12\x11\n\rARGO_ROLLOUTS\x10\x05\x42MZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/runtimesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/runtimes/features.proto\x12\x11prodvana.runtimes*s\n\x0b\x46\x65\x61tureType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x13\n\x0f\x45XPOSED_SERVICE\x10\x01\x12\x0f\n\x0bTLS_SERVICE\x10\x02\x12\x11\n\rCOST_ANALYSIS\x10\x03\x12\x0b\n\x07\x44\x41TADOG\x10\x04\x12\x11\n\rARGO_ROLLOUTS\x10\x05\x42MZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/runtimesb\x06proto3')
 
-_EXTENSIONTYPE = DESCRIPTOR.enum_types_by_name['ExtensionType']
-ExtensionType = enum_type_wrapper.EnumTypeWrapper(_EXTENSIONTYPE)
+_FEATURETYPE = DESCRIPTOR.enum_types_by_name['FeatureType']
+FeatureType = enum_type_wrapper.EnumTypeWrapper(_FEATURETYPE)
 UNKNOWN = 0
 EXPOSED_SERVICE = 1
 TLS_SERVICE = 2
 COST_ANALYSIS = 3
 DATADOG = 4
 ARGO_ROLLOUTS = 5
 
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZKgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/runtimes'
-  _EXTENSIONTYPE._serialized_start=57
-  _EXTENSIONTYPE._serialized_end=174
+  _FEATURETYPE._serialized_start=55
+  _FEATURETYPE._serialized_end=170
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class _ExtensionType:
+class _FeatureType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ExtensionTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ExtensionType.ValueType], builtins.type):  # noqa: F821
+class _FeatureTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_FeatureType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    UNKNOWN: _ExtensionType.ValueType  # 0
-    EXPOSED_SERVICE: _ExtensionType.ValueType  # 1
-    TLS_SERVICE: _ExtensionType.ValueType  # 2
-    COST_ANALYSIS: _ExtensionType.ValueType  # 3
-    DATADOG: _ExtensionType.ValueType  # 4
-    ARGO_ROLLOUTS: _ExtensionType.ValueType  # 5
+    UNKNOWN: _FeatureType.ValueType  # 0
+    EXPOSED_SERVICE: _FeatureType.ValueType  # 1
+    TLS_SERVICE: _FeatureType.ValueType  # 2
+    COST_ANALYSIS: _FeatureType.ValueType  # 3
+    DATADOG: _FeatureType.ValueType  # 4
+    ARGO_ROLLOUTS: _FeatureType.ValueType  # 5
 
-class ExtensionType(_ExtensionType, metaclass=_ExtensionTypeEnumTypeWrapper): ...
+class FeatureType(_FeatureType, metaclass=_FeatureTypeEnumTypeWrapper): ...
 
-UNKNOWN: ExtensionType.ValueType  # 0
-EXPOSED_SERVICE: ExtensionType.ValueType  # 1
-TLS_SERVICE: ExtensionType.ValueType  # 2
-COST_ANALYSIS: ExtensionType.ValueType  # 3
-DATADOG: ExtensionType.ValueType  # 4
-ARGO_ROLLOUTS: ExtensionType.ValueType  # 5
-global___ExtensionType = ExtensionType
+UNKNOWN: FeatureType.ValueType  # 0
+EXPOSED_SERVICE: FeatureType.ValueType  # 1
+TLS_SERVICE: FeatureType.ValueType  # 2
+COST_ANALYSIS: FeatureType.ValueType  # 3
+DATADOG: FeatureType.ValueType  # 4
+ARGO_ROLLOUTS: FeatureType.ValueType  # 5
+global___FeatureType = FeatureType
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xe9\x06\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x41\n\x0fgeneric_runtime\x18\r \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"X\n\x14GenericRuntimeConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xe1\x0c\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x12 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\xc5\x0c\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x16 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xed\x06\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xe5\x0c\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\xc9\x0c\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 
 
 _REPLICASCONFIG = DESCRIPTOR.message_types_by_name['ReplicasConfig']
 _METRICANALYSIS = DESCRIPTOR.message_types_by_name['MetricAnalysis']
 _METRICANALYSIS_SUCCESSRATECONFIG = _METRICANALYSIS.nested_types_by_name['SuccessRateConfig']
 _METRICANALYSIS_LATENCYCONFIG = _METRICANALYSIS.nested_types_by_name['LatencyConfig']
@@ -49,15 +49,15 @@
 _COMPILEDCAPABILITYCONFIG = DESCRIPTOR.message_types_by_name['CompiledCapabilityConfig']
 _PROGRAMREFERENCE = DESCRIPTOR.message_types_by_name['ProgramReference']
 _TASKREFERENCE = DESCRIPTOR.message_types_by_name['TaskReference']
 _TASKCONFIG = DESCRIPTOR.message_types_by_name['TaskConfig']
 _RUNTIMESPECIFICCONFIG = DESCRIPTOR.message_types_by_name['RuntimeSpecificConfig']
 _RUNTIMESPECIFICCONFIG_K8SCONFIG = _RUNTIMESPECIFICCONFIG.nested_types_by_name['K8SConfig']
 _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY = _RUNTIMESPECIFICCONFIG_K8SCONFIG.nested_types_by_name['ServiceAnnotationsEntry']
-_GENERICRUNTIMECONFIG = DESCRIPTOR.message_types_by_name['GenericRuntimeConfig']
+_RUNTIMEEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['RuntimeExtensionConfig']
 _AUTOROLLBACKCONFIG = DESCRIPTOR.message_types_by_name['AutoRollbackConfig']
 _PROTECTIONCONVERGENCEATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionConvergenceAttachment']
 _SERVICECONFIG = DESCRIPTOR.message_types_by_name['ServiceConfig']
 _COMPILEDSERVICEINSTANCECONFIG = DESCRIPTOR.message_types_by_name['CompiledServiceInstanceConfig']
 _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY = _COMPILEDSERVICEINSTANCECONFIG.nested_types_by_name['EnvEntry']
 _COMPILEDJOBCONFIG = DESCRIPTOR.message_types_by_name['CompiledJobConfig']
 _SERVICECONFIG_PARAMETERSAUTOGEN = _SERVICECONFIG.enum_types_by_name['ParametersAutogen']
@@ -180,20 +180,20 @@
   '__module__' : 'prodvana.service.service_config_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.RuntimeSpecificConfig)
   })
 _sym_db.RegisterMessage(RuntimeSpecificConfig)
 _sym_db.RegisterMessage(RuntimeSpecificConfig.K8SConfig)
 _sym_db.RegisterMessage(RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry)
 
-GenericRuntimeConfig = _reflection.GeneratedProtocolMessageType('GenericRuntimeConfig', (_message.Message,), {
-  'DESCRIPTOR' : _GENERICRUNTIMECONFIG,
+RuntimeExtensionConfig = _reflection.GeneratedProtocolMessageType('RuntimeExtensionConfig', (_message.Message,), {
+  'DESCRIPTOR' : _RUNTIMEEXTENSIONCONFIG,
   '__module__' : 'prodvana.service.service_config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.GenericRuntimeConfig)
+  # @@protoc_insertion_point(class_scope:prodvana.service.RuntimeExtensionConfig)
   })
-_sym_db.RegisterMessage(GenericRuntimeConfig)
+_sym_db.RegisterMessage(RuntimeExtensionConfig)
 
 AutoRollbackConfig = _reflection.GeneratedProtocolMessageType('AutoRollbackConfig', (_message.Message,), {
   'DESCRIPTOR' : _AUTOROLLBACKCONFIG,
   '__module__' : 'prodvana.service.service_config_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.AutoRollbackConfig)
   })
 _sym_db.RegisterMessage(AutoRollbackConfig)
@@ -303,41 +303,41 @@
   _TLSSECRET._serialized_start=1421
   _TLSSECRET._serialized_end=1523
   _TLSCERTIFICATE._serialized_start=1526
   _TLSCERTIFICATE._serialized_end=1655
   _CERTIFICATE._serialized_start=1657
   _CERTIFICATE._serialized_end=1763
   _PERRELEASECHANNELCONFIG._serialized_start=1766
-  _PERRELEASECHANNELCONFIG._serialized_end=2639
-  _CAPABILITYREFERENCE._serialized_start=2641
-  _CAPABILITYREFERENCE._serialized_end=2685
-  _COMPILEDCAPABILITYCONFIG._serialized_start=2687
-  _COMPILEDCAPABILITYCONFIG._serialized_end=2772
-  _PROGRAMREFERENCE._serialized_start=2774
-  _PROGRAMREFERENCE._serialized_end=2820
-  _TASKREFERENCE._serialized_start=2822
-  _TASKREFERENCE._serialized_end=2876
-  _TASKCONFIG._serialized_start=2879
-  _TASKCONFIG._serialized_end=3120
-  _RUNTIMESPECIFICCONFIG._serialized_start=3123
-  _RUNTIMESPECIFICCONFIG._serialized_end=3407
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3215
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3389
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3332
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3389
-  _GENERICRUNTIMECONFIG._serialized_start=3409
-  _GENERICRUNTIMECONFIG._serialized_end=3497
-  _AUTOROLLBACKCONFIG._serialized_start=3499
-  _AUTOROLLBACKCONFIG._serialized_end=3537
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=3540
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=3776
-  _SERVICECONFIG._serialized_start=3779
-  _SERVICECONFIG._serialized_end=5412
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5231
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5308
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5415
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7020
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=6877
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=6953
-  _COMPILEDJOBCONFIG._serialized_start=7023
-  _COMPILEDJOBCONFIG._serialized_end=7287
+  _PERRELEASECHANNELCONFIG._serialized_end=2643
+  _CAPABILITYREFERENCE._serialized_start=2645
+  _CAPABILITYREFERENCE._serialized_end=2689
+  _COMPILEDCAPABILITYCONFIG._serialized_start=2691
+  _COMPILEDCAPABILITYCONFIG._serialized_end=2776
+  _PROGRAMREFERENCE._serialized_start=2778
+  _PROGRAMREFERENCE._serialized_end=2824
+  _TASKREFERENCE._serialized_start=2826
+  _TASKREFERENCE._serialized_end=2880
+  _TASKCONFIG._serialized_start=2883
+  _TASKCONFIG._serialized_end=3124
+  _RUNTIMESPECIFICCONFIG._serialized_start=3127
+  _RUNTIMESPECIFICCONFIG._serialized_end=3411
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3219
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3393
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3336
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3393
+  _RUNTIMEEXTENSIONCONFIG._serialized_start=3413
+  _RUNTIMEEXTENSIONCONFIG._serialized_end=3503
+  _AUTOROLLBACKCONFIG._serialized_start=3505
+  _AUTOROLLBACKCONFIG._serialized_end=3543
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=3546
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=3782
+  _SERVICECONFIG._serialized_start=3785
+  _SERVICECONFIG._serialized_end=5422
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5241
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5318
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5425
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7034
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=6891
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=6967
+  _COMPILEDJOBCONFIG._serialized_start=7037
+  _COMPILEDJOBCONFIG._serialized_end=7301
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     CERT_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
-    GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
+    RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     release_channel: builtins.str
     @property
     def custom_hostnames(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
@@ -236,15 +236,15 @@
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     runtime_connection: builtins.str
     """which runtime connection to use in each release channel.
     optional if only one runtime makes sense for the service config.
     """
     @property
-    def generic_runtime(self) -> global___GenericRuntimeConfig: ...
+    def runtime_extension(self) -> global___RuntimeExtensionConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def external_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig:
         """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
@@ -257,22 +257,22 @@
         cert: global___Certificate | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         replicas: global___ReplicasConfig | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
-        generic_runtime: global___GenericRuntimeConfig | None = ...,
+        runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "external_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___PerReleaseChannelConfig = PerReleaseChannelConfig
 
 class CapabilityReference(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
@@ -418,28 +418,28 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["k8s", b"k8s", "runtime_config", b"runtime_config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["k8s", b"k8s", "runtime_config", b"runtime_config"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["runtime_config", b"runtime_config"]) -> typing_extensions.Literal["k8s"] | None: ...
 
 global___RuntimeSpecificConfig = RuntimeSpecificConfig
 
-class GenericRuntimeConfig(google.protobuf.message.Message):
+class RuntimeExtensionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     @property
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     def __init__(
         self,
         *,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["parameter_values", b"parameter_values"]) -> None: ...
 
-global___GenericRuntimeConfig = GenericRuntimeConfig
+global___RuntimeExtensionConfig = RuntimeExtensionConfig
 
 class AutoRollbackConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISABLED_FIELD_NUMBER: builtins.int
     disabled: builtins.bool
     def __init__(
@@ -514,15 +514,15 @@
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
-    GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
+    RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     PARAMETERS_AUTOGEN_FIELD_NUMBER: builtins.int
     AUTO_ROLLBACK_FIELD_NUMBER: builtins.int
     name: builtins.str
     application: builtins.str
@@ -557,15 +557,15 @@
     @property
     def parameter_values(self) -> prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues:
         """only valid to set in compiled configs by Prodvana"""
     @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
-    def generic_runtime(self) -> global___GenericRuntimeConfig: ...
+    def runtime_extension(self) -> global___RuntimeExtensionConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def external_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig:
         """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
@@ -589,24 +589,24 @@
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
-        generic_runtime: global___GenericRuntimeConfig | None = ...,
+        runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType = ...,
         auto_rollback: global___AutoRollbackConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "external_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___ServiceConfig = ServiceConfig
 
 class CompiledServiceInstanceConfig(google.protobuf.message.Message):
     """a compiled version of ServiceConfig specific to a service instance, with release-channel configs applied"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -645,15 +645,15 @@
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
-    GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
+    RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
     service: builtins.str
     application: builtins.str
     release_channel: builtins.str
     @property
@@ -689,15 +689,15 @@
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
-    def generic_runtime(self) -> global___GenericRuntimeConfig: ...
+    def runtime_extension(self) -> global___RuntimeExtensionConfig: ...
     @property
     def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     @property
     def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """The compiled environment for this instance's context, e.g.  Release Channel.
@@ -723,22 +723,22 @@
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
-        generic_runtime: global___GenericRuntimeConfig | None = ...,
+        runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "env", b"env", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "helm"] | None: ...
 
 global___CompiledServiceInstanceConfig = CompiledServiceInstanceConfig
 
 class CompiledJobConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_PREFIX_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.6/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.6/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/utils/desired_states.py` & `prodvana-0.1.6/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/utils/service_config.py` & `prodvana-0.1.6/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.6/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.5/pyproject.toml` & `prodvana-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.5"
+version = "0.1.6"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.1.5/PKG-INFO` & `prodvana-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

