# Comparing `tmp/duckduckgo_search-3.8.0.tar.gz` & `tmp/duckduckgo_search-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.8.0.tar", last modified: Thu Jun  1 23:59:52 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.8.1.tar", last modified: Sat Jun  3 07:39:55 2023, max compression
```

## Comparing `duckduckgo_search-3.8.0.tar` & `duckduckgo_search-3.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13924 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    31374 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 23:59:52.000000 duckduckgo_search-3.8.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:59:52.440648 duckduckgo_search-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-01 23:59:36.000000 duckduckgo_search-3.8.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.760635 duckduckgo_search-3.8.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.8.0/LICENSE.md` & `duckduckgo_search-3.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.0/PKG-INFO` & `duckduckgo_search-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.8.0
+Version: 3.8.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -62,14 +62,16 @@
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download any xls files from a specific site
+ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
@@ -182,15 +184,15 @@
 with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
-## 1. text() - text search by by duckduckgo.com
+## 1. text() - text search by duckduckgo.com
 `html` and `lite` backend differ from `api`:</br>
 * don't do an extra request first to get vqd,</br>
 * use POST requests,</br>
 * pause 0.75 seconds between paginations.</br>
 
 If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
 Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
```

### Comparing `duckduckgo_search-3.8.0/README.md` & `duckduckgo_search-3.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download any xls files from a specific site
+ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
@@ -157,15 +159,15 @@
 with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
-## 1. text() - text search by by duckduckgo.com
+## 1. text() - text search by duckduckgo.com
 `html` and `lite` backend differ from `api`:</br>
 * don't do an extra request first to get vqd,</br>
 * use POST requests,</br>
 * pause 0.75 seconds between paginations.</br>
 
 If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
 Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
```

### Comparing `duckduckgo_search-3.8.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.8.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.8.1/duckduckgo_search/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
+import asyncio
 import csv
 import json
 import logging
 import os
-from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from random import choice
 from urllib.parse import unquote
 
 import click
 import httpx
 
-# isort: off
 from .duckduckgo_search import DDGS, USERAGENTS
 from .version import __version__
 
