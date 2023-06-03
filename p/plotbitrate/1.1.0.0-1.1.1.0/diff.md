# Comparing `tmp/plotbitrate-1.1.0.0-py3-none-any.whl.zip` & `tmp/plotbitrate-1.1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11621 bytes, number of entries: 10
--rw-r--r--  2.0 unx    22701 b- defN 23-May-28 03:53 plotbitrate.py
+Zip file size: 12013 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    22973 b- defN 23-Jun-03 20:44 plotbitrate.py
 -rw-r--r--  2.0 unx      323 b- defN 21-Apr-04 22:56 frame/__init__.py
 -rw-r--r--  2.0 unx      231 b- defN 21-Apr-04 22:56 frame/_frame_class.py
 -rw-r--r--  2.0 unx      252 b- defN 21-Apr-04 22:56 frame/_frame_dataclass.py
--rw-r--r--  2.0 unx     1364 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2992 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/RECORD
-10 files, 28842 bytes uncompressed, 10215 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     1364 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3881 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-03 20:50 plotbitrate-1.1.1.0.dist-info/RECORD
+10 files, 30003 bytes uncompressed, 10607 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: frame/_frame_class.py
 Comment: 
 
 Filename: frame/_frame_dataclass.py
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/LICENSE
+Filename: plotbitrate-1.1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/METADATA
+Filename: plotbitrate-1.1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/WHEEL
+Filename: plotbitrate-1.1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/entry_points.txt
+Filename: plotbitrate-1.1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/top_level.txt
+Filename: plotbitrate-1.1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: plotbitrate-1.1.0.0.dist-info/RECORD
+Filename: plotbitrate-1.1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plotbitrate.py

```diff
@@ -25,73 +25,70 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = "1.1.0.0"
+__version__ = "1.1.1.0"
 
 import argparse
 import csv
 import datetime
 import math
 import multiprocessing
+import os
 import platform
 import shutil
 import statistics
 import subprocess
 import sys
 from collections import OrderedDict
-from importlib import util
 from enum import Enum
+from importlib import util
 from typing import Callable, Union, List, IO, Iterable, Optional, Dict, Tuple, \
     Generator
 from frame import Frame
 
 
 class Color(Enum):
     I = "red"
     P = "green"
     B = "blue"
     AUDIO = "C2"
     FRAME = "C0"
 
 
 class ConsoleColors:
-    WARNING = '\033[93m'  # yellow
-    ERROR = '\033[91m'  # red
-    END_COLOR = '\033[0m'  # restore default color
+    WARNING = "\033[93m"  # yellow
+    ERROR = "\033[91m"  # red
+    END_COLOR = "\033[0m"  # restore default color
 
 
 def exit_with_error(error_message: str) -> None:
     sys.exit(ConsoleColors.ERROR + "Error: " + error_message +
              ConsoleColors.END_COLOR)
 
 
 def print_warning(warning_message: str) -> None:
     print(ConsoleColors.WARNING + "Warning: " + warning_message +
           ConsoleColors.END_COLOR)
 
 
 def is_wsl() -> bool:
     platform_info = platform.uname()
-    return platform_info.system == "Linux" and 'microsoft' in platform_info.release.lower()
+    return platform_info.system == "Linux" and "microsoft" in platform_info.release.lower()
 
 
 # prefer C-based ElementTree
 try:
     import xml.etree.cElementTree as eTree
 except ImportError:
     import xml.etree.ElementTree as eTree  # type: ignore
 
-# check for PyQt5 or PyQt6
-if util.find_spec("PyQt6") is None and util.find_spec("PyQt5") is None:
-    exit_with_error("Missing package 'PyQt5' or 'PyQt6'")
-
 # check for matplot lib
 try:
     import matplotlib  # type: ignore
     import matplotlib.pyplot as matplot  # type: ignore
 except ImportError as err:
     # satisfy undefined variable warnings
     matplotlib = None
@@ -120,16 +117,16 @@
     format_list.append("xml_raw")
     format_list.append("csv_raw")
 
     # parse command line arguments
     parser = argparse.ArgumentParser(
         description="Graph bitrate for audio/video stream")
     parser.add_argument("input", help="input file/stream", metavar="INPUT")
-    parser.add_argument('--version', action='version',
-                        version='%(prog)s {version}'.format(
+    parser.add_argument("--version", action="version",
+                        version="%(prog)s {version}".format(
                             version=__version__))
     parser.add_argument("-s", "--stream", help="Stream type (default: video)",
                         choices=["audio", "video"], default="video")
     parser.add_argument("-o", "--output", help="Output file")
     parser.add_argument("-f", "--format", help="Output file format",
                         choices=format_list)
     parser.add_argument("--no-progress", help="Hides progress",
@@ -288,16 +285,16 @@
                 print(flush=True)
 
 
 def save_raw_csv(raw_frames: Iterable[Frame], target_path: str) -> None:
     """ Saves raw_frames as a csv file. """
     fields = Frame.get_fields()
 
-    with open(target_path, "w") as file:
-        wr = csv.writer(file, quoting=csv.QUOTE_NONE)
+    with open(target_path, "w", newline="") as file:
+        wr = csv.writer(file, quoting=csv.QUOTE_NONE, lineterminator=os.linesep)
         wr.writerow(fields)
         for frame in raw_frames:
             wr.writerow(getattr(frame, field) for field in fields)
 
 
 def media_duration(source: str) -> float:
     if source.endswith(".xml"):
@@ -622,21 +619,25 @@
     # check if an output is requested, otherwise try to initialize backend, and exit if it fails
     if not args.output:
         # init backend
         try:
             if is_wsl():
                 backend = "TkAgg"
             else:
+                # check for PyQt5 or PyQt6
+                if util.find_spec("PyQt6") is None and util.find_spec("PyQt5") is None:
+                    exit_with_error("Missing package 'PyQt5' or 'PyQt6'")
                 backend = "QtAgg"
             matplotlib.use(backend)
         except ImportError as err:
             exit_with_error(err.msg)
 
     # if the output is raw xml, just call the function and exit
-    if args.format == "xml_raw":
+    if args.format == "xml_raw" \
+            or (args.output and args.output.endswith(".xml") and args.format is None):
         save_raw_xml(
             args.input, args.output, args.stream_spec, args.no_progress
         )
         sys.exit(0)
 
     duration = math.floor(media_duration(args.input))
     if duration == 0:
@@ -644,15 +645,16 @@
 
     progress_func = create_progress(duration) if not args.no_progress else None
     frames = read_frame_data_gen(
         args.input, args.stream_spec, progress_func
     )
 
     # if the output is csv raw, write the file and we're done
-    if args.format == "csv_raw":
+    if args.format == "csv_raw" \
+            or (args.output and args.output.endswith(".csv") and args.format is None):
         save_raw_csv(frames, args.output)
         sys.exit(0)
 
     prepare_matplot(args.input, duration, args.min, args.max)
 
     legend = None
     if args.show_frame_types and args.stream == "video":
```

