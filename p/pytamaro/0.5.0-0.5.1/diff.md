# Comparing `tmp/pytamaro-0.5.0.tar.gz` & `tmp/pytamaro-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytamaro-0.5.0.tar", max compression
+gzip compressed data, was "pytamaro-0.5.1.tar", max compression
```

## Comparing `pytamaro-0.5.0.tar` & `pytamaro-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.5.0/LICENSE
--rw-r--r--   0        0        0      818 2023-05-29 07:51:55.773691 pytamaro-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      472 2023-05-29 07:51:55.777560 pytamaro-0.5.0/pytamaro/__init__.py
--rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.5.0/pytamaro/checks.py
--rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.5.0/pytamaro/color.py
--rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.5.0/pytamaro/color_functions.py
--rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.5.0/pytamaro/color_names.py
--rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.5.0/pytamaro/de/__init__.py
--rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.5.0/pytamaro/de/color.py
--rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.5.0/pytamaro/de/color_names.py
--rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.5.0/pytamaro/de/graphic.py
--rw-r--r--   0        0        0     3211 2023-05-29 07:53:52.456525 pytamaro-0.5.0/pytamaro/de/io.py
--rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.5.0/pytamaro/de/operations.py
--rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.5.0/pytamaro/de/point.py
--rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.5.0/pytamaro/de/point_names.py
--rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.5.0/pytamaro/de/primitives.py
--rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.5.0/pytamaro/debug.py
--rw-r--r--   0        0        0     8147 2023-02-27 12:54:43.441456 pytamaro-0.5.0/pytamaro/graphic.py
--rw-r--r--   0        0        0     8534 2023-05-24 07:48:53.130050 pytamaro-0.5.0/pytamaro/io.py
--rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.5.0/pytamaro/it/__init__.py
--rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.5.0/pytamaro/it/color.py
--rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.5.0/pytamaro/it/color_names.py
--rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.5.0/pytamaro/it/graphic.py
--rw-r--r--   0        0        0     2949 2023-05-24 07:12:31.769928 pytamaro-0.5.0/pytamaro/it/io.py
--rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.5.0/pytamaro/it/operations.py
--rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.5.0/pytamaro/it/point.py
--rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.5.0/pytamaro/it/point_names.py
--rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.5.0/pytamaro/it/primitives.py
--rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.5.0/pytamaro/localization.py
--rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.5.0/pytamaro/operations.py
--rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.5.0/pytamaro/point.py
--rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.5.0/pytamaro/point_names.py
--rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.5.0/pytamaro/primitives.py
--rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.5.0/pytamaro/py.typed
--rw-r--r--   0        0        0     1032 2023-04-06 12:16:34.179637 pytamaro-0.5.0/pytamaro/utils.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pytamaro-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2022-03-04 16:39:39.043278 pytamaro-0.5.1/LICENSE
+-rw-r--r--   0        0        0      818 2023-06-03 07:06:56.646268 pytamaro-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      472 2023-06-03 07:06:56.651499 pytamaro-0.5.1/pytamaro/__init__.py
+-rw-r--r--   0        0        0     3659 2023-02-27 12:54:43.437950 pytamaro-0.5.1/pytamaro/checks.py
+-rw-r--r--   0        0        0      962 2023-02-27 12:54:43.438236 pytamaro-0.5.1/pytamaro/color.py
+-rw-r--r--   0        0        0     4641 2023-02-27 12:54:43.438488 pytamaro-0.5.1/pytamaro/color_functions.py
+-rw-r--r--   0        0        0      799 2023-02-27 12:54:43.438694 pytamaro-0.5.1/pytamaro/color_names.py
+-rw-r--r--   0        0        0      456 2023-02-27 12:54:43.439015 pytamaro-0.5.1/pytamaro/de/__init__.py
+-rw-r--r--   0        0        0     3948 2023-02-27 12:54:43.439329 pytamaro-0.5.1/pytamaro/de/color.py
+-rw-r--r--   0        0        0     1093 2022-03-04 16:39:39.049297 pytamaro-0.5.1/pytamaro/de/color_names.py
+-rw-r--r--   0        0        0      445 2023-02-27 12:54:43.439701 pytamaro-0.5.1/pytamaro/de/graphic.py
+-rw-r--r--   0        0        0     3211 2023-05-29 08:23:29.417046 pytamaro-0.5.1/pytamaro/de/io.py
+-rw-r--r--   0        0        0     4206 2023-02-27 12:54:43.440314 pytamaro-0.5.1/pytamaro/de/operations.py
+-rw-r--r--   0        0        0      119 2023-02-27 12:54:43.440547 pytamaro-0.5.1/pytamaro/de/point.py
+-rw-r--r--   0        0        0     1364 2023-02-27 12:54:43.440806 pytamaro-0.5.1/pytamaro/de/point_names.py
+-rw-r--r--   0        0        0     4626 2023-02-27 12:54:43.441003 pytamaro-0.5.1/pytamaro/de/primitives.py
+-rw-r--r--   0        0        0     2643 2023-02-27 12:54:43.441184 pytamaro-0.5.1/pytamaro/debug.py
+-rw-r--r--   0        0        0     8147 2023-06-02 09:48:23.048575 pytamaro-0.5.1/pytamaro/graphic.py
+-rw-r--r--   0        0        0     9313 2023-06-03 06:56:26.725254 pytamaro-0.5.1/pytamaro/io.py
+-rw-r--r--   0        0        0      457 2023-02-27 12:54:43.441979 pytamaro-0.5.1/pytamaro/it/__init__.py
+-rw-r--r--   0        0        0     3370 2023-02-27 12:54:43.442282 pytamaro-0.5.1/pytamaro/it/color.py
+-rw-r--r--   0        0        0      923 2022-11-30 08:45:09.899740 pytamaro-0.5.1/pytamaro/it/color_names.py
+-rw-r--r--   0        0        0      459 2023-02-27 12:54:43.442558 pytamaro-0.5.1/pytamaro/it/graphic.py
+-rw-r--r--   0        0        0     2949 2023-05-29 08:23:29.417817 pytamaro-0.5.1/pytamaro/it/io.py
+-rw-r--r--   0        0        0     4512 2023-02-27 12:54:43.442887 pytamaro-0.5.1/pytamaro/it/operations.py
+-rw-r--r--   0        0        0      111 2023-02-27 12:54:43.443014 pytamaro-0.5.1/pytamaro/it/point.py
+-rw-r--r--   0        0        0     1626 2023-02-27 12:54:43.443240 pytamaro-0.5.1/pytamaro/it/point_names.py
+-rw-r--r--   0        0        0     4636 2023-02-27 12:54:43.443425 pytamaro-0.5.1/pytamaro/it/primitives.py
+-rw-r--r--   0        0        0     5786 2023-02-27 12:54:43.443621 pytamaro-0.5.1/pytamaro/localization.py
+-rw-r--r--   0        0        0     5834 2023-02-27 12:54:43.443786 pytamaro-0.5.1/pytamaro/operations.py
+-rw-r--r--   0        0        0     1900 2023-02-27 12:54:43.443994 pytamaro-0.5.1/pytamaro/point.py
+-rw-r--r--   0        0        0     1233 2023-02-27 12:54:43.444184 pytamaro-0.5.1/pytamaro/point_names.py
+-rw-r--r--   0        0        0     4997 2023-02-27 12:54:43.444392 pytamaro-0.5.1/pytamaro/primitives.py
+-rw-r--r--   0        0        0        0 2022-10-31 08:45:16.764275 pytamaro-0.5.1/pytamaro/py.typed
+-rw-r--r--   0        0        0     1032 2023-05-29 08:23:29.418250 pytamaro-0.5.1/pytamaro/utils.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pytamaro-0.5.1/PKG-INFO
```

### Comparing `pytamaro-0.5.0/LICENSE` & `pytamaro-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pyproject.toml` & `pytamaro-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytamaro"
-version = "0.5.0"
+version = "0.5.1"
 description = "Educational library for teaching problem decompositon using graphics"
 authors = ["Luca Chiodini <luca@chiodini.org>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 Pillow = "^9.0.0"
 skia-python = "^87.4"
```

### Comparing `pytamaro-0.5.0/pytamaro/checks.py` & `pytamaro-0.5.1/pytamaro/checks.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/color.py` & `pytamaro-0.5.1/pytamaro/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/color_functions.py` & `pytamaro-0.5.1/pytamaro/color_functions.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/color_names.py` & `pytamaro-0.5.1/pytamaro/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/color.py` & `pytamaro-0.5.1/pytamaro/de/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/color_names.py` & `pytamaro-0.5.1/pytamaro/de/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/io.py` & `pytamaro-0.5.1/pytamaro/de/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/operations.py` & `pytamaro-0.5.1/pytamaro/de/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/point_names.py` & `pytamaro-0.5.1/pytamaro/de/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/de/primitives.py` & `pytamaro-0.5.1/pytamaro/de/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/debug.py` & `pytamaro-0.5.1/pytamaro/debug.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/graphic.py` & `pytamaro-0.5.1/pytamaro/graphic.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/io.py` & `pytamaro-0.5.1/pytamaro/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,20 @@
     Draws a graphic to a canvas, correcting for the top-left position.
 
     :param canvas: canvas onto which to draw
     :param graphic: graphic to be drawn
     """
     bounds = graphic.bounds()
     canvas.translate(-bounds.left(), -bounds.top())
+    # Temporarily set the recursion limit to a high value so that we can
+    # traverse the (potentially deeply nested) tree that represents the graphic.
+    current_recursion_limit = sys.getrecursionlimit()
+    sys.setrecursionlimit(100000)
     graphic.draw(canvas)
+    sys.setrecursionlimit(current_recursion_limit)
 
 
 # pylint: disable-next=invalid-name
 def _save_as_SVG(filename: str, graphic: Graphic):
     """
     Save a graphic to an SVG file.
 
@@ -105,14 +110,28 @@
 
     :param filename: name of the file to be created, ending in ".png"
     :param graphic: graphic to be saved
     """
     graphic_to_image(graphic).save(filename, kPNG)
 
 
+def _print_data_uri(mime_type: str, b64_content: str):
+    """
+    Prints a data URI to standard output with a special prefix and suffix so
+    that it can be recognized in the context of a larger output.
+
+    :param mime_type: MIME type of the data (e.g., "image/png")
+    :param b64_content: base64-encoded content
+    """
+    prefix = "@@@PYTAMARO_DATA_URI_BEGIN@@@"
+    suffix = "@@@PYTAMARO_DATA_URI_END@@@"
+    uri = f"data:{mime_type};base64,{b64_content}"
+    print(f"{prefix}{uri}{suffix}", end="")
+
+
 @export
 def show_graphic(graphic: Graphic, debug: bool = False):
     """
     Show a graphic. Graphics with no area cannot be shown.
 
     When `debug` is `True`, adorns the visualization with useful information
     for debugging: a red border around the bounding box and a yellowish cross
@@ -131,15 +150,15 @@
         if is_notebook():
             # pylint: disable-next=undefined-variable
             display(pil_image)  # type: ignore[name-defined]
         elif "PYTAMARO_OUTPUT_DATA_URI" in os.environ:
             buffer = io.BytesIO()
             pil_image.save(buffer, format="PNG")
             b64_str = base64.b64encode(buffer.getvalue()).decode("utf-8")
-            print(f"data:image/png;base64,{b64_str}", end="")
+            _print_data_uri("image/png", b64_str)
         else:
             pil_image.show()
 
 
 @export
 def save_graphic(filename: str, graphic: Graphic, debug: bool = False):
     """
@@ -223,14 +242,14 @@
             from IPython.display import Image as IPythonImage  # type: ignore[import]
             with open(file.name, "rb") as stream:
                 # pylint: disable-next=undefined-variable
                 display(IPythonImage(stream.read()))  # type: ignore[name-defined]
         elif "PYTAMARO_OUTPUT_DATA_URI" in os.environ:
             with open(file.name, "rb") as stream:
                 b64_str = base64.b64encode(stream.read()).decode("utf-8")
-                print(f"data:image/gif;base64,{b64_str}", end="")
+                _print_data_uri("image/gif", b64_str)
         elif sys.platform == "win32":
             os.startfile(file.name)
         elif sys.platform == "darwin":
             subprocess.call(["open", "-a", "Safari", file.name])
         else:
             subprocess.call(["xdg-open", file.name])
```

### Comparing `pytamaro-0.5.0/pytamaro/it/color.py` & `pytamaro-0.5.1/pytamaro/it/color.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/it/color_names.py` & `pytamaro-0.5.1/pytamaro/it/color_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/it/io.py` & `pytamaro-0.5.1/pytamaro/it/io.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/it/operations.py` & `pytamaro-0.5.1/pytamaro/it/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/it/point_names.py` & `pytamaro-0.5.1/pytamaro/it/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/it/primitives.py` & `pytamaro-0.5.1/pytamaro/it/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/localization.py` & `pytamaro-0.5.1/pytamaro/localization.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/operations.py` & `pytamaro-0.5.1/pytamaro/operations.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/point.py` & `pytamaro-0.5.1/pytamaro/point.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/point_names.py` & `pytamaro-0.5.1/pytamaro/point_names.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/primitives.py` & `pytamaro-0.5.1/pytamaro/primitives.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/pytamaro/utils.py` & `pytamaro-0.5.1/pytamaro/utils.py`

 * *Files identical despite different names*

### Comparing `pytamaro-0.5.0/PKG-INFO` & `pytamaro-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytamaro
-Version: 0.5.0
+Version: 0.5.1
 Summary: Educational library for teaching problem decompositon using graphics
 Author: Luca Chiodini
 Author-email: luca@chiodini.org
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