-# isort: on
-
 logger = logging.getLogger(__name__)
 
 COLORS = {
     0: "black",
     1: "red",
     2: "green",
     3: "yellow",
@@ -54,15 +51,23 @@
     if data:
         for i, e in enumerate(data, start=1):
             click.secho(f"{i}. {'-' * 78}", bg="black", fg="white")
             for j, (k, v) in enumerate(e.items(), start=1):
                 if v:
                     width = (
                         300
-                        if k in ("href", "url", "image", "thumbnail", "content")
+                        if k
+                        in (
+                            "content",
+                            "href",
+                            "image",
+                            "source",
+                            "thumbnail",
+                            "url",
+                        )
                         else 78
                     )
                     k = "language" if k == "detected_language" else k
                     text = click.wrap_text(
                         f"{v}",
                         width=width,
                         initial_indent="",
@@ -85,58 +90,67 @@
         .replace("/", "_")
         .replace("\\", "_")
         .replace(" ", "")
     )
     return keywords
 
 
-def download_file(url, dir_path, filename):
-    headers = {
-        "User-Agent": choice(USERAGENTS),
-    }
+async def download_file(url, dir_path, filename, sem):
+    headers = {"User-Agent": choice(USERAGENTS)}
     try:
-        with httpx.stream("GET", url, headers=headers) as resp:
-            with open(os.path.join(dir_path, filename), "wb") as file:
-                for chunk in resp.iter_bytes():
-                    file.write(chunk)
-        logger.info(f"File downloaded {url}")
+        async with sem:
+            async with httpx.AsyncClient() as client:
+                async with client.stream("GET", url, headers=headers) as resp:
+                    if resp.status_code == 200:
+                        with open(os.path.join(dir_path, filename), "wb") as file:
+                            async for chunk in resp.aiter_bytes():
+                                file.write(chunk)
+                logger.info(f"File downloaded {url}")
     except Exception as ex:
         logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
-def download_results(keywords, results, images=False):
+async def _download_results(keywords, results, images=False):
     if images:
         path = f"images_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     else:
         path = f"text_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
-    futures = []
-    with ThreadPoolExecutor(10) as executor:
-        for i, res in enumerate(results, start=1):
-            if images:
-                filename = unquote(res["image"].split("/")[-1].split("?")[0])
-                future = executor.submit(
-                    download_file, res["image"], path, f"{i}_{filename}"
-                )
-            else:
-                filename = unquote(res["href"].split("/")[-1].split("?")[0])
-                future = executor.submit(
-                    download_file, res["href"], path, f"{i}_{filename}"
-                )
-            futures.append(future)
-        with click.progressbar(
-            as_completed(futures),
-            label="Downloading",
-            length=len(futures),
-            show_percent=True,
-            show_pos=True,
-            width=0,
-        ) as as_completed_futures:
-            for i, future in enumerate(as_completed_futures, start=1):
-                logger.info("%s/%s", i, len(results))
+
+    tasks = []
+    sem = asyncio.Semaphore(20)
+    for i, res in enumerate(results, start=1):
+        if images:
+            filename = unquote(res["image"].split("/")[-1].split("?")[0])
+            task = asyncio.create_task(
+                download_file(res["image"], path, f"{i}_{filename}", sem)
+            )
+        else:
+            filename = unquote(res["href"].split("/")[-1].split("?")[0])
+            task = asyncio.create_task(
+                download_file(res["href"], path, f"{i}_{filename}", sem)
+            )
+        tasks.append(task)
+
+    with click.progressbar(
+        length=len(tasks),
+        label="Downloading",
+        show_percent=True,
+        show_pos=True,
+        width=50,
+    ) as bar:
+        for future in asyncio.as_completed(tasks):
+            await future
+            bar.update(1)
+
+    await asyncio.gather(*tasks)
+
+
+def download_results(keywords, results, images=False):
+    asyncio.run(_download_results(keywords, results, images))
 
 
 @click.group(chain=True)
 def cli():
     pass
```

### Comparing `duckduckgo_search-3.8.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.8.1/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.8.1/duckduckgo_search/duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,18 @@
 
     def _normalize(self, raw_html: str) -> str:
         """strip HTML tags"""
         if raw_html:
             return unescape(re.sub(REGEX_STRIP_TAGS, "", raw_html))
         return ""
 
+    def _normalize_url(self, url: str) -> str:
+        """unquote url and replace spaces with '+'"""
+        return unquote(url).replace(" ", "+")
+
     def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         backend: str = "api",
@@ -217,15 +221,15 @@
                 ):
                     cache.add(href)
                     body = self._normalize(row["a"])
                     if body:
                         result_exists = True
                         yield {
                             "title": self._normalize(row["t"]),
-                            "href": href,
+                            "href": self._normalize_url(href),
                             "body": self._normalize(body),
                         }
             if result_exists is False:
                 break
 
     def _text_html(
         self,
@@ -278,15 +282,15 @@
                 ):
                     cache.add(href)
                     title = e.xpath('.//a[contains(@class, "result__a")]/text()')
                     body = e.xpath('.//a[contains(@class, "result__snippet")]//text()')
                     result_exists = True
                     yield {
                         "title": self._normalize(title[0]) if title else None,
-                        "href": href,
+                        "href": self._normalize_url(href),
                         "body": self._normalize("".join(body)) if body else None,
                     }
 
             next_page = tree.xpath('.//div[@class="nav-link"]')
             next_page = next_page[-1] if next_page else None
             if next_page is None or result_exists is False:
                 return
