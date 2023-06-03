# Comparing `tmp/nonebot_plugin_bilichat-2.2.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.2.0.tar", last modified: Thu Jun  1 15:18:15 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.3.0.tar", last modified: Sat Jun  3 07:40:57 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.2.0.tar` & `nonebot_plugin_bilichat-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-01 15:18:03.956801 nonebot_plugin_bilichat-2.2.0/LICENSE
--rw-r--r--   0        0        0    11979 2023-06-01 15:18:03.956801 nonebot_plugin_bilichat-2.2.0/README.md
--rw-r--r--   0        0        0     8467 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4842 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1470 2023-06-01 15:18:15.592819 nonebot_plugin_bilichat-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    13347 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-03 07:40:49.184950 nonebot_plugin_bilichat-2.3.0/LICENSE
+-rw-r--r--   0        0        0    12309 2023-06-03 07:40:49.184950 nonebot_plugin_bilichat-2.3.0/README.md
+-rw-r--r--   0        0        0     8846 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1470 2023-06-03 07:40:57.568942 nonebot_plugin_bilichat-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13677 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.2.0/LICENSE` & `nonebot_plugin_bilichat-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/README.md` & `nonebot_plugin_bilichat-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,27 +149,29 @@
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_show_error_msg     | bool      | True  | 是否在解析失败时发送错误信息 |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_basic_info          | bool | True | 是否开启视频基本信息 |
+| bilichat_basic_info_url      | bool | True | 开启视频进本信息的情况下，是否一同回复一个链接 |
 | bilichat_reply_to_basic_info | bool | True | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
@@ -236,11 +238,12 @@
 
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 - [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
+- [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项BUG修复和代码参考
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -42,27 +42,30 @@
 æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
 | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
-True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
-ç±äº OneBot
+True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
+bilichat_show_error_msg | bool | True |
+æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_reply_to_basic_info | bool | True |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_url | bool | True |
+å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
+bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | ###
 è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
 bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_word_cloud | bool | True |
 æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
 `wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
 ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
@@ -113,10 +116,12 @@
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
-Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè ## â³ Star è¶å¿
-[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè - [Misaka-Mikoto-
+Tech](https://github.com/Misaka-Mikoto-Tech)
+ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè ## â³ Star è¶å¿ [!
+[Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,17 +147,17 @@
 async def video_info(
     bot: BOT,
     event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
-    # sourcery skip: hoist-similar-statement-from-if, swap-nested-ifs, use-fstring-for-concatenation
+    # sourcery skip: raise-from-previous-error, use-fstring-for-concatenation
     DISABLE_REPLY = isinstance(bot, Mirai_Bot)  # 部分平台Reply暂不可用
-    DISABLE_LINK = isinstance(bot, QG_Bot)  # 部分平台发送链接都要审核
+    DISABLE_LINK = isinstance(bot, QG_Bot) and plugin_config.bilichat_basic_info_url  # 部分平台发送链接都要审核
     SEND_IMAGE_SEPARATELY = isinstance(bot, QG_Bot)  # 部分平台无法一次性发送多张图片，或无法与其他消息组合发出
     reply = "" if DISABLE_REPLY else await SegmentBuilder.reply()
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
     if bili_number[:2] in ["BV", "bv", "av"]:
         msg, img, info = await get_video_basic(bili_number, uid)
         if not msg or not info:
@@ -190,36 +190,44 @@
         raise FinishedException
 
     # get video cache
     try:
         cache = await get_content_cache(info, options)
     except AbortError as e:
         logger.exception(e)
-        await matcher.finish(reply + f"视频字幕获取失败: {str(e)}")
+        if plugin_config.bilichat_show_error_msg:
+            await matcher.finish(reply + f"视频字幕获取失败: {str(e)}")
+        raise FinishedException
     except Exception as e:
         capture_exception()
         logger.exception(e)
-        await matcher.finish(reply + f"未知错误: {e}")
+        if plugin_config.bilichat_show_error_msg:
+            await matcher.finish(reply + f"未知错误: {e}")
+        raise FinishedException
 
     # wordcloud
     wc_image = ""
     if plugin_config.bilichat_word_cloud:
         if image := await wordcloud(cache=cache, cid=str(info.cid)):
             wc_image = await SegmentBuilder.image(image=image)
         else:
-            await matcher.finish(reply + "视频无有效字幕")
+            if plugin_config.bilichat_show_error_msg:
+                await matcher.finish(reply + "视频无有效字幕")
+            raise FinishedException
 
     # summary
     summary = ""
     if ENABLE_SUMMARY:
         if summary := await summarization(cache=cache, cid=str(info.cid)):
             if isinstance(summary, bytes):
                 summary = await SegmentBuilder.image(image=summary)
         else:
-            await matcher.finish(reply + "视频无有效字幕")
+            if plugin_config.bilichat_show_error_msg:
+                await matcher.finish(reply + "视频无有效字幕")
+            raise FinishedException
 
     if wc_image:
         if SEND_IMAGE_SEPARATELY:
             await matcher.send(wc_image)
             if summary:
                 await matcher.finish(summary)
         await matcher.finish(reply + wc_image + summary)  # type: ignore
```

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,20 @@
     bilichat_only_self: bool = False
     bilichat_enable_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
-    bilichat_neterror_retry = 3
-    nickname: List[str] = ["awesome-nonebot"]
+    bilichat_neterror_retry: int = 3
+    bilichat_show_error_msg: bool = True
 
     # basic info
     bilichat_basic_info: bool = True
+    bilichat_basic_info_url: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
```

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.2.0/pyproject.toml` & `nonebot_plugin_bilichat-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.2.0"
+version = "2.3.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-2.2.0/PKG-INFO` & `nonebot_plugin_bilichat-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.2.0
+Version: 2.3.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -184,27 +184,29 @@
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
 | bilichat_use_bcut_asr       | bool      | True  | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_show_error_msg     | bool      | True  | 是否在解析失败时发送错误信息 |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_basic_info          | bool | True | 是否开启视频基本信息 |
+| bilichat_basic_info_url      | bool | True | 开启视频进本信息的情况下，是否一同回复一个链接 |
 | bilichat_reply_to_basic_info | bool | True | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
@@ -271,11 +273,12 @@
 
 - [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
 - [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 - [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 - [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 - [nonebot-plugin-bing-chat](https://github.com/Harry-Jing/nonebot-plugin-bing-chat): newbing解析的代码参考
+- [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项BUG修复和代码参考
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.3.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-
@@ -61,27 +61,30 @@
 æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
 | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
-True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
-ç±äº OneBot
+True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
+bilichat_show_error_msg | bool | True |
+æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_reply_to_basic_info | bool | True |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_url | bool | True |
+å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
+bilichat_reply_to_basic_info | bool | True |
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | ###
 è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
 bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_word_cloud | bool | True |
 æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
 `wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
 ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
@@ -132,10 +135,12 @@
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
 åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
 BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
 github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [nonebot-plugin-bing-chat](https://github.com/Harry-
-Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè ## â³ Star è¶å¿
-[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+Jing/nonebot-plugin-bing-chat): newbingè§£æçä»£ç åè - [Misaka-Mikoto-
+Tech](https://github.com/Misaka-Mikoto-Tech)
+ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹BUGä¿®å¤åä»£ç åè ## â³ Star è¶å¿ [!
+[Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

