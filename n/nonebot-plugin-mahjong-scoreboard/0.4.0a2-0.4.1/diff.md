# Comparing `tmp/nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar.gz` & `tmp/nonebot_plugin_mahjong_scoreboard-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar", max compression
+gzip compressed data, was "nonebot_plugin_mahjong_scoreboard-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2.tar` & `nonebot_plugin_mahjong_scoreboard-0.4.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.0a2/LICENSE
--rw-r--r--   0        0        0     1054 2023-06-01 04:55:22.897241 nonebot_plugin_mahjong_scoreboard-0.4.0a2/pyproject.toml
--rw-r--r--   0        0        0     6759 2023-05-07 03:20:47.530795 nonebot_plugin_mahjong_scoreboard-0.4.0a2/README.MD
--rw-r--r--   0        0        0     2335 2023-05-31 16:17:02.523326 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-31 16:17:02.544324 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/config.py
--rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
--rw-r--r--   0        0        0     2610 2023-06-01 14:08:16.854206 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
--rw-r--r--   0        0        0     5582 2023-06-01 14:47:11.381807 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
--rw-r--r--   0        0        0    11016 2023-06-01 15:07:16.677379 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
--rw-r--r--   0        0        0     4870 2023-06-01 14:08:16.864205 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
--rw-r--r--   0        0        0     1404 2023-05-31 07:27:37.121738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
--rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
--rw-r--r--   0        0        0     2443 2023-05-31 13:06:45.874125 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
--rw-r--r--   0        0        0     3756 2023-06-01 14:46:47.079404 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
--rw-r--r--   0        0        0      935 2023-06-01 14:43:05.933065 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py
--rw-r--r--   0        0        0     1947 2023-05-31 07:27:37.123736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
--rw-r--r--   0        0        0     2873 2023-05-31 13:38:31.556446 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
--rw-r--r--   0        0        0      928 2023-05-31 07:27:37.124738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
--rw-r--r--   0        0        0    12214 2023-06-01 06:38:55.812825 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
--rw-r--r--   0        0        0     1787 2023-05-31 13:38:31.575444 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
--rw-r--r--   0        0        0     1834 2023-06-01 14:21:07.726683 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
--rw-r--r--   0        0        0     4476 2023-06-01 06:29:06.042508 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
--rw-r--r--   0        0        0     2879 2023-06-01 15:12:26.336136 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
--rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
--rw-r--r--   0        0        0     7607 2023-06-01 06:39:56.154899 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
--rw-r--r--   0        0        0     4318 2023-06-01 06:19:38.626043 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
--rw-r--r--   0        0        0      628 2023-06-01 06:19:38.613979 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
--rw-r--r--   0        0        0     2778 2023-06-01 15:03:14.755037 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
--rw-r--r--   0        0        0      189 2022-10-12 05:26:13.228228 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/errors.py
--rw-r--r--   0        0        0     2185 2023-05-31 13:38:31.528445 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
--rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
--rw-r--r--   0        0        0        0 2023-05-31 07:27:37.128738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-01 03:48:42.054855 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
--rw-r--r--   0        0        0     1287 2023-05-31 13:06:45.863127 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
--rw-r--r--   0        0        0      755 2023-05-31 12:07:55.000532 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
--rw-r--r--   0        0        0      772 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-31 13:51:24.924727 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
--rw-r--r--   0        0        0      928 2023-06-01 03:54:03.408815 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
--rw-r--r--   0        0        0      122 2023-05-31 07:27:37.130736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-31 07:27:37.131737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
--rw-r--r--   0        0        0      258 2023-05-31 16:16:01.029716 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
--rw-r--r--   0        0        0     2022 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
--rw-r--r--   0        0        0      163 2023-05-31 07:27:37.132737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
--rw-r--r--   0        0        0      263 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
--rw-r--r--   0        0        0     2523 2023-05-31 07:27:37.133737 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
--rw-r--r--   0        0        0      399 2023-05-31 07:27:37.134736 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
--rw-r--r--   0        0        0     7261 2023-05-31 12:28:17.427163 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
--rw-r--r--   0        0        0     4450 2023-06-01 14:09:26.708031 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
--rw-r--r--   0        0        0      797 2023-05-31 12:27:53.584832 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
--rw-r--r--   0        0        0      174 2023-06-01 14:10:09.416142 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/pagination.py
--rw-r--r--   0        0        0     8821 2023-06-01 14:21:07.713682 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
--rw-r--r--   0        0        0        0 2023-05-31 07:27:37.135740 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
--rw-r--r--   0        0        0      510 2023-05-31 07:27:37.136738 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
--rw-r--r--   0        0        0      736 2023-05-31 12:27:53.606829 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
--rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
--rw-r--r--   0        0        0    18332 2023-06-01 15:12:26.327144 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
--rw-r--r--   0        0        0     1027 2023-05-31 12:27:53.572832 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
--rw-r--r--   0        0        0     4122 2023-05-31 13:43:41.683542 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
--rw-r--r--   0        0        0     4128 2023-05-31 12:27:53.612405 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
--rw-r--r--   0        0        0     2851 2023-06-01 14:21:07.722683 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
--rw-r--r--   0        0        0      356 2023-05-31 11:33:58.053326 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
--rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
--rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
--rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
--rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
--rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
--rw-r--r--   0        0        0      758 2023-05-31 13:06:45.885125 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
--rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
--rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-10-29 01:06:44.421764 nonebot_plugin_mahjong_scoreboard-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1049 2023-06-03 01:15:57.707633 nonebot_plugin_mahjong_scoreboard-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6690 2023-06-02 03:44:53.162732 nonebot_plugin_mahjong_scoreboard-0.4.1/README.MD
+-rw-r--r--   0        0        0     2912 2023-06-03 01:17:07.997602 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-02 00:08:25.892232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/config.py
+-rw-r--r--   0        0        0      287 2023-03-13 11:15:04.246316 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-03 01:11:07.278231 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py
+-rw-r--r--   0        0        0     6192 2023-06-03 01:12:04.997398 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py
+-rw-r--r--   0        0        0    11880 2023-06-03 01:10:38.251192 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py
+-rw-r--r--   0        0        0     5262 2023-06-03 01:12:05.029399 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py
+-rw-r--r--   0        0        0     1551 2023-06-03 01:13:59.870976 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-07 03:44:28.905567 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py
+-rw-r--r--   0        0        0     2640 2023-06-03 00:45:52.599182 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py
+-rw-r--r--   0        0        0     3937 2023-06-03 00:45:52.625179 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py
+-rw-r--r--   0        0        0      935 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py
+-rw-r--r--   0        0        0     1947 2023-06-02 00:08:25.897230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py
+-rw-r--r--   0        0        0     2873 2023-06-02 00:08:25.898229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py
+-rw-r--r--   0        0        0      928 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py
+-rw-r--r--   0        0        0      229 2023-06-02 00:08:25.899230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mg.py
+-rw-r--r--   0        0        0    13031 2023-06-03 01:12:05.024401 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py
+-rw-r--r--   0        0        0     2030 2023-06-03 01:12:04.988398 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py
+-rw-r--r--   0        0        0     1985 2023-06-03 01:12:05.015398 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py
+-rw-r--r--   0        0        0     4763 2023-06-03 01:12:05.003402 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py
+-rw-r--r--   0        0        0     3150 2023-06-03 01:12:05.010398 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py
+-rw-r--r--   0        0        0        0 2023-03-13 11:15:04.257743 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/__init__.py
+-rw-r--r--   0        0        0     7606 2023-06-03 01:10:38.238192 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py
+-rw-r--r--   0        0        0     4318 2023-06-02 00:08:25.903232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py
+-rw-r--r--   0        0        0      481 2023-06-02 03:44:53.191732 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/message.py
+-rw-r--r--   0        0        0     2778 2023-06-02 00:08:25.904230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py
+-rw-r--r--   0        0        0      378 2023-06-03 01:10:38.228192 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/errors.py
+-rw-r--r--   0        0        0     2185 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py
+-rw-r--r--   0        0        0      492 2022-10-25 11:55:32.743202 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/model/enums.py
+-rw-r--r--   0        0        0        0 2023-06-02 00:08:25.905230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py
+-rw-r--r--   0        0        0     1287 2023-06-02 00:08:25.906230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py
+-rw-r--r--   0        0        0      755 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py
+-rw-r--r--   0        0        0      772 2023-06-02 00:08:25.907233 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py
+-rw-r--r--   0        0        0      928 2023-06-02 00:08:25.908230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py
+-rw-r--r--   0        0        0      122 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-02 00:08:25.909232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/data_source.py
+-rw-r--r--   0        0        0     2022 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py
+-rw-r--r--   0        0        0      163 2023-06-02 00:08:25.910232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v1_to_v2.py
+-rw-r--r--   0        0        0     2523 2023-06-02 00:08:25.911229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py
+-rw-r--r--   0        0        0      399 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/base.py
+-rw-r--r--   0        0        0     7261 2023-06-02 00:08:25.912229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py
+-rw-r--r--   0        0        0     4444 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/game.py
+-rw-r--r--   0        0        0      797 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/group.py
+-rw-r--r--   0        0        0      174 2023-06-02 00:08:25.913229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/pagination.py
+-rw-r--r--   0        0        0     8813 2023-06-03 01:10:38.219196 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py
+-rw-r--r--   0        0        0        0 2023-06-02 00:08:25.914233 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/types/__init__.py
+-rw-r--r--   0        0        0      510 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/types/pydantic.py
+-rw-r--r--   0        0        0      736 2023-06-02 00:08:25.915229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/user.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:02:12.038461 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/__init__.py
+-rw-r--r--   0        0        0    18263 2023-06-03 01:10:38.189194 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py
+-rw-r--r--   0        0        0     1027 2023-06-02 00:08:25.916229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py
+-rw-r--r--   0        0        0     4122 2023-06-02 00:08:25.917229 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py
+-rw-r--r--   0        0        0     4108 2023-06-03 01:10:38.193191 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py
+-rw-r--r--   0        0        0     2797 2023-06-03 01:10:38.206194 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py
+-rw-r--r--   0        0        0      356 2023-06-02 00:08:25.918232 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/user_service.py
+-rw-r--r--   0        0        0        0 2022-10-25 10:53:45.022120 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/__init__.py
+-rw-r--r--   0        0        0      288 2022-10-25 10:55:21.893872 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/date.py
+-rw-r--r--   0        0        0     1240 2022-10-25 10:57:00.084086 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py
+-rw-r--r--   0        0        0      101 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/nonebot.py
+-rw-r--r--   0        0        0      482 2023-03-13 11:15:04.267743 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/rank.py
+-rw-r--r--   0        0        0      758 2023-06-02 00:08:25.919230 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/session.py
+-rw-r--r--   0        0        0      761 2023-03-13 11:15:04.268743 nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py
+-rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 nonebot_plugin_mahjong_scoreboard-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/LICENSE` & `nonebot_plugin_mahjong_scoreboard-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/pyproject.toml` & `nonebot_plugin_mahjong_scoreboard-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "nonebot-plugin-mahjong-scoreboard"
-version = "0.4.0a2"
+version = "0.4.1"
 description = "日麻寄分器（NoneBot插件）"
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.MD"
 license = "MIT"
 repository = "https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard"
 packages = [
     { include = "nonebot_plugin_mahjong_scoreboard", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot2 = "^2.0.0rc4"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot_plugin_apscheduler = "^0.2.0"
+nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.5"
+nonebot-plugin-localstore = "^0.4.1"
 nonebot-plugin-sqlalchemy = "^0.2.1"
 nonebot-plugin-session = "^0.0.3"
-nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.5"
 aiosqlite = ">=0.17,<0.19"
 tzlocal = "^4.2"
 cachetools = "^5.2.0"
-nonebot-plugin-localstore = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0rc3" }
 nonebot-adapter-qqguild = "^0.2.2"
 nonebug = "^0.2.1"
 flake8 = "^5.0.4"
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/README.MD` & `nonebot_plugin_mahjong_scoreboard-0.4.1/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-mahjong-scoreboard">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-mahjong-scoreboard.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 </p>
 
-支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)
-
-支持驱动器：[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-driver)
+支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)、[QQ Guild](https://github.com/nonebot/adapter-qqguild)
 
 ## 功能
 
 为群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。
 
 PT精算算法为（点数-返点+马点）/1000，返点和马点在创建赛季时进行设置。
 
@@ -112,15 +110,15 @@
     - 别名：`/对局PT`
 - `/删除对局 [对局<编号>]`
 - `/设置对局进度 <东/南x局y本场 或 完成> [对局<编号>]`
     - 别名：`/对局进度`
 - `/设置对局备注 [对局<编号>] <对局备注>`
     - 别名：`/对局备注`
 
-与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。也可以通过回复Bot发出的对局消息来代替指定对局编号。
+与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。
 
 对局相关指令在对局完成超过24小时后需要拥有群主或管理员身份才能使用。（`/删除对局`除外，该指令需要拥有群主或管理员身份才能使用）
 
 未完成且未设置进度的对局会在创建24小时后自动删除。赛季结束后，未完成对局会自动删除，所有已完成对局均无法再进行修改。
 
 ### 对局查询
 
@@ -163,15 +161,15 @@
 ### 数据统计
 
 - `/对战数据`
 - `/赛季对战数据 [<赛季代号>]`
 - `/最近走势 [@<用户>]`
     - 别名：`/走势`
 
-与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用。当未指定参数时进入问答模式，回复`/q`可退出问答模式。
+与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用（QQ频道暂不支持私聊）。当未指定参数时进入问答模式，回复`/q`可退出问答模式。
 
 与赛季/赛季PT相关的指令（查询、导出除外）需要拥有群主或管理员身份才能使用。
 
 ## 配置
 
 ### mahjong_scoreboard_database_conn_url
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
                                    [nonebot]
           nonebot-plugin-mahjong-scoreboard ============ _â¨ NoneBot
                           æ¥éº»è®°åå¨æä»¶ â¨_
                            [license] [pypi] [python]
-æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
-) æ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
-driver) ## åè½
+æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/)ã[QQ
+Guild](https://github.com/nonebot/adapter-qqguild) ## åè½
 ä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
 PTç²¾ç®ç®æ³ä¸ºï¼ç¹æ°-è¿ç¹+é©¬ç¹ï¼/
 1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã ## å¸¸ç¨Workflow ###
 å¼å¯èµå­£ ``` /æ°å»ºèµå­£ ``` ### è®°å½ååºå¯¹å± ``` ä»»ä½äººï¼/
 æ°å»ºå¯¹å± A: /ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç®
 25000 ``` ### è®°å½ä¸åºå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± åäººä¸ A: /
 ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç® 25000 ``` ###
@@ -26,15 +25,15 @@
 [åäººå|åäººä¸]` - å«åï¼`/æ°å¯¹å±` - `/ç»ç®å¯¹å± <æç»©>
 [å¯¹å±<ç¼å·>] [@<ç¨æ·>] [<èªé£>]` - å«åï¼`/ç»ç®` - `/
 æ¤éç»ç®å¯¹å± [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/æ¤éç»ç®` -
 `/è®¾ç½®å¯¹å±PT  [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/å¯¹å±PT` - `/
 å é¤å¯¹å± [å¯¹å±<ç¼å·>]` - `/è®¾ç½®å¯¹å±è¿åº¦ <ä¸/åxå±yæ¬åº æ
 å®æ> [å¯¹å±<ç¼å·>]` - å«åï¼`/å¯¹å±è¿åº¦` - `/è®¾ç½®å¯¹å±å¤æ³¨
 [å¯¹å±<ç¼å·>] <å¯¹å±å¤æ³¨>` - å«åï¼`/å¯¹å±å¤æ³¨`
-ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ãä¹å¯ä»¥éè¿åå¤Botååºçå¯¹å±æ¶æ¯æ¥ä»£æ¿æå®å¯¹å±ç¼å·ã
+ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ã
 å¯¹å±ç¸å³æä»¤å¨å¯¹å±å®æè¶è¿24å°æ¶åéè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ãï¼`/
 å é¤å¯¹å±`é¤å¤ï¼è¯¥æä»¤éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ï¼
 æªå®æä¸æªè®¾ç½®è¿åº¦çå¯¹å±ä¼å¨åå»º24å°æ¶åèªå¨å é¤ãèµå­£ç»æåï¼æªå®æå¯¹å±ä¼èªå¨å é¤ï¼ææå·²å®æå¯¹å±åæ æ³åè¿è¡ä¿®æ¹ã
 ### å¯¹å±æ¥è¯¢ - `/æ¥è¯¢å¯¹å± [<ç¼å·>]` - å«åï¼`/å¯¹å±` - `/
 ä¸ªäººæè¿å¯¹å± [@<ç¨æ·>]` - å«åï¼`/æè¿å¯¹å±` - `/ç¾¤æè¿å¯¹å±`
 - `/ä¸ªäººæªå®æå¯¹å± [@<ç¨æ·>]` - å«åï¼`/æªå®æå¯¹å±` - `/
 ç¾¤æªå®æå¯¹å±` - `/å¯¼åºèµå­£å¯¹å± [<ä»£å·>]` - å«åï¼`/
@@ -45,15 +44,15 @@
 `/æ¥è¯¢æ¦å` - å«åï¼`/æ¦å` - `/å¯¼åºæ¦å` - `/æ¥è¯¢PT
 [@<ç¨æ·>]` - å«åï¼`/PT` - `/è®¾ç½®ç¨æ·PT  @<ç¨æ·>` - å«åï¼`/
 è®¾ç½®ç¨æ·pt`, `/è®¾ç½®PT`, `/è®¾ç½®pt` - `/éç½®ç¨æ·PT @<ç¨æ·>` -
 å«åï¼`/éç½®ç¨æ·pt`, `/éç½®PT`, `/éç½®pt` ### æ°æ®ç»è®¡ - `/
 å¯¹ææ°æ®` - `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]` - `/æè¿èµ°å¿
 [@<ç¨æ·>]` - å«åï¼`/èµ°å¿` ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤åå¯éè¿ç§è/
-ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
+ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ï¼QQé¢éæä¸æ¯æç§èï¼ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
 q`å¯éåºé®ç­æ¨¡å¼ã ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤ï¼æ¥è¯¢ãå¯¼åºé¤å¤ï¼éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ã
 ## éç½® ### mahjong_scoreboard_database_conn_url
 æ°æ®åºè¿æ¥URLï¼å¿é¡»ä½¿ç¨å¼æ­¥SQLAlchemyé©±å¨å¨ã
 é»è®¤å¼ï¼sqlite+aiosqlite:///mahjong_scoreboard.db ### callback_host
 åè°HOSTï¼è¥ä¸ºéå®¹å¨ç¯å¢é¨ç½²ï¼go-
 cqhttpä¸nonebotåè¿è¡å¨åä¸ç¯å¢ï¼åä¿æé»è®¤å¼ãè¥ä¸ºDockerç¯å¢é¨ç½²åè®¾ç½®ä¸ºDockerå®¹å¨åãç¨äºä¸ä¼ æä»¶æ¶è®©go-
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/config.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from datetime import datetime
 from io import StringIO
 
 import tzlocal
-from nonebot import on_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent
 
 from .interceptor import handle_error
 from .mapper.game_csv_mapper import write_games_csv
+from .mg import matcher_group
 from .utils.dep import GroupDep, SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import Group, Season
 from ..model.enums import SeasonState
 from ..platform.upload_file import upload_file
 from ..service.game_service import get_games
 from ..utils.date import encode_date
+from ..utils.nonebot import default_cmd_start
 
 # ========== 导出赛季对局 ==========
-export_season_games_matcher = on_command("导出赛季对局", aliases={"导出对局"}, priority=5)
+export_season_games_matcher = matcher_group.on_command("导出赛季对局", aliases={"导出对局"}, priority=5)
+export_season_games_matcher.__help_info__ = f"{default_cmd_start}导出赛季对局 [<赛季代号>]"
 
 require_store_command_args(export_season_games_matcher)
 require_platform_group_id(export_season_games_matcher)
 
 
 @export_season_games_matcher.handle()
 @handle_error()
 async def export_season_games(bot: Bot, event: MessageEvent, group: Group = GroupDep(),
                               season: Season = SeasonFromUnaryArgOrRunningSeason()):
     games = await get_games(group_id=group.id, season_id=season.id)
 
     if games.total == 0:
-        raise BadRequestError("本赛季还没有创建过对局")
+        raise ResultError("本赛季还没有创建过对局")
 
     filename = f"赛季对局 {season.name}"
     if season.state == SeasonState.finished:
         filename += "（已结束）"
     else:
         now = datetime.now(tzlocal.get_localzone())
         filename += f"（截至{encode_date(now)}）"
@@ -44,27 +46,28 @@
         await write_games_csv(sio, games.data)
 
         data = sio.getvalue().encode("utf_8_sig")
         await upload_file(bot, event, filename, data)
 
 
 # ========== 导出所有对局 ==========
-export_group_games_matcher = on_command("导出所有对局", priority=5)
+export_group_games_matcher = matcher_group.on_command("导出所有对局", priority=5)
+export_group_games_matcher.__help_info__ = f"{default_cmd_start}导出所有对局"
 
 require_store_command_args(export_season_games_matcher)
 require_platform_group_id(export_season_games_matcher)
 
 
 @export_group_games_matcher.handle()
 @handle_error()
 async def export_group_games(bot: Bot, event: MessageEvent, group: Group = GroupDep()):
     games = await get_games(group.id)
 
     if games.total == 0:
-        raise BadRequestError("本群还没有创建过对局")
+        raise ResultError("本群还没有创建过对局")
 
     now = datetime.now(tzlocal.get_localzone())
     filename = f"所有对局（截至{encode_date(now)}）.csv"
 
     with StringIO() as sio:
         await write_games_csv(sio, games.data)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from datetime import datetime, date, timedelta, time
 
-from nonebot import on_command, Bot
+from nonebot import Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 
 from .interceptor import handle_error
 from .mapper.game_mapper import map_game, map_game_lite
 from .mapper.pagination_mapper import map_pagination
+from .mg import matcher_group
 from .utils.dep import GroupDep, UnaryArg, UserDep
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
 from .utils.parse import parse_int_or_error
-from ..errors import BadRequestError
+from ..errors import BadRequestError, ResultError
 from ..model import Group, User
 from ..platform.get_user_nickname import get_user_nickname
 from ..platform.send_messages import send_msgs
 from ..service import game_service
 from ..service.game_service import get_games
+from ..utils.nonebot import default_cmd_start
 
 # =============== 查询对局 ===============
-query_by_code_matcher = on_command("查询对局", aliases={"对局"}, priority=5)
+query_by_code_matcher = matcher_group.on_command("查询对局", aliases={"对局"}, priority=5)
+query_by_code_matcher.__help_info__ = f"{default_cmd_start}查询对局 [<编号>]"
 
 require_store_command_args(query_by_code_matcher)
 require_platform_group_id(query_by_code_matcher)
 
 
 @query_by_code_matcher.handle()
 @handle_error()
 async def query_by_code(matcher: Matcher, group: Group = GroupDep(),
                         game_code=UnaryArg(parser=lambda x: parse_int_or_error(x, '对局编号'))):
     if game_code is None:
         raise BadRequestError("请指定对局编号")
 
     game = await game_service.get_game(game_code, group.id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     msg = await map_game(game, detailed=True)
     await matcher.send(msg)
 
 
 # ========== 个人最近对局 ==========
-query_user_recent_games_matcher = on_command("个人最近对局", priority=5)
+query_user_recent_games_matcher = matcher_group.on_command("个人最近对局", priority=5)
+query_user_recent_games_matcher.__help_info__ = f"{default_cmd_start}个人最近对局 [@<用户>]"
 
 require_store_command_args(query_user_recent_games_matcher)
 require_platform_group_id(query_user_recent_games_matcher)
 require_platform_user_id(query_user_recent_games_matcher)
 
 
 @query_user_recent_games_matcher.handle()
@@ -59,19 +63,20 @@
     msgs = await map_pagination(games.data, map_game_lite)
     if games.total != 0:
         msgs.insert(0, f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
                        f"最近七天的对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        raise BadRequestError("用户最近七天还没有进行过对局")
+        raise ResultError("用户最近七天还没有进行过对局")
 
 
 # ========== 群最近对局 ==========
-query_group_recent_games_matcher = on_command("群最近对局", aliases={"最近对局"}, priority=5)
+query_group_recent_games_matcher = matcher_group.on_command("群最近对局", aliases={"最近对局"}, priority=5)
+query_group_recent_games_matcher.__help_info__ = f"{default_cmd_start}群最近对局"
 
 require_store_command_args(query_group_recent_games_matcher)
 require_platform_group_id(query_group_recent_games_matcher)
 
 
 @query_group_recent_games_matcher.handle()
 @handle_error()
@@ -82,19 +87,20 @@
     games = await get_games(group.id, reverse_order=True, time_span=(start_time, end_time))
     msgs = await map_pagination(games.data, map_game_lite)
     if games.total != 0:
         msgs.insert(0, f"以下是本群最近七天的对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        raise BadRequestError("本群最近七天还没有进行过对局")
+        raise ResultError("本群最近七天还没有进行过对局")
 
 
 # ========== 个人未完成对局 ==========
-query_user_uncompleted_games_matcher = on_command("个人未完成对局", priority=5)
+query_user_uncompleted_games_matcher = matcher_group.on_command("个人未完成对局", priority=5)
+query_user_uncompleted_games_matcher.__help_info__ = f"{default_cmd_start}个人未完成对局 [@<用户>]"
 
 require_store_command_args(query_user_uncompleted_games_matcher)
 require_platform_group_id(query_user_uncompleted_games_matcher)
 require_platform_user_id(query_user_uncompleted_games_matcher)
 
 
 @query_user_uncompleted_games_matcher.handle()
@@ -106,19 +112,20 @@
     msgs = await map_pagination(games.data, map_game_lite)
     if games.total != 0:
         msgs.insert(0, f"以下是[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]"
                        f"的未完成对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        raise BadRequestError("用户没有未完成的对局")
+        raise ResultError("用户没有未完成的对局")
 
 
 # ========== 群未完成对局 ==========
-query_group_uncompleted_games_matcher = on_command("群未完成对局", aliases={"未完成对局"}, priority=5)
+query_group_uncompleted_games_matcher = matcher_group.on_command("群未完成对局", aliases={"未完成对局"}, priority=5)
+query_group_uncompleted_games_matcher.__help_info__ = f"{default_cmd_start}群未完成对局"
 
 require_store_command_args(query_group_uncompleted_games_matcher)
 require_platform_group_id(query_group_uncompleted_games_matcher)
 
 
 @query_group_uncompleted_games_matcher.handle()
 @handle_error()
@@ -126,8 +133,8 @@
     games = await get_games(group.id, uncompleted_only=True, reverse_order=True)
     msgs = await map_pagination(games.data, map_game_lite)
     if games.total != 0:
         msgs.insert(0, f"以下是本群的未完成对局：")
 
         await send_msgs(bot, event, msgs)
     else:
-        raise BadRequestError("本群没有未完成的对局")
+        raise ResultError("本群没有未完成的对局")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from io import StringIO
 from typing import Optional, NamedTuple
 
 from cachetools import TTLCache
-from nonebot import on_command
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import Depends
 from nonebot_plugin_session import Session
 
 from .interceptor import handle_error
 from .mapper.game_mapper import map_game
+from .mg import matcher_group
 from .utils.dep import GroupDep, UserDep, UnaryArg, SessionDep, SplitCommandArgs, SenderUserDep
 from .utils.parse import parse_int_or_error, try_parse_wind, parse_float_or_error, try_parse_game_code
 from ..errors import BadRequestError
 from ..model import Group, User
 from ..model.enums import PlayerAndWind, GameState, Wind
 from ..service import game_service
 from ..utils.nonebot import default_cmd_start
@@ -28,15 +28,16 @@
         if platform_group_id in group_latest_game_code:
             return group_latest_game_code[platform_group_id]
 
     return Depends(dependency)
 
 
 # =============== 新建对局 ===============
-new_game_matcher = on_command("新建对局", aliases={"新对局"}, priority=5)
+new_game_matcher = matcher_group.on_command("新建对局", aliases={"新对局"}, priority=5)
+new_game_matcher.__help_info__ = f"{default_cmd_start}新建对局 [四人南|四人东]"
 
 
 @new_game_matcher.handle()
 @handle_error()
 async def new_game(matcher: Matcher, player_and_wind=UnaryArg(), session: Session = SessionDep(),
                    group=GroupDep(), promoter=SenderUserDep()):
     if player_and_wind == "四人东":
@@ -52,15 +53,16 @@
     msg += f'\n\n新建对局成功，对此消息回复“{default_cmd_start}结算 <成绩>”指令记录你的成绩'
     await matcher.send(msg)
 
     group_latest_game_code[get_platform_group_id(session)] = game.code
 
 
 # =============== 结算 ===============
-record_matcher = on_command("结算对局", aliases={"结算"}, priority=5)
+record_matcher = matcher_group.on_command("结算对局", aliases={"结算"}, priority=5)
+record_matcher.__help_info__ = f"{default_cmd_start}结算对局 <成绩> [对局<编号>] [@<用户>] [<自风>]"
 
 
 class RecordArgs(NamedTuple):
     game_code: int
     score: int
     wind: Optional[Wind]
 
@@ -108,15 +110,16 @@
     msg += '\n\n结算成功'
     if game.state == GameState.invalid_total_point:
         msg += f"\n警告：对局的成绩之和不正确，对此消息回复“{default_cmd_start}结算 <成绩>”指令重新记录你的成绩"
     await matcher.send(msg)
 
 
 # =============== 撤销结算 ===============
-revert_record_matcher = on_command("撤销结算对局", aliases={"撤销结算"}, priority=5)
+revert_record_matcher = matcher_group.on_command("撤销结算对局", aliases={"撤销结算"}, priority=5)
+revert_record_matcher.__help_info__ = f"{default_cmd_start}撤销结算对局 [对局<编号>] [@<用户>]"
 
 
 @revert_record_matcher.handle()
 @handle_error()
 async def revert_record(matcher: Matcher,
                         group: Group = GroupDep(),
                         user: User = UserDep(),
@@ -133,15 +136,16 @@
 
     msg = await map_game(game)
     msg += '\n\n撤销结算成功'
     await matcher.send(msg)
 
 
 # =============== 设置对局PT ===============
-set_record_point_matcher = on_command("设置对局PT", aliases={"对局PT"}, priority=5)
+set_record_point_matcher = matcher_group.on_command("设置对局PT", aliases={"对局PT"}, priority=5)
+set_record_point_matcher.__help_info__ = f"{default_cmd_start}设置对局PT <PT> [对局<编号>] [@<用户>]"
 
 
 class SetRecordPointArgs(NamedTuple):
     game_code: int
     point: float
 
 
@@ -178,15 +182,16 @@
 
     msg = await map_game(game)
     msg += '\n\n设置PT成功'
     await matcher.send(msg)
 
 
 # =============== 删除对局 ===============
-delete_game_matcher = on_command("删除对局", priority=5)
+delete_game_matcher = matcher_group.on_command("删除对局", priority=5)
+delete_game_matcher.__help_info__ = f"{default_cmd_start}删除对局 [对局<编号>]"
 
 
 @delete_game_matcher.handle()
 @handle_error()
 async def delete_game(matcher: Matcher, group: Group = GroupDep(), operator: User = SenderUserDep(),
                       game_code=UnaryArg(parser=try_parse_game_code)):
     if game_code is None:
@@ -194,15 +199,16 @@
 
     await game_service.delete_game(game_code, group.id, operator.id)
 
     await matcher.send(f'成功删除对局{game_code}')
 
 
 # =============== 设置对局进度 ===============
-make_game_progress_matcher = on_command("设置对局进度", aliases={"对局进度"}, priority=5)
+make_game_progress_matcher = matcher_group.on_command("设置对局进度", aliases={"对局进度"}, priority=5)
+make_game_progress_matcher.__help_info__ = f"{default_cmd_start}设置对局进度 <东/南x局y本场 或 完成> [对局<编号>]"
 
 round_honba_pattern = r"([东南])([一二三四1234])局([0123456789零一两二三四五六七八九十百千万亿]+)本场"
 
 
 class MakeGameProgressArgs(NamedTuple):
     game_code: int
     completed: bool
@@ -257,15 +263,16 @@
 
     msg = await map_game(game)
     msg += "\n\n成功设置对局进度"
     await matcher.send(msg)
 
 
 # ========== 设置对局备注 ===========
-set_game_comment_matcher = on_command("设置对局备注", aliases={"对局备注"}, priority=5)
+set_game_comment_matcher = matcher_group.on_command("设置对局备注", aliases={"对局备注"}, priority=5)
+set_game_comment_matcher.__help_info__ = f"{default_cmd_start}设置对局备注 [对局<编号>] <备注文本>"
 
 
 class SetGameCommentArgs(NamedTuple):
     game_code: int
     comment: str
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/game_statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # ========== 查询最近走势 ==========
 from io import StringIO
 
-from nonebot import on_command, Bot
+from nonebot import Bot
 from nonebot.internal.matcher import Matcher, current_bot
 from nonebot_plugin_session import Session
 
 from .interceptor import handle_error
 from .mapper import map_point, digit_mapping, percentile_str, map_real_point
+from .mg import matcher_group
 from .utils.dep import GroupDep, SessionDep, RunningSeasonDep, UserDep, SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import GameStatistics, Group, Season, User
 from ..platform.get_user_nickname import get_user_nickname
 from ..service.game_service import get_game_statistics, get_games, get_season_game_statistics
+from ..utils.nonebot import default_cmd_start
 from ..utils.session import get_platform_group_id
 
 # ============ 查询最近走势 ============
-query_season_user_trend_matcher = on_command("查询最近走势", aliases={"最近走势", "走势"}, priority=5)
+query_season_user_trend_matcher = matcher_group.on_command("最近走势", aliases={"走势"}, priority=5)
+query_season_user_trend_matcher.__help_info__ = f"{default_cmd_start}最近走势 [@<用户>]"
 
 require_store_command_args(query_season_user_trend_matcher)
 require_platform_group_id(query_season_user_trend_matcher)
 require_platform_user_id(query_season_user_trend_matcher)
 
 
 @query_season_user_trend_matcher.handle()
@@ -44,15 +47,15 @@
 
                 sio.write(f"  {record.rank}位    {record.score}点  "
                           f"({map_point(record.raw_point, record.point_scale)})  "
                           f"对局{game.code}\n")
 
             await matcher.send(sio.getvalue().strip())
     else:
-        raise BadRequestError("用户还没有参加过对局")
+        raise ResultError("用户还没有参加过对局")
 
 
 # ============ 对战数据 ============
 async def map_game_statistics(game_statistics: GameStatistics, user: User, group: Group) -> str:
     bot = current_bot.get()
     with StringIO() as sio:
         sio.write(f"用户[{await get_user_nickname(bot, user.platform_user_id, group.platform_group_id)}]的对战数据：\n")
@@ -64,15 +67,16 @@
         if game_statistics.pt_expectation is not None:
             sio.write(f"  PT期望：{map_real_point(game_statistics.pt_expectation, 2)}\n")
         sio.write(f"  被飞率：{percentile_str(game_statistics.flying_rate)}")
 
         return sio.getvalue().strip()
 
 
-query_user_statistics_matcher = on_command("对战数据", priority=5)
+query_user_statistics_matcher = matcher_group.on_command("对战数据", priority=5)
+query_user_statistics_matcher.__help_info__ = f"{default_cmd_start}对战数据 [@<用户>]"
 
 require_store_command_args(query_user_statistics_matcher)
 require_platform_group_id(query_user_statistics_matcher)
 require_platform_user_id(query_user_statistics_matcher)
 
 
 @query_user_statistics_matcher.handle()
@@ -81,15 +85,16 @@
                                 user: User = UserDep()):
     game_statistics = await get_game_statistics(group.id, user.id)
     msg = await map_game_statistics(game_statistics, user, group)
     await matcher.send(msg)
 
 
 # ============ 赛季对战数据 ============
-query_season_user_statistics_matcher = on_command("赛季对战数据", priority=5)
+query_season_user_statistics_matcher = matcher_group.on_command("赛季对战数据", priority=5)
+query_season_user_statistics_matcher.__help_info__ = f"{default_cmd_start}赛季对战数据 [<赛季代号>] [@<用户>]"
 
 require_store_command_args(query_season_user_statistics_matcher)
 require_platform_group_id(query_season_user_statistics_matcher)
 require_platform_user_id(query_season_user_statistics_matcher)
 
 
 @query_season_user_statistics_matcher.handle()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/interceptor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from functools import wraps
 
 from nonebot import logger
 from nonebot.exception import MatcherException, ActionFailed
 from nonebot.internal.matcher import current_event, current_matcher
 
-from ...errors import BadRequestError
+from ...errors import BadRequestError, ResultError
 
 
 def handle_error():
     def decorator(func):
         @wraps(func)
         async def wrapped_func(*args, **kwargs):
             matcher = current_matcher.get()
             try:
                 return await func(*args, **kwargs)
             except MatcherException as e:
                 raise e
             except BadRequestError as e:
+                await matcher.finish(f"{e.message}\n\n指令用法：{matcher.__help_info__}")
+            except ResultError as e:
                 await matcher.finish(e.message)
             except ActionFailed as e:
                 # 避免当发送消息错误时再尝试发送
                 logger.exception(e)
             except Exception as e:
                 logger.exception(e)
                 await matcher.finish(f"内部错误：{type(e)}{str(e)}")
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_csv_mapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import csv
 from typing import TextIO, Iterable
 
 from nonebot.internal.matcher import current_bot
 
 from nonebot_plugin_mahjong_scoreboard.controller.mapper import game_state_mapping, \
-    player_and_wind_mapping, map_datetime, map_point
+    player_and_wind_mapping, map_datetime, map_point, wind_mapping
 from nonebot_plugin_mahjong_scoreboard.controller.mapper.game_mapper import map_game_progress
 from nonebot_plugin_mahjong_scoreboard.model import Game
 from nonebot_plugin_mahjong_scoreboard.model.enums import GameState
 from nonebot_plugin_mahjong_scoreboard.platform.get_user_nickname import get_user_nickname
 from nonebot_plugin_mahjong_scoreboard.utils.session import get_real_id
 
 
 async def write_games_csv(f: TextIO, games: Iterable[Game]):
     bot = current_bot.get()
 
     writer = csv.writer(f)
     writer.writerow(['对局编号', '对局类型', '状态', '完成时间',
                      '所属赛季', '发起者',
-                     '一位', '一位分数', '一位PT收支',
-                     '二位', '二位分数', '二位PT收支',
-                     '三位', '三位分数', '三位PT收支',
-                     '四位', '四位分数', '四位PT收支',
+                     '一位', '一位分数', '一位PT收支', '一位座次',
+                     '二位', '二位分数', '二位PT收支', '二位座次',
+                     '三位', '三位分数', '三位PT收支', '三位座次',
+                     '四位', '四位分数', '四位PT收支', '四位座次',
                      '进度', '备注'])
     for g in games:
         row = [
             g.code, player_and_wind_mapping[g.player_and_wind],
             game_state_mapping[g.state],
         ]
 
@@ -45,15 +45,16 @@
         else:
             row.append("")
 
         for r in sorted(g.records, key=lambda x: x.raw_point, reverse=True):
             row.extend([f"{await get_user_nickname(bot, r.user.platform_user_id, g.group.platform_group_id)}"
                         f" ({get_real_id(r.user.platform_user_id)})",
                         r.score,
-                        map_point(r.raw_point, r.point_scale)])
+                        map_point(r.raw_point, r.point_scale) if g.state == GameState.completed else '',
+                        wind_mapping[r.wind] if r.wind is not None else ''])
 
         if g.progress is not None:
             row.append(map_game_progress(g.progress))
         else:
             row.append("")
 
         row.append(g.comment)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/game_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,12 +89,17 @@
 
         if game.progress is not None:
             io.write(f"[{map_game_progress(game.progress)}]")
         else:
             io.write(f"[{game_state_mapping[game.state]}]")
 
         for r in sorted(game.records, key=lambda r: r.raw_point, reverse=True):
-            io.write(f"  {await get_user_nickname(bot, r.user.platform_user_id, game.group.platform_group_id)}")
+            io.write("  ")
+            if r.wind is not None:
+                io.write(f"[{wind_mapping[r.wind]}]")
+            io.write(f"{await get_user_nickname(bot, r.user.platform_user_id, game.group.platform_group_id)}")
             if game.state == GameState.completed:
                 io.write(f"({map_point(r.raw_point, r.point_scale)})")
+            else:
+                io.write(f"({r.score}点)")
 
         return io.getvalue().strip()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/pagination_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_csv_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/mapper/season_user_point_mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_manage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 import re
 
-from nonebot import on_command
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import ArgPlainText
 
 from .interceptor import handle_interruption, handle_error
 from .mapper.season_mapper import map_season
-from .utils.dep import GroupDep, UnaryArg, RunningSeasonDep, SenderUserDep, GroupAdminDep
-from .utils.general_handlers import hint_for_question_flow_on_first, require_store_command_args
+from .mg import matcher_group
+from .utils.dep import GroupDep, UnaryArg, RunningSeasonDep, SenderUserDep, IsGroupAdminDep
+from .utils.general_handlers import hint_for_question_flow_on_first, require_platform_group_id, \
+    require_store_command_args
 from .utils.parse import parse_int_or_reject
-from ..errors import BadRequestError
+from ..errors import BadRequestError, ResultError
 from ..model import Group, Season, User, SeasonConfig
 from ..model.enums import SeasonState
 from ..service import season_service
 from ..service.season_service import get_season_by_code, new_season, start_season, finish_season
+from ..utils.nonebot import default_cmd_start
 
 # ========== 新赛季 ==========
-new_season_matcher = on_command("新建赛季", aliases={"新赛季"}, priority=5)
+new_season_matcher = matcher_group.on_command("新建赛季", aliases={"新赛季"}, priority=5)
+new_season_matcher.__help_info__ = f"{default_cmd_start}新建赛季"
 
 new_season_matcher.append_handler(hint_for_question_flow_on_first)
 
+require_platform_group_id(new_season_matcher)
+
 
 @new_season_matcher.got("code", "赛季代号？")
 @handle_error()
 @handle_interruption()
 async def new_season_got_code(matcher: Matcher,
                               raw_arg=ArgPlainText("code"),
                               group: Group = GroupDep(),
-                              group_admin=GroupAdminDep()):
+                              group_admin=IsGroupAdminDep()):
     match_result = re.match(r"[_a-zA-Z]\w*", raw_arg)
     if match_result is None:
         await matcher.reject("赛季代号不合法。请重新输入。（赛季代号只允许包含字母、数字和下划线，且必须以字母或下划线开头）")
 
     season = await get_season_by_code(raw_arg, group.id)
     if season is not None:
         await matcher.reject("该赛季代号已被使用。请重新输入")
@@ -106,15 +111,15 @@
         matcher.state["east_game_enabled"] = True
     else:
         matcher.state["east_game_enabled"] = False
         matcher.set_arg("east_game_origin_point", Message())
         matcher.set_arg("east_game_horse_point", Message())
 
     if not matcher.state["south_game_enabled"] and not matcher.state["east_game_enabled"]:
-        raise BadRequestError("半庄战、东风战至少需要开启一种")
+        raise ResultError("半庄战、东风战至少需要开启一种")
 
 
 @new_season_matcher.got("east_game_origin_point", "东风战返点？")
 @handle_error()
 @handle_interruption()
 async def new_season_got_south_game_origin_point(matcher: Matcher,
                                                  raw_arg=ArgPlainText("east_game_origin_point")):
@@ -200,28 +205,32 @@
         await start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send(f"稍后可以使用“/开启赛季 {matcher.state['season'].code}”命令开启赛季")
 
 
 # ========== 开启赛季 ==========
-start_season_matcher = on_command("开启赛季", priority=5)
+start_season_matcher = matcher_group.on_command("开启赛季", priority=5)
+start_season_matcher.__help_info__ = f"{default_cmd_start}开启赛季 [<代号>]"
+
+require_store_command_args(start_season_matcher)
+require_platform_group_id(start_season_matcher)
 
 
 @start_season_matcher.handle()
 @handle_error()
 async def start_season_matcher_confirm(matcher: Matcher, group: Group = GroupDep(),
                                        season_code=UnaryArg(),
-                                       group_admin=GroupAdminDep()):
+                                       group_admin=IsGroupAdminDep()):
     if season_code is None:
         raise BadRequestError("请指定赛季编号。使用“/新赛季”指令创建赛季")
 
     season = await get_season_by_code(season_code, group.id)
     if season is None:
-        raise BadRequestError("找不到该赛季。使用“/新赛季”指令创建赛季")
+        raise ResultError("找不到该赛季。使用“/新赛季”指令创建赛季")
 
     matcher.state["season"] = season
 
     msg = map_season(season)
     if season.state != SeasonState.initial:
         msg += "\n\n赛季未处于初始状态，操作失败"
         await matcher.finish(msg)
@@ -237,21 +246,25 @@
         await season_service.start_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季开启成功")
     else:
         await matcher.send("取消开启赛季")
 
 
 # ========== 结束赛季 ==========
-finish_season_matcher = on_command("结束赛季", priority=5)
+finish_season_matcher = matcher_group.on_command("结束赛季", priority=5)
+finish_season_matcher.__help_info__ = f"{default_cmd_start}结束赛季"
+
+require_store_command_args(finish_season_matcher)
+require_platform_group_id(finish_season_matcher)
 
 
 @finish_season_matcher.handle()
 @handle_error()
 async def finish_season_confirm(matcher: Matcher, season: Season = RunningSeasonDep(),
-                                group_admin=GroupAdminDep()):
+                                group_admin=IsGroupAdminDep()):
     matcher.state["season"] = season
     msg = map_season(season)
     msg += "\n\n结束赛季将删除赛季的所有未完成对局，并且无法再修改赛季的已完成对局。\n确定结束赛季吗？(y/n)"
     await matcher.pause(msg)
 
 
 @finish_season_matcher.handle()
@@ -261,28 +274,32 @@
         await finish_season(matcher.state["season"].id, operator.id)
         await matcher.send("赛季结束成功")
     else:
         await matcher.send("取消结束赛季")
 
 
 # ========== 删除赛季 ==========
-remove_season_matcher = on_command("删除赛季", priority=5)
+remove_season_matcher = matcher_group.on_command("删除赛季", priority=5)
+remove_season_matcher.__help_info__ = f"{default_cmd_start}删除赛季 [<代号>]"
+
+require_store_command_args(remove_season_matcher)
+require_platform_group_id(remove_season_matcher)
 
 
 @remove_season_matcher.handle()
 @handle_error()
 async def remove_season_confirm(matcher: Matcher, group: Group = GroupDep(),
                                 season_code=UnaryArg(),
-                                group_admin=GroupAdminDep()):
+                                group_admin=IsGroupAdminDep()):
     if season_code is None:
         raise BadRequestError("请指定赛季编号")
 
     season = await get_season_by_code(season_code, group.id)
     if season is None:
