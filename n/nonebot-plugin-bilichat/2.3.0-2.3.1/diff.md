# Comparing `tmp/nonebot_plugin_bilichat-2.3.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.3.0.tar", last modified: Sat Jun  3 07:40:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.3.1.tar", last modified: Sat Jun  3 07:51:41 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.3.0.tar` & `nonebot_plugin_bilichat-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-03 07:40:49.184950 nonebot_plugin_bilichat-2.3.0/LICENSE
--rw-r--r--   0        0        0    12309 2023-06-03 07:40:49.184950 nonebot_plugin_bilichat-2.3.0/README.md
--rw-r--r--   0        0        0     8846 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-03 07:40:49.192950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-03 07:40:49.196950 nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1470 2023-06-03 07:40:57.568942 nonebot_plugin_bilichat-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    13677 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-03 07:51:31.244194 nonebot_plugin_bilichat-2.3.1/LICENSE
+-rw-r--r--   0        0        0    12309 2023-06-03 07:51:31.244194 nonebot_plugin_bilichat-2.3.1/README.md
+-rw-r--r--   0        0        0     8846 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-03 07:51:31.256195 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-03 07:51:31.260196 nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1470 2023-06-03 07:51:41.613080 nonebot_plugin_bilichat-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13677 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.3.0/LICENSE` & `nonebot_plugin_bilichat-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/README.md` & `nonebot_plugin_bilichat-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,14 @@
     bilichat_newbing_token_limit: int = 0
     bilichat_newbing_preprocess: bool = True
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
     bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
-    @validator("nickname")
-    def check_nickname(cls, v):
-        return list(v) or ["awesome-nonebot"]
-
     @validator("bilichat_openai_proxy")
     def check_openai_proxy(cls, v, values):
         if not (values["bilichat_openai_token"] or values["bilichat_newbing_cookie"]):
             return v
         if v is None:
             logger.warning("you have enabled openai summary without a proxy, this may cause request failure.")
         return v
```

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.3.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.3.0/pyproject.toml` & `nonebot_plugin_bilichat-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.3.0"
+version = "2.3.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-2.3.0/PKG-INFO` & `nonebot_plugin_bilichat-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.3.0
+Version: 2.3.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.3.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-
```

