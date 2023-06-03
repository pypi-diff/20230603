# Comparing `tmp/bclib-3.8.8.tar.gz` & `tmp/bclib-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bclib-3.8.8.tar", last modified: Sat May  7 10:38:29 2022, max compression
+gzip compressed data, was "bclib-3.9.1.tar", last modified: Tue May 17 12:28:53 2022, max compression
```

## Comparing `bclib-3.8.8.tar` & `bclib-3.9.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.878000 bclib-3.8.8/
--rw-rw-rw-   0        0        0    35562 2022-01-12 07:22:12.000000 bclib-3.8.8/LICENCE
--rw-rw-rw-   0        0        0      705 2022-05-07 10:38:29.872996 bclib-3.8.8/PKG-INFO
--rw-rw-rw-   0        0        0       89 2022-01-12 07:22:12.000000 bclib-3.8.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.332171 bclib-3.8.8/bclib/
--rw-rw-rw-   0        0        0       23 2022-05-07 10:37:58.000000 bclib-3.8.8/bclib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.383164 bclib-3.8.8/bclib/cache/
--rw-rw-rw-   0        0        0      101 2022-01-12 08:52:12.000000 bclib-3.8.8/bclib/cache/__init__.py
--rw-rw-rw-   0        0        0      663 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/cache/cache_manager.py
--rw-rw-rw-   0        0        0      638 2022-01-12 08:52:10.000000 bclib-3.8.8/bclib/cache/factory.py
--rw-rw-rw-   0        0        0     2678 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/cache/in_memory_cache_manager.py
--rw-rw-rw-   0        0        0      518 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/cache/no_cache.py
--rw-rw-rw-   0        0        0      521 2022-01-12 08:52:12.000000 bclib-3.8.8/bclib/cache/signal_base_cache_manager.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.411162 bclib-3.8.8/bclib/cache/signaler/
--rw-rw-rw-   0        0        0        0 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/cache/signaler/__init__.py
--rw-rw-rw-   0        0        0      667 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/cache/signaler/factory.py
--rw-rw-rw-   0        0        0      205 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/cache/signaler/no_signaler.py
--rw-rw-rw-   0        0        0     1765 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/cache/signaler/rabbit_signaler.py
--rw-rw-rw-   0        0        0      335 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/cache/signaler/signaler_base.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.499117 bclib-3.8.8/bclib/context/
--rw-rw-rw-   0        0        0      796 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/context/__init__.py
--rw-rw-rw-   0        0        0     1123 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/client_source_context.py
--rw-rw-rw-   0        0        0      923 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/client_source_member_context.py
--rw-rw-rw-   0        0        0     2177 2022-05-07 07:55:54.000000 bclib-3.8.8/bclib/context/context.py
--rw-rw-rw-   0        0        0     1131 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/context/json_base_request_context.py
--rw-rw-rw-   0        0        0      116 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/context/merge_type.py
--rw-rw-rw-   0        0        0      979 2022-01-12 08:52:10.000000 bclib-3.8.8/bclib/context/rabbit_context.py
--rw-rw-rw-   0        0        0     3238 2022-05-07 07:55:54.000000 bclib-3.8.8/bclib/context/request_context.py
--rw-rw-rw-   0        0        0     1187 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/restful_context.py
--rw-rw-rw-   0        0        0      913 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/server_source_context.py
--rw-rw-rw-   0        0        0      844 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/server_source_member_context.py
--rw-rw-rw-   0        0        0      836 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/context/socket_context.py
--rw-rw-rw-   0        0        0      585 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/context/source_context.py
--rw-rw-rw-   0        0        0      888 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/context/source_member_context.py
--rw-rw-rw-   0        0        0      727 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/context/web_context.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.546104 bclib-3.8.8/bclib/db_manager/
--rw-rw-rw-   0        0        0      322 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/__init__.py
--rw-rw-rw-   0        0        0      259 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/db.py
--rw-rw-rw-   0        0        0     2218 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/db_manager.py
--rw-rw-rw-   0        0        0      418 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/mongo_db.py
--rw-rw-rw-   0        0        0      515 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/odbc_db.py
--rw-rw-rw-   0        0        0     1401 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/rabbit_connection.py
--rw-rw-rw-   0        0        0     1178 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/db_manager/restful_connection.py
--rw-rw-rw-   0        0        0      117 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/sql_db.py
--rw-rw-rw-   0        0        0      416 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/db_manager/sqlite_db.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.586092 bclib-3.8.8/bclib/dispatcher/
--rw-rw-rw-   0        0        0      310 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/dispatcher/__init__.py
--rw-rw-rw-   0        0        0      862 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/dispatcher/callback_info.py
--rw-rw-rw-   0        0        0      727 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/dispatcher/dev_server_dispatcher.py
--rw-rw-rw-   0        0        0    16961 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/dispatcher/dispatcher.py
--rw-rw-rw-   0        0        0     4279 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/dispatcher/dispatcher_helper.py
--rw-rw-rw-   0        0        0     1680 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/dispatcher/idispatcher.py
--rw-rw-rw-   0        0        0     6753 2022-04-20 10:49:28.000000 bclib-3.8.8/bclib/dispatcher/routing_dispatcher.py
--rw-rw-rw-   0        0        0      890 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/dispatcher/socket_dispatcher.py
--rw-rw-rw-   0        0        0     3595 2022-04-20 10:50:53.000000 bclib-3.8.8/bclib/edge.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.616079 bclib-3.8.8/bclib/exception/
--rw-rw-rw-   0        0        0      317 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/exception/__init__.py
--rw-rw-rw-   0        0        0      223 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/exception/handler_not_found_err.py
--rw-rw-rw-   0        0        0      299 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/exception/internal_server_err.py
--rw-rw-rw-   0        0        0      281 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/exception/not_found_err.py
--rw-rw-rw-   0        0        0      253 2022-05-07 07:55:54.000000 bclib-3.8.8/bclib/exception/short_circuit_err.py
--rw-rw-rw-   0        0        0      288 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/exception/unauthorized_err.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.655068 bclib-3.8.8/bclib/listener/
--rw-rw-rw-   0        0        0      495 2022-02-05 09:03:22.000000 bclib-3.8.8/bclib/listener/__init__.py
--rw-rw-rw-   0        0        0      378 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/listener/endpoint.py
--rw-rw-rw-   0        0        0      391 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/listener/event_handler.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.678083 bclib-3.8.8/bclib/listener/http_listener/
--rw-rw-rw-   0        0        0      227 2022-01-12 08:52:10.000000 bclib-3.8.8/bclib/listener/http_listener/__init__.py
--rw-rw-rw-   0        0        0      540 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/listener/http_listener/http_base_data_name.py
--rw-rw-rw-   0        0        0      221 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/listener/http_listener/http_base_data_type.py
--rw-rw-rw-   0        0        0     9777 2022-04-20 10:49:28.000000 bclib-3.8.8/bclib/listener/http_listener/http_listener.py
--rw-rw-rw-   0        0        0     3273 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/listener/message.py
--rw-rw-rw-   0        0        0      137 2022-01-12 07:22:12.000000 bclib-3.8.8/bclib/listener/message_type.py
--rw-rw-rw-   0        0        0     1017 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/listener/rabbit_bus_listener.py
--rw-rw-rw-   0        0        0     1697 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/listener/rabbit_listener.py
--rw-rw-rw-   0        0        0     5791 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/listener/socket_listener.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.718048 bclib-3.8.8/bclib/logger/
--rw-rw-rw-   0        0        0       97 2022-02-09 08:20:47.000000 bclib-3.8.8/bclib/logger/__init__.py
--rw-rw-rw-   0        0        0      190 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/logger/ilogger.py
--rw-rw-rw-   0        0        0     1655 2022-05-07 10:14:58.000000 bclib-3.8.8/bclib/logger/log_schema.py
--rw-rw-rw-   0        0        0     1180 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/logger/logger_factory.py
--rw-rw-rw-   0        0        0      174 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/logger/no_logger.py
--rw-rw-rw-   0        0        0     1126 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/logger/rabbit_schema_base_logger.py
--rw-rw-rw-   0        0        0      953 2022-03-02 06:52:47.000000 bclib-3.8.8/bclib/logger/restful_schema_base_logger.py
--rw-rw-rw-   0        0        0     2030 2022-05-07 10:25:46.000000 bclib-3.8.8/bclib/logger/schema_base_logger.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.722046 bclib-3.8.8/bclib/parser/
--rw-rw-rw-   0        0        0      214 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.742040 bclib-3.8.8/bclib/parser/answer/
--rw-rw-rw-   0        0        0      170 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/answer/__init__.py
--rw-rw-rw-   0        0        0     5724 2022-03-30 08:35:45.000000 bclib-3.8.8/bclib/parser/answer/answer.py
--rw-rw-rw-   0        0        0     1241 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/answer/user_action.py
--rw-rw-rw-   0        0        0      126 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/answer/user_action_types.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.755036 bclib-3.8.8/bclib/parser/html/
--rw-rw-rw-   0        0        0       59 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/html/__init__.py
--rw-rw-rw-   0        0        0     1545 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/html/html_parser_ex.py
--rw-rw-rw-   0        0        0      187 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/parser/html/html_tag.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.838008 bclib-3.8.8/bclib/predicate/
--rw-rw-rw-   0        0        0      700 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/__init__.py
--rw-rw-rw-   0        0        0      670 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/all.py
--rw-rw-rw-   0        0        0      666 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/any.py
--rw-rw-rw-   0        0        0      633 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/between.py
--rw-rw-rw-   0        0        0      653 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/callback.py
--rw-rw-rw-   0        0        0      538 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/equal.py
--rw-rw-rw-   0        0        0      557 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/greater_than.py
--rw-rw-rw-   0        0        0      569 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/greater_than_equal.py
--rw-rw-rw-   0        0        0      560 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/has_value.py
--rw-rw-rw-   0        0        0      572 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/in_list.py
--rw-rw-rw-   0        0        0      551 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/less_than.py
--rw-rw-rw-   0        0        0      567 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/less_than_equal.py
--rw-rw-rw-   0        0        0      587 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/match.py
--rw-rw-rw-   0        0        0      579 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/not_equal.py
--rw-rw-rw-   0        0        0      380 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/predicate.py
--rw-rw-rw-   0        0        0     2925 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/predicate/url.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.869997 bclib-3.8.8/bclib/utility/
--rw-rw-rw-   0        0        0      268 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/utility/__init__.py
--rw-rw-rw-   0        0        0     1683 2022-05-07 08:12:16.000000 bclib-3.8.8/bclib/utility/dict_ex.py
--rw-rw-rw-   0        0        0     2881 2022-02-09 08:20:48.000000 bclib-3.8.8/bclib/utility/http_headers.py
--rw-rw-rw-   0        0        0     2644 2022-01-29 07:01:33.000000 bclib-3.8.8/bclib/utility/http_mime_types.py
--rw-rw-rw-   0        0        0     2915 2022-05-07 07:55:54.000000 bclib-3.8.8/bclib/utility/http_status_codes.py
--rw-rw-rw-   0        0        0      140 2022-05-07 07:55:54.000000 bclib-3.8.8/bclib/utility/response_types.py
-drwxrwxrwx   0        0        0        0 2022-05-07 10:38:29.352165 bclib-3.8.8/bclib.egg-info/
--rw-rw-rw-   0        0        0      705 2022-05-07 10:38:28.000000 bclib-3.8.8/bclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3409 2022-05-07 10:38:29.000000 bclib-3.8.8/bclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-07 10:38:28.000000 bclib-3.8.8/bclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-05-07 10:38:28.000000 bclib-3.8.8/bclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-07 10:38:29.879008 bclib-3.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1103 2022-01-29 07:01:33.000000 bclib-3.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:53.185836 bclib-3.9.1/
+-rw-rw-rw-   0        0        0    35562 2022-01-12 07:22:12.000000 bclib-3.9.1/LICENCE
+-rw-rw-rw-   0        0        0      705 2022-05-17 12:28:53.182836 bclib-3.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2022-01-12 07:22:12.000000 bclib-3.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:51.999165 bclib-3.9.1/bclib/
+-rw-rw-rw-   0        0        0       23 2022-05-17 12:16:10.000000 bclib-3.9.1/bclib/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.125783 bclib-3.9.1/bclib/cache/
+-rw-rw-rw-   0        0        0      101 2022-01-12 08:52:12.000000 bclib-3.9.1/bclib/cache/__init__.py
+-rw-rw-rw-   0        0        0      663 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/cache/cache_manager.py
+-rw-rw-rw-   0        0        0      638 2022-01-12 08:52:10.000000 bclib-3.9.1/bclib/cache/factory.py
+-rw-rw-rw-   0        0        0     2678 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/cache/in_memory_cache_manager.py
+-rw-rw-rw-   0        0        0      518 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/cache/no_cache.py
+-rw-rw-rw-   0        0        0      521 2022-01-12 08:52:12.000000 bclib-3.9.1/bclib/cache/signal_base_cache_manager.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.176767 bclib-3.9.1/bclib/cache/signaler/
+-rw-rw-rw-   0        0        0        0 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/cache/signaler/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/cache/signaler/factory.py
+-rw-rw-rw-   0        0        0      205 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/cache/signaler/no_signaler.py
+-rw-rw-rw-   0        0        0     1765 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/cache/signaler/rabbit_signaler.py
+-rw-rw-rw-   0        0        0      335 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/cache/signaler/signaler_base.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.408084 bclib-3.9.1/bclib/context/
+-rw-rw-rw-   0        0        0      796 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/context/__init__.py
+-rw-rw-rw-   0        0        0     1123 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/client_source_context.py
+-rw-rw-rw-   0        0        0      923 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/client_source_member_context.py
+-rw-rw-rw-   0        0        0     2177 2022-05-07 07:55:54.000000 bclib-3.9.1/bclib/context/context.py
+-rw-rw-rw-   0        0        0     1131 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/context/json_base_request_context.py
+-rw-rw-rw-   0        0        0      116 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/context/merge_type.py
+-rw-rw-rw-   0        0        0      979 2022-01-12 08:52:10.000000 bclib-3.9.1/bclib/context/rabbit_context.py
+-rw-rw-rw-   0        0        0     3238 2022-05-07 07:55:54.000000 bclib-3.9.1/bclib/context/request_context.py
+-rw-rw-rw-   0        0        0     1187 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/restful_context.py
+-rw-rw-rw-   0        0        0      913 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/server_source_context.py
+-rw-rw-rw-   0        0        0      844 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/server_source_member_context.py
+-rw-rw-rw-   0        0        0      836 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/context/socket_context.py
+-rw-rw-rw-   0        0        0      585 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/context/source_context.py
+-rw-rw-rw-   0        0        0      888 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/context/source_member_context.py
+-rw-rw-rw-   0        0        0      727 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/context/web_context.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.514051 bclib-3.9.1/bclib/db_manager/
+-rw-rw-rw-   0        0        0      322 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/__init__.py
+-rw-rw-rw-   0        0        0      259 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/db.py
+-rw-rw-rw-   0        0        0     2218 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/db_manager.py
+-rw-rw-rw-   0        0        0      418 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/mongo_db.py
+-rw-rw-rw-   0        0        0      515 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/odbc_db.py
+-rw-rw-rw-   0        0        0     1401 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/rabbit_connection.py
+-rw-rw-rw-   0        0        0     1178 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/db_manager/restful_connection.py
+-rw-rw-rw-   0        0        0      117 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/sql_db.py
+-rw-rw-rw-   0        0        0      416 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/db_manager/sqlite_db.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.631013 bclib-3.9.1/bclib/dispatcher/
+-rw-rw-rw-   0        0        0      310 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/dispatcher/__init__.py
+-rw-rw-rw-   0        0        0      862 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/dispatcher/callback_info.py
+-rw-rw-rw-   0        0        0      727 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/dispatcher/dev_server_dispatcher.py
+-rw-rw-rw-   0        0        0    16961 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/dispatcher/dispatcher.py
+-rw-rw-rw-   0        0        0     4666 2022-05-11 07:03:18.000000 bclib-3.9.1/bclib/dispatcher/dispatcher_helper.py
+-rw-rw-rw-   0        0        0     1680 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/dispatcher/idispatcher.py
+-rw-rw-rw-   0        0        0     6753 2022-04-20 10:49:28.000000 bclib-3.9.1/bclib/dispatcher/routing_dispatcher.py
+-rw-rw-rw-   0        0        0      890 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/dispatcher/socket_dispatcher.py
+-rw-rw-rw-   0        0        0     3595 2022-04-20 10:50:53.000000 bclib-3.9.1/bclib/edge.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.693992 bclib-3.9.1/bclib/exception/
+-rw-rw-rw-   0        0        0      317 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/exception/__init__.py
+-rw-rw-rw-   0        0        0      223 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/exception/handler_not_found_err.py
+-rw-rw-rw-   0        0        0      299 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/exception/internal_server_err.py
+-rw-rw-rw-   0        0        0      281 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/exception/not_found_err.py
+-rw-rw-rw-   0        0        0      253 2022-05-07 07:55:54.000000 bclib-3.9.1/bclib/exception/short_circuit_err.py
+-rw-rw-rw-   0        0        0      288 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/exception/unauthorized_err.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.756972 bclib-3.9.1/bclib/listener/
+-rw-rw-rw-   0        0        0      495 2022-02-05 09:03:22.000000 bclib-3.9.1/bclib/listener/__init__.py
+-rw-rw-rw-   0        0        0      378 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/listener/endpoint.py
+-rw-rw-rw-   0        0        0      391 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/listener/event_handler.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.821954 bclib-3.9.1/bclib/listener/http_listener/
+-rw-rw-rw-   0        0        0      227 2022-01-12 08:52:10.000000 bclib-3.9.1/bclib/listener/http_listener/__init__.py
+-rw-rw-rw-   0        0        0      540 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/listener/http_listener/http_base_data_name.py
+-rw-rw-rw-   0        0        0      221 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/listener/http_listener/http_base_data_type.py
+-rw-rw-rw-   0        0        0     9777 2022-04-20 10:49:28.000000 bclib-3.9.1/bclib/listener/http_listener/http_listener.py
+-rw-rw-rw-   0        0        0     3273 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/listener/message.py
+-rw-rw-rw-   0        0        0      137 2022-01-12 07:22:12.000000 bclib-3.9.1/bclib/listener/message_type.py
+-rw-rw-rw-   0        0        0     1017 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/listener/rabbit_bus_listener.py
+-rw-rw-rw-   0        0        0     1697 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/listener/rabbit_listener.py
+-rw-rw-rw-   0        0        0     5791 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/listener/socket_listener.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.887931 bclib-3.9.1/bclib/logger/
+-rw-rw-rw-   0        0        0       97 2022-02-09 08:20:47.000000 bclib-3.9.1/bclib/logger/__init__.py
+-rw-rw-rw-   0        0        0      190 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/logger/ilogger.py
+-rw-rw-rw-   0        0        0     1655 2022-05-07 10:14:58.000000 bclib-3.9.1/bclib/logger/log_schema.py
+-rw-rw-rw-   0        0        0     1180 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/logger/logger_factory.py
+-rw-rw-rw-   0        0        0      174 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/logger/no_logger.py
+-rw-rw-rw-   0        0        0     1126 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/logger/rabbit_schema_base_logger.py
+-rw-rw-rw-   0        0        0      953 2022-03-02 06:52:47.000000 bclib-3.9.1/bclib/logger/restful_schema_base_logger.py
+-rw-rw-rw-   0        0        0     2030 2022-05-07 10:25:46.000000 bclib-3.9.1/bclib/logger/schema_base_logger.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.893928 bclib-3.9.1/bclib/parser/
+-rw-rw-rw-   0        0        0      214 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.933915 bclib-3.9.1/bclib/parser/answer/
+-rw-rw-rw-   0        0        0      170 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/answer/__init__.py
+-rw-rw-rw-   0        0        0     5724 2022-03-30 08:35:45.000000 bclib-3.9.1/bclib/parser/answer/answer.py
+-rw-rw-rw-   0        0        0     1241 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/answer/user_action.py
+-rw-rw-rw-   0        0        0      126 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/answer/user_action_types.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.964909 bclib-3.9.1/bclib/parser/html/
+-rw-rw-rw-   0        0        0       59 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/html/__init__.py
+-rw-rw-rw-   0        0        0     1545 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/html/html_parser_ex.py
+-rw-rw-rw-   0        0        0      187 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/parser/html/html_tag.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:53.115857 bclib-3.9.1/bclib/predicate/
+-rw-rw-rw-   0        0        0      700 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/__init__.py
+-rw-rw-rw-   0        0        0      670 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/all.py
+-rw-rw-rw-   0        0        0      666 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/any.py
+-rw-rw-rw-   0        0        0      633 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/between.py
+-rw-rw-rw-   0        0        0      653 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/callback.py
+-rw-rw-rw-   0        0        0      538 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/equal.py
+-rw-rw-rw-   0        0        0      557 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/greater_than.py
+-rw-rw-rw-   0        0        0      569 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/greater_than_equal.py
+-rw-rw-rw-   0        0        0      560 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/has_value.py
+-rw-rw-rw-   0        0        0      572 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/in_list.py
+-rw-rw-rw-   0        0        0      551 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/less_than.py
+-rw-rw-rw-   0        0        0      567 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/less_than_equal.py
+-rw-rw-rw-   0        0        0      587 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/match.py
+-rw-rw-rw-   0        0        0      579 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/not_equal.py
+-rw-rw-rw-   0        0        0      380 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/predicate/predicate.py
+-rw-rw-rw-   0        0        0     2893 2022-05-17 12:15:12.000000 bclib-3.9.1/bclib/predicate/url.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:53.178837 bclib-3.9.1/bclib/utility/
+-rw-rw-rw-   0        0        0      268 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/utility/__init__.py
+-rw-rw-rw-   0        0        0     1683 2022-05-07 08:12:16.000000 bclib-3.9.1/bclib/utility/dict_ex.py
+-rw-rw-rw-   0        0        0     2881 2022-02-09 08:20:48.000000 bclib-3.9.1/bclib/utility/http_headers.py
+-rw-rw-rw-   0        0        0     2644 2022-01-29 07:01:33.000000 bclib-3.9.1/bclib/utility/http_mime_types.py
+-rw-rw-rw-   0        0        0     2915 2022-05-07 07:55:54.000000 bclib-3.9.1/bclib/utility/http_status_codes.py
+-rw-rw-rw-   0        0        0      140 2022-05-07 07:55:54.000000 bclib-3.9.1/bclib/utility/response_types.py
+drwxrwxrwx   0        0        0        0 2022-05-17 12:28:52.031153 bclib-3.9.1/bclib.egg-info/
+-rw-rw-rw-   0        0        0      705 2022-05-17 12:28:50.000000 bclib-3.9.1/bclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3409 2022-05-17 12:28:50.000000 bclib-3.9.1/bclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-17 12:28:50.000000 bclib-3.9.1/bclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2022-05-17 12:28:50.000000 bclib-3.9.1/bclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-17 12:28:53.186843 bclib-3.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2022-01-29 07:01:33.000000 bclib-3.9.1/setup.py
```

### Comparing `bclib-3.8.8/LICENCE` & `bclib-3.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/PKG-INFO` & `bclib-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bclib
-Version: 3.8.8
+Version: 3.9.1
 Summary: Python base gateway for communicate with basiscore webserver
 Home-page: https://github.com/Manzoomeh/BasisCore.Server.Edge/wiki
 Author: Manzoomeh Negaran
 Author-email: info@manzoomeh.ir
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Manzoomeh/BasisCore.Server.Edge/issues
 Platform: UNKNOWN
