# Comparing `tmp/moonrise-1.1.0.tar.gz` & `tmp/moonrise-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonrise-1.1.0.tar", last modified: Wed May 24 17:42:04 2023, max compression
+gzip compressed data, was "moonrise-1.1.1.tar", last modified: Sat Jun  3 21:47:22 2023, max compression
```

## Comparing `moonrise-1.1.0.tar` & `moonrise-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.544958 moonrise-1.1.0/
--rw-rw-rw-   0        0        0     1103 2023-05-01 03:19:38.000000 moonrise-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6448 2023-05-24 17:42:04.544958 moonrise-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5878 2023-05-15 20:49:18.000000 moonrise-1.1.0/README.md
--rw-rw-rw-   0        0        0      104 2023-05-01 03:19:38.000000 moonrise-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      846 2023-05-24 17:42:04.547958 moonrise-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.480956 moonrise-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.511958 moonrise-1.1.0/src/moonrise/
--rw-rw-rw-   0        0        0     6864 2023-05-23 21:39:47.000000 moonrise-1.1.0/src/moonrise/Base_Test.py
--rw-rw-rw-   0        0        0     5711 2023-05-22 01:31:15.000000 moonrise-1.1.0/src/moonrise/Moon_Browser.py
--rw-rw-rw-   0        0        0     6562 2023-05-15 15:31:11.000000 moonrise-1.1.0/src/moonrise/Moon_Methods.py
--rw-rw-rw-   0        0        0     2053 2023-05-22 01:31:15.000000 moonrise-1.1.0/src/moonrise/Moon_Movie.py
--rw-rw-rw-   0        0        0     1876 2023-05-15 20:38:47.000000 moonrise-1.1.0/src/moonrise/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-05-11 19:30:47.000000 moonrise-1.1.0/src/moonrise/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:42:04.542960 moonrise-1.1.0/src/moonrise.egg-info/
--rw-rw-rw-   0        0        0     6448 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 17:42:04.000000 moonrise-1.1.0/src/moonrise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.516444 moonrise-1.1.1/
+-rw-rw-rw-   0        0        0     1103 2023-05-01 03:19:38.000000 moonrise-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6448 2023-06-03 21:47:22.517445 moonrise-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5878 2023-05-15 20:49:18.000000 moonrise-1.1.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-01 03:19:38.000000 moonrise-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      846 2023-06-03 21:47:22.529445 moonrise-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.441448 moonrise-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.470447 moonrise-1.1.1/src/moonrise/
+-rw-rw-rw-   0        0        0     6864 2023-05-23 21:39:47.000000 moonrise-1.1.1/src/moonrise/Base_Test.py
+-rw-rw-rw-   0        0        0     6040 2023-06-02 13:56:46.000000 moonrise-1.1.1/src/moonrise/Moon_Browser.py
+-rw-rw-rw-   0        0        0     6562 2023-05-15 15:31:11.000000 moonrise-1.1.1/src/moonrise/Moon_Methods.py
+-rw-rw-rw-   0        0        0     2126 2023-06-02 13:56:46.000000 moonrise-1.1.1/src/moonrise/Moon_Movie.py
+-rw-rw-rw-   0        0        0     1876 2023-05-15 20:38:47.000000 moonrise-1.1.1/src/moonrise/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-05-11 19:30:47.000000 moonrise-1.1.1/src/moonrise/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.514443 moonrise-1.1.1/src/moonrise.egg-info/
+-rw-rw-rw-   0        0        0     6448 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/top_level.txt
```

### Comparing `moonrise-1.1.0/LICENSE` & `moonrise-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/PKG-INFO` & `moonrise-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.0
+Version: 1.1.1
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moonrise-1.1.0/README.md` & `moonrise-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/setup.cfg` & `moonrise-1.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6f 6e72 6973 650d 0a76 6572   = moonrise..ver
-00000020: 7369 6f6e 203d 2031 2e31 2e30 0d0a 6175  sion = 1.1.0..au
+00000020: 7369 6f6e 203d 2031 2e31 2e31 0d0a 6175  sion = 1.1.1..au
 00000030: 7468 6f72 203d 2043 6872 6973 746f 7068  thor = Christoph
 00000040: 6572 2044 6961 6d6f 6e64 2d4a 6f6e 6573  er Diamond-Jones
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2063 6872 6973 746f 7068 6572 2e6a 6f6e   christopher.jon
 00000070: 6573 3131 3338 4067 6d61 696c 2e63 6f6d  es1138@gmail.com
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5465 7374 2073 7569 7465 2063 7265 6174  Test suite creat
```

### Comparing `moonrise-1.1.0/src/moonrise/Base_Test.py` & `moonrise-1.1.1/src/moonrise/Base_Test.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/src/moonrise/Moon_Browser.py` & `moonrise-1.1.1/src/moonrise/Moon_Browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 
 
 class MoonBrowser:
 
     moon_driver = None
     video_thread = None
 