@@ -350,15 +354,15 @@
                 elif i == 2:
                     body = e.xpath(".//td[@class='result-snippet']//text()")
                     body = "".join(body).strip()
                 elif i == 3:
                     result_exists = True
                     yield {
                         "title": self._normalize(title),
-                        "href": href,
+                        "href": self._normalize_url(href),
                         "body": self._normalize(body),
                     }
             if result_exists is False:
                 break
             sleep(0.75)
 
     def images(
@@ -435,17 +439,17 @@
             for row in page_data:
                 image_url = row.get("image", None)
                 if image_url and image_url not in cache:
                     cache.add(image_url)
                     result_exists = True
                     yield {
                         "title": row["title"],
-                        "image": image_url,
-                        "thumbnail": row["thumbnail"],
-                        "url": row["url"],
+                        "image": self._normalize_url(image_url),
+                        "thumbnail": self._normalize_url(row["thumbnail"]),
+                        "url": self._normalize_url(row["url"]),
                         "height": row["height"],
                         "width": row["width"],
                         "source": row["source"],
                     }
             next = resp_json.get("next", None)
             if next:
                 payload["s"] = next.split("s=")[-1].split("&")[0]
@@ -573,21 +577,22 @@
             if page_data is None:
                 break
 
             result_exists = False
             for row in page_data:
                 if row["url"] not in cache:
                     cache.add(row["url"])
+                    image_url = row.get("image", None)
                     result_exists = True
                     yield {
                         "date": datetime.utcfromtimestamp(row["date"]).isoformat(),
                         "title": row["title"],
                         "body": self._normalize(row["excerpt"]),
-                        "url": row["url"],
-                        "image": row.get("image", None),
+                        "url": self._normalize_url(row["url"]),
+                        "image": self._normalize_url(image_url) if image_url else None,
                         "source": row["source"],
                     }
             next = resp_json.get("next", None)
             if next:
                 payload["s"] = next.split("s=")[-1].split("&")[0]
             if not result_exists or not next:
                 break
@@ -823,19 +828,19 @@
                 result.title = res["name"]
                 result.address = res["address"]
                 if f"{result.title} {result.address}" in cache:
                     continue
                 else:
                     cache.add(f"{result.title} {result.address}")
                     result.country_code = res["country_code"]
-                    result.url = res["website"]
+                    result.url = self._normalize_url(res["website"])
                     result.phone = res["phone"]
                     result.latitude = res["coordinates"]["latitude"]
                     result.longitude = res["coordinates"]["longitude"]
-                    result.source = unquote(res["url"])
+                    result.source = self._normalize_url(res["url"])
                     if res["embed"]:
                         result.image = res["embed"].get("image", "")
                         result.links = res["embed"].get("third_party_links", "")
                         result.desc = res["embed"].get("description", "")
                     result.hours = res["hours"]
                     yield result.__dict__
```

### Comparing `duckduckgo_search-3.8.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.8.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.8.0
+Version: 3.8.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -62,14 +62,16 @@
 ```python3
 # text search
 ddgs text -k 'ayrton senna'
 # find and download pdf files
 ddgs text -k "russia filetype:pdf" -m 50 -d
 # find and download xls files from a specific site
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
+# find and download any xls files from a specific site
+ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
 ```
 [Go To TOP](#TOP)
 
@@ -182,15 +184,15 @@
 with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
     for r in ddgs.text("something you need"):
         print(r)
 ```
 
 [Go To TOP](#TOP)
 
-## 1. text() - text search by by duckduckgo.com
+## 1. text() - text search by duckduckgo.com
 `html` and `lite` backend differ from `api`:</br>
 * don't do an extra request first to get vqd,</br>
 * use POST requests,</br>
 * pause 0.75 seconds between paginations.</br>
 
 If you use `html` or `lite` backend, pause at least 0.75 seconds between text() calls. 
 Otherwise the site will return a 403 status code after a few requests and block your ip for a few seconds.
```

### Comparing `duckduckgo_search-3.8.0/pyproject.toml` & `duckduckgo_search-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.8.1/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

