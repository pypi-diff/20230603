# Comparing `tmp/aunly-bbot-1.3.2.tar.gz` & `tmp/aunly-bbot-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly-bbot-1.3.2.tar", last modified: Mon Apr  3 09:31:44 2023, max compression
+gzip compressed data, was "aunly-bbot-1.4.0.tar", last modified: Sat Jun  3 19:02:12 2023, max compression
```

## Comparing `aunly-bbot-1.3.2.tar` & `aunly-bbot-1.4.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rwxr-xr-x   0        0        0    34523 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/LICENSE
--rw-r--r--   0        0        0       61 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/__main__.py
--rw-r--r--   0        0        0     3361 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/bot.py
--rw-r--r--   0        0        0     1740 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/cli/__init__.py
--rw-r--r--   0        0        0     2197 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/cli/api.py
--rw-r--r--   0        0        0    21531 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/cli/config.py
--rw-r--r--   0        0        0      380 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/cli/run.py
--rw-r--r--   0        0        0     1981 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/core/__init__.py
--rw-r--r--   0        0        0     3054 2023-04-03 09:31:33.357189 aunly-bbot-1.3.2/aunly_bbot/core/announcement.py
--rw-r--r--   0        0        0      944 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/bot_config.py
--rw-r--r--   0        0        0      162 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/context.py
--rw-r--r--   0        0        0     5470 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/control.py
--rw-r--r--   0        0        0    10709 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/data.py
--rw-r--r--   0        0        0     1796 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/group_config.py
--rw-r--r--   0        0        0     2304 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/log.py
--rw-r--r--   0        0        0     2957 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/core/subgroup_config.py
--rw-r--r--   0        0        0     1996 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/__init__.py
--rw-r--r--   0        0        0      322 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/add_talk.py
--rw-r--r--   0        0        0     1526 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/admin/add.py
--rw-r--r--   0        0        0     1523 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/admin/remove.py
--rw-r--r--   0        0        0     1088 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/announcement.py
--rw-r--r--   0        0        0     2264 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/configure/atall.py
--rw-r--r--   0        0        0     2280 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/configure/nick.py
--rwxr-xr-x   0        0        0    13275 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/content_resolve.py
--rw-r--r--   0        0        0     1415 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/init.py
--rw-r--r--   0        0        0     2441 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/menu/__init__.py
--rw-r--r--   0        0        0     2491 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/quit_group.py
--rw-r--r--   0        0        0     1068 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/status.py
--rw-r--r--   0        0        0     1456 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/add.py
--rw-r--r--   0        0        0     2455 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/add_up.py
--rw-r--r--   0        0        0     1336 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/get_subgroup.py
--rw-r--r--   0        0        0     1355 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/remove.py
--rw-r--r--   0        0        0     2259 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/remove_up.py
--rw-r--r--   0        0        0     1666 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/up/get_subscribe.py
--rw-r--r--   0        0        0     2547 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/up/subscribe.py
--rw-r--r--   0        0        0     2101 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/up/unsubscribe.py
--rw-r--r--   0        0        0     1447 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/vip/add.py
--rw-r--r--   0        0        0     1446 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/vip/remove.py
--rw-r--r--   0        0        0     3017 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/vive_dynamic.py
--rw-r--r--   0        0        0     1554 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/web_auth.py
--rw-r--r--   0        0        0     1454 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/add.py
--rw-r--r--   0        0        0     1015 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/close.py
--rw-r--r--   0        0        0     1014 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/open.py
--rw-r--r--   0        0        0     1566 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/remove.py
--rw-r--r--   0        0        0     3945 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/bot_launch.py
--rw-r--r--   0        0        0     1432 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/exception.py
--rw-r--r--   0        0        0     1912 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/invited_join_group.py
--rw-r--r--   0        0        0     1762 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/join_group.py
--rw-r--r--   0        0        0     1923 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/leave_group.py
--rw-r--r--   0        0        0     1291 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/mute.py
--rw-r--r--   0        0        0     1475 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/new_friend.py
--rw-r--r--   0        0        0      919 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/offline.py
--rw-r--r--   0        0        0     1183 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/event/prem_change.py
--rw-r--r--   0        0        0    16456 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/pusher/dynamic.py
--rw-r--r--   0        0        0    15163 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/pusher/init.py
--rw-r--r--   0        0        0    10660 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/pusher/live.py
--rw-r--r--   0        0        0     2102 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/scheduler/refresh_token.py
--rw-r--r--   0        0        0      946 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/function/scheduler/version_update.py
--rw-r--r--   0        0        0     2856 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/model/bcut_asr.py
--rw-r--r--   0        0        0     7146 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/model/config.py
--rw-r--r--   0        0        0       93 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/model/exception.py
--rw-r--r--   0        0        0     1742 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/model/fastapi.py
--rw-r--r--   0        0        0      148 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/model/openai.py
--rw-r--r--   0        0        0     2904 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/static/bot_config.exp.yaml
--rw-r--r--   0        0        0     9159 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/static/mobile_style.js
--rw-r--r--   0        0        0      684 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/static/mobile_style_bak.js
--rw-r--r--   0        0        0      850 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/test.py
--rw-r--r--   0        0        0      675 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/b23_extract.py
--rw-r--r--   0        0        0     6184 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/bcut_asr.py
--rw-r--r--   0        0        0     4546 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/bilibili_request.py
--rw-r--r--   0        0        0     6027 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/browser_shot.py
--rw-r--r--   0        0        0      902 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/column_resolve.py
--rw-r--r--   0        0        0      797 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/content_summarise.py
--rw-r--r--   0        0        0     2166 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/detect_package.py
--rw-r--r--   0        0        0     8979 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/draw_bili_image.py
--rw-r--r--   0        0        0      465 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/dynamic_shot.py
--rw-r--r--   0        0        0      310 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/fastapi.py
--rw-r--r--   0        0        0     4384 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/fonts_provider.py
--rw-r--r--   0        0        0      774 2023-04-03 09:31:33.361189 aunly-bbot-1.3.2/aunly_bbot/utils/message_resolve.py
--rw-r--r--   0        0        0     4380 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/openai.py
--rw-r--r--   0        0        0     1103 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/pil_shot.py
--rw-r--r--   0        0        0     5069 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/send_action.py
--rw-r--r--   0        0        0     1867 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/strings.py
--rw-r--r--   0        0        0     3030 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/text2image.py
--rw-r--r--   0        0        0      516 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/time_tools.py
--rw-r--r--   0        0        0     2474 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/uid_extract.py
--rw-r--r--   0        0        0     5876 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/up_operation.py
--rw-r--r--   0        0        0     1089 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/update_version.py
--rw-r--r--   0        0        0     1666 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/verify_mah.py
--rw-r--r--   0        0        0     3619 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/video_subtitle.py
--rw-r--r--   0        0        0      713 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/utils/wordcloud.py
--rw-r--r--   0        0        0     1509 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/__init__.py
--rw-r--r--   0        0        0      415 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/__init__.py
--rw-r--r--   0        0        0     4953 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/auth.py
--rw-r--r--   0        0        0     1266 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/config.py
--rw-r--r--   0        0        0     2730 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/follow.py
--rw-r--r--   0        0        0     1664 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/home.py
--rw-r--r--   0        0        0     1459 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/user.py
--rw-r--r--   0        0        0     4009 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/api/router/ws.py
--rw-r--r--   0        0        0    87542 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/static/html/favicon.ico
--rw-r--r--   0        0        0      306 2023-04-03 09:31:33.365189 aunly-bbot-1.3.2/aunly_bbot/website/static/html/index.html
--rw-r--r--   0        0        0     1659 2023-04-03 09:31:33.373189 aunly-bbot-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5120 2023-04-03 09:31:33.373189 aunly-bbot-1.3.2/readme.md
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0    34523 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/__main__.py
+-rw-r--r--   0        0        0     3361 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/bot.py
+-rw-r--r--   0        0        0     1753 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/cli/__init__.py
+-rw-r--r--   0        0        0     2197 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/cli/api.py
+-rw-r--r--   0        0        0    22390 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/cli/config.py
+-rw-r--r--   0        0        0      380 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/cli/run.py
+-rw-r--r--   0        0        0     1981 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/__init__.py
+-rw-r--r--   0        0        0     3054 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/announcement.py
+-rw-r--r--   0        0        0      944 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/bot_config.py
+-rw-r--r--   0        0        0      162 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/context.py
+-rw-r--r--   0        0        0     5470 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/control.py
+-rw-r--r--   0        0        0    10888 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/data.py
+-rw-r--r--   0        0        0     1796 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/group_config.py
+-rw-r--r--   0        0        0     2562 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/log.py
+-rw-r--r--   0        0        0     2957 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/core/subgroup_config.py
+-rw-r--r--   0        0        0     1996 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/add_talk.py
+-rw-r--r--   0        0        0     1526 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/admin/add.py
+-rw-r--r--   0        0        0     1523 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/admin/remove.py
+-rw-r--r--   0        0        0     1088 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/announcement.py
+-rw-r--r--   0        0        0     2264 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/configure/atall.py
+-rw-r--r--   0        0        0     2316 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/configure/nick.py
+-rwxr-xr-x   0        0        0    13590 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/content_resolve.py
+-rw-r--r--   0        0        0     1415 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/init.py
+-rw-r--r--   0        0        0     2480 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/menu/__init__.py
+-rw-r--r--   0        0        0     2491 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/quit_group.py
+-rw-r--r--   0        0        0     1068 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/status.py
+-rw-r--r--   0        0        0     1456 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/add.py
+-rw-r--r--   0        0        0     2455 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/add_up.py
+-rw-r--r--   0        0        0     1336 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/get_subgroup.py
+-rw-r--r--   0        0        0     1355 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/remove.py
+-rw-r--r--   0        0        0     2259 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/remove_up.py
+-rw-r--r--   0        0        0     1666 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/up/get_subscribe.py
+-rw-r--r--   0        0        0     2547 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/up/subscribe.py
+-rw-r--r--   0        0        0     2101 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/up/unsubscribe.py
+-rw-r--r--   0        0        0     1447 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/vip/add.py
+-rw-r--r--   0        0        0     1446 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/vip/remove.py
+-rw-r--r--   0        0        0     3017 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/vive_dynamic.py
+-rw-r--r--   0        0        0     1554 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/web_auth.py
+-rw-r--r--   0        0        0     1454 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/add.py
+-rw-r--r--   0        0        0     1015 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/close.py
+-rw-r--r--   0        0        0     1014 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/open.py
+-rw-r--r--   0        0        0     1566 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/remove.py
+-rw-r--r--   0        0        0     4026 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/bot_launch.py
+-rw-r--r--   0        0        0     1432 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/exception.py
+-rw-r--r--   0        0        0     1912 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/invited_join_group.py
+-rw-r--r--   0        0        0     1762 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/join_group.py
+-rw-r--r--   0        0        0     1923 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/leave_group.py
+-rw-r--r--   0        0        0     1291 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/mute.py
+-rw-r--r--   0        0        0     1475 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/new_friend.py
+-rw-r--r--   0        0        0      919 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/offline.py
+-rw-r--r--   0        0        0     1183 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/event/prem_change.py
+-rw-r--r--   0        0        0    16940 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/pusher/dynamic.py
+-rw-r--r--   0        0        0    15163 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/pusher/init.py
+-rw-r--r--   0        0        0    10666 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/pusher/live.py
+-rw-r--r--   0        0        0     2102 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/scheduler/refresh_token.py
+-rw-r--r--   0        0        0      946 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/function/scheduler/version_update.py
+-rw-r--r--   0        0        0     2856 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/model/bcut_asr.py
+-rw-r--r--   0        0        0     7654 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/model/config.py
+-rw-r--r--   0        0        0       93 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/model/exception.py
+-rw-r--r--   0        0        0     1742 2023-06-03 19:01:58.643142 aunly-bbot-1.4.0/aunly_bbot/model/fastapi.py
+-rw-r--r--   0        0        0      322 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/model/openai.py
+-rw-r--r--   0        0        0     3985 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/static/bot_config.exp.yaml
+-rw-r--r--   0        0        0     9159 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/static/mobile_style.js
+-rw-r--r--   0        0        0      684 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/static/mobile_style_bak.js
+-rw-r--r--   0        0        0      850 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/test.py
+-rw-r--r--   0        0        0      675 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/b23_extract.py
+-rw-r--r--   0        0        0     6184 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/bcut_asr.py
+-rw-r--r--   0        0        0      780 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/bilibili_parse.py
+-rw-r--r--   0        0        0     4760 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/bilibili_request.py
+-rw-r--r--   0        0        0     6398 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/browser_shot.py
+-rw-r--r--   0        0        0     1160 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/column_resolve.py
+-rw-r--r--   0        0        0      735 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/content_summarise.py
+-rw-r--r--   0        0        0     2166 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/detect_package.py
+-rw-r--r--   0        0        0     8979 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/draw_bili_image.py
+-rw-r--r--   0        0        0      551 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/dynamic_shot.py
+-rw-r--r--   0        0        0      310 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/fastapi.py
+-rw-r--r--   0        0        0     4384 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     6164 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/openai.py
+-rw-r--r--   0        0        0     1103 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/pil_shot.py
+-rw-r--r--   0        0        0     5069 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/send_action.py
+-rw-r--r--   0        0        0     1867 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/strings.py
+-rw-r--r--   0        0        0     3030 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/text2image.py
+-rw-r--r--   0        0        0      516 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/time_tools.py
+-rw-r--r--   0        0        0     2474 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/uid_extract.py
+-rw-r--r--   0        0        0     5876 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/up_operation.py
+-rw-r--r--   0        0        0     1089 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/update_version.py
+-rw-r--r--   0        0        0     1666 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/verify_mah.py
+-rw-r--r--   0        0        0     3803 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/video_subtitle.py
+-rw-r--r--   0        0        0      713 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/utils/wordcloud.py
+-rw-r--r--   0        0        0     1509 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/__init__.py
+-rw-r--r--   0        0        0     4953 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/auth.py
+-rw-r--r--   0        0        0     1266 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/config.py
+-rw-r--r--   0        0        0     2730 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/follow.py
+-rw-r--r--   0        0        0     1664 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/home.py
+-rw-r--r--   0        0        0     1459 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/user.py
+-rw-r--r--   0        0        0     4009 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/api/router/ws.py
+-rw-r--r--   0        0        0    87542 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/static/html/favicon.ico
+-rw-r--r--   0        0        0      306 2023-06-03 19:01:58.647142 aunly-bbot-1.4.0/aunly_bbot/website/static/html/index.html
+-rw-r--r--   0        0        0     1676 2023-06-03 19:01:58.655142 aunly-bbot-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5120 2023-06-03 19:01:58.655142 aunly-bbot-1.4.0/readme.md
+-rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.4.0/PKG-INFO
```

### Comparing `aunly-bbot-1.3.2/LICENSE` & `aunly-bbot-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/bot.py` & `aunly-bbot-1.4.0/aunly_bbot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     font_init()
 except httpx.TimeoutException:
     logger.error("获取字体超时，请手动下载后放置于（data/font）目录或稍后重试")
     sys.exit()
 logger.success("字体下载完成！")
 
 host = BotConfig.Mirai.mirai_host
