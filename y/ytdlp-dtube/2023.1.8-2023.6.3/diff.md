# Comparing `tmp/ytdlp_dtube-2023.1.8-py3-none-any.whl.zip` & `tmp/ytdlp_dtube-2023.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7565 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    16211 b- defN 23-Jan-09 00:26 yt_dlp_plugins/extractor/dtube.py
--rw-rw-rw-  2.0 fat     1236 b- defN 23-Jan-09 00:26 ytdlp_dtube-2023.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2760 b- defN 23-Jan-09 00:26 ytdlp_dtube-2023.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-09 00:26 ytdlp_dtube-2023.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Jan-09 00:26 ytdlp_dtube-2023.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      512 b- defN 23-Jan-09 00:26 ytdlp_dtube-2023.1.8.dist-info/RECORD
-6 files, 20836 bytes uncompressed, 6633 bytes compressed:  68.2%
+Zip file size: 7293 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    15329 b- defN 23-Jun-03 09:55 yt_dlp_plugins/extractor/dtube.py
+-rw-rw-rw-  2.0 fat     1236 b- defN 23-Jun-03 09:55 ytdlp_dtube-2023.6.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2761 b- defN 23-Jun-03 09:55 ytdlp_dtube-2023.6.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 09:55 ytdlp_dtube-2023.6.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-03 09:55 ytdlp_dtube-2023.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      512 b- defN 23-Jun-03 09:55 ytdlp_dtube-2023.6.3.dist-info/RECORD
+6 files, 19955 bytes uncompressed, 6361 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: yt_dlp_plugins/extractor/dtube.py
 Comment: 
 
-Filename: ytdlp_dtube-2023.1.8.dist-info/LICENSE
+Filename: ytdlp_dtube-2023.6.3.dist-info/LICENSE
 Comment: 
 
-Filename: ytdlp_dtube-2023.1.8.dist-info/METADATA
+Filename: ytdlp_dtube-2023.6.3.dist-info/METADATA
 Comment: 
 
-Filename: ytdlp_dtube-2023.1.8.dist-info/WHEEL
+Filename: ytdlp_dtube-2023.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: ytdlp_dtube-2023.1.8.dist-info/top_level.txt
+Filename: ytdlp_dtube-2023.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ytdlp_dtube-2023.1.8.dist-info/RECORD
+Filename: ytdlp_dtube-2023.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yt_dlp_plugins/extractor/dtube.py