## Comparing `plotbitrate-1.1.0.0.dist-info/LICENSE` & `plotbitrate-1.1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plotbitrate-1.1.0.0.dist-info/RECORD` & `plotbitrate-1.1.1.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-plotbitrate.py,sha256=iUQkJWY6u8PhoDTT1RBy_hIx6u0QSBliiPF3XvVj8fQ,22701
+plotbitrate.py,sha256=9oe_PegICLdv7WkD8W-40YAO6cG3m415C2Sges8ftXE,22973
 frame/__init__.py,sha256=lreLJjeFT9pLvyyf2stOlYFdyFzQRyhwKan6l3GIk8s,323
 frame/_frame_class.py,sha256=13_0I0ppVdU8CwzuawmEWlHdYbLONKAQULdaeYzrPOY,231
 frame/_frame_dataclass.py,sha256=-e_aeJVO6tMx64o0tYFodaT3iHtlrh715RIHv-PLfSE,252
-plotbitrate-1.1.0.0.dist-info/LICENSE,sha256=TbeSqT2UnRfLzmdFG7iGXZMBzRQB1cfzFyJPq6E8qG4,1364
-plotbitrate-1.1.0.0.dist-info/METADATA,sha256=b1jMfQ13d4ZyXp0WGyA-VWLuI4vHv5G44SgQRgoF3Ik,2992
-plotbitrate-1.1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-plotbitrate-1.1.0.0.dist-info/entry_points.txt,sha256=DCDetfld1tV6cn8F2n8ZJJrGvq-RUtlR-a4Bqi1B2tA,49
-plotbitrate-1.1.0.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
-plotbitrate-1.1.0.0.dist-info/RECORD,,
+plotbitrate-1.1.1.0.dist-info/LICENSE,sha256=TbeSqT2UnRfLzmdFG7iGXZMBzRQB1cfzFyJPq6E8qG4,1364
+plotbitrate-1.1.1.0.dist-info/METADATA,sha256=DcoGBFUR1L2vum6NfWNn0vCHVFkOkTMhALhN0Mm7aFE,3881
+plotbitrate-1.1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+plotbitrate-1.1.1.0.dist-info/entry_points.txt,sha256=DCDetfld1tV6cn8F2n8ZJJrGvq-RUtlR-a4Bqi1B2tA,49
+plotbitrate-1.1.1.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
+plotbitrate-1.1.1.0.dist-info/RECORD,,
```