-    def open_browser(self, browser_type, *browser_args, persist=False, record_test=True):
+    def open_browser(self, browser_type, *browser_args, persist=False, record_test=True, shutter_speed=0.05):
         """Opens a selenium browser of a specified browser type
            Arguments:
            - browser_type: The desired browser (Chrome, Firefox, Edge, or IE).
            - browser_args: Selenium browser arguments, e.g. --headless.
            - persist: If set to True, will keep the browser open for later use.
            - record_test: If set to True, will create a video recording during the time that the browser is open.
+           - shutter_speed: The delay in seconds between screenshots taken for the purpose of creating the video recording.
+           Default is 0.05 seconds, or one screenshot every 20th of a second.
+           Lower values wil result in more detailed videos, but larger performance hits.
 
            Creates class variable moon_driver for access to selenium webdriver methods.
         """ 
 
         browser_options = {
             'edge': {
                 'options': webdriver.EdgeOptions(),
@@ -58,15 +61,15 @@
         self.moon_driver = browser_options[browser_type]['webdriver_create'](options=options)
 
         # Creates VideoThread object.
         if persist != True and record_test == True:
             # Stops any previously running screenshot threads
             if self.video_thread:
                 self.video_thread.stop()
-            self.video_thread = VideoThread(self.moon_driver)
+            self.video_thread = VideoThread(self.moon_driver, shutter_speed)
             if self.video_folder:
                 self.video_thread.video_folder = self.video_folder
 
         # write executor_url and session_id to a file named session_info.py for future use
         try:
             session_info_file = open(os.path.dirname(os.path.realpath(__file__))+'/session_info.py', 'w')
             session_info_file.write(f'executor_url="{self.moon_driver.command_executor._url}"\nsession_id="{self.moon_driver.session_id}"')
```

### Comparing `moonrise-1.1.0/src/moonrise/Moon_Methods.py` & `moonrise-1.1.1/src/moonrise/Moon_Methods.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/src/moonrise/Moon_Movie.py` & `moonrise-1.1.1/src/moonrise/Moon_Movie.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 from datetime import datetime
 import os
 import ffmpeg
 
 class VideoThread(threading.Thread):
     """Creates a new thread that handles the creation of video recordings for browser sessions.
     """
-    def __init__(self, driver):
+    def __init__(self, driver, shutter_speed):
         """Receives a webdriver to create an additional thread where screenshots are taken during test execution.
            These screenshots are converted to an mp4 file when the webdriver is killed or after the moonrise test execution has completed.
         """
         threading.Thread.__init__(self)
         self.stop_event = threading.Event()
         self.driver = driver
         self.video_folder = None
+        self.shutter_speed = shutter_speed
         self.start()
 
     def run(self):
         while not self.stop_event.is_set():
             try:
                 timestamp = str(datetime.now()).replace(" ", "_").replace(":", "_")
                 self.driver.save_screenshot(f"{self.video_folder}/{timestamp}.png")
-                time.sleep(0.05)
+                time.sleep(self.shutter_speed)
             except Exception:
                 self.stop()
 
     def stop(self):
         self.stop_event.set()
 
     def create_video_from_pngs(self, output_file):
```

### Comparing `moonrise-1.1.0/src/moonrise/__init__.py` & `moonrise-1.1.1/src/moonrise/__init__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/src/moonrise/__main__.py` & `moonrise-1.1.1/src/moonrise/__main__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.0/src/moonrise.egg-info/PKG-INFO` & `moonrise-1.1.1/src/moonrise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.0
+Version: 1.1.1
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

