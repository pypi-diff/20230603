# Comparing `tmp/douyin_tiktok_scraper-1.2.0.tar.gz` & `tmp/douyin_tiktok_scraper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "douyin_tiktok_scraper-1.2.0.tar", last modified: Wed Mar  8 00:16:20 2023, max compression
+gzip compressed data, was "douyin_tiktok_scraper-1.2.1.tar", last modified: Sat Jun  3 10:01:25 2023, max compression
```

## Comparing `douyin_tiktok_scraper-1.2.0.tar` & `douyin_tiktok_scraper-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:20.352102 douyin_tiktok_scraper-1.2.0/
--rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    15665 2023-03-08 00:16:20.351101 douyin_tiktok_scraper-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:20.337101 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper/
--rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper/__init__.py
--rw-rw-rw-   0        0        0    36236 2023-03-08 00:16:18.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:20.349101 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/
--rw-rw-rw-   0        0        0    15665 2023-03-08 00:16:20.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-03-08 00:16:20.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 00:16:20.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-03-08 00:16:20.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-08 00:16:20.000000 douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 00:16:20.352102 douyin_tiktok_scraper-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1384 2023-03-08 00:16:18.000000 douyin_tiktok_scraper-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.644900 douyin_tiktok_scraper-1.2.1/
+-rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:01:25.643900 douyin_tiktok_scraper-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.619901 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/
+-rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/__init__.py
+-rw-rw-rw-   0        0        0    35210 2023-06-03 09:59:44.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.639904 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 10:01:25.644900 douyin_tiktok_scraper-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1384 2023-06-03 10:01:23.000000 douyin_tiktok_scraper-1.2.1/setup.py
```

### Comparing `douyin_tiktok_scraper-1.2.0/LICENSE` & `douyin_tiktok_scraper-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.0/PKG-INFO` & `douyin_tiktok_scraper-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin_tiktok_scraper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Douyin/TikTok async data scraper.
 Home-page: https://github.com/Evil0ctal/Douyin_TikTok_Download_API
 Author: Evil0ctal
 Author-email: Evil0ctal1985@gmail.com
 License: MIT License
 Keywords: TikTok,Douyin,抖音,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.1 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.0/README.md` & `douyin_tiktok_scraper-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper/scraper.py` & `douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,47 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # @Author: https://github.com/Evil0ctal/
 # @Time: 2021/11/06
-# @Update: 2023/03/06
+# @Update: 2023/03/08
 # @Version: 3.3.0
 # @Function:
 # 核心代码，估值1块(๑•̀ㅂ•́)و✧
 # 用于爬取Douyin/TikTok数据并以字典形式返回。
 # input link, output dictionary.
 
 
 import re
 import os
 import time
-import urllib.parse
-
+import execjs
 import aiohttp
 import platform
 import asyncio
 import traceback
 import configparser
+import urllib.parse
 
 from typing import Union
-
-import execjs
 from tenacity import *
 
 
 class Scraper:
-    """
-    简介/Introduction
-
-    Scraper.get_url(text: str) -> Union[str, None]
-    用于检索出文本中的链接并返回/Used to retrieve the link in the text and return it.
-
-    Scraper.convert_share_urls(self, url: str) -> Union[str, None]\n
-    用于转换分享链接为原始链接/Convert share links to original links
-
-    Scraper.get_douyin_video_id(self, original_url: str) -> Union[str, None]\n
-    用于获取抖音视频ID/Get Douyin video ID
-
-    Scraper.get_douyin_video_data(self, video_id: str) -> Union[dict, None]\n
-    用于获取抖音视频数据/Get Douyin video data
-
-    Scraper.get_douyin_live_video_data(self, original_url: str) -> Union[str, None]\n
-    用于获取抖音直播视频数据/Get Douyin live video data
-
-    Scraper.get_tiktok_video_id(self, original_url: str) -> Union[str, None]\n
-    用于获取TikTok视频ID/Get TikTok video ID
-
-    Scraper.get_tiktok_video_data(self, video_id: str) -> Union[dict, None]\n
-    用于获取TikTok视频数据/Get TikTok video data
-
-    Scraper.hybrid_parsing(self, video_url: str) -> dict\n
-    用于混合解析/ Hybrid parsing
-
-    Scraper.hybrid_parsing_minimal(data: dict) -> dict\n
-    用于混合解析最小化/Hybrid parsing minimal
-    """
-
     """__________________________________________⬇️initialization(初始化)⬇️______________________________________"""
 
     # 初始化/initialization
     def __init__(self):
         self.headers = {
-            'User-Agent': "Mozilla/5.0 (Linux; Android 8.0; Pixel 2 Build/OPD3.170816.012) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Mobile Safari/537.36 Edg/87.0.664.66"
+            'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"
         }
         self.douyin_api_headers = {
             'accept-encoding': 'gzip, deflate, br',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
             'referer': 'https://www.douyin.com/',
-            'cookie': 's_v_web_id=verify_leytkxgn_kvO5kOmO_SdMs_4t1o_B5ml_BUqtWM1mP6BF;'
+            # 'cookie': "s_v_web_id=verify_leytkxgn_kvO5kOmO_SdMs_4t1o_B5ml_BUqtWM1mP6BF;"
         }
         self.tiktok_api_headers = {
             'User-Agent': 'com.ss.android.ugc.trill/494+Mozilla/5.0+(Linux;+Android+12;+2112123G+Build/SKQ1.211006.001;+wv)+AppleWebKit/537.36+(KHTML,+like+Gecko)+Version/4.0+Chrome/107.0.5304.105+Mobile+Safari/537.36'
         }
         # 判断配置文件是否存在/Check if the configuration file exists
         if os.path.exists('config.ini'):
             self.config = configparser.ConfigParser()