```

### Comparing `bclib-3.8.8/bclib/cache/cache_manager.py` & `bclib-3.9.1/bclib/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/factory.py` & `bclib-3.9.1/bclib/cache/factory.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/in_memory_cache_manager.py` & `bclib-3.9.1/bclib/cache/in_memory_cache_manager.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/no_cache.py` & `bclib-3.9.1/bclib/cache/no_cache.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/signal_base_cache_manager.py` & `bclib-3.9.1/bclib/cache/signal_base_cache_manager.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/signaler/factory.py` & `bclib-3.9.1/bclib/cache/signaler/factory.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/cache/signaler/rabbit_signaler.py` & `bclib-3.9.1/bclib/cache/signaler/rabbit_signaler.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/__init__.py` & `bclib-3.9.1/bclib/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/client_source_context.py` & `bclib-3.9.1/bclib/context/client_source_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/client_source_member_context.py` & `bclib-3.9.1/bclib/context/client_source_member_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/context.py` & `bclib-3.9.1/bclib/context/context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/json_base_request_context.py` & `bclib-3.9.1/bclib/context/json_base_request_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/rabbit_context.py` & `bclib-3.9.1/bclib/context/rabbit_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/request_context.py` & `bclib-3.9.1/bclib/context/request_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/restful_context.py` & `bclib-3.9.1/bclib/context/restful_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/server_source_context.py` & `bclib-3.9.1/bclib/context/server_source_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/server_source_member_context.py` & `bclib-3.9.1/bclib/context/server_source_member_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/socket_context.py` & `bclib-3.9.1/bclib/context/socket_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/source_context.py` & `bclib-3.9.1/bclib/context/source_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/source_member_context.py` & `bclib-3.9.1/bclib/context/source_member_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/context/web_context.py` & `bclib-3.9.1/bclib/context/web_context.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/db_manager/db_manager.py` & `bclib-3.9.1/bclib/db_manager/db_manager.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/db_manager/odbc_db.py` & `bclib-3.9.1/bclib/db_manager/odbc_db.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/db_manager/rabbit_connection.py` & `bclib-3.9.1/bclib/db_manager/rabbit_connection.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/db_manager/restful_connection.py` & `bclib-3.9.1/bclib/db_manager/restful_connection.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/callback_info.py` & `bclib-3.9.1/bclib/dispatcher/callback_info.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/dev_server_dispatcher.py` & `bclib-3.9.1/bclib/dispatcher/dev_server_dispatcher.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/dispatcher.py` & `bclib-3.9.1/bclib/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/dispatcher_helper.py` & `bclib-3.9.1/bclib/dispatcher/dispatcher_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,64 +78,76 @@
     def callback(callback: 'Callable[[Context],Coroutine[bool]]') -> Predicate:
         """Create Callback cheking predicate"""
 
         return Callback(callback)
 
     @staticmethod
     def is_post() -> Predicate:
-        """create http post request cheking predicate"""
+        """create http POST request cheking predicate"""
 
         return Equal("context.cms.request.methode", "post")
 
     @staticmethod
     def is_get() -> Predicate:
-        """create http get request cheking predicate"""
+        """create http GET request cheking predicate"""
 
         return Equal("context.cms.request.methode", "get")
 
     @staticmethod
     def is_put() -> Predicate:
-        """create http put request cheking predicate"""
+        """create http PUT request cheking predicate"""
 
         return Equal("context.cms.request.methode", "put")
 
     @staticmethod
     def is_delete() -> Predicate:
-        """create http delete request cheking predicate"""
+        """create http DELETE request cheking predicate"""
 
         return Equal("context.cms.request.methode", "delete")
 
     @staticmethod
+    def is_options() -> Predicate:
+        """create http OPTIONS request cheking predicate"""
+
+        return Equal("context.cms.request.methode", "options")
+
+    @staticmethod
     def all(*predicates: 'Predicate') -> Predicate:
         """create all cheking predicate"""
 
         return All(predicates)
 
     @staticmethod
     def any(*predicates: 'Predicate') -> Predicate:
         """create any cheking predicate"""
 
         return predicate.Any(predicates)
 
     @staticmethod
     def post(url: str) -> Predicate:
-        """create http post request cheking predicate"""
+        """create http POST request cheking predicate"""
 
         return All(DispatcherHelper.url(url), DispatcherHelper.is_post())
 
     @staticmethod
     def get(url: str) -> Predicate:
-        """create http get request cheking predicate"""
+        """create http GET request cheking predicate"""
 
         return All(DispatcherHelper.url(url), DispatcherHelper.is_get())
 
     @staticmethod
     def put(url: str) -> Predicate:
-        """create http put request cheking predicate"""
+        """create http PUT request cheking predicate"""
 
         return All(DispatcherHelper.url(url), DispatcherHelper.is_put())
 
     @staticmethod
     def delete(url: str) -> Predicate:
-        """create http delete request cheking predicate"""
+        """create http DELETE request cheking predicate"""
 
         return All(DispatcherHelper.url(url), DispatcherHelper.is_delete())
+
+    @staticmethod
+    def options(url: str) -> Predicate:
+        """create http OPTIONS request cheking predicate"""
+
+        return All(DispatcherHelper.url(url), DispatcherHelper.is_options())
```

### Comparing `bclib-3.8.8/bclib/dispatcher/idispatcher.py` & `bclib-3.9.1/bclib/dispatcher/idispatcher.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/routing_dispatcher.py` & `bclib-3.9.1/bclib/dispatcher/routing_dispatcher.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/dispatcher/socket_dispatcher.py` & `bclib-3.9.1/bclib/dispatcher/socket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/edge.py` & `bclib-3.9.1/bclib/edge.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/http_listener/http_base_data_name.py` & `bclib-3.9.1/bclib/listener/http_listener/http_base_data_name.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/http_listener/http_listener.py` & `bclib-3.9.1/bclib/listener/http_listener/http_listener.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/message.py` & `bclib-3.9.1/bclib/listener/message.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/rabbit_bus_listener.py` & `bclib-3.9.1/bclib/listener/rabbit_bus_listener.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/rabbit_listener.py` & `bclib-3.9.1/bclib/listener/rabbit_listener.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/listener/socket_listener.py` & `bclib-3.9.1/bclib/listener/socket_listener.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/logger/log_schema.py` & `bclib-3.9.1/bclib/logger/log_schema.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/logger/logger_factory.py` & `bclib-3.9.1/bclib/logger/logger_factory.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/logger/rabbit_schema_base_logger.py` & `bclib-3.9.1/bclib/logger/rabbit_schema_base_logger.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/logger/restful_schema_base_logger.py` & `bclib-3.9.1/bclib/logger/restful_schema_base_logger.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/logger/schema_base_logger.py` & `bclib-3.9.1/bclib/logger/schema_base_logger.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/parser/answer/answer.py` & `bclib-3.9.1/bclib/parser/answer/answer.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/parser/answer/user_action.py` & `bclib-3.9.1/bclib/parser/answer/user_action.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/parser/html/html_parser_ex.py` & `bclib-3.9.1/bclib/parser/html/html_parser_ex.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/__init__.py` & `bclib-3.9.1/bclib/predicate/__init__.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/all.py` & `bclib-3.9.1/bclib/predicate/all.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/any.py` & `bclib-3.9.1/bclib/predicate/any.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/between.py` & `bclib-3.9.1/bclib/predicate/between.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/callback.py` & `bclib-3.9.1/bclib/predicate/callback.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/equal.py` & `bclib-3.9.1/bclib/predicate/equal.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/greater_than.py` & `bclib-3.9.1/bclib/predicate/greater_than.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/greater_than_equal.py` & `bclib-3.9.1/bclib/predicate/greater_than_equal.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/has_value.py` & `bclib-3.9.1/bclib/predicate/has_value.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/in_list.py` & `bclib-3.9.1/bclib/predicate/in_list.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/less_than.py` & `bclib-3.9.1/bclib/predicate/less_than.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/less_than_equal.py` & `bclib-3.9.1/bclib/predicate/less_than_equal.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/match.py` & `bclib-3.9.1/bclib/predicate/match.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/not_equal.py` & `bclib-3.9.1/bclib/predicate/not_equal.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/predicate/url.py` & `bclib-3.9.1/bclib/predicate/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,22 +41,22 @@
                     return_dict_property_names.append(
                         f'"{name}" : __{name}')
                     name = f"__{name}"
             else:
                 where_part_list.append(
                     f"url_parts[{index}].lower() == '{value.lower()}'")
             segment_list.append(name)
