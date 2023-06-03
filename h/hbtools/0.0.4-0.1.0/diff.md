# Comparing `tmp/hbtools-0.0.4.tar.gz` & `tmp/hbtools-0.1.0.tar.gz`

## Comparing `hbtools-0.0.4.tar` & `hbtools-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 hbtools-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hbtools-0.0.4/noxfile.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/README.md
--rw-r--r--   0        0        0    18614 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements-build.txt
--rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements-flake8.txt
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements-terminal.txt
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements-test.txt
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 hbtools-0.0.4/requirements/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbtools-0.0.4/src/hbtools/__init__.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 hbtools-0.0.4/src/hbtools/logger.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hbtools-0.0.4/src/hbtools/misc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hbtools-0.0.4/src/hbtools/py.typed
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 hbtools-0.0.4/src/hbtools/show_img.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 hbtools-0.0.4/tests/test_call_fn.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hbtools-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hbtools-0.0.4/LICENSE
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hbtools-0.0.4/README.md
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 hbtools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 hbtools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 hbtools-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hbtools-0.1.0/noxfile.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/README.md
+-rw-r--r--   0        0        0    18614 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements-build.txt
+-rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements-flake8.txt
+-rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements-terminal.txt
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements-test.txt
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 hbtools-0.1.0/requirements/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbtools-0.1.0/src/hbtools/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 hbtools-0.1.0/src/hbtools/logger.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 hbtools-0.1.0/src/hbtools/misc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hbtools-0.1.0/src/hbtools/py.typed
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 hbtools-0.1.0/src/hbtools/show_img.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 hbtools-0.1.0/tests/test_call_fn.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hbtools-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hbtools-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hbtools-0.1.0/README.md
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 hbtools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 hbtools-0.1.0/PKG-INFO
```

### Comparing `hbtools-0.0.4/.pre-commit-config.yaml` & `hbtools-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/noxfile.py` & `hbtools-0.1.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/README.md` & `hbtools-0.1.0/requirements/README.md`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements-build.txt` & `hbtools-0.1.0/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements-dev.txt` & `hbtools-0.1.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements-flake8.txt` & `hbtools-0.1.0/requirements/requirements-flake8.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements-terminal.txt` & `hbtools-0.1.0/requirements/requirements-terminal.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements-test.txt` & `hbtools-0.1.0/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/requirements/requirements.txt` & `hbtools-0.1.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/src/hbtools/logger.py` & `hbtools-0.1.0/src/hbtools/logger.py`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/src/hbtools/misc.py` & `hbtools-0.1.0/src/hbtools/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,19 +20,20 @@
             print("Input invalid, please enter 'y' or 'n'")
             continue
         return answer == "y"
 
     return default
 
 
-def clean_print(msg: str, fallback: tuple[int, int] = (156, 38), end: str = "\n") -> None:
+def clean_print(msg: str, fallback: tuple[int, int] = (156, 38), end: str = "\n", **kwargs: object) -> None:
     r"""Print the given string to the console and erase any character previously written on the line.
 
     Args:
         msg: String to print to the console.
         fallback: If using Windows, size of the terminal to use if it cannot be determined by shutil.
         end: What to add at the end of the print. Usually '\n' (new line), or '\r' (back to the start of the line).
+        kwargs: Print function kwargs.
     """
     if sys.platform != "win32":
-        print("\033[2K" + msg, end=end, flush=True)
+        print("\r\033[K" + msg, end=end, flush=True, **kwargs)
     else:
-        print(msg + " " * (get_terminal_size(fallback=fallback).columns - len(msg)), end=end, flush=True)
+        print(msg + " " * (get_terminal_size(fallback=fallback).columns - len(msg)), end=end, flush=True, **kwargs)
```

### Comparing `hbtools-0.0.4/src/hbtools/show_img.py` & `hbtools-0.1.0/src/hbtools/show_img.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """Module providing function to display an image using OpenCV (or term_image as a backup)."""
 import os
+import sys
 
-try:
-    import cv2
-except ModuleNotFoundError:
-    print("Install the package with hbtools[opencv] or hbtools[opencv-headless] to use this functionality")
 import numpy as np
 import numpy.typing as npt
 
 
 def show_img(img: npt.NDArray[np.uint8], window_name: str = "Image", *, is_bgr: bool = True) -> None:
     """Display the given image.
 
@@ -16,14 +13,21 @@
     Otherwise try to display the image to the terminal.
 
     Args:
         img: The image that is to be displayed.
         window_name: The name of the window in which the image will be displayed.
         is_bgr: Should be True if the image format is BGR, False otherwise.
     """
+    try:
+        import cv2
+    except ModuleNotFoundError:
+        print("Install the package with hbtools[opencv] or hbtools[opencv-headless] to use this functionality",
+              file=sys.stderr)
+        sys.exit(-1)
+
     if "DISPLAY" in os.environ:
         # Make the image full screen if it's above a given size (assume the screen isn't too small^^)
         if any(img.shape[:2] > np.asarray([1080, 1440])):
             cv2.namedWindow(window_name, cv2.WND_PROP_FULLSCREEN)
             cv2.setWindowProperty(window_name, cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN)
 
         if not is_bgr and img.shape[2] == 3:
```

### Comparing `hbtools-0.0.4/tests/test_call_fn.py` & `hbtools-0.1.0/tests/test_call_fn.py`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/LICENSE` & `hbtools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/README.md` & `hbtools-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/pyproject.toml` & `hbtools-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.4/PKG-INFO` & `hbtools-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbtools
-Version: 0.0.4
+Version: 0.1.0
 Summary: Package containing a few python utils functions.
 Project-URL: Homepage, https://github.com/hoel-bagard/hbtools
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/hbtools/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