-        raise BadRequestError("找不到该赛季")
+        raise ResultError("找不到该赛季")
 
     matcher.state["season"] = season
 
     msg = map_season(season)
     if season.state != SeasonState.initial:
         msg += "\n\n赛季未处于初始状态，操作失败"
         await matcher.finish(msg)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from io import StringIO
 
-from nonebot import on_command
 from nonebot.internal.matcher import Matcher
 
 from .interceptor import handle_error
 from .mapper import season_state_mapping
 from .mapper.season_mapper import map_season
+from .mg import matcher_group
 from .utils.dep import GroupDep, SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id
 from ..model import Group, Season
 from ..service.season_service import get_group_seasons
+from ..utils.nonebot import default_cmd_start
 
 # ========== 查询赛季 ==========
-query_season_matcher = on_command("查询赛季", aliases={"赛季", "当前赛季"}, priority=5)
+query_season_matcher = matcher_group.on_command("查询赛季", aliases={"赛季", "当前赛季"}, priority=10)
+query_season_matcher.__help_info__ = f"{default_cmd_start}查询赛季 [<代号>]"
 
 require_store_command_args(query_season_matcher)
 require_platform_group_id(query_season_matcher)
 
 
 @query_season_matcher.handle()
 @handle_error()
 async def query_running_season(matcher: Matcher,
                                season: Season = SeasonFromUnaryArgOrRunningSeason()):
     msg = map_season(season)
     await matcher.send(msg)
 
 
 # ========== 查询所有赛季 ==========
