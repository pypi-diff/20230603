# Comparing `tmp/douyin_tiktok_scraper-1.2.1.tar.gz` & `tmp/douyin_tiktok_scraper-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "douyin_tiktok_scraper-1.2.1.tar", last modified: Sat Jun  3 10:01:25 2023, max compression
+gzip compressed data, was "douyin_tiktok_scraper-1.2.2.tar", last modified: Sat Jun  3 10:08:21 2023, max compression
```

## Comparing `douyin_tiktok_scraper-1.2.1.tar` & `douyin_tiktok_scraper-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.644900 douyin_tiktok_scraper-1.2.1/
--rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    15665 2023-06-03 10:01:25.643900 douyin_tiktok_scraper-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.619901 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/
--rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/__init__.py
--rw-rw-rw-   0        0        0    35210 2023-06-03 09:59:44.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:01:25.639904 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/
--rw-rw-rw-   0        0        0    15665 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-03 10:01:25.000000 douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 10:01:25.644900 douyin_tiktok_scraper-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1384 2023-06-03 10:01:23.000000 douyin_tiktok_scraper-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:08:21.417156 douyin_tiktok_scraper-1.2.2/
+-rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:08:21.416162 douyin_tiktok_scraper-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 10:08:21.391156 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper/
+-rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper/__init__.py
+-rw-rw-rw-   0        0        0    35210 2023-06-03 09:59:44.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:08:21.412161 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:08:21.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-03 10:08:21.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:08:21.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 10:08:21.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-03 10:08:21.000000 douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 10:08:21.417156 douyin_tiktok_scraper-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1386 2023-06-03 10:08:10.000000 douyin_tiktok_scraper-1.2.2/setup.py
```

### Comparing `douyin_tiktok_scraper-1.2.1/LICENSE` & `douyin_tiktok_scraper-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.1/PKG-INFO` & `douyin_tiktok_scraper-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin_tiktok_scraper
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.2 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.1/README.md` & `douyin_tiktok_scraper-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper/scraper.py` & `douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.1/douyin_tiktok_scraper.egg-info/PKG-INFO` & `douyin_tiktok_scraper-1.2.2/douyin_tiktok_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-tiktok-scraper
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.2 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.1/setup.py` & `douyin_tiktok_scraper-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='douyin_tiktok_scraper',
     author='Evil0ctal',
-    version='1.2.1',
+    version='1.2.2',
     license='MIT License',
     description='Douyin/TikTok async data scraper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='Evil0ctal1985@gmail.com',
     url='https://github.com/Evil0ctal/Douyin_TikTok_Download_API',
     packages=setuptools.find_packages(),
     keywords='TikTok, Douyin, 抖音, Scraper, Crawler, API, Download, Video, No Watermark, Async',
     # 依赖包
     install_requires=[
         'aiohttp',
         "orjson",
         "tenacity",
-        "execjs",
+        "PyExecJS",
         "Brotli",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

