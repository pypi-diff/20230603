# Comparing `tmp/bondzai.media-handler-0.0.11.tar.gz` & `tmp/bondzai.media-handler-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.media-handler-0.0.11.tar", last modified: Fri Jun  2 23:30:30 2023, max compression
+gzip compressed data, was "bondzai.media-handler-0.0.12.tar", last modified: Sat Jun  3 00:12:51 2023, max compression
```

## Comparing `bondzai.media-handler-0.0.11.tar` & `bondzai.media-handler-0.0.12.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-02 23:30:30.979911 bondzai.media-handler-0.0.11/
--rw-r--r--   0 theo       (501) staff       (20)     1273 2023-05-30 21:40:00.000000 bondzai.media-handler-0.0.11/LICENCE.txt
--rw-r--r--   0 theo       (501) staff       (20)     1614 2023-06-02 23:30:30.980006 bondzai.media-handler-0.0.11/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1246 2023-06-02 23:30:18.000000 bondzai.media-handler-0.0.11/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-02 23:30:30.976797 bondzai.media-handler-0.0.11/bondzai/
--rw-r--r--   0 theo       (501) staff       (20)      243 2023-05-30 21:18:51.000000 bondzai.media-handler-0.0.11/bondzai/__init__.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-02 23:30:30.979378 bondzai.media-handler-0.0.11/bondzai/media_handler/
--rw-r--r--   0 theo       (501) staff       (20)     1116 2023-06-02 23:29:43.000000 bondzai.media-handler-0.0.11/bondzai/media_handler/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      664 2023-06-02 23:29:19.000000 bondzai.media-handler-0.0.11/bondzai/media_handler/audio.py
--rw-r--r--   0 theo       (501) staff       (20)      661 2023-06-01 17:38:23.000000 bondzai.media-handler-0.0.11/bondzai/media_handler/base.py
--rw-r--r--   0 theo       (501) staff       (20)      888 2023-06-02 23:29:27.000000 bondzai.media-handler-0.0.11/bondzai/media_handler/image.py
--rw-r--r--   0 theo       (501) staff       (20)      868 2023-06-02 23:29:35.000000 bondzai.media-handler-0.0.11/bondzai/media_handler/video.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-02 23:30:30.977938 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)     1614 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      542 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       79 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-02 23:30:30.000000 bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-05-30 10:20:03.000000 bondzai.media-handler-0.0.11/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      576 2023-06-02 23:30:30.980425 bondzai.media-handler-0.0.11/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-03 00:12:51.204628 bondzai.media-handler-0.0.12/
+-rw-r--r--   0 theo       (501) staff       (20)     1273 2023-05-30 21:40:00.000000 bondzai.media-handler-0.0.12/LICENCE.txt
+-rw-r--r--   0 theo       (501) staff       (20)     1614 2023-06-03 00:12:51.204788 bondzai.media-handler-0.0.12/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1246 2023-06-02 23:30:18.000000 bondzai.media-handler-0.0.12/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-03 00:12:51.200074 bondzai.media-handler-0.0.12/bondzai/
+-rw-r--r--   0 theo       (501) staff       (20)      243 2023-05-30 21:18:51.000000 bondzai.media-handler-0.0.12/bondzai/__init__.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-03 00:12:51.203246 bondzai.media-handler-0.0.12/bondzai/media_handler/
+-rw-r--r--   0 theo       (501) staff       (20)     1116 2023-06-03 00:12:32.000000 bondzai.media-handler-0.0.12/bondzai/media_handler/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)      616 2023-06-03 00:11:10.000000 bondzai.media-handler-0.0.12/bondzai/media_handler/audio.py
+-rw-r--r--   0 theo       (501) staff       (20)      661 2023-06-01 17:38:23.000000 bondzai.media-handler-0.0.12/bondzai/media_handler/base.py
+-rw-r--r--   0 theo       (501) staff       (20)      757 2023-06-03 00:11:53.000000 bondzai.media-handler-0.0.12/bondzai/media_handler/image.py
+-rw-r--r--   0 theo       (501) staff       (20)      820 2023-06-03 00:12:01.000000 bondzai.media-handler-0.0.12/bondzai/media_handler/video.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-06-03 00:12:51.201177 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)     1614 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      542 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       79 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-06-03 00:12:51.000000 bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-05-30 10:20:03.000000 bondzai.media-handler-0.0.12/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      576 2023-06-03 00:12:51.205394 bondzai.media-handler-0.0.12/setup.cfg
```

### Comparing `bondzai.media-handler-0.0.11/LICENCE.txt` & `bondzai.media-handler-0.0.12/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.11/PKG-INFO` & `bondzai.media-handler-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.media-handler
-Version: 0.0.11
+Version: 0.0.12
 Summary: Bondzai Media Handler
 Home-page: UNKNOWN
 Author: Bondzai
 License: UNKNOWN
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.media-handler-0.0.11/README.rst` & `bondzai.media-handler-0.0.12/README.rst`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.11/bondzai/media_handler/__init__.py` & `bondzai.media-handler-0.0.12/bondzai/media_handler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .base import get_file_mime, load_binary, save_binary
 from .audio import AUDIO_ALLOWED_MIME, get_audio_metadata, get_audio_raw_data
 from .image import IMAGE_ALLOWED_MIME, get_image_metadata, get_image_raw_data
 from .video import VIDEO_ALLOWED_MIME, get_video_metadata, get_video_raw_data
 
 
-VERSION = "0.0.11"
+VERSION = "0.0.12"
 
 
 def get_raw_data(file_path: Path) -> list[float]:
     mime = get_file_mime(file_path)
     if mime in AUDIO_ALLOWED_MIME:
         return get_audio_raw_data(file_path)
     elif mime in IMAGE_ALLOWED_MIME:
```