-query_all_seasons_matcher = on_command("查询所有赛季", aliases={"所有赛季"}, priority=5)
+query_all_seasons_matcher = matcher_group.on_command("查询所有赛季", aliases={"所有赛季"}, priority=5)
+query_all_seasons_matcher.__help_info__ = f"{default_cmd_start}查询所有赛季"
 
 require_store_command_args(query_all_seasons_matcher)
 require_platform_group_id(query_all_seasons_matcher)
 
 
 @query_all_seasons_matcher.handle()
 @handle_error()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from datetime import datetime
 from io import StringIO
 
 import tzlocal
-from nonebot import on_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent
 from nonebot_plugin_gocqhttp_cross_machine_upload_file import upload_file
 
 from .interceptor import handle_error
 from .mapper.season_user_point_csv_mapper import write_season_user_point_change_logs_csv
+from .mg import matcher_group
 from .utils.dep import SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import Season
 from ..model.enums import SeasonState
 from ..service.season_user_point_service import get_season_user_point_change_logs
 from ..utils.date import encode_date
+from ..utils.nonebot import default_cmd_start
 
 # ========== 导出榜单 ==========
-export_season_ranking_matcher = on_command("导出榜单", priority=5)
+export_season_ranking_matcher = matcher_group.on_command("导出榜单", priority=5)
+export_season_ranking_matcher.__help_info__ = f"{default_cmd_start}导出榜单 [<赛季代号>]"
 
 require_store_command_args(export_season_ranking_matcher)
 require_platform_group_id(export_season_ranking_matcher)
 
 
 @export_season_ranking_matcher.handle()
 @handle_error()
 async def export_season_ranking(bot: Bot, event: MessageEvent,
                                 season: Season = SeasonFromUnaryArgOrRunningSeason()):
     logs = await get_season_user_point_change_logs(season.id)
 
     if len(logs) == 0:
-        raise BadRequestError("还没有用户参与该赛季")
+        raise ResultError("还没有用户参与该赛季")
 
     filename = f"赛季榜单 {season.name}"
     if season.state == SeasonState.finished:
         filename += "（已结束）"
     else:
         now = datetime.now(tzlocal.get_localzone())
         filename += f"（截至{encode_date(now)}）"
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_manage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from nonebot import on_command, Bot
+from nonebot import Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher
 from nonebot_plugin_session import Session
 
 from .interceptor import handle_error
 from .mapper.season_user_point_mapper import map_season_user_point
-from .utils.dep import UserDep, GroupDep, RunningSeasonDep, SessionDep, UnaryArg, SenderUserDep, GroupAdminDep
+from .mg import matcher_group
+from .utils.dep import UserDep, GroupDep, RunningSeasonDep, SessionDep, UnaryArg, SenderUserDep, IsGroupAdminDep
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
 from .utils.parse import parse_float_or_error
 from ..model import Group, User, Season
 from ..platform.get_user_nickname import get_user_nickname
 from ..service.season_user_point_service import reset_season_user_point, change_season_user_point_manually
+from ..utils.nonebot import default_cmd_start
 from ..utils.session import get_platform_group_id
 
 # ========== 设置用户PT ==========
-set_season_user_point_matcher = on_command("设置用户PT", aliases={"设置用户pt", "设置PT", "设置pt"}, priority=5)
+set_season_user_point_matcher = matcher_group.on_command("设置用户PT", aliases={"设置用户pt", "设置PT", "设置pt"}, priority=5)
+set_season_user_point_matcher.__help_info__ = f"{default_cmd_start}设置PT <PT> [@<用户>]"
 
 require_store_command_args(set_season_user_point_matcher)
 require_platform_group_id(set_season_user_point_matcher)
 require_platform_user_id(set_season_user_point_matcher, use_sender_on_group_message=False)
 
 
 @set_season_user_point_matcher.handle()
 @handle_error()
 async def set_season_user_point_confirm(bot: Bot, matcher: Matcher, session: Session = SessionDep(),
                                         user: User = UserDep(use_sender=False),
                                         pt=UnaryArg(parser=lambda x: parse_float_or_error(x, 'PT')),
-                                        group_admin=GroupAdminDep()):
+                                        group_admin=IsGroupAdminDep()):
     await matcher.pause(
         f"确定设置用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
         f"PT为{pt}吗？(y/n)")
 
 
 @set_season_user_point_matcher.handle()
 @handle_error()
