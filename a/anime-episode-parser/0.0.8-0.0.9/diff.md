# Comparing `tmp/anime_episode_parser-0.0.8.tar.gz` & `tmp/anime_episode_parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anime_episode_parser-0.0.8.tar", max compression
+gzip compressed data, was "anime_episode_parser-0.0.9.tar", max compression
```

## Comparing `anime_episode_parser-0.0.8.tar` & `anime_episode_parser-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1117 2023-03-26 10:49:40.552307 anime_episode_parser-0.0.8/LICENSE
--rw-r--r--   0        0        0      603 2023-03-26 10:49:40.552307 anime_episode_parser-0.0.8/README.md
--rw-r--r--   0        0        0     3014 2023-03-26 10:49:40.552307 anime_episode_parser-0.0.8/anime_episode_parser/__init__.py
--rw-r--r--   0        0        0     1279 2023-03-26 10:49:40.552307 anime_episode_parser-0.0.8/anime_episode_parser/cn.py
--rw-r--r--   0        0        0     2560 2023-03-26 10:49:40.552307 anime_episode_parser-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 anime_episode_parser-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-25 22:13:48.530092 anime_episode_parser-0.0.9/LICENSE
+-rw-r--r--   0        0        0      603 2023-04-25 22:13:48.530092 anime_episode_parser-0.0.9/README.md
+-rw-r--r--   0        0        0     3116 2023-04-25 22:13:48.530092 anime_episode_parser-0.0.9/anime_episode_parser/__init__.py
+-rw-r--r--   0        0        0     1279 2023-04-25 22:13:48.530092 anime_episode_parser-0.0.9/anime_episode_parser/cn.py
+-rw-r--r--   0        0        0     2560 2023-04-25 22:13:48.530092 anime_episode_parser-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 anime_episode_parser-0.0.9/PKG-INFO
```

### Comparing `anime_episode_parser-0.0.8/LICENSE` & `anime_episode_parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anime_episode_parser-0.0.8/README.md` & `anime_episode_parser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `anime_episode_parser-0.0.8/anime_episode_parser/__init__.py` & `anime_episode_parser-0.0.9/anime_episode_parser/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,23 +54,23 @@
     spare = None
 
     _ = _EPISODE_RANGE_ALL_ZH_1.findall(episode_title)
     if _ and _[0]:
         return None, None
 
     _ = _EPISODE_RANGE_ALL_ZH_2.findall(episode_title)
-    if _ and _[0]:
+    if _ and _[0] and (int(_[0][0]) < int(_[0][1])):
         return episode_range(_)
 
     _ = _EPISODE_RANGE.findall(episode_title)
-    if _ and _[0]:
+    if _ and _[0] and (int(_[0][0]) < int(_[0][1])):
         return episode_range(_)
 
     _ = _EPISODE_RANGE_ZH.findall(episode_title)
-    if _ and _[0]:
+    if _ and _[0] and (int(_[0][0]) < int(_[0][1])):
         return int(_[0]), int(_[1]) - int(_[0])
 
     _ = _EPISODE_ZH.findall(episode_title)
     if _ and _[0].isdigit():
         return int(_[0]), 1
 
     _ = _EPISODE_ALL_ZH.findall(episode_title)
```

### Comparing `anime_episode_parser-0.0.8/anime_episode_parser/cn.py` & `anime_episode_parser-0.0.9/anime_episode_parser/cn.py`

 * *Files identical despite different names*

### Comparing `anime_episode_parser-0.0.8/pyproject.toml` & `anime_episode_parser-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "anime-episode-parser"
-version = "0.0.8"
+version = "0.0.9"
 description = 'A library to parse episode info from anime title'
 authors = ["Trim21 <trim21.me@gmail.com>", "RicterZ <ricterzheng@gmail.com>"]
 readme = 'README.md'
 license = 'MIT'
 homepage = 'https://github.com/BGmi/anime-episode-parser'
 repository = 'https://github.com/BGmi/anime-episode-parser'
 keywords = ['anime']
```

### Comparing `anime_episode_parser-0.0.8/PKG-INFO` & `anime_episode_parser-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anime-episode-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library to parse episode info from anime title
 Home-page: https://github.com/BGmi/anime-episode-parser
 License: MIT
 Keywords: anime
 Author: Trim21
 Author-email: trim21.me@gmail.com
 Requires-Python: >=3.7,<4.0
```