-if cache.get("skip_verfiy"):
+if cache.get("skip_verify"):
     if verify_mirai(host, BotConfig.Mirai.account, BotConfig.Mirai.verify_key):
         logger.success("Mirai HTTP API 验证成功！")
     else:
         sys.exit(1)
 app_config = config(
     BotConfig.Mirai.account,
     BotConfig.Mirai.verify_key,
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/cli/__init__.py` & `aunly-bbot-1.4.0/aunly_bbot/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from ..core.announcement import PROJECT_VERSION
 
 
-@click.group(help="BBot 命令行工具")
+@click.group("BBot Cli", help="BBot 命令行工具")
 @click.version_option(
     PROJECT_VERSION,
     "-v",
     "--version",
     package_name="aunly-bbot",
     prog_name="BBot",
     message="%(prog)s 当前版本：%(version)s",
@@ -15,21 +15,22 @@
 @click.help_option("-h", "--help", help="显示帮助信息")
 def main():
     pass
 
 
 @click.command(name="run", help="运行 BBot")
 @click.option("-t", "--test", is_flag=True, help="测试模式")
-@click.option("-s", "--skip-verfiy", is_flag=True, help="跳过 MAH 可用性检查")
+@click.option("-s", "--skip-verify", is_flag=True, help="跳过 MAH 可用性检查")
 @click.option("-i", "--ignore-sub", is_flag=True, help="忽略登录模式下的账户订阅列表")
 @click.help_option("-h", "--help", help="显示帮助信息")
-def run_bot(test: bool, skip_verfiy: bool, ignore_sub: bool):
+def run_bot(test: bool, skip_verify: bool, ignore_sub: bool):
     from ..core import cache
+
     cache["test"] = test
-    cache["skip_verfiy"] = skip_verfiy
+    cache["skip_verify"] = skip_verify
     cache["ignore_sub"] = ignore_sub
 
     from .run import run_bot
 
     run_bot()
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/cli/api.py` & `aunly-bbot-1.4.0/aunly_bbot/cli/api.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/cli/config.py` & `aunly-bbot-1.4.0/aunly_bbot/cli/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
     def __init__(self) -> None:
         self.skip_verify = cache.get("skip_verify", False)
         self.mirai_mirai_host()
         self.mirai_verify_key()
         self.debug()
         self.use_browser()
-        self.bilibili_mobile_style()
         self.bilibili_concurrent()
         self.openai_summary()
         self.bilibili_username()
         self.use_bilibili_login()
         self.wordcloud()
         self.bcut_asr()
         self.event()
@@ -51,15 +50,15 @@
         self.name()
         self.access_control()
         self.master()
         self.admins()
         self.max_subscriptions()
         self.update_check()
 
-        if data.get("session", None):
+        if data.get("session"):
             httpx.post(
                 f"{self.config['Mirai']['mirai_host']}/release",
                 json={
                     "sessionKey": self.__session,
                     "qq": self.config["Mirai"]["account"],
                 },
             )
@@ -107,14 +106,20 @@
                     click.secho(
                         "Mirai HTTP API 版本低于 2.6.1，可能会导致部分功能无法使用！请注意及时升级至最新版",
                         fg="bright_red",
                         bold=True,
                     )
                 self.config["Mirai"]["mirai_host"] = mirai_host
                 return
+            except KeyError:
+                click.secho(
+                    "你输入的地址可能不是 Mirai HTTP API 的地址或 Mirai HTTP API 运行异常，请检查后重试！",
+                    fg="bright_red",
+                    bold=True,
+                )
             except httpx.HTTPError:
                 click.secho("无法连接到 Mirai HTTP API，请检查地址是否正确！", fg="bright_red", bold=True)
                 continue
 
     def mirai_verify_key(self):
         while True:
             mirai_key: str = InputPrompt(
@@ -221,14 +226,16 @@
                 "是否使用浏览器进行动态页面截图？",
                 [Choice("是（开启）"), Choice("否（关闭）")],
                 allow_filter=False,
                 default_select=1,
                 annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
             ).prompt()
             self.config["Bilibili"]["use_browser"] = browser.name == "是（开启）"
+            self.bilibili_mobile_style()
+            self.allow_fallback()
         else:
             self.config["Bilibili"]["use_browser"] = False
 
     def bilibili_mobile_style(self):
         if is_full:
             mobile_style = ListPrompt(
                 "是否在浏览器中使用手机端样式？",
@@ -236,25 +243,36 @@
                 allow_filter=False,
                 annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
             ).prompt()
             self.config["Bilibili"]["mobile_style"] = mobile_style.name == "是（开启）"
         else:
             self.config["Bilibili"]["mobile_style"] = False
 
+    def allow_fallback(self):
+        allow_fallback = ListPrompt(
+            "是否允许使用备用动态图片渲染（在浏览器截图失败时尝试使用）？",
+            [Choice("是（开启）"), Choice("否（关闭）")],
+            allow_filter=False,
+            annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
+        ).prompt()
+        self.config["Bilibili"]["allow_fallback"] = allow_fallback.name == "是（开启）"
+
     def openai_summary(self):
         openai_summary = ListPrompt(
             "是否使用 OpenAI 进行视频和专栏内容摘要提取？",
             [Choice("是（开启）"), Choice("否（关闭）")],
             allow_filter=False,
             annotation="使用键盘的 ↑ 和 ↓ 来选择, 按回车确认",
         ).prompt()
         if openai_summary.name == "是（开启）":
             self.config["Bilibili"]["openai_summarization"] = True
             self.openai_api_token()
             self.openai_model()
+        else:
+            self.config["Bilibili"]["openai_summarization"] = False
 
     def openai_api_token(self):
         openai_token = InputPrompt("请输入 OpenAI Token: ").prompt()
         if len(openai_token) != 51:
             click.secho("输入的 OpenAI Token 不合法（长度应为 51 位）", fg="bright_red", bold=True)
             self.openai_api_token()
         if openai_token.startswith("sk-"):
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/__init__.py` & `aunly-bbot-1.4.0/aunly_bbot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/announcement.py` & `aunly-bbot-1.4.0/aunly_bbot/core/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/bot_config.py` & `aunly-bbot-1.4.0/aunly_bbot/core/bot_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/control.py` & `aunly-bbot-1.4.0/aunly_bbot/core/control.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/data.py` & `aunly-bbot-1.4.0/aunly_bbot/core/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     IntegerField,
     BooleanField,
     DateTimeField,
     SqliteDatabase,
 )
 
 
-data_version = 4
+data_version = 5
 db = SqliteDatabase("data/data.db")
 
 
 class BaseModel(Model):
     class Meta:
         database = db
 
@@ -110,15 +110,18 @@
 
     version = IntegerField()
 
     class Meta:
         table_name = "data_version"
 
 
-db.create_tables([DynamicPush, GroupPush, LivePush, SubList, TalkCount, DataVersion, ContentResolveArchive], safe=True)
+db.create_tables(
+    [DynamicPush, GroupPush, LivePush, SubList, TalkCount, DataVersion, ContentResolveArchive],
+    safe=True,
+)
 
 
 if not DataVersion.select().exists():
     logger.info(f"数据库版本记录不存在，正在创建，当前版本：{data_version}")
     DataVersion(version=data_version).save()
 elif DataVersion.get().version != data_version:
     logger.info(f"数据库版本不匹配，当前当前最新版本：{data_version}，正在更新")
@@ -134,14 +137,17 @@
             db.execute_sql("ALTER TABLE sub_list ADD COLUMN live_tips VARCHAR(255) NULL")
             DataVersion.update(version=3).execute()
         elif DataVersion.get().version == 3:
             logger.info("当前数据版本为 3，正在更新至 4")
             # 在 SubList 表中添加 cover_img 字段，允许为空
             db.execute_sql("ALTER TABLE sub_list ADD COLUMN cover_img VARCHAR(255) NULL")
             DataVersion.update(version=4).execute()
+        elif DataVersion.get().version == 4:
+            logger.info("当前数据版本为 4，正在更新至 5")
+            DataVersion.update(version=5).execute()
 
     logger.success("数据库更新完成")
     time.sleep(2)
 
 
 def insert_dynamic_push(
     uid: Union[str, int],
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/group_config.py` & `aunly-bbot-1.4.0/aunly_bbot/core/group_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/log.py` & `aunly-bbot-1.4.0/aunly_bbot/core/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,53 +25,62 @@
     with contextlib.suppress(psutil.NoSuchProcess):
         for proc in psutil.Process().parents():
             if proc.name() in ["screen", "tmux", "node", "python"]:
                 return proc.name() != "node" or "vscode" not in str(proc.cmdline())
     return psutil.Process().pid == 1
 
 
-if in_screen() or is_package:
-    logger.info("检测到当前运行在各类容器中，或运行为打包（nuitka、pyinstaller）版本，已禁用 richuru")
+if in_screen() or is_package or not BotConfig.use_richuru:
+    logger.info("检测到当前运行在各类容器中、运行为打包（nuitka、pyinstaller）版本或未在配置文件中启用，已禁用 richuru")
     logger.remove(0)
-    logger.add(sys.stderr, level=log_level, backtrace=True, diagnose=True)
+    logger.add(
+        sys.stderr,
+        level=log_level,
+        backtrace=True,
+        diagnose=True,
+        filter=lambda record: (
+            "sentry_patched_callhandlers" not in record["function"]
+            or "HTTP Request" not in record["message"]
+        ),
+    )
 else:
     richuru.install(level=log_level)
 
 # add latest logger
 logger.add(
     LOGPATH.joinpath("latest.log"),
     encoding="utf-8",
     backtrace=True,
     diagnose=True,
     rotation="00:00",
-    retention="1 years",
+    retention="1 week",
     compression="tar.xz",
     level="INFO",
 )
 
 # add debug logger
 logger.add(
     LOGPATH.joinpath("debug.log"),
     encoding="utf-8",
     backtrace=True,
     diagnose=True,
     rotation="00:00",
-    retention="15 days",
+    retention="3 days",
     compression="tar.xz",
     level="DEBUG",
 )
 
 # add warning logger
 logger.add(
     LOGPATH.joinpath("warning.log"),
     encoding="utf-8",
     backtrace=True,
     diagnose=True,
     rotation="00:00",
-    retention="15 days",
+    retention="3 days",
     compression="tar.xz",
     level="WARNING",
 )
 
 logger.success(f"成功重载 logger，当前日志等级为 {log_level}")
 
 # logger.trace("TRACE 等级将会输出至控制台")
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/core/subgroup_config.py` & `aunly-bbot-1.4.0/aunly_bbot/core/subgroup_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/__init__.py` & `aunly-bbot-1.4.0/aunly_bbot/function/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 import aunly_bbot.function.event.mute
 import aunly_bbot.function.event.offline
 import aunly_bbot.function.event.new_friend
 import aunly_bbot.function.event.prem_change
 import aunly_bbot.function.pusher.init
 import aunly_bbot.function.pusher.dynamic
 import aunly_bbot.function.pusher.live
-import aunly_bbot.function.scheduler.version_update  # noqa
-
-# import function.scheduler.refresh_token  # noqa
+import aunly_bbot.function.scheduler.version_update
+import aunly_bbot.function.scheduler.refresh_token  # noqa
 
 from loguru import logger
 
 logger.success("[function] 加载完成")
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/admin/add.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/admin/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/admin/remove.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/admin/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/announcement.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/configure/atall.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/configure/atall.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/configure/nick.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/configure/nick.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 @channel.use(
     ListenerSchema(
         listening_events=[GroupMessage],
         inline_dispatchers=[
             Twilight(
                 [
                     "at" @ ElementMatch(At, optional=True),
-                    "act" @ RegexMatch(r"设定|删除"),
+                    "act" @ RegexMatch(r"添加|修改|设定|删除"),
                     RegexMatch(r"昵称|别名"),
                     "uid" @ ParamMatch(optional=True),
                     "nick" @ ParamMatch(optional=True),
                 ]
             )
         ],
         decorators=[Permission.require(Permission.GROUP_ADMIN), Interval.require()],
@@ -52,15 +52,15 @@
         if at_element.target != BotConfig.Mirai.account:
             return
 
     if uid.matched:
         uid = await uid_extract(uid.result.display, group.id)
         if uid:
             acts = act.result.display
-            if acts == "设定":
+            if acts in ["设定", "修改", "添加"]:
                 nicks = nick.result.display
                 if len(nicks) > 24:
                     msg = "昵称过长，设定失败"
                 else:
                     msg = f"{uid} 昵称设定成功" if set_nick(uid, group.id, nicks) else "该群未关注此 UP"
             else:
                 msg = f"{uid} 昵称删除成功" if set_nick(uid, group.id, None) else "该群未关注此 UP"
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/content_resolve.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/content_resolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,62 +17,38 @@
 
 from ...core.bot_config import BotConfig
 from ...model.exception import AbortError
 from ...utils.column_resolve import get_cv
 from ...core.data import ContentResolveData
 from ...core.control import Interval, Permission
 from ...utils.video_subtitle import get_subtitle
-from ...utils.message_resolve import message_resolve
+from ...utils.bilibili_parse import extract_bilibili_info
 from ...utils.draw_bili_image import binfo_image_create
 from ...utils.text2image import rich_text2image, browser_text2image
 from ...utils.bilibili_request import get_b23_url, grpc_get_view_info
 from ...utils.content_summarise import column_summarise, subtitle_summarise
 
 channel = Channel.current()
 
 
 @channel.use(ListenerSchema(listening_events=[GroupMessage], decorators=[Permission.require()]))
 async def main(
     app: Ariadne, group: Group, member: Member, message: MessageChain, source: Source
 ):
-    bili_number = await message_resolve(message)
+    bili_number = await extract_bilibili_info(message)
     if not bili_number:
         return
 
     if bili_number[:2] in ["BV", "bv", "av"]:
         try:
-            if (video_info := await video_info_get(bili_number)) is None:
-                await Interval.manual(group.id, 5)
-                return
-            elif video_info.ecode == 1:
-                await app.send_group_message(
-                    group, MessageChain(f"未找到视频 {bili_number}，可能已被 UP 主删除。"), quote=source
-                )
-                return
-        except (AioRpcError, GrpcError) as e:
+            aid, cid, bvid, title, video_info = await extract_video_info(bili_number)
+        except AbortError as e:
             await Interval.manual(group.id, 5)
-            logger.exception(e)
-            return await app.send_group_message(
-                group, MessageChain(f"{bili_number} 视频信息获取失败，错误信息：{type(e)} {e}"), quote=source
-            )
-        except Exception as e:
-            capture_exception()
-            await Interval.manual(group.id, 5)
-            logger.exception(e)
-            return await app.send_group_message(
-                group, MessageChain(f"{bili_number} 视频信息解析失败，错误信息：{type(e)} {e}"), quote=source
-            )
-        aid = video_info.activity_season.arc.aid or video_info.arc.aid
-        cid = (
-            video_info.activity_season.pages[0].page.cid
-            if video_info.activity_season.pages
-            else video_info.pages[0].page.cid
-        )
-        bvid = video_info.activity_season.bvid or video_info.bvid
-        title = video_info.activity_season.arc.title or video_info.arc.title
+            return await app.send_group_message(group, MessageChain(e.message), quote=source)
+
         archive_data = ContentResolveData(aid=aid)
         archive_data.title = title
         await Interval.manual(aid + group.id, 30)
         try:
             logger.info(f"开始生成视频信息图片：{aid}")
             b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
             image = await binfo_image_create(video_info, b23_url)
@@ -106,43 +82,46 @@
                         try:
                             if archive_data.openai:
                                 logger.info(f"{aid} 已存在总结缓存，跳过总结请求")
                                 summarise = archive_data.openai
                             else:
                                 logger.info(f"{aid} 总结不存在，正在尝试请求......")
                                 try:
-                                    await Interval.manual(member, 600)
+                                    if (
+                                        BotConfig.Bilibili.openai_whitelist_users
+                                        and member.id
+                                        not in BotConfig.Bilibili.openai_whitelist_users
+                                    ):
+                                        await Interval.manual(
+                                            member, BotConfig.Bilibili.openai_cooldown
+                                        )
                                 except ExecutionStop:
                                     msg = f"{member.id} 在 10 分钟内已经请求过总结，跳过本次请求"
                                     logger.info(msg)
                                     raise AbortError(msg)
                                 ai_summary = await subtitle_summarise(subtitle, title)
-                                if ai_summary.summary:
-                                    summarise = ai_summary.summary
+                                if ai_summary.response:
+                                    summarise = ai_summary.response
                                     archive_data.openai = summarise
                                 else:
                                     logger.warning(f"视频 {aid} 总结失败：{ai_summary.raw}")
                                     return
 
-                            if "no meaning" in summarise.lower():
+                            if "no meaning" in summarise.lower() or len(summarise) < 20:
                                 nonlocal chatgpt_thinks
                                 chatgpt_thinks = False
                                 raise AbortError("ChatGPT 认为这些字幕没有意义")
 
                             logger.debug(summarise)
                             if BotConfig.Bilibili.use_browser:
                                 image = await browser_text2image(summarise)
                             else:
                                 image = await rich_text2image(summarise)
                             if image:
-                                await app.send_group_message(
-                                    group,
-                                    MessageChain(Image(data_bytes=image)),
-                                    quote=info_message.source,
-                                )
+                                images.append(image)
                         except AbortError as e:
                             logger.warning(f"视频 {aid} 总结被终止：{e}")
                         except Exception:
                             capture_exception()
                             logger.exception(f"视频 {aid} 总结出错")
 
                     async def wordcloud():
@@ -160,34 +139,39 @@
                                 )
                                 archive_data.jieba = json.dumps(
                                     word_frequencies, ensure_ascii=False
                                 )
 
                             wordcloud = await get_worldcloud_image(word_frequencies)
                             if wordcloud:
-                                await app.send_group_message(
-                                    group,
-                                    MessageChain(Image(data_bytes=wordcloud)),
-                                    quote=info_message.source,
-                                )
+                                images.append(wordcloud)
                         except Exception:
                             capture_exception()
                             logger.exception(f"视频 {aid} 词云出错")
 
+                    images = []
                     if BotConfig.Bilibili.openai_summarization:
                         await openai_summarization()
                     if BotConfig.Bilibili.use_wordcloud and chatgpt_thinks:
                         await wordcloud()
 
+                    if images:
+                        await app.send_group_message(
+                            group,
+                            MessageChain([Image(data_bytes=x) for x in images]),
+                            quote=info_message.source,
+                        )
+
                 except AbortError as e:
                     logger.warning(f"视频 {aid} 总结失败：{e.message}")
                     return
                 archive_data.save()
 
         except TimeoutException:
+            logger.exception(f"视频 {aid} 信息生成超时")
             await app.send_group_message(
                 group, MessageChain(f"{bili_number} 视频信息生成超时，请稍后再试。"), quote=source
             )
         except Exception as e:
             capture_exception()
             logger.exception("视频解析 API 调用出错")
             await app.send_group_message(
@@ -209,16 +193,16 @@
 
                 async def openai_summarization():
                     try:
                         if archive_data.openai:
                             summarise = archive_data.openai
                         else:
                             ai_summary = await column_summarise(cv_title, cv_text)
-                            if ai_summary.summary:
-                                summarise = ai_summary.summary
+                            if ai_summary.response:
+                                summarise = ai_summary.response
                                 archive_data.openai = summarise
                             else:
                                 return
 
                         if BotConfig.Bilibili.use_browser:
                             image = await browser_text2image(summarise)
                         else:
@@ -278,7 +262,33 @@
 
 
 async def video_info_get(vid_id: str):
     if vid_id[:2].lower() == "av":
         aid = int(vid_id[2:])
         return await grpc_get_view_info(aid=aid) if aid > 1 else None
     return await grpc_get_view_info(bvid=vid_id)
+
+
+async def extract_video_info(bili_number: str):
+    try:
+        if (video_info := await video_info_get(bili_number)) is None:
+            raise AbortError(f"无法获取视频 {bili_number}。")
+        elif video_info.ecode == 1:
+            raise AbortError(f"未找到视频 {bili_number}，可能已被 UP 主删除。")
+    except (AioRpcError, GrpcError) as e:
+        logger.exception(e)
+        raise AbortError(f"{bili_number} 视频信息获取失败，错误信息：{type(e)} {e}")
+    except Exception as e:
+        capture_exception()
+        logger.exception(e)
+        raise AbortError(f"{bili_number} 视频信息解析失败，错误信息：{type(e)} {e}")
+
+    aid = video_info.activity_season.arc.aid or video_info.arc.aid
+    cid = (
+        video_info.activity_season.pages[0].page.cid
+        if video_info.activity_season.pages
+        else video_info.pages[0].page.cid
+    )
+    bvid = video_info.activity_season.bvid or video_info.bvid
+    title = video_info.activity_season.arc.title or video_info.arc.title
+
+    return aid, cid, bvid, title, video_info
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/init.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/menu/__init__.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/menu/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 channel = Channel.current()
 menu_image = None
 help_text = (
     "BBot 功能菜单：\n"
     "=================================================================\n"
     " 0. /quit\n"
-    " 1. BiliBili 视频解析\n"
+    " 1. BiliBili 视频、专栏内容解析，支持 OpenAI 总结\n"
     " 2. 查看关注列表\n"
     f" 3. @{BotConfig.name} 关注 <uid>\n    > @{BotConfig.name} (订阅|关注)(主播|[uU][pP])?\n"
     f" 4. @{BotConfig.name} 取关 <uid>\n    > @{BotConfig.name} (退订|取消?关注?)\\s?(主播|[uU][pP])?\n"
     " 5. 查看动态 <uid> <offset>\n    > offset 可以填写数字，用来代表该 UP 的倒数第几条动态\n"
     " 6. 设定|删除 昵称 <uid> [昵称]\n"
     " 7. 开启|关闭 @全体成员 <uid>\n"
     "=================================================================\n"
@@ -41,15 +41,15 @@
 @channel.use(
     ListenerSchema(
         listening_events=[GroupMessage],
         inline_dispatchers=[
             Twilight(
                 [
                     "at" @ ElementMatch(At, optional=True),
-                    RegexMatch("([/.。?？!！])?(帮助|菜单|功能|help|menu)([/.。?？!！])?"),
+                    RegexMatch(r"([/.。?？!！])?(帮助|菜单|功能|help|menu)([/.。?？!！])?"),
                 ]
             )
         ],
         decorators=[Permission.require(), Interval.require()],
         priority=15,
     )
 )
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/quit_group.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/quit_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/status.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/status.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/add.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/add_up.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/add_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/get_subgroup.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/get_subgroup.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/remove.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/subgroup/remove_up.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/subgroup/remove_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/up/get_subscribe.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/up/get_subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/up/subscribe.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/up/subscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/up/unsubscribe.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/up/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/vip/add.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/vip/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/vip/remove.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/vip/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/vive_dynamic.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/vive_dynamic.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/web_auth.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/web_auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/add.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/close.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/close.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/open.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/open.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/command/whitelist/remove.py` & `aunly-bbot-1.4.0/aunly_bbot/function/command/whitelist/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/bot_launch.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/bot_launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                 BotConfig.master, MessageChain(f"检测到新版本：{new_version} > {old_version}")
             )
         else:
             logger.success("[版本更新] 当前版本为最新版本")
 
     if is_full and BotConfig.Bilibili.use_browser:
         from graiax.playwright.interface import PlaywrightContext
+
         try:
             logger.info("[Playwright] 正在获取浏览器版本")
             browser_context = app.launch_manager.get_interface(PlaywrightContext)
             if not BotConfig.Bilibili.mobile_style:
                 await browser_context.context.add_cookies(
                     [
                         {
@@ -68,14 +69,16 @@
         except Exception as e:
             logger.error(f"[BiliBili推送] 获取首页 Cookie 失败 {e}，正在重试")
             await asyncio.sleep(2)
     else:
         logger.error("[BiliBili推送] 获取首页 Cookie 失败，已达最大重试次数")
         sys.exit(1)
 
+    logger.info(f"[BiliBili推送] 获取首页 Cookie 成功，{hc.cookies}")
+
     logger.info("Graia 成功启动")
     group_list = await app.get_group_list()
     group_num = len(group_list)
     master = await app.get_friend(BotConfig.master)
     if not master:
         logger.error(f"当前未添加主人好友（{BotConfig.master}），请手动添加")
         sys.exit(1)
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/exception.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/exception.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/invited_join_group.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/invited_join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/join_group.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/leave_group.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/leave_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/mute.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/mute.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/new_friend.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/new_friend.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/offline.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/offline.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/event/prem_change.py` & `aunly-bbot-1.4.0/aunly_bbot/function/event/prem_change.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/pusher/dynamic.py` & `aunly-bbot-1.4.0/aunly_bbot/function/pusher/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,21 +276,26 @@
                 except AccountMuted:
                     group = await app.get_group(int(data.group))
                     group = f"{group.name}（{group.id}）" if group else data.group
                     logger.warning(
                         f"[BiliBili推送] {dynid} | {up_name}({up_id}) 推送失败，账号在 {group} 被禁言"
                     )
                 except RemoteException as e:
-                    if "resultType=46" in str(e):
+                    if "LIMITED_MESSAGING" in str(e):
                         logger.error(
                             f"[BiliBili推送] {dynid} | {up_name}({up_id}) 推送失败，Bot 被限制发送群聊消息"
                         )
                         await app.send_friend_message(
                             BotConfig.master,
-                            MessageChain("Bot 被限制发送群聊消息（46 代码），请尽快处理后发送 /init 重新开启推送进程"),
+                            MessageChain(
+                                "Bot 被限制发送群聊消息（46 代码），问题原因可能是账号被多次举报或被服务器认为不安全. "
+                                "若账号在官方客户端也无法发出消息, 可尝试用手机 QQ 登录后访问 "
+                                "https://accounts.qq.com/safe/message/unlock?lock_info=5_5 解冻。"
+                                "请尽快处理后发送 /init 重新开启推送进程"
+                            ),
                         )
                         BOT_Status.set_status(Status.DYNAMIC_IDLE, True)
                         BOT_Status.set_status(Status.INITIALIZED, False)
                         raise ExecutionStop() from e
                     elif "resultType=110" in str(e):  # 110: 可能为群被封
                         logger.warning(
                             f"[BiliBili推送] {dynid} | {up_name}({up_id}) 推送失败，Bot 因未知原因被移出群聊"
@@ -334,16 +339,18 @@
 
 async def check_uid(app: Ariadne, uid):
     try:
         resp = await asyncio.wait_for(grpc_get_user_dynamics(int(uid)), timeout=10)
     except asyncio.TimeoutError:
         logger.warning(f"[BiliBili推送] {uid} 获取动态超时！")
         return
-    except GrpcError as e:
-        logger.error(f"[BiliBili推送] {uid} 获取动态失败：[{e.code}] {e.msg}")
+    except (GrpcError, AioRpcError) as e:
+        logger.error(
+            f"[BiliBili推送] {uid} 获取动态失败：[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
+        )
         return
     except Exception as e:  # noqa
         capture_exception(e)
         raise e
     if resp:
         resp = [
             x
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/pusher/init.py` & `aunly-bbot-1.4.0/aunly_bbot/function/pusher/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/pusher/live.py` & `aunly-bbot-1.4.0/aunly_bbot/function/pusher/live.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                             nick = (
                                 f"*{up_nick} "
                                 if (up_nick := data.nick)
                                 else f"UP {up_name}（{up_id}）"
                             )
                             msg = [
                                 f"{nick}在 {room_area} 区开播啦 ！\n标题：{title}\n",
-                                cover_img,
+                                cover_img or "",
                                 "\n" if cover_img else "",
                                 await get_b23_url(f"https://live.bilibili.com/{room_id}"),
                             ]
 
                             if data.atall:  # 判断是否开启@全体推送
                                 bot_perm = group.account_perm if group else MemberPerm.Member
                                 if bot_perm in [
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/scheduler/refresh_token.py` & `aunly-bbot-1.4.0/aunly_bbot/function/scheduler/refresh_token.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/function/scheduler/version_update.py` & `aunly-bbot-1.4.0/aunly_bbot/function/scheduler/version_update.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/model/bcut_asr.py` & `aunly-bbot-1.4.0/aunly_bbot/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/model/config.py` & `aunly-bbot-1.4.0/aunly_bbot/model/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,22 +46,26 @@
 
 
 class _Bilibili(BaseModel, extra=Extra.ignore):
     username: Optional[int]
     password: Optional[str]
     use_login: bool = False
     use_browser: bool = True
+    allow_fallback: bool = True
     mobile_style: bool = True
     concurrency: int = 5
     dynamic_font: str = "HarmonyOS_Sans_SC_Medium.ttf"
     dynamic_font_source: Literal["local", "remote"] = "local"
     openai_summarization: bool = False
     openai_api_token: Optional[str] = None
     openai_model: str = "gpt-3.5-turbo"
     openai_proxy: Optional[AnyHttpUrl] = None
+    openai_cooldown: int = 60
+    openai_whitelist_users: Optional[list[int]] = None
+    openai_promot_version: int = 2
     use_wordcloud: bool = False
     use_bcut_asr: bool = False
     asr_length_threshold: int = 60
 
     # 验证是否可以登录
     @validator("use_login", always=True)
     def can_use_login(cls, use_login, values):
@@ -98,14 +102,22 @@
             import wordcloud  # noqa  # type: ignore
 
             return use_wordcloud
         except ImportError:
             click.secho("未安装 wordcloud，如需使用词云，请安装 wordcloud", fg="bright_red")
             sys.exit()
 
+    # 验证 openai promt version
+    @validator("openai_promot_version")
+    def valid_openai_promot_version(cls, openai_promot_version):
+        if openai_promot_version in [1, 2]:
+            return openai_promot_version
+        click.secho("openai_promot_version 只能为 1 或 2", fg="bright_yellow")
+        sys.exit()
+
     # 验证 Bilibili gRPC 并发数
     @validator("concurrency")
     def limit_concurrency(cls, concurrency):
         if concurrency > 50:
             click.secho("gRPC 并发数超过 50，已自动调整为 50", fg="bright_yellow")
             return 50
         elif concurrency < 1:
@@ -137,14 +149,15 @@
     log_level: str = "INFO"
     name: str = "BBot"
     master: int = 123
     admins: Optional[list[int]]
     max_subsubscribe: int = 4
     access_control: bool = True
     update_check: bool = True
+    use_richuru: bool = True
 
     # 验证 admins 列表
     @validator("admins")
     def verify_admins(cls, admins, values):
         if type(admins) == int:
             click.secho("admins 格式为 int, 已重置为 list[admins]", fg="bright_yellow")
             admins = [admins]
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/model/fastapi.py` & `aunly-bbot-1.4.0/aunly_bbot/model/fastapi.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/static/bot_config.exp.yaml` & `aunly-bbot-1.4.0/aunly_bbot/static/bot_config.exp.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 # 警告: 在 bot 第一次成功运行后配置文件将会被规范化, 此文件中的注释均会被清除,
 # 并且配置项顺序可能会出现变动, 若需要查看配置项的详细信息可参考配置文档
 # https://github.com/djkcyl/BBot-Graia/wiki/fill-config
 
 Mirai:
-  mirai_host: https://localhost:8080  # **需要** 填入 mirai-api-http 的监听地址
-  verify_key: xxxxxxxxx               # **需要** 填入 mirai 的密钥
-  account: 123456789                  # **需要** 填入 bot 的 qq 号
+  mirai_host: https://localhost:8080      # **需要** 填入 mirai-api-http 的监听地址
+  verify_key: xxxxxxxxx                   # **需要** 填入 mirai 的密钥
+  account: 123456789                      # **需要** 填入 bot 的 qq 号
 Debug:
-  enable: false      # 是否开启 debug
-  groups:            # 若开启 debug 则 **需要** 填入群号, list 里填 int
+  enable: false                           # 是否开启 debug
+  groups:                                 # 若开启 debug 则 **需要** 填入群号, list 里填 int
     - 123456789
 Bilibili:
-  mobile_style: true # 是否采用手机的 Web 样式进行截图
-  use_login: false   # 是否使用登录的 BiliBili 账号进行动态监听（不要开）
-  username:          # BiliBili 账号，若填写则会在启动后自动登录，并且用于部分功能，如 AI 字幕
-  password:          # BiliBili 密码
-  concurrency: 5     # 未登录时发送 gRPC 请求的并发数量(1 ~ 50)
+  mobile_style: true                      # 是否采用手机的 Web 样式进行截图
+  use_login: false                        # 是否使用登录的 BiliBili 账号进行动态监听（没事不建议开）
+  use_browser: true                       # 是否使用浏览器进行动态截图
+  allow_fallback: true                    # 是否允许使用截图失败后的备用方案（PIL）渲染动态
+  username:                               # BiliBili 账号，若填写则会在启动后自动登录，并且用于部分功能，如 AI 字幕
+  password:                               # BiliBili 密码
+  concurrency: 5                          # 未登录时发送 gRPC 请求的并发数量(1 ~ 50)
   dynamic_font: "HarmonyOS_Sans_SC_Medium.ttf" # 自定义动态字体
-  dynamic_font_source: "local"            # 自定义动态字体来源, 可选值: "local", "remote", "system", 为 "local" 时请将字体文件放在 data/font 目录下
+  dynamic_font_source: "local"            # 自定义动态字体来源, 可选值: "local", "remote", 为 "local" 时请将字体文件放在 data/font 目录下
   openai_summarization: false             # 是否使用 OpenAI 进行视频和专栏的 AI 总结
   openai_api_token: "sk-xxxxxxxxxxxxxx"   # OpenAI API Token
   openai_model: "gpt-3.5-turbo-0301"      # OpenAI 模型
   openai_proxy: "http://localhost:7890"   # 请求 OpenAI 所用的代理
+  openai_cooldown: 60                     # OpenAI 调用冷却时间（秒）
+  openai_whitelist_users: []              # OpenAI 调用冷却白名单用户（即使在冷却时间内也可以调用）
+  openai_promot_version: 2                # OpenAI 提示词版本，当前可选值: 1, 2
   use_wordcloud: true                     # 是否使用词云
-  use_bcut_asr: true                      # 是否使用 BCut 进行 AI 语音识别
+  use_bcut_asr: true                      # 是否使用 BCut 接口进行 AI 语音识别
   asr_length_threshold: 60                # 调用语音识别的最小长度阈值（秒）
 Event:
-  mute: true         # 是否向管理员发送被禁言的事件提醒。
-  permchange: true   # 是否向管理员发送权限变更的事件提醒。
-  push: true         # 是否向管理员发送推送的事件提醒。
-  subscribe: true    # 是否向管理员发送订阅的事件提醒。
+  mute: true                              # 是否向管理员发送被禁言的事件提醒。
+  permchange: true                        # 是否向管理员发送权限变更的事件提醒。
+  push: true                              # 是否向管理员发送推送的事件提醒。
+  subscribe: true                         # 是否向管理员发送订阅的事件提醒。
 Webui:
-  webui_host: "0.0.0.0"
-  webui_port: 6080
-  webui_enable: true
-log_level: INFO      # 控制台输出的日志等级
-name: BBot           # bot 的自称
-access_control: true # 是否开启白名单模式
-master: 123456789    # **需要** 填入 bot 主人的 qq 号
-admins:              # 可以填入 bot 管理员的 qq 号, list 里填 int
+  webui_host: "0.0.0.0"                   # WebUI 监听地址
+  webui_port: 6080                        # WebUI 监听端口
+  webui_enable: true                      # 是否开启 WebUI
+log_level: INFO                           # 控制台输出的日志等级
+name: BBot                                # bot 的自称
+access_control: true                      # 是否开启白名单模式
+master: 123456789                         # **需要** 填入 bot 主人的 qq 号
+admins:                                   # 可以填入 bot 管理员的 qq 号, list 里填 int
   - 123456789
-max_subsubscribe: 4  # 非 vip 群聊最大可订阅数量
-update_check: true   # 是否检查更新
+max_subsubscribe: 4                       # 非 vip 群聊最大可订阅数量
+update_check: true                        # 是否检查更新
+use_richuru: true                         # 是否使用 Richuru Log
 
 # 警告: 在 bot 第一次成功运行后配置文件将会被规范化, 此文件中的注释均会被清除, 
 # 并且配置项顺序可能会出现变动, 若需要查看配置项的详细信息可参考配置文档
 # https://github.com/djkcyl/BBot-Graia/wiki/fill-config
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/static/mobile_style.js` & `aunly-bbot-1.4.0/aunly_bbot/static/mobile_style.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/static/mobile_style_bak.js` & `aunly-bbot-1.4.0/aunly_bbot/static/mobile_style_bak.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/test.py` & `aunly-bbot-1.4.0/aunly_bbot/test.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/b23_extract.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/b23_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/bcut_asr.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/bilibili_request.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/bilibili_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,32 @@
 from bilireq.grpc.utils import grpc_request
 from bilireq.grpc.dynamic import grpc_get_followed_dynamics
 from bilireq.grpc.protos.bilibili.app.view.v1.view_pb2_grpc import ViewStub
 from bilireq.grpc.protos.bilibili.app.view.v1.view_pb2 import ViewReq, ViewReply
 from bilireq.grpc.protos.bilibili.community.service.dm.v1.dm_pb2_grpc import DMStub
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2_grpc import DynamicStub
 from bilireq.grpc.protos.bilibili.app.playurl.v1.playurl_pb2_grpc import PlayURLStub
-from bilireq.grpc.protos.bilibili.community.service.dm.v1.dm_pb2 import DmViewReq, DmViewReply
 from bilireq.grpc.protos.bilibili.app.playurl.v1.playurl_pb2 import PlayViewReq, PlayViewReply
+from bilireq.grpc.protos.bilibili.community.service.dm.v1.dm_pb2 import DmViewReq, DmViewReply
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import (
     DynamicType,
     DynDetailsReq,
     DynDetailsReply,
 )
 
 from ..core import Bili_Auth
 
-hc = httpx.AsyncClient()
+hc = httpx.AsyncClient(
+    headers={
+        "User-Agent": (
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
+            "(KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.39"
+        )
+    }
+)
 
 
 async def relation_modify(uid: Union[str, int], act: int):
     """
     修改关系
 
     Args:
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/browser_shot.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/browser_shot.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 
 
 async def fill_font(route: Route, request: Request):
     url = URL(request.url)
     if not url.is_absolute():
         raise ValueError("字体地址不合法")
     try:
-        logger.debug(f"Font {url.name} requested")
+        logger.debug(f"Font {url.query['name']} requested")
         await route.fulfill(
             path=await get_font(url.query["name"]),
-            content_type=font_mime_map.get(url.suffix, None),
+            content_type=font_mime_map.get(url.suffix),
         )
         return
     except Exception:
-        logger.error(f"找不到字体 {url.name}")
+        logger.error(f"找不到字体 {url.query['name']}")
         await route.fallback()
 
 
 async def browser_dynamic(dynid: str):
     app = Ariadne.current()
     browser_context = app.launch_manager.get_interface(PlaywrightContext).context
     return await screenshot(dynid, browser_context)
@@ -62,15 +62,18 @@
             if log:
                 page.on("requestfinished", network_request)
             page.on("requestfailed", network_requestfailed)
             if BotConfig.Bilibili.mobile_style:
                 page, clip = await get_mobile_screenshot(page, dynid)
             else:
                 page, clip = await get_pc_screenshot(page, dynid)
+            clip["height"] = min(clip["height"], 32766)  # 限制高度
             return await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98)
+        except TimeoutError:
+            logger.error(f"[BiliBili推送] {dynid} 动态截图超时，正在重试：")
         except Notfound:
             logger.error(f"[Bilibili推送] {dynid} 动态不存在")
         except AssertionError:
             logger.exception(f"[BiliBili推送] {dynid} 动态截图失败，正在重试：")
             await page.screenshot(
                 path=f"{error_path}/{dynid}_{i}_{st}.jpg",
                 full_page=True,
@@ -82,20 +85,23 @@
                 logger.error(f"[Bilibili推送] {dynid} 动态不存在")
                 break
             elif "waiting until" in str(e):
                 logger.error(f"[BiliBili推送] {dynid} 动态截图超时，正在重试：")
             else:
                 capture_exception()
                 logger.exception(f"[BiliBili推送] {dynid} 动态截图失败，正在重试：")
-                await page.screenshot(
-                    path=f"{error_path}/{dynid}_{i}_{st}.jpg",
-                    full_page=True,
-                    type="jpeg",
-                    quality=80,
-                )
+                try:
+                    await page.screenshot(
+                        path=f"{error_path}/{dynid}_{i}_{st}.jpg",
+                        full_page=True,
+                        type="jpeg",
+                        quality=80,
+                    )
+                except Exception:
+                    logger.exception(f"[BiliBili推送] {dynid} 动态截图失败：")
         finally:
             with contextlib.suppress():
                 await page.close()
 
 
 async def network_request(request: Request):
     url = request.url
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/column_resolve.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/column_resolve.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 
 from .bilibili_request import hc
 
 XPATH = "//p//text() | //h1/text() | //h2/text() | //h3/text() | //h4/text() | //h5/text() | //h6/text()"
 
 
 async def get_cv(cvid: str) -> tuple[str, str]:
-    cv = await hc.get(f"https://www.bilibili.com/read/cv{cvid}")
+    cv = await hc.get(f"https://www.bilibili.com/read/cv{cvid}", follow_redirects=True)
     if cv.status_code != 200:
         raise AbortError("专栏获取失败")
+    elif cv.url != f"https://www.bilibili.com/read/cv{cvid}":
+        if cv.url == "https://www.bilibili.com/read/error":
+            raise AbortError("专栏不存在")
+        else:
+            raise AbortError("专栏获取失败")
     cv.encoding = "utf-8"
     cv = cv.text
 
     http_parser: _Element = etree.fromstring(cv, etree.HTMLParser(encoding="utf-8"))
     title: str = http_parser.xpath('//h1[@class="title"]/text()')[0]
     main_article: _Element = http_parser.xpath('//div[@id="read-article-holder"]')[0]
     plist: _ElementUnicodeResult = main_article.xpath(XPATH)
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/detect_package.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/detect_package.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/draw_bili_image.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/fonts_provider.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/openai.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/openai.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,34 +2,62 @@
 import random
 import asyncio
 import tiktoken_async
 
 from loguru import logger
 from typing import Optional
 from collections import OrderedDict
+from httpx import HTTPError, Response
 
-from ..model.openai import AISummary
 from ..core.bot_config import BotConfig
+from ..model.openai import OpenAI, TokenUsage
 
 LIMIT_COUNT = {"gpt-3.5-turbo-0301": 3500, "gpt-4-0314": 7600, "gpt-4-32k-0314": 32200}.get(
     BotConfig.Bilibili.openai_model or "gpt-3.5-turbo-0301", 3500
 )
 
 if BotConfig.Bilibili.openai_summarization:
     logger.info("正在加载 OpenAI Token 计算模型")
     tiktoken_enc = asyncio.run(
         tiktoken_async.encoding_for_model(BotConfig.Bilibili.openai_model)
     )
     logger.info(f"{tiktoken_enc.name} 加载成功")
 
 
-def get_user_prompt(title: str, transcript: str) -> str:
+def get_summarise_prompt(title: str, transcript: str) -> list[dict[str, str]]:
     title = title.replace("\n", " ").strip() if title else ""
     transcript = transcript.replace("\n", " ").strip() if transcript else ""
-    return f'Title: "{title}"\nTranscript: "{transcript}"'
+    if BotConfig.Bilibili.openai_promot_version == 1:
+        language = "Chinese"
+        sys_prompt = (
+            "Your output should use the following template:\n## Summary\n## Highlights\n"
+            "- [Emoji] Bulletpoint\n\n"
+            "Your task is to summarise the video I have given you in up to 2 to 6 concise bullet points. "
+            "First, use a simple sentence to summarize, each bullet point is at least 15 words. "
+            "Choose an appropriate emoji for each bullet point. "
+            "Use the video above: {{Title}} {{Transcript}}."
+            "\nIf you think that the content in the transcript is meaningless, "
+            "Or if there is very little content that cannot be well summarized, "
+            "then you can simply output the two words 'no meaning'. Remember, not to output anything else."
+        )
+        return get_full_prompt(
+            f'Title: "{title}"\nTranscript: "{transcript}"', sys_prompt, language
+        )
+    return get_full_prompt(
+        prompt=(
+            "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
+            "\n## 概述"
+            "\n{内容，尽可能精简总结内容不要太详细}"
+            "\n## 要点"
+            "\n- {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}"
+            "\n不要随意翻译任何内容。仅使用中文总结。"
+            "\n不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
+            f"\n视频标题名称为“{title}”，视频字幕数据如下，立刻开始总结：“{transcript}”"
+        )
+    )
 
 
 def count_tokens(prompts: list[dict[str, str]]):
     """根据内容计算 token 数"""
 
     if BotConfig.Bilibili.openai_model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4
@@ -49,66 +77,74 @@
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
 def get_small_size_transcripts(text_data: list[str], token_limit: int = LIMIT_COUNT):
     unique_texts = list(OrderedDict.fromkeys(text_data))
-    while (
-        count_tokens(
-            get_full_prompt(get_user_prompt("", " ".join(unique_texts)), system=True)
-        )
-        > token_limit
-    ):
+    while count_tokens(get_summarise_prompt("", " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
-def get_full_prompt(prompt: str, system: bool = False):
+def get_full_prompt(
+    prompt: Optional[str] = None, system: Optional[str] = None, language: Optional[str] = None
+):
     plist: list[dict[str, str]] = []
     if system:
-        language = "Chinese"
-        sys_prompt = (
-            "Your output should use the following template:\n## Summary\n## Highlights\n"
-            "- [Emoji] Bulletpoint\n\n"
-            "Your task is to summarise the video I have given you in up to 2 to 6 concise bullet points, "
-            "starting with a short highlight, each bullet point is at least 15 words. "
-            "Choose an appropriate emoji for each bullet point. "
-            f"Use the video above: {{Title}} {{Transcript}}."
-            "If you think that the content in the transcript is meaningless, "
-            "Or if there is very little content that cannot be well summarized, "
-            "then you can simply output the three words 'no meaning' Remember not to output anything else."
-            f"\n\nReply in {language} Language."
+        plist.append({"role": "system", "content": system})
+    if prompt:
+        plist.append({"role": "user", "content": prompt})
+    if language:
+        plist.extend(
+            (
+                {
+                    "role": "assistant",
+                    "content": "What language do you want to output?",
+                },
+                {"role": "user", "content": language},
+            )
         )
-        plist.append({"role": "system", "content": sys_prompt})
-    plist.append({"role": "user", "content": prompt})
+    if not plist:
+        raise ValueError("No prompt provided")
     return plist
 
 
 async def openai_req(
     prompt_message: list[dict[str, str]],
     token: Optional[str] = BotConfig.Bilibili.openai_api_token,
     model: str = BotConfig.Bilibili.openai_model,
-) -> AISummary:
+    temperature: Optional[float] = None,
+) -> OpenAI:
     if not token:
-        return AISummary(error=True, message="未配置 OpenAI API Token")
+        return OpenAI(error=True, message="未配置 OpenAI API Token")
     async with httpx.AsyncClient(
         proxies=BotConfig.Bilibili.openai_proxy,
         headers={
             "Authorization": f"Bearer {token}",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)"
             " Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.69",
         },
         timeout=100,
     ) as client:
-        req = await client.post(
-            "https://api.openai.com/v1/chat/completions",
-            json={
-                "model": model,
-                "messages": prompt_message,
-            },
-        )
+        data = {
+            "model": model,
+            "messages": prompt_message,
+        }
+        if temperature:
+            data["temperature"] = temperature
+        try:
+            req: Response = await client.post(
+                "https://api.openai.com/v1/chat/completions", json=data
+            )
+        except HTTPError as e:
+            return OpenAI(error=True, message=f"OpenAI 请求失败 {type(e)} {e}")
         if req.status_code != 200:
-            return AISummary(error=True, message=req.text, raw=req.json())
-        logger.info(f"[OpenAI] Response: {req.json()['choices'][0]['message']['content']}")
-        logger.info(f"[OpenAI] Response token 实际: {req.json()['usage']}")
-        return AISummary(summary=req.json()["choices"][0]["message"]["content"], raw=req.json())
+            return OpenAI(error=True, message=req.text, raw=req.json())
+        logger.info(f"[OpenAI] Response:\n{req.json()['choices'][0]['message']['content']}")
+        usage = req.json()["usage"]
+        logger.info(f"[OpenAI] Response 实际 token 消耗: {usage}")
+        return OpenAI(
+            response=req.json()["choices"][0]["message"]["content"],
+            raw=req.json(),
+            token_usage=TokenUsage(**usage),
+        )
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/pil_shot.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/pil_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/send_action.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/send_action.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/strings.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/strings.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/text2image.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/text2image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/time_tools.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/uid_extract.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/uid_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/up_operation.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/up_operation.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/update_version.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/update_version.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/verify_mah.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/verify_mah.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/video_subtitle.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/video_subtitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import httpx
 import asyncio
 
 from loguru import logger
 from typing import Optional
+from httpx import TimeoutException
 from sentry_sdk import capture_exception
 
 from ..core.bot_config import BotConfig
 from ..model.exception import AbortError
 from ..model.bcut_asr import ResultStateEnum
 
 from .bcut_asr import BcutASR
@@ -67,14 +68,17 @@
                 if playview.video_info.dash_audio[-1].backup_url
                 else playview.video_info.dash_audio[-1].baseUrl,
             )
         audio_resp.raise_for_status()
         audio = audio_resp.content
         try:
             asr = await get_bcut_asr(audio)
+        except TimeoutException as e:
+            logger.error("BCut-ASR 连接超时")
+            raise AbortError("BCut-ASR 连接超时") from e
         except Exception as e:
             logger.exception("BCut-ASR 识别失败")
             capture_exception()
             raise AbortError("BCut-ASR 识别失败") from e
         return [x.transcript for x in asr]
     else:
         raise AbortError("未找到字幕且未开启 AI 语音识别")
```

### Comparing `aunly-bbot-1.3.2/aunly_bbot/utils/wordcloud.py` & `aunly-bbot-1.4.0/aunly_bbot/utils/wordcloud.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/__init__.py` & `aunly-bbot-1.4.0/aunly_bbot/website/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/auth.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/config.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/follow.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/follow.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/home.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/home.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/user.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/user.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/api/router/ws.py` & `aunly-bbot-1.4.0/aunly_bbot/website/api/router/ws.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/aunly_bbot/website/static/html/favicon.ico` & `aunly-bbot-1.4.0/aunly_bbot/website/static/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/pyproject.toml` & `aunly-bbot-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aunly-bbot"
-version = "1.3.2"
+version = "1.4.0"
 description = "一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人"
 readme = "readme.md"
 keywords = [
     "graia",
     "graiax",
     "bilibili",
     "qqbot",
@@ -16,30 +16,30 @@
     "chatgpt",
 ]
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
 ]
 requires-python = ">=3.9,<4.0"
 dependencies = [
-    "graia-ariadne[standard]>=0.11.3",
-    "peewee>=3.16.0",
+    "graia-ariadne[standard]>=0.11.5",
+    "peewee>=3.16.2",
     "pyyaml>=6.0",
-    "bilireq>=0.2.4",
-    "psutil>=5.9.4",
-    "uvicorn>=0.21.1",
-    "sentry-sdk>=1.18.0",
+    "bilireq>=0.2.6",
+    "psutil>=5.9.5",
+    "uvicorn>=0.22.0",
+    "sentry-sdk>=1.25.0",
     "python-jose[cryptography]>=3.3.0",
     "passlib[bcrypt]>=1.7.4",
     "python-multipart>=0.0.6",
-    "fastapi>=0.95.0",
-    "websockets>=10.4",
+    "fastapi>=0.96.0",
+    "websockets>=11.0.2",
     "qrcode>=7.4.2",
     "pillow>=9.5.0",
     "noneprompt>=0.1.9",
-    "minidynamicrender>=1.1.9",
+    "minidynamicrender>=1.2.6",
     "lxml>=4.9.2",
     "tiktoken-async>=0.3.2",
 ]
 
 [project.license]
 text = "AGPL3.0"
 
@@ -50,14 +50,15 @@
 
 [project.optional-dependencies]
 full = [
     "graiax-playwright",
     "graiax-text2img-playwright",
     "wordcloud",
     "jieba",
+    "edgegpt",
 ]
 
 [project.scripts]
 bbot = "aunly_bbot.__main__:main"
 
 [tool.pdm.build]
 includes = [
@@ -65,15 +66,15 @@
 ]
 excludes = [
     "aunly_bbot/static/browser",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "yamllint>=1.29.0",
+    "yamllint>=1.31.0",
     "black>=23.3.0",
     "flake8>=6.0.0",
 ]
 
 [tool.black]
 line-length = 96
```

### Comparing `aunly-bbot-1.3.2/readme.md` & `aunly-bbot-1.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.3.2/PKG-INFO` & `aunly-bbot-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aunly-bbot
-Version: 1.3.2
+Version: 1.4.0
 Summary: 一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人
 License: AGPL3.0
 Keywords: graia,graiax,bilibili,qqbot,grpc,playwright,fastapi,bot,openai,chatgpt
 Author-email: djkcyl <cyl@cyllive.cn>
 Requires-Python: >=3.9,<4.0
 Provides-Extra: full
 Project-URL: documentation, https://github.com/djkcyl/BBot-Graia/blob/master/readme.md
```