@@ -49,26 +52,27 @@
         msg += "\n\n设置用户PT成功"
         await matcher.send(msg)
     else:
         await matcher.finish("取消设置用户PT")
 
 
 # ========== 重置用户PT ==========
-reset_season_user_point_matcher = on_command("重置用户PT", aliases={"重置用户pt", "重置PT", "重置pt"}, priority=5)
+reset_season_user_point_matcher = matcher_group.on_command("重置用户PT", aliases={"重置用户pt", "重置PT", "重置pt"}, priority=5)
+reset_season_user_point_matcher.__help_info__ = f"{default_cmd_start}重置PT [@<用户>]"
 
 require_store_command_args(reset_season_user_point_matcher)
 require_platform_group_id(reset_season_user_point_matcher)
 require_platform_user_id(reset_season_user_point_matcher, use_sender_on_group_message=False)
 
 
 @reset_season_user_point_matcher.handle()
 @handle_error()
 async def reset_season_user_point_confirm(bot: Bot, matcher: Matcher, session: Session = SessionDep(),
                                           user: User = UserDep(use_sender=False),
-                                          group_admin=GroupAdminDep()):
+                                          group_admin=IsGroupAdminDep()):
     await matcher.pause(
         f"确定重置用户[{await get_user_nickname(bot, user.platform_user_id, get_platform_group_id(session))}]"
         f"PT吗？(y/n)")
 
 
 @reset_season_user_point_matcher.handle()
 @handle_error()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/season_user_point_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from io import StringIO
 