@@ -98,27 +65,35 @@
             self.proxies = None
         # 针对Windows系统的异步事件规则/Asynchronous event rules for Windows systems
         if platform.system() == 'Windows':
             asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
     """__________________________________________⬇️utils(实用程序)⬇️______________________________________"""
 
-    # 检索字符串中的链接
+    # 检索字符串中的链接/Retrieve links from string
     @staticmethod
     def get_url(text: str) -> Union[str, None]:
         try:
             # 从输入文字中提取索引链接存入列表/Extract index links from input text and store in list
             url = re.findall('http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+', text)
             # 判断是否有链接/Check if there is a link
             if len(url) > 0:
                 return url[0]
         except Exception as e:
             print('Error in get_url:', e)
             return None
 
+    # 生成X-Bogus签名/Generate X-Bogus signature
+    @staticmethod
+    def generate_x_bogus_url(url: str, headers: dict) -> str:
+        query = urllib.parse.urlparse(url).query
+        xbogus = execjs.compile(open('./X-Bogus.js').read()).call('sign', query, headers['User-Agent'])
+        new_url = url + "&X-Bogus=" + xbogus
+        return new_url
+
     # 转换链接/convert url
     @retry(stop=stop_after_attempt(4), wait=wait_fixed(7))
     async def convert_share_urls(self, url: str) -> Union[str, None]:
         """
         用于将分享链接(短链接)转换为原始链接/Convert share links (short links) to original links
         :return: 原始链接/Original link
         """
@@ -261,26 +236,23 @@
                 return key
         except Exception as e:
             print('获取抖音视频ID出错了:{}'.format(e))
             return None
 
     # 获取单个抖音视频数据/Get single Douyin video data
     @retry(stop=stop_after_attempt(4), wait=wait_fixed(7))
-    async def get_douyin_video_data(self, video_id: str, s_v_web_id: str = None) -> Union[dict, None]:
+    async def get_douyin_video_data(self, video_id: str) -> Union[dict, None]:
         """
         :param video_id: str - 抖音视频id
-        :param s_v_web_id: str - Example: "s_v_web_id=verify_leytkxgn_kvO5kOmO_SdMs_4t1o_B5ml_BUqtWM1mP6BF; "
         :return:dict - 包含信息的字典
         """
         print('正在获取抖音视频数据...')
-        if s_v_web_id:
-            self.douyin_api_headers['cookie'] = s_v_web_id
         try:
             # 构造访问链接/Construct the access link
-            api_url = f"https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0&cookie_enabled=true&screen_width=1344&screen_height=756&browser_language=zh-CN&browser_platform=Win32&browser_name=Evil0ctal&browser_version=110.0&browser_online=true&engine_name=Gecko&engine_version=109.0&os_name=Windows&os_version=10&cpu_core_num=128&device_memory=2333&platform=PC&webid=7158288523463362079"
+            api_url = f"https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0&cookie_enabled=true&screen_width=1344&screen_height=756&browser_language=zh-CN&browser_platform=Win32&browser_name=Firefox&browser_version=110.0&browser_online=true&engine_name=Gecko&engine_version=109.0&os_name=Windows&os_version=10&cpu_core_num=16&device_memory=&platform=PC&webid=7158288523463362079&msToken=abL8SeUTPa9-EToD8qfC7toScSADxpg6yLh2dbNcpWHzE0bT04txM_4UwquIcRvkRb9IU8sifwgM1Kwf1Lsld81o9Irt2_yNyUbbQPSUO8EfVlZJ_78FckDFnwVBVUVK"
             api_url = self.generate_x_bogus_url(api_url)
             # 访问API/Access API
             print("正在获取视频数据API: {}".format(api_url))
             async with aiohttp.ClientSession() as session:
                 async with session.get(api_url, headers=self.douyin_api_headers, proxy=self.proxies,
                                        timeout=10) as response:
                     response = await response.json()
```

### Comparing `douyin_tiktok_scraper-1.2.0/douyin_tiktok_scraper.egg-info/PKG-INFO` & `douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-tiktok-scraper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Douyin/TikTok async data scraper.
 Home-page: https://github.com/Evil0ctal/Douyin_TikTok_Download_API
 Author: Evil0ctal
 Author-email: Evil0ctal1985@gmail.com
 License: MIT License
 Keywords: TikTok,Douyin,抖音,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.1 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.0/setup.py` & `douyin_tiktok_scraper-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='douyin_tiktok_scraper',
     author='Evil0ctal',
-    version='1.2.0',
+    version='1.2.1',
     license='MIT License',
     description='Douyin/TikTok async data scraper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='Evil0ctal1985@gmail.com',
     url='https://github.com/Evil0ctal/Douyin_TikTok_Download_API',
     packages=setuptools.find_packages(),
```