```diff
@@ -1,46 +1,38 @@
 # coding: utf-8
 import json
 import re
-from contextlib import suppress
 from datetime import datetime, timedelta
 from itertools import count
 from urllib.parse import unquote_plus
 
-from yt_dlp import extractor
 from yt_dlp.extractor.common import InfoExtractor
 from yt_dlp.utils import (
     ExtractorError,
     LazyList,
     OnDemandPagedList,
     float_or_none,
     int_or_none,
     parse_duration,
     parse_iso8601,
     traverse_obj,
     update_url_query,
 )
 from ytdlp_plugins.probe import probe_media
 
-__version__ = "2023.01.08"
-_VALID_URL = r"""(?x)
-                https?://(?:www\.)?d\.tube/
-                (?:\#!/)?v/
-                (?P<id>[0-9a-z.-]+/[\w-]+)
-                """
-
-# dirty way to override existing extractor, since we change the URL regex
-# pylint: disable=protected-access
-with suppress(AttributeError):
-    extractor._extractors.DTubeIE._VALID_URL = _VALID_URL
-    extractor.lazy_extractors.DTubeIE._VALID_URL = _VALID_URL
+__version__ = "2023.06.03"
+
 
 # pylint: disable=abstract-method
-class DTubeIE(InfoExtractor):
-    _VALID_URL = _VALID_URL
+class DTubePluginIE(InfoExtractor):
+    _VALID_URL = r"""(?x)
+                    https?://(?:www\.)?d\.tube/
+                    (?:\#!/)?v/
+                    (?P<id>[0-9a-z.-]+/[\w-]+)
+                    """
     IE_NAME = "d.tube"
 
     GATEWAY_URLS = {
         "ipfs": [
             "https://player.d.tube/ipfs",
             "https://ipfs.d.tube/ipfs",
             "https://ipfs.io/ipfs",
@@ -56,49 +48,30 @@
         "facebook": "https://www.facebook.com/video.php?v={}",
         "dailymotion": "https://www.dailymotion.com/video/{}",
     }
 
     # pylint: disable=line-too-long
     _TESTS = [
         {
-            "url": "https://d.tube/v/famigliacurione/QmUJquzf7DALjwUExoHtTjS8PgGqfGohzMr4W3XJ56q9pR",
-            "md5": "4ad5272197655dc033bfd0cc039b71f2",
+            "url": "https://d.tube/v/truehnchannel3.0/QmNXrihTWmHiLVXxLabfXFakFzJVLq1LimfH2X1sNma5ak",
+            "md5": "d7b147de74210442e6b14d934f96c585",
             "info_dict": {
-                "id": "famigliacurione/QmUJquzf7DALjwUExoHtTjS8PgGqfGohzMr4W3XJ56q9pR",
-                "title": "La Prova by SOSO",
-                "description": "md5:c942bfe98693a2e81510464d10869449",
+                "id": "truehnchannel3.0/QmNXrihTWmHiLVXxLabfXFakFzJVLq1LimfH2X1sNma5ak",
+                "title": "HAPPY WEEKEND #TRUEHNERS #TRUEHNER FROM THE TEAM OF TRUE_HUMANNATURE - THE TRUEHN BACKED FASHION & BEAUTY BRAND ",
+                "description": "md5:452385a9aef03447baa2aae9c801eb14",
                 "ext": "mp4",
-                "thumbnail": "https://cdn.steemitimages.com/DQmbCfaJkTRrjerNhcyDCoviBqpXB8ZDh31NhQPWvcyEj6U/laprovathumb.jpg",
-                "tags": ["music", "hiphop"],
-                "duration": 71,
-                "uploader_id": "famigliacurione",
-                "upload_date": "20211223",
-                "timestamp": 1640297596.628,
+                "thumbnail": "https://ipfs.io/ipfs/QmcFBCAx8c8PLew7JfjVmn3VK6MjrSMfCerq5b5y9iNdp8?filename=AAAAAAAAAAA%20TRUEHUMAN%20NATURE.jpg",
+                "tags": ["truehnchannel"],
+                "duration": 3,
+                "uploader_id": "truehnchannel3.0",
+                "upload_date": "20230603",
+                "timestamp": 1685782622.873,
             },
             "params": {
-                "format": "480",
-            },
-        },
-        # fallback files
-        {
-            "url": "https://d.tube/#!/v/reeta0119/QmX9rAqkTzYfUoi5VFuitzYQXyybFtURyUUWcYkyPXzkkz",
-            "md5": "179f4435eb5068d3b1c6188ec3065d9a",
-            "info_dict": {
-                "id": "reeta0119/QmX9rAqkTzYfUoi5VFuitzYQXyybFtURyUUWcYkyPXzkkz",
-                "title": "Splinterlands Battle Share Theme: DIVINE SORCERESS",
-                "description": "md5:4521cc098e7dcad3e9a7f73095c9ffe9",
-                "ext": "mp4",
-                "thumbnail": "https://snap1.d.tube/ipfs/QmWYECptp7XKVEUk4tBf9R6d5XaRUo6Hcow6abtuy1Q3Vt",
-                "duration": 181,
-                "uploader_id": "reeta0119",
-                "upload_date": "20200306",
-                "timestamp": 1583519894.482,
-            },
-            "params": {
-                "format": "480",
+                "format": "src",
             },
         },
         {
             # using steemit API
             "url": "https://d.tube/v/cahlen/hcyx513ospn",
             "md5": "fd03f59d2c1f7b1e0ed5a2098116e443",
             "info_dict": {
@@ -281,19 +254,23 @@
         else:
             tags = []
 
         entry_info = {
             "_type": _type,
             "url": redirect_url or f"https://d.tube/v/{video_id}",
             "id": video_id,
-            "title": info.get("title"),
-            "description": info.get("desc") or info.get("description"),
+            "title": traverse_obj(info, ("title",), ("info", "title")),
+            "description": traverse_obj(
+                info, ("desc",), ("description",), ("content", "description")
+            ),
             "thumbnail": info.get("thumbnailUrl"),
             "tags": tags,
-            "duration": float_or_none(info.get("duration"))
+            "duration": float_or_none(
+                traverse_obj(info, ("duration",), ("info", "duration"))
+            )
             or int_or_none(info.get("dur"))
             or parse_duration(info.get("dur")),
             "timestamp": float_or_none(result.get("ts"), scale=1000),
             "uploader_id": result.get("author"),
         }
 
         if formats is not None:
@@ -306,15 +283,15 @@
         result = self.avalon_api(f"content/{video_id}", video_id)
         if not result:
             result = self.steemit_api(video_id)
 
         return self.entry_from_avalon_result(result)
 
 
-class DTubeUserIE(DTubeIE):
+class DTubeUserPluginIE(DTubePluginIE):
     _VALID_URL = r"""(?x)
                     https?://(?:www\.)?d\.tube/
                     (?:\#!/)?c/
                     (?P<id>[0-9a-z.-]+)
                     """
     IE_NAME = "d.tube:user"
 
@@ -356,15 +333,15 @@
         return self.playlist_result(
             LazyList(self.iter_entries(user_id, endpoint)),
             playlist_id=user_id,
             playlist_title=user_id,
         )
 
 
-class DTubeQueryIE(DTubeUserIE):
+class DTubeQueryPluginIE(DTubeUserPluginIE):
     _VALID_URL = r"""(?x)
                     https?://(?:www\.)?d\.tube/
                     (?:\#!/)?
                     (?P<id>hotvideos|trendingvideos|newvideos)
                     """
     IE_NAME = "d.tube:query"
 
@@ -403,15 +380,15 @@
         return self.playlist_result(
             LazyList(self.iter_entries(query_id, endpoint)),
             playlist_id=query_id,
             playlist_title=query_id,
         )
 
 
-class DTubeSearchIE(DTubeIE):
+class DTubeSearchPluginIE(DTubePluginIE):
     _VALID_URL = r"""(?x)
                     https?://(?:www\.)?d\.tube/
                     (?:\#!/)?[st]/
                     (?P<id>[^?]+)
                     """
     IE_NAME = "d.tube:search"
```

## Comparing `ytdlp_dtube-2023.1.8.dist-info/LICENSE` & `ytdlp_dtube-2023.6.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ytdlp_dtube-2023.1.8.dist-info/METADATA` & `ytdlp_dtube-2023.6.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ytdlp-dtube
-Version: 2023.1.8
+Version: 2023.6.3
 Summary: yt-dlp extractor for d.tube
 Home-page: https://github.com/flashdagger/ytdlp-plugins/tree/dtube
 Author: flashdagger
 Author-email: flashdagger@googlemail.com
 License: The Unlicense
 Keywords: yt-dlp,youtube-dl,dtube,extractors,plugins
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Topic :: Multimedia :: Video
```