-from nonebot import on_command, Bot
+from nonebot import Bot
 from nonebot.internal.adapter import Event
 from nonebot.internal.matcher import Matcher, current_bot
 
 from .interceptor import handle_error
 from .mapper import season_state_mapping, map_point
 from .mapper.pagination_mapper import map_pagination
 from .mapper.season_user_point_mapper import map_season_user_point
+from .mg import matcher_group
 from .utils.dep import RunningSeasonDep, UserDep, SeasonFromUnaryArgOrRunningSeason
 from .utils.general_handlers import require_store_command_args, require_platform_group_id, require_platform_user_id
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import Season, User, SeasonUserPoint
 from ..platform.get_user_nickname import get_user_nickname
 from ..platform.send_messages import send_msgs
 from ..service.season_user_point_service import get_season_user_point, get_season_user_points
+from ..utils.nonebot import default_cmd_start
 
 # ========== 查询PT ==========
-query_season_point_matcher = on_command("查询PT", aliases={"查询pt", "PT", "pt"}, priority=5)
+query_season_point_matcher = matcher_group.on_command("查询PT", aliases={"查询pt", "PT", "pt"}, priority=5)
+query_season_point_matcher.__help_info__ = f"{default_cmd_start}查询PT [@<用户>]"
 
 require_store_command_args(query_season_point_matcher)
 require_platform_group_id(query_season_point_matcher)
 require_platform_user_id(query_season_point_matcher)
 
 
 @query_season_point_matcher.handle()
 @handle_error()
 async def query_season_point(matcher: Matcher, season: Season = RunningSeasonDep(),
                              user: User = UserDep()):
     sup = await get_season_user_point(season.id, user.id)
     if sup is None:
-        raise BadRequestError("用户还没有参加过对局")
+        raise ResultError("用户还没有参加过对局")
 
     msg = await map_season_user_point(sup, season)
     await matcher.send(msg)
 
 
 # ========== 查询榜单 ==========
-query_season_ranking_matcher = on_command("查询榜单", aliases={"榜单"}, priority=5)
+query_season_ranking_matcher = matcher_group.on_command("查询榜单", aliases={"榜单"}, priority=5)
+query_season_ranking_matcher.__help_info__ = f"{default_cmd_start}查询榜单 [<赛季代号>]"
 
 require_store_command_args(query_season_ranking_matcher)
 require_platform_group_id(query_season_ranking_matcher)
 
 
 async def map_sup(sup: SeasonUserPoint, season: Season):
     bot = current_bot.get()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/dep.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import Depends
 from nonebot.params import CommandArg
 from nonebot_plugin_session import extract_session
 
 from .message import split_message
 from ..interceptor import handle_error
-from ...errors import BadRequestError
+from ...errors import BadRequestError, ResultError
 from ...model import Group
 from ...platform.mention import extract_mention_user
 from ...service.group_service import get_group, is_group_admin
 from ...service.season_service import get_group_running_season, get_season_by_code
 from ...service.user_service import get_user
 from ...utils.session import get_platform_group_id, get_platform_user_id
 
@@ -69,24 +69,24 @@
 def UserDep(*, lookup_matcher_state: bool = True,
             lookup_matcher_state_key: str = "platform_user_id",
             use_mention_user_arg: bool = True,
             mention_user_arg_lookup_matcher_state: bool = True,
             mention_user_arg_lookup_matcher_state_key: str = "command_args_store",
             use_sender: bool = True,
             raise_on_missing: bool = True):
-    # 优先级：matcher.state、消息中的提及、事件发送者
+    # 优先级：消息中的提及、matcher.state、事件发送者
     @handle_error()
     async def dependency(matcher: Matcher, session=SessionDep(),
                          mention=MentionUserArg(lookup_matcher_state=mention_user_arg_lookup_matcher_state,
                                                 lookup_matcher_state_key=mention_user_arg_lookup_matcher_state_key)):
         platform_user_id = None
-        if lookup_matcher_state:
-            platform_user_id = matcher.state.get(lookup_matcher_state_key)
-        if platform_user_id is None and use_mention_user_arg and mention is not None:
+        if use_mention_user_arg and mention is not None:
             platform_user_id = mention
+        if platform_user_id is None and lookup_matcher_state:
+            platform_user_id = matcher.state.get(lookup_matcher_state_key)
         if platform_user_id is None and use_sender:
             platform_user_id = get_platform_user_id(session)
 
         if platform_user_id is None:
             if raise_on_missing:
                 raise BadRequestError("请指定用户")
             else:
@@ -111,15 +111,15 @@
     async def dependency(matcher: Matcher, group=GroupDep(lookup_matcher_state=group_lookup_matcher_state,
                                                           lookup_matcher_state_key=group_lookup_matcher_state_key)):
         if "db_mutex" not in matcher.state:
             matcher.state["db_mutex"] = Lock()
         async with matcher.state["db_mutex"]:
             season = await get_group_running_season(group.id)
             if season is None and raise_on_missing:
-                raise BadRequestError("当前没有运行中的赛季")
+                raise ResultError("当前没有运行中的赛季")
             return season
 
     return Depends(dependency)
 
 
 def UnaryArg(*, lookup_matcher_state: bool = True,
              lookup_matcher_state_key: str = "command_args_store",
@@ -164,26 +164,26 @@
                                               lookup_matcher_state_key=unary_arg_lookup_matcher_state_key)):
         if "db_mutex" not in matcher.state:
             matcher.state["db_mutex"] = Lock()
         async with matcher.state["db_mutex"]:
             if season_code:
                 season = await get_season_by_code(season_code, group.id)
                 if season is None:
-                    raise BadRequestError("找不到指定赛季")
+                    raise ResultError("找不到指定赛季")
             else:
                 season = await get_group_running_season(group.id)
                 if season is None:
-                    raise BadRequestError("当前没有运行中的赛季")
+                    raise ResultError("当前没有运行中的赛季")
             return season
 
     return Depends(dependency)
 
 
-def GroupAdminDep(raise_on_false: bool = True):
+def IsGroupAdminDep(raise_on_false: bool = True):
     @handle_error()
     async def dependency(group=GroupDep(), sender=SenderUserDep()):
         admin = await is_group_admin(sender.id, group.id)
         if not admin and raise_on_false:
-            raise BadRequestError("权限不足")
+            raise ResultError("权限不足")
         return admin
 
     return dependency
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/general_handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/controller/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/get_user_nickname.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/is_group_admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/mention.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/send_messages/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/platform/upload_file.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/metainfo.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/_data_source/migrations/v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/data_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/game.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta
-from typing import List, Optional, Tuple, overload
+from typing import Optional, Tuple, overload
 
 from sqlalchemy import update, Select, select, func
 from sqlalchemy.orm import selectinload
 
 from .base import Repository
 from .data_model import GameOrm, GameProgressOrm, GameRecordOrm
 from .pagination import Page
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/group.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/season.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/season.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 
 from sqlalchemy import update, select, and_, delete, func
 from sqlalchemy.sql.functions import count
 
 from .base import Repository
 from .data_model import GameOrm, SeasonOrm, SeasonUserPointOrm, SeasonUserPointChangeLogOrm
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model.enums import GameState, SeasonUserPointChangeType
 from ..utils.rank import ranked
 
 
 class SeasonRepository(Repository[SeasonOrm]):
     async def get_by_pk(self, pk: int) -> Optional[SeasonOrm]:
         stmt = select(SeasonOrm).where(
@@ -155,15 +155,15 @@
                 SeasonUserPointChangeLogOrm.season_id == change_log.season_id,
                 SeasonUserPointChangeLogOrm.user_id == change_log.user_id,
                 SeasonUserPointChangeLogOrm.id > change_log.id
             )
             cnt = (await self.session.execute(stmt)).scalar_one()
 
             if cnt != 0:
-                raise BadRequestError("撤销结算失败，在该对局之后该用户PT发生了改变")
+                raise ResultError("撤销结算失败，在该对局之后该用户PT发生了改变")
 
             user_point.point -= change_log.change_point
             await self.session.delete(change_log)
 
             # 若用户只有这一次PT变动，则删除PT记录
             stmt = select(func.count(SeasonUserPointChangeLogOrm.id)).where(
                 SeasonUserPointChangeLogOrm.season_id == user_point.season_id,
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/repository/user.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/repository/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/game_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nonebot import logger
 from nonebot_plugin_apscheduler import scheduler
 from sqlalchemy import delete
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .group_service import is_group_admin
 from .mapper import map_game
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import Game, GameStatistics
 from ..model.enums import GameState, PlayerAndWind, Wind, SeasonState
 from ..repository import data_source
 from ..repository.data_model import GroupOrm, GameOrm, GameRecordOrm, GameProgressOrm, SeasonOrm
 from ..repository.game import GameRepository
 from ..repository.pagination import Page
 from ..repository.season import SeasonRepository
@@ -33,25 +33,25 @@
 async def _ensure_updatable(game: GameOrm):
     session = data_source.session()
     repo = SeasonRepository(session)
 
     if game.season_id is not None:
         season = await repo.get_by_pk(game.season_id)
         if season.state != SeasonState.running:
-            raise BadRequestError("赛季已经结束，无法再修改对局")
+            raise ResultError("赛季已经结束，无法再修改对局")
 
 
 async def _ensure_permission(game: GameOrm, group_id: int, operator_user_id: int):
     if game.state == GameState.completed:
         completed_before_24h = datetime.utcnow() - game.complete_time >= timedelta(days=1)
 
         if not completed_before_24h or await is_group_admin(operator_user_id, group_id):
             return
 
-        raise BadRequestError("对局已完成超过24小时，需要管理员权限才能操作")
+        raise ResultError("对局已完成超过24小时，需要管理员权限才能操作")
 
 
 async def new_game(promoter_user_id: int,
                    group_id: int,
                    player_and_wind: Optional[PlayerAndWind]) -> Game:
     session = data_source.session()
 
@@ -82,15 +82,15 @@
         else:
             player_and_wind = PlayerAndWind.four_men_south
     else:
         if group.running_season_id is not None:
             season = await season_repo.get_by_pk(group.running_season_id)
             if player_and_wind == PlayerAndWind.four_men_south and not season.config.south_game_enabled \
                     or player_and_wind == PlayerAndWind.four_men_east and not season.config.east_game_enabled:
-                raise BadRequestError("当前赛季未开放此类型对局")
+                raise ResultError("当前赛季未开放此类型对局")
 
     game = GameOrm(code=game_code,
                    group_id=group_id,
                    promoter_user_id=promoter_user_id,
                    player_and_wind=player_and_wind,
                    season_id=group.running_season_id,
                    records=[])
@@ -118,26 +118,26 @@
     session = data_source.session()
 
     game_repo = GameRepository(session)
     season_repo = SeasonRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
     await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
         if r.user_id == user_id:
             record = r
             break
     else:
         if len(game.records) == 4:
-            raise BadRequestError("这场对局已经存在4人记录")
+            raise ResultError("这场对局已经存在4人记录")
 
         record = GameRecordOrm(game_id=game.id, user_id=user_id)
         session.add(record)
         game.records.append(record)
 
     if game.state == GameState.completed and game.season_id:
         await season_repo.revert_season_user_point_by_game(game)
@@ -253,25 +253,25 @@
     session = data_source.session()
 
     game_repo = GameRepository(session)
     season_repo = SeasonRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
     await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
         if r.user_id == user_id:
             record = r
             break
     else:
-        raise BadRequestError("用户还没有记录过这场对局")
+        raise ResultError("用户还没有记录过这场对局")
 
     if game.state == GameState.completed and game.season_id:
         await season_repo.revert_season_user_point_by_game(game)
 
     game.state = GameState.uncompleted
     game.records.remove(record)
     await session.delete(record)
@@ -287,20 +287,20 @@
     session = data_source.session()
 
     game_repo = GameRepository(session)
     season_repo = SeasonRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
 
     if not await is_group_admin(operator_user_id, group_id):
-        raise BadRequestError("需要管理员权限进行该操作")
+        raise ResultError("需要管理员权限进行该操作")
 
     if game.state == GameState.completed and game.season_id:
         await season_repo.revert_season_user_point_by_game(game)
 
     game.accessible = False
     game.delete_time = datetime.utcnow()
     game.update_time = datetime.utcnow()
@@ -318,15 +318,15 @@
     session = data_source.session()
 
     game_repo = GameRepository(session)
     season_repo = SeasonRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
     await _ensure_permission(game, group_id, operator_user_id)
 
     if game.state == GameState.completed and game.season_id:
         await season_repo.revert_season_user_point_by_game(game)
 
@@ -349,15 +349,15 @@
 async def remove_game_progress(game_code: int, group_id: int):
     session = data_source.session()
 
     game_repo = GameRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
 
     progress = await game_repo.get_progress(game.id)
     if progress is not None:
         # 不能用session.delete，否则之后session.get还能获取到
         stmt = delete(GameProgressOrm).where(GameProgressOrm.game_id == game.id)
@@ -375,31 +375,31 @@
     session = data_source.session()
 
     game_repo = GameRepository(session)
     season_repo = SeasonRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
     await _ensure_permission(game, group_id, operator_user_id)
 
     for r in game.records:
         if r.user_id == user_id:
             record = r
             break
     else:
-        raise BadRequestError("用户还没有记录过这场对局")
+        raise ResultError("用户还没有记录过这场对局")
 
     if game.state != GameState.completed:
-        raise BadRequestError("这场对局未处于完成状态")
+        raise ResultError("这场对局未处于完成状态")
 
     if game.season_id is None:
-        raise BadRequestError("这场对局不属于赛季")
+        raise ResultError("这场对局不属于赛季")
 
     await season_repo.revert_season_user_point_by_game(game)
 
     season = await season_repo.get_by_pk(game.season_id)
     record.point_scale = season.config.point_precision
     record.raw_point = int(point * (10 ** -season.config.point_precision))
 
@@ -413,15 +413,15 @@
 async def set_game_comment(game_code: int, group_id: int, comment: str, operator_user_id: int):
     session = data_source.session()
 
     game_repo = GameRepository(session)
 
     game = await game_repo.get_by_code(game_code, group_id)
     if game is None:
-        raise BadRequestError("未找到指定对局")
+        raise ResultError("未找到指定对局")
 
     await _ensure_updatable(game)
     await _ensure_permission(game, group_id, operator_user_id)
 
     game.comment = comment
 
     game.update_time = datetime.utcnow()
@@ -449,15 +449,15 @@
     data = [await map_game(g, session) for g in games.data]
     return Page(data=data, total=games.total)
 
 
 def _get_game_statistics_by_games(games: List[GameOrm], user_id: int,
                                   is_same_season: bool = False) -> GameStatistics:
     if len(games) == 0:
-        raise BadRequestError("你还没有进行对局")
+        raise ResultError("用户还没有进行对局")
 
     total = len(games)
 
     total_east = 0
     total_south = 0
 
     for g in games:
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/group_service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/mapper.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/season_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Optional, List
 
 from .game_service import delete_uncompleted_season_games
 from .group_service import is_group_admin
 from .mapper import map_season
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import Season, SeasonConfig
 from ..model.enums import SeasonState
 from ..repository import data_source
 from ..repository.data_model import GroupOrm, SeasonOrm
 from ..repository.season import SeasonRepository
 
 
@@ -71,17 +71,17 @@
 
     season = await repo.get_by_pk(season_id)
 
     await _ensure_permission(season, operator_user_id)
 
     group: GroupOrm = await session.get(GroupOrm, season.group_id)
     if season.state != SeasonState.initial:
-        raise BadRequestError("该赛季已经开启或已经结束")
+        raise ResultError("该赛季已经开启或已经结束")
     if group.running_season_id:
-        raise BadRequestError("当前已经有开启的赛季")
+        raise ResultError("当前已经有开启的赛季")
 
     season.state = SeasonState.running
     season.start_time = datetime.utcnow()
     group.running_season_id = season.id
 
     season.update_time = datetime.utcnow()
     await session.commit()
@@ -93,15 +93,15 @@
     repo = SeasonRepository(session)
 
     season = await repo.get_by_pk(season_id)
 
     await _ensure_permission(season, operator_user_id)
 
     if season.state != SeasonState.running:
-        raise BadRequestError("该赛季尚未开启或已经结束")
+        raise ResultError("该赛季尚未开启或已经结束")
 
     await delete_uncompleted_season_games(season.id)
 
     season.state = SeasonState.finished
     season.finish_time = datetime.utcnow()
 
     group = await session.get(GroupOrm, season.group_id)
@@ -117,13 +117,13 @@
     repo = SeasonRepository(session)
 
     season = await repo.get_by_pk(season_id)
 
     await _ensure_permission(season, operator_user_id)
 
     if season.state != SeasonState.initial:
-        raise BadRequestError("该赛季已经开启或已经结束")
+        raise ResultError("该赛季已经开启或已经结束")
 
     season.accessible = False
     season.delete_time = datetime.utcnow()
     season.update_time = datetime.utcnow()
     await session.commit()
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/service/season_user_point_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional, List
 
 from .group_service import is_group_admin
 from .mapper import map_season_user_point, map_season_user_point_change_log
-from ..errors import BadRequestError
+from ..errors import ResultError
 from ..model import SeasonUserPoint, SeasonUserPointChangeLog
 from ..repository import data_source
-from ..repository.pagination import Page
 from ..repository.season import SeasonRepository
 
 
 async def get_season_user_point(season_id: int, user_id: int) -> Optional[SeasonUserPoint]:
     session = data_source.session()
     repo = SeasonRepository(session)
     sup = await repo.get_season_user_point(season_id, user_id)
@@ -45,28 +44,28 @@
 
 
 async def reset_season_user_point(season_id: int,
                                   group_id: int,
                                   user_id: int,
                                   operator_user_id: int):
     if not await is_group_admin(operator_user_id, group_id):
-        raise BadRequestError("没有权限")
+        raise ResultError("没有权限")
 
     session = data_source.session()
     repo = SeasonRepository(session)
 
     await repo.reset_season_user_point(season_id, user_id)
 
 
 async def change_season_user_point_manually(season_id: int,
                                             group_id: int,
                                             user_id: int,
                                             point: float,
                                             operator_user_id: int) -> SeasonUserPoint:
     if not await is_group_admin(operator_user_id, group_id):
-        raise BadRequestError("没有权限")
+        raise ResultError("没有权限")
 
     session = data_source.session()
     repo = SeasonRepository(session)
 
     sup = await repo.change_season_user_point_manually(season_id, user_id, point)
     return await map_season_user_point(sup, session)
```

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/session.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py` & `nonebot_plugin_mahjong_scoreboard-0.4.1/src/nonebot_plugin_mahjong_scoreboard/utils/userdict.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mahjong_scoreboard-0.4.0a2/PKG-INFO` & `nonebot_plugin_mahjong_scoreboard-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mahjong-scoreboard
-Version: 0.4.0a2
+Version: 0.4.1
 Summary: 日麻寄分器（NoneBot插件）
 Home-page: https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: aiosqlite (>=0.17,<0.19)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.5,<0.2.0)
 Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
 Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4)
 Requires-Dist: nonebot-plugin-sqlalchemy (>=0.2.1,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard
 Description-Content-Type: text/plain
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
@@ -46,17 +46,15 @@
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-mahjong-scoreboard">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-mahjong-scoreboard.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 </p>
 
-支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)
-
-支持驱动器：[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-driver)
+支持适配器：[OneBot V11](https://onebot.adapters.nonebot.dev/)、[QQ Guild](https://github.com/nonebot/adapter-qqguild)
 
 ## 功能
 
 为群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。
 
 PT精算算法为（点数-返点+马点）/1000，返点和马点在创建赛季时进行设置。
 
@@ -139,15 +137,15 @@
     - 别名：`/对局PT`
 - `/删除对局 [对局<编号>]`
 - `/设置对局进度 <东/南x局y本场 或 完成> [对局<编号>]`
     - 别名：`/对局进度`
 - `/设置对局备注 [对局<编号>] <对局备注>`
     - 别名：`/对局备注`
 
-与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。也可以通过回复Bot发出的对局消息来代替指定对局编号。
+与对局相关的指令可以省略对局编号，省略时默认对最近新建的对局进行操作。
 
 对局相关指令在对局完成超过24小时后需要拥有群主或管理员身份才能使用。（`/删除对局`除外，该指令需要拥有群主或管理员身份才能使用）
 
 未完成且未设置进度的对局会在创建24小时后自动删除。赛季结束后，未完成对局会自动删除，所有已完成对局均无法再进行修改。
 
 ### 对局查询
 
@@ -190,15 +188,15 @@
 ### 数据统计
 
 - `/对战数据`
 - `/赛季对战数据 [<赛季代号>]`
 - `/最近走势 [@<用户>]`
     - 别名：`/走势`
 
-与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用。当未指定参数时进入问答模式，回复`/q`可退出问答模式。
+与赛季/赛季PT相关的指令均可通过私聊/群聊两种方式使用（QQ频道暂不支持私聊）。当未指定参数时进入问答模式，回复`/q`可退出问答模式。
 
 与赛季/赛季PT相关的指令（查询、导出除外）需要拥有群主或管理员身份才能使用。
 
 ## 配置
 
 ### mahjong_scoreboard_database_conn_url
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.4.0a2
+Metadata-Version: 2.1 Name: nonebot-plugin-mahjong-scoreboard Version: 0.4.1
 Summary: æ¥éº»å¯åå¨ï¼NoneBotæä»¶ï¼ Home-page: https://github.com/
 ssttkkl/nonebot-plugin-mahjong-scoreboard License: MIT Author: ssttkkl Author-
 email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiosqlite (>=0.17,<0.19) Requires-Dist:
 cachetools (>=5.2.0,<6.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
 file (>=0.1.5,<0.2.0) Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
 Requires-Dist: nonebot-plugin-session (>=0.0.3,<0.0.4) Requires-Dist: nonebot-
-plugin-sqlalchemy (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+plugin-sqlalchemy (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
 tzlocal (>=4.2,<5.0) Project-URL: Repository, https://github.com/ssttkkl/
 nonebot-plugin-mahjong-scoreboard Description-Content-Type: text/plain
                                    [nonebot]
           nonebot-plugin-mahjong-scoreboard ============ _â¨ NoneBot
                           æ¥éº»è®°åå¨æä»¶ â¨_
                            [license] [pypi] [python]
-æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/
-) æ¯æé©±å¨å¨ï¼[FastAPI](https://v2.nonebot.dev/docs/tutorial/choose-
-driver) ## åè½
+æ¯æééå¨ï¼[OneBot V11](https://onebot.adapters.nonebot.dev/)ã[QQ
+Guild](https://github.com/nonebot/adapter-qqguild) ## åè½
 ä¸ºç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
 PTç²¾ç®ç®æ³ä¸ºï¼ç¹æ°-è¿ç¹+é©¬ç¹ï¼/
 1000ï¼è¿ç¹åé©¬ç¹å¨åå»ºèµå­£æ¶è¿è¡è®¾ç½®ã ## å¸¸ç¨Workflow ###
 å¼å¯èµå­£ ``` /æ°å»ºèµå­£ ``` ### è®°å½ååºå¯¹å± ``` ä»»ä½äººï¼/
 æ°å»ºå¯¹å± A: /ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç®
 25000 ``` ### è®°å½ä¸åºå¯¹å± ``` ä»»ä½äººï¼/æ°å»ºå¯¹å± åäººä¸ A: /
 ç»ç® 25000 B: /ç»ç® 25000 C: /ç»ç® 25000 D: /ç»ç® 25000 ``` ###
@@ -42,15 +41,15 @@
 [åäººå|åäººä¸]` - å«åï¼`/æ°å¯¹å±` - `/ç»ç®å¯¹å± <æç»©>
 [å¯¹å±<ç¼å·>] [@<ç¨æ·>] [<èªé£>]` - å«åï¼`/ç»ç®` - `/
 æ¤éç»ç®å¯¹å± [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/æ¤éç»ç®` -
 `/è®¾ç½®å¯¹å±PT  [å¯¹å±<ç¼å·>] [@<ç¨æ·>]` - å«åï¼`/å¯¹å±PT` - `/
 å é¤å¯¹å± [å¯¹å±<ç¼å·>]` - `/è®¾ç½®å¯¹å±è¿åº¦ <ä¸/åxå±yæ¬åº æ
 å®æ> [å¯¹å±<ç¼å·>]` - å«åï¼`/å¯¹å±è¿åº¦` - `/è®¾ç½®å¯¹å±å¤æ³¨
 [å¯¹å±<ç¼å·>] <å¯¹å±å¤æ³¨>` - å«åï¼`/å¯¹å±å¤æ³¨`
-ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ãä¹å¯ä»¥éè¿åå¤Botååºçå¯¹å±æ¶æ¯æ¥ä»£æ¿æå®å¯¹å±ç¼å·ã
+ä¸å¯¹å±ç¸å³çæä»¤å¯ä»¥çç¥å¯¹å±ç¼å·ï¼çç¥æ¶é»è®¤å¯¹æè¿æ°å»ºçå¯¹å±è¿è¡æä½ã
 å¯¹å±ç¸å³æä»¤å¨å¯¹å±å®æè¶è¿24å°æ¶åéè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ãï¼`/
 å é¤å¯¹å±`é¤å¤ï¼è¯¥æä»¤éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ï¼
 æªå®æä¸æªè®¾ç½®è¿åº¦çå¯¹å±ä¼å¨åå»º24å°æ¶åèªå¨å é¤ãèµå­£ç»æåï¼æªå®æå¯¹å±ä¼èªå¨å é¤ï¼ææå·²å®æå¯¹å±åæ æ³åè¿è¡ä¿®æ¹ã
 ### å¯¹å±æ¥è¯¢ - `/æ¥è¯¢å¯¹å± [<ç¼å·>]` - å«åï¼`/å¯¹å±` - `/
 ä¸ªäººæè¿å¯¹å± [@<ç¨æ·>]` - å«åï¼`/æè¿å¯¹å±` - `/ç¾¤æè¿å¯¹å±`
 - `/ä¸ªäººæªå®æå¯¹å± [@<ç¨æ·>]` - å«åï¼`/æªå®æå¯¹å±` - `/
 ç¾¤æªå®æå¯¹å±` - `/å¯¼åºèµå­£å¯¹å± [<ä»£å·>]` - å«åï¼`/
@@ -61,15 +60,15 @@
 `/æ¥è¯¢æ¦å` - å«åï¼`/æ¦å` - `/å¯¼åºæ¦å` - `/æ¥è¯¢PT
 [@<ç¨æ·>]` - å«åï¼`/PT` - `/è®¾ç½®ç¨æ·PT  @<ç¨æ·>` - å«åï¼`/
 è®¾ç½®ç¨æ·pt`, `/è®¾ç½®PT`, `/è®¾ç½®pt` - `/éç½®ç¨æ·PT @<ç¨æ·>` -
 å«åï¼`/éç½®ç¨æ·pt`, `/éç½®PT`, `/éç½®pt` ### æ°æ®ç»è®¡ - `/
 å¯¹ææ°æ®` - `/èµå­£å¯¹ææ°æ® [<èµå­£ä»£å·>]` - `/æè¿èµ°å¿
 [@<ç¨æ·>]` - å«åï¼`/èµ°å¿` ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤åå¯éè¿ç§è/
-ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
+ç¾¤èä¸¤ç§æ¹å¼ä½¿ç¨ï¼QQé¢éæä¸æ¯æç§èï¼ãå½æªæå®åæ°æ¶è¿å¥é®ç­æ¨¡å¼ï¼åå¤`/
 q`å¯éåºé®ç­æ¨¡å¼ã ä¸èµå­£/
 èµå­£PTç¸å³çæä»¤ï¼æ¥è¯¢ãå¯¼åºé¤å¤ï¼éè¦æ¥æç¾¤ä¸»æç®¡çåèº«ä»½æè½ä½¿ç¨ã
 ## éç½® ### mahjong_scoreboard_database_conn_url
 æ°æ®åºè¿æ¥URLï¼å¿é¡»ä½¿ç¨å¼æ­¥SQLAlchemyé©±å¨å¨ã
 é»è®¤å¼ï¼sqlite+aiosqlite:///mahjong_scoreboard.db ### callback_host
 åè°HOSTï¼è¥ä¸ºéå®¹å¨ç¯å¢é¨ç½²ï¼go-
 cqhttpä¸nonebotåè¿è¡å¨åä¸ç¯å¢ï¼åä¿æé»è®¤å¼ãè¥ä¸ºDockerç¯å¢é¨ç½²åè®¾ç½®ä¸ºDockerå®¹å¨åãç¨äºä¸ä¼ æä»¶æ¶è®©go-
```