### Comparing `bondzai.media-handler-0.0.11/bondzai/media_handler/audio.py` & `bondzai.media-handler-0.0.12/bondzai/media_handler/audio.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,11 +19,10 @@
         "mime": mime,
         "sample_rate": audio["streaminfo"].sample_rate,
         "channels": audio["streaminfo"].channels
     }
 
 
 def get_audio_raw_data(file_path: Path) -> list[float]:
-    # check_mime(file_path, AUDIO_ALLOWED_MIME)
     with open(file_path, 'rb') as f:
         data, _ = sf.read(f)
     return data.flatten().tolist()
```

### Comparing `bondzai.media-handler-0.0.11/bondzai/media_handler/base.py` & `bondzai.media-handler-0.0.12/bondzai/media_handler/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.11/bondzai/media_handler/image.py` & `bondzai.media-handler-0.0.12/bondzai/media_handler/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
-from imageio.v3 import imread, immeta, improps, imopen
-import cv2
+from imageio.v3 import imread, immeta, improps
 
 from .base import check_mime
 
 
 IMAGE_ALLOWED_MIME = [
     "image/jpeg",
     "image/png",
@@ -22,18 +21,15 @@
         "height": img['shape'][1],
         "mode": img['mode'],
         "dim": props.shape
     }
 
 
 def get_image_raw_data(file_path: Path) -> list[float]:
-    # check_mime(file_path, IMAGE_ALLOWED_MIME)
-    with imopen(file_path, "r") as f:
-        return f.read()
-    # return process_raw_img_data(imread(file_path))
+    return process_raw_img_data(imread(file_path))
 
 
 def process_raw_img_data(data) -> list[float]:
     data = data.astype("float32")\
         .flatten()\
         .tolist()
     return data
```

### Comparing `bondzai.media-handler-0.0.11/bondzai/media_handler/video.py` & `bondzai.media-handler-0.0.12/bondzai/media_handler/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,13 +24,12 @@
         "fps": img['fps'],
         "channels": props.shape[-1],
         "dim": props.shape
     }
 
 
 def get_video_raw_data(file_path: Path) -> list[float]:
-    # check_mime(file_path, VIDEO_ALLOWED_MIME)
     video = imageio.get_reader(file_path) 
     results = []
     for frame in video.iter_data(): 
         results += process_raw_img_data(frame[0])
     return results
```

### Comparing `bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/PKG-INFO` & `bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.media-handler
-Version: 0.0.11
+Version: 0.0.12
 Summary: Bondzai Media Handler
 Home-page: UNKNOWN
 Author: Bondzai
 License: UNKNOWN
 Keywords: davinsy,bondzai
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.media-handler-0.0.11/bondzai.media_handler.egg-info/SOURCES.txt` & `bondzai.media-handler-0.0.12/bondzai.media_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.11/setup.cfg` & `bondzai.media-handler-0.0.12/setup.cfg`

 * *Files identical despite different names*

