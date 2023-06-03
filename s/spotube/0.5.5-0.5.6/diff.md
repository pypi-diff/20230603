# Comparing `tmp/spotube-0.5.5.tar.gz` & `tmp/spotube-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotube-0.5.5.tar", max compression
+gzip compressed data, was "spotube-0.5.6.tar", max compression
```

## Comparing `spotube-0.5.5.tar` & `spotube-0.5.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3184 2023-06-03 14:15:43.647479 spotube-0.5.5/LICENSE
--rw-r--r--   0        0        0     6178 2023-06-03 14:15:43.647479 spotube-0.5.5/README.md
--rw-r--r--   0        0        0      742 2023-06-03 14:19:44.326730 spotube-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/__init__.py
--rw-r--r--   0        0        0     3196 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/downloader_class.py
--rw-r--r--   0        0        0    15584 2023-06-03 14:15:43.647479 spotube-0.5.5/spotube/downloader_utils.py
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 spotube-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     3184 2023-06-03 14:20:17.592777 spotube-0.5.6/LICENSE
+-rw-r--r--   0        0        0     6182 2023-06-03 14:20:17.592777 spotube-0.5.6/README.md
+-rw-r--r--   0        0        0      742 2023-06-03 14:24:49.067513 spotube-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/__init__.py
+-rw-r--r--   0        0        0     3638 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/downloader_class.py
+-rw-r--r--   0        0        0    15914 2023-06-03 14:20:17.592777 spotube-0.5.6/spotube/downloader_utils.py
+-rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 spotube-0.5.6/PKG-INFO
```

### Comparing `spotube-0.5.5/LICENSE` & `spotube-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spotube-0.5.5/README.md` & `spotube-0.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,18 +101,18 @@
 
 ```
 my_downloaded = set_directory("./Songs")
 ```
 
 ### Stopping the Downloader
 
-You can stop the download process using the `stop_downloader` method on a downloader object:
+You can stop the download process using the `cancel_downloader` method on a downloader object:
 
 ```
-my_downloaded = stop_downloader()
+my_downloaded = cancel_downloader()
 ```
 
 This will reset all download information, like the ETA and progress.
 
 ### Validate Playlist URL
 
 You can examine if a Spotify playlist URL is valid by using the `validate_playlist_url` method:
```

### Comparing `spotube-0.5.5/pyproject.toml` & `spotube-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotube"
-version = "0.5.5"
+version = "0.5.6"
 description = "A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs."
 authors = ["GiorgosNik <giorgosnl17@gmail.com>"]
 license = "Free for non-commercial use"
 readme = "README.md"
 repository = 'https://github.com/GiorgosNik/spotube-package'
 packages = [{include = "spotube"}]
```

### Comparing `spotube-0.5.5/spotube/downloader_class.py` & `spotube-0.5.6/spotube/downloader_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import threading
 import queue
 from . import downloader_utils as utils
 import os
 import subprocess
 from zipfile import ZipFile
 import urllib.request
+import shutil
 
 class downloader:
     def __init__(
         self,
         spotify_client_id,
         spotify_client_secret,
         genius_api_key,
@@ -23,14 +24,16 @@
         self.eta = None
         self.thread = None
         self.spotify_client_id = spotify_client_id
         self.spotify_client_secret = spotify_client_secret
         self.genius_api_key = genius_api_key
         self.directory = directory
         self.display_bar = display_bar
+        self.success_counter = 0
+        self.fail_counter = 0
 
         # Set the channel that will handle the messages from the worker
         self.channel = queue.Queue()
 
         # Set the channel that will handle the messages from the worker
         self.termination_channel = queue.Queue()
 
@@ -58,32 +61,36 @@
                 self.directory,
                 self.display_bar
             ],
         )
         self.working = True
         self.thread.start()
 
-    def stop_downloader(self):
+    def cancel_downloader(self):
         self.termination_channel.put("EXIT")
 
         # Wait for thread to exit
         if self.thread is not None:
             self.thread.join()
 
         self.working = False
         self.progress = 0
         self.total = None
         self.current_song = None
         self.eta = None
         self.thread = None
         self.channel = queue.Queue()
         self.termination_channel = queue.Queue()
+        self.success_counter = 0
+        self.fail_counter = 0
         self.tokens = utils.auth_handler(
             self.spotify_client_id, self.spotify_client_secret, self.genius_api_key
         )
+        if os.path.isdir(self.directory):
+            shutil.rmtree(self.directory)
 
     def validate_playlist_url(self, playlist_url):
         try:
             self.tokens["spotify"].playlist_items(
                 playlist_url, additional_types=("track",)
             )
         except Exception:
@@ -104,8 +111,16 @@
 
     def get_eta(self):
         utils.fetch_messages(self)
         return self.eta
 
     def downloader_active(self):
         utils.fetch_messages(self)
-        return self.working
+        return self.working
+    
+    def get_success_counter(self):
+        utils.fetch_messages(self)
+        return self.success_counter
+    
+    def get_fail_counter(self):
+        utils.fetch_messages(self)
+        return self.fail_counter
```

### Comparing `spotube-0.5.5/spotube/downloader_utils.py` & `spotube-0.5.6/spotube/downloader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from zipfile import ZipFile
 import subprocess
 from pydub import AudioSegment
 import urllib.request
 from platform import machine
 import tarfile
 import zipfile
+from pathlib import Path
 
