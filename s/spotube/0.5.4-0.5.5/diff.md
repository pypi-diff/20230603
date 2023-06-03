# Comparing `tmp/spotube-0.5.4.tar.gz` & `tmp/spotube-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotube-0.5.4.tar", max compression
+gzip compressed data, was "spotube-0.5.5.tar", max compression
```

## Comparing `spotube-0.5.4.tar` & `spotube-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3184 2023-04-23 19:06:37.024075 spotube-0.5.4/LICENSE
--rw-r--r--   0        0        0     6178 2023-04-23 19:06:37.024075 spotube-0.5.4/README.md
--rw-r--r--   0        0        0      742 2023-04-23 19:10:07.551084 spotube-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       40 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/__init__.py
--rw-r--r--   0        0        0     3196 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/downloader_class.py
--rw-r--r--   0        0        0    15638 2023-04-23 19:06:37.024075 spotube-0.5.4/spotube/downloader_utils.py
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     3184 2023-06-03 14:15:43.647479 spotube-0.5.5/LICENSE
+-rw-r--r--   0        0        0     6178 2023-06-03 14:15:43.647479 spotube-0.5.5/README.md
+-rw-r--r--   0        0        0      742 2023-06-03 14:19:44.326730 spotube-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/__init__.py
+-rw-r--r--   0        0        0     3196 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/downloader_class.py
+-rw-r--r--   0        0        0    15584 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/downloader_utils.py
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.5/PKG-INFO
```

### Comparing `spotube-0.5.4/LICENSE` & `spotube-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spotube-0.5.4/README.md` & `spotube-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `spotube-0.5.4/pyproject.toml` & `spotube-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotube"
-version = "0.5.4"
+version = "0.5.5"
 description = "A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs."
 authors = ["GiorgosNik <giorgosnl17@gmail.com>"]
 license = "Free for non-commercial use"
 readme = "README.md"
 repository = 'https://github.com/GiorgosNik/spotube-package'
 packages = [{include = "spotube"}]
```

### Comparing `spotube-0.5.4/spotube/downloader_class.py` & `spotube-0.5.5/spotube/downloader_class.py`

 * *Files identical despite different names*

### Comparing `spotube-0.5.4/spotube/downloader_utils.py` & `spotube-0.5.5/spotube/downloader_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,20 @@
 
 def download_song(given_link, song_info, downloader, directory):
     attempts = 0
 
     while attempts <= 3:
         try:
             downloader.extract_info(given_link)
-            list_of_files = glob.glob(directory + "/*.mp3")
-            latest_file = max(list_of_files, key=os.path.getctime)
+            default_song_name = "/downloaded_song.mp3"
 
             # Overwrite the file, if it exists
             if os.path.exists(directory + "/" + song_info["name"] + ".mp3"):
                 os.remove(directory + "/" + song_info["name"] + ".mp3")
-            os.rename(latest_file, directory + "/" + song_info["name"] + ".mp3")
+            os.rename(directory + default_song_name, directory + "/" + song_info["name"] + ".mp3")
             return
 
         except Exception as e:  # pragma: no cover
             print(str(e))
             attempts += 1
             continue
```

### Comparing `spotube-0.5.4/PKG-INFO` & `spotube-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotube
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs.
 Home-page: https://github.com/GiorgosNik/spotube-package
 License: Free for non-commercial use
 Author: GiorgosNik
 Author-email: giorgosnl17@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