-            if len(where_part_list) == 0:
-                if len(return_dict_property_names) == 0:
-                    where_part_list.append("True")
-                else:
-                    where_part_list.append(
-                        f"len(url_parts) == {len(return_dict_property_names)}")
-                    if len(return_dict_property_names) == 1:
-                        where_part_list.append("len(url_parts[0]) > 0")
+        if len(where_part_list) == 0:
+            if len(return_dict_property_names) == 0:
+                where_part_list.append("True")
+            else:
+                where_part_list.append(
+                    f"len(url_parts) == {len(return_dict_property_names)}")
+                if len(return_dict_property_names) == 1:
+                    where_part_list.append("len(url_parts[0]) > 0")
 
         if len(return_dict_property_names) > 0:
             body = f"""
 def url_function(url):
     try:
         url_parts = url.split("/")
         if {" and ".join(where_part_list)}:
```

### Comparing `bclib-3.8.8/bclib/utility/dict_ex.py` & `bclib-3.9.1/bclib/utility/dict_ex.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/utility/http_headers.py` & `bclib-3.9.1/bclib/utility/http_headers.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/utility/http_mime_types.py` & `bclib-3.9.1/bclib/utility/http_mime_types.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib/utility/http_status_codes.py` & `bclib-3.9.1/bclib/utility/http_status_codes.py`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/bclib.egg-info/PKG-INFO` & `bclib-3.9.1/bclib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bclib
-Version: 3.8.8
+Version: 3.9.1
 Summary: Python base gateway for communicate with basiscore webserver
 Home-page: https://github.com/Manzoomeh/BasisCore.Server.Edge/wiki
 Author: Manzoomeh Negaran
 Author-email: info@manzoomeh.ir
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Manzoomeh/BasisCore.Server.Edge/issues
 Platform: UNKNOWN
```

### Comparing `bclib-3.8.8/bclib.egg-info/SOURCES.txt` & `bclib-3.9.1/bclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bclib-3.8.8/setup.py` & `bclib-3.9.1/setup.py`

 * *Files identical despite different names*