-
+COVER_PHOTO = "/cover_photo.jpg"
 FFMPEG_UNIX_X64 = "https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linux64-gpl.tar.xz"
 FFMPEG_UNIX_ARM = "https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-linuxarm64-gpl.tar.xz"
 FFMPEG_WINDOWS_X64 = "https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip"
 FFMPEG_WINDOWS_X86 = "https://github.com/yt-dlp/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win32-gpl.zip"
 
 
 def get_lyrics(name_search, artist_search, genius_obj):
@@ -47,15 +48,15 @@
 def set_tags(song_info, genius_obj, directory):
     audio_file = eyed3.load(directory + "/" + song_info["name"] + ".mp3")
 
     if audio_file.tag is None:
         audio_file.initTag()
 
     audio_file.tag.images.set(
-        3, open(directory + "/cover_photo.jpg", "rb").read(), "image/jpeg"
+        3, open(directory + COVER_PHOTO, "rb").read(), "image/jpeg"
     )
     formatted_artist_string = song_info["artist"].replace(",", ";")
     audio_file.tag.artist = formatted_artist_string
     audio_file.tag.title = song_info["name"]
     audio_file.tag.album = song_info["album"]
     audio_file.tag.year = song_info["year"]
 
@@ -63,15 +64,15 @@
         audio_file.tag.lyrics.set(
             get_lyrics(song_info["name"], song_info["artist"], genius_obj)
         )
     except Exception:
         pass
 
     audio_file.tag.save()
-    os.remove(directory + "/cover_photo.jpg")
+    os.remove(directory + COVER_PHOTO)
 
 
 def format_artists(artist_list):
     artist_combined = ""
 
     for artist_in_list in artist_list:
         if artist_combined != "":
@@ -100,15 +101,15 @@
     return best_link
 
 
 def download_image(song_info, directory):
     # Get the Cover Art
     image_url = song_info["url"]
     r = requests.get(image_url)
-    with open(directory + "/cover_photo.jpg", "wb") as f:
+    with open(directory + COVER_PHOTO, "wb") as f:
         f.write(r.content)
 
 
 def download_song(given_link, song_info, downloader, directory):
     attempts = 0
 
     while attempts <= 3:
@@ -181,43 +182,46 @@
 
 
 def download_playlist(
     playlist_url, tokens, channel, termination_channel, directory, display_bar=True
 ):
     # Set up the folder for the songs
     if not os.path.isdir(directory):
-        os.mkdir(directory)
+        Path(directory).mkdir(parents=True, exist_ok=True)
 
     audio_downloader = create_audio_downloader(directory)
 
     songs = get_songs(playlist_url, tokens["spotify"])
 
     if display_bar:
-        file = None
+        filename = None
     else:
-        file = open(os.devnull, "w")
+        filename = open(os.devnull, "w")
 
     # Set the tqdm progress bar
     playlist_size = len(songs)
     playlist_progress = tqdm(
         total=playlist_size,
         desc="Playlist Progress",
         position=0,
         leave=False,
-        file=file,
+        file=filename,
     )
 
+    success_counter = 0
+    failure_counter = 0
+
     for song in songs:
         # Set song progress bar
         song_progress = tqdm(
             total=4,
             desc=song["track"]["name"],
             position=1,
             leave=False,
-            file=file,
+            file=filename,
         )
 
         # Retrieve Formatted Song Data
         song_progress.set_description(song_progress.desc + ": Formatting Information")
         song_progress.update(n=1)
         info_dict = format_song_data(song)
 
@@ -252,26 +256,28 @@
             set_tags(info_dict, tokens["genius"], directory)
 
             # Move to the designated folder
             song_progress.set_description(
                 info_dict["name"] + ": Moving to designated folder"
             )
             song_progress.update(n=1)
+            success_counter += 1
 
         except Exception as e:  # pragma: no cover
+            failure_counter += 1
             print(str(e))
             continue
         song_progress.close()
 
         # Update tqdm progress bar
         playlist_progress.update(n=1)
         send_message(
             channel,
             type="progress",
-            contents=[playlist_progress.n, playlist_progress.total],
+            contents=[playlist_progress.n, playlist_progress.total, success_counter, failure_counter],
         )
 
         elapsed = get_elapsed(playlist_progress)
         eta = get_eta(playlist_progress)
         send_message(channel, type="eta_update", contents=[elapsed, eta])
 
         # Check for termination message
@@ -368,14 +374,16 @@
 # Save the state of the worker thread based on the message
 def handle_message(downloader, message):
     contents = message["contents"]
 
     if message["type"] == "progress":
         downloader.progress = contents[0]
         downloader.total = contents[1]
+        downloader.success_counter = contents[2]
+        downloader.failure_counter = contents[3]
 
     elif message["type"] == "song_title":
         downloader.current_song = contents
 
     elif message["type"] == "eta_update":
         downloader.eta = contents[1]
```

### Comparing `spotube-0.5.5/PKG-INFO` & `spotube-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotube
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Python package to download Spotify playlists locally including the cover art, metadata and lyrics by leveraging the Spotify, YouTube and Genius APIs.
 Home-page: https://github.com/GiorgosNik/spotube-package
 License: Free for non-commercial use
 Author: GiorgosNik
 Author-email: giorgosnl17@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -126,18 +126,18 @@
 
 ```
 my_downloaded = set_directory("./Songs")
 ```
 
 ### Stopping the Downloader
 
-You can stop the download process using the `stop_downloader` method on a downloader object:
+You can stop the download process using the `cancel_downloader` method on a downloader object:
 
 ```
-my_downloaded = stop_downloader()
+my_downloaded = cancel_downloader()
 ```
 
 This will reset all download information, like the ETA and progress.
 
 ### Validate Playlist URL
 
 You can examine if a Spotify playlist URL is valid by using the `validate_playlist_url` method:
```

