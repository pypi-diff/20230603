# Comparing `tmp/pollenflug-0.1.1.tar.gz` & `tmp/pollenflug-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollenflug-0.1.1.tar", last modified: Wed Feb 16 20:59:44 2022, max compression
+gzip compressed data, was "pollenflug-0.2.1.tar", max compression
```

## Comparing `pollenflug-0.1.1.tar` & `pollenflug-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,9 @@
-drwxrwxr-x   0 tanto     (1000) tanto     (1000)        0 2022-02-16 20:59:44.743840 pollenflug-0.1.1/
--rw-rw-r--   0 tanto     (1000) tanto     (1000)    35149 2021-11-17 10:56:48.000000 pollenflug-0.1.1/LICENSE
--rw-rw-r--   0 tanto     (1000) tanto     (1000)       70 2022-01-17 00:45:35.000000 pollenflug-0.1.1/MANIFEST.in
--rw-rw-r--   0 tanto     (1000) tanto     (1000)     1673 2022-02-16 20:59:44.742840 pollenflug-0.1.1/PKG-INFO
--rw-rw-r--   0 tanto     (1000) tanto     (1000)     1082 2022-01-17 21:46:02.000000 pollenflug-0.1.1/README.md
-drwxrwxr-x   0 tanto     (1000) tanto     (1000)        0 2022-02-16 20:59:44.741840 pollenflug-0.1.1/config/
--rw-rw-r--   0 tanto     (1000) tanto     (1000)       41 2022-01-17 00:28:03.000000 pollenflug-0.1.1/config/pollenflug.ini
-drwxrwxr-x   0 tanto     (1000) tanto     (1000)        0 2022-02-16 20:59:44.741840 pollenflug-0.1.1/lib/
--rw-rw-r--   0 tanto     (1000) tanto     (1000)        0 2022-01-15 12:47:55.000000 pollenflug-0.1.1/lib/__init__.py
--rw-rw-r--   0 tanto     (1000) tanto     (1000)     1326 2022-01-17 00:05:44.000000 pollenflug-0.1.1/lib/color.py
--rw-rw-r--   0 tanto     (1000) tanto     (1000)      631 2022-01-15 12:47:55.000000 pollenflug-0.1.1/lib/consts.py
--rw-rw-r--   0 tanto     (1000) tanto     (1000)     3984 2022-02-16 20:02:23.000000 pollenflug-0.1.1/lib/functions.py
--rwxrwxr-x   0 tanto     (1000) tanto     (1000)     2517 2022-01-17 21:51:12.000000 pollenflug-0.1.1/pollenflug
-drwxrwxr-x   0 tanto     (1000) tanto     (1000)        0 2022-02-16 20:59:44.742840 pollenflug-0.1.1/pollenflug.egg-info/
--rw-rw-r--   0 tanto     (1000) tanto     (1000)     1673 2022-02-16 20:59:44.000000 pollenflug-0.1.1/pollenflug.egg-info/PKG-INFO
--rw-rw-r--   0 tanto     (1000) tanto     (1000)      300 2022-02-16 20:59:44.000000 pollenflug-0.1.1/pollenflug.egg-info/SOURCES.txt
--rw-rw-r--   0 tanto     (1000) tanto     (1000)        1 2022-02-16 20:59:44.000000 pollenflug-0.1.1/pollenflug.egg-info/dependency_links.txt
--rw-rw-r--   0 tanto     (1000) tanto     (1000)        9 2022-02-16 20:59:44.000000 pollenflug-0.1.1/pollenflug.egg-info/requires.txt
--rw-rw-r--   0 tanto     (1000) tanto     (1000)        4 2022-02-16 20:59:44.000000 pollenflug-0.1.1/pollenflug.egg-info/top_level.txt
--rw-rw-r--   0 tanto     (1000) tanto     (1000)       38 2022-02-16 20:59:44.743840 pollenflug-0.1.1/setup.cfg
--rw-rw-r--   0 tanto     (1000) tanto     (1000)      910 2022-02-16 20:58:29.000000 pollenflug-0.1.1/setup.py
+-rw-r--r--   0        0        0    35149 2022-12-14 00:12:43.679194 pollenflug-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1279 2023-06-03 10:59:02.248456 pollenflug-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 12:22:51.970324 pollenflug-0.2.1/pollenflug/lib/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-03 12:22:47.882269 pollenflug-0.2.1/pollenflug/lib/color.py
+-rw-r--r--   0        0        0      682 2023-06-03 12:22:45.020231 pollenflug-0.2.1/pollenflug/lib/consts.py
+-rw-r--r--   0        0        0     3948 2023-06-03 12:22:41.695186 pollenflug-0.2.1/pollenflug/lib/functions.py
+-rwxr-xr-x   0        0        0     2526 2023-06-03 12:22:34.607091 pollenflug-0.2.1/pollenflug/pollenflug.py
+-rw-r--r--   0        0        0     1127 2023-06-03 13:36:37.904835 pollenflug-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pollenflug-0.2.1/PKG-INFO
```

### Comparing `pollenflug-0.1.1/LICENSE` & `pollenflug-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pollenflug-0.1.1/README.md` & `pollenflug-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # pollenflug
 ## CLI pollen/allergy calendar
 
+[![Python package](https://github.com/BaderSZ/pollenflug/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/BaderSZ/pollenflug/actions/workflows/python-package.yml)
+
 ![Screenshot](https://raw.githubusercontent.com/BaderSZ/pollenflug/master/img/screenshot.png)
 
 This script uses [Hexal's Pollenflugkalendar](https://allergie.hexal.de/pollenflug/vorhersage/) to fetch the predictions for the next week.
 
 Currently, the intensity is printed as a numerical value between 0 and 3: 0 being none, 3 being severe.
 
 pollenflug currently supports a configuration file as `~/.pollenflug.ini`, with an example configuration included in the repo
```

### Comparing `pollenflug-0.1.1/lib/color.py` & `pollenflug-0.2.1/pollenflug/lib/color.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,35 +14,36 @@
         ORANGE
         ORANGE_TOO
         RED
 
     Methods:
         __str__(self) -> str
         format_color(cls, string: str, color: Type[COLORT] = None) ->str
-        """
+    """
+
     GREEN = "0"
     ORANGE, ORANGE_TOO = "1", "2"
     RED = "3"
 
     def __str__(self):
         return self.value
 
-    COLORT = TypeVar('ColorT', bound='Color')
+    COLORT = TypeVar("ColorT", bound="Color")
 
     @classmethod
     def format_color(cls, string: str, color: Type[COLORT] = None) -> str:
         """Give each pollen value an appropriate color in the table
 
         Input Arguments: `string` to colorise, and `Color` as defined in the parent class
         Returns: `string` with additional ASCII color codes.
         """
-        green = '\033[92m'
-        orange = '\033[93m'
-        red = '\033[91m'
-        endc = '\033[0m'
+        green = "\033[92m"
+        orange = "\033[93m"
+        red = "\033[91m"
+        endc = "\033[0m"
 
         if color == cls.GREEN:
             return green + string + endc
         if color in (cls.ORANGE, cls.ORANGE_TOO):
             return orange + string + endc
         if color == cls.RED:
             return red + string + endc
```

### Comparing `pollenflug-0.1.1/lib/consts.py` & `pollenflug-0.2.1/pollenflug/lib/consts.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,13 +3,28 @@
     REQ_URL: hexal.de request URL
     ENG_LIST: the english translation of the array of allergens from the site.
     SHORT_OPT: command line options called with a single dash.
     LONG_OPT: command line options called with a double dash.
 """
 
 REQ_URL = "https://allergie.hexal.de/pollenflug/vorhersage/load_pollendaten.php"
-ENG_LIST = ["Ambrosia", "Dock", "Artemisia", "Birch", "Beech", "Oak", "Alder", "Ash", "Grass",
-            "Hazel", "Popplar", "Rye", "Elm", "Plantain", "Willow"]
+ENG_LIST = [
+    "Ambrosia",
+    "Dock",
+    "Artemisia",
+    "Birch",
+    "Beech",
+    "Oak",
+    "Alder",
+    "Ash",
+    "Grass",
+    "Hazel",
+    "Popplar",
+    "Rye",
+    "Elm",
+    "Plantain",
+    "Willow",
+]
 
 # Define input options
 SHORT_OPT = "d:p:hve"
 LONG_OPT = ["date=", "plz=", "help", "verbose", "english"]
```

### Comparing `pollenflug-0.1.1/lib/functions.py` & `pollenflug-0.2.1/pollenflug/lib/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,63 +34,61 @@
 
     # Load config file
     config = configparser.ConfigParser()
     config.read(config_location)
 
     # Check config file for postal code, and set appropriately
     try:
-        plz = int(config['DEFAULT']['plz'])
+        plz = int(config["DEFAULT"]["plz"])
     except (TypeError, KeyError):
         # plz not defined in config file, use default
         plz = 20095
     except ValueError:
-        print(Color.format_color("Error") +
-              ": invalid postal code in config!")
+        print(Color.format_color("Error") + ": invalid postal code in config!")
         sys.exit(os.EX_CONFIG)
 
     # Check config file for debug flag, and set appropriately
     try:
-        debug_str = config['DEFAULT']['debug'].lower()
+        debug_str = config["DEFAULT"]["debug"].lower()
         if debug_str in ("true", "1"):
             debug = True
         elif debug_str in ("false", "0", ""):
             debug = False
         else:
-            print(Color.format_color("Error") +
-                  ": invalid debug flag in config!")
+            print(Color.format_color("Error") + ": invalid debug flag in config!")
             sys.exit(os.EX_CONFIG)
     except KeyError:
         # Don't fail on undefined
         debug = False
 
     # Check config file for english flag, and set if given.
     try:
-        eng = config['DEFAULT']['en'].lower()
+        eng = config["DEFAULT"]["en"].lower()
         if eng in ("true", "1"):
             use_eng = True
         elif eng in ("false", "0", ""):
             use_eng = False
         else:
-            print(Color.format_color("Error") +
-                  ": invalid language flag in config!")
+            print(Color.format_color("Error") + ": invalid language flag in config!")
             sys.exit(os.EX_CONFIG)
     except KeyError:
         # Don't fail on undefined
         use_eng = False
 
     return plz, use_eng, debug
 
 
 def print_help() -> None:
     """Print help menu with argument, usage, copyright and Github.
 
     Input Arguments: None
     Returns: None
     """
-    print("""Usage: pollenflug.py [options]
+    print(
+        """Usage: pollenflug.py [options]
 
     -h,--help               Print this help menu
     -d,--date=YYYY-MM-DD    Set start date of pollen calendar
     -p,--plz=iiiii          Set postal code/plz
     -e,--english            Print plant names in English
     -v,--verbose            Print verbose
 
@@ -100,15 +98,16 @@
 
 pollenflug  Copyright (C) 2022  Bader Zaidan
 This program comes with ABSOLUTELY NO WARRANTY;
 This is free software, and you are welcome to redistribute it
 under certain conditions; read LICENSE for details.
 
 For bug reports and feature requests, see:
-https://github.com/BaderSZ/pollenflug""")
+https://github.com/BaderSZ/pollenflug"""
+    )
 
 
 def print_calendar(data: Dict, eng: bool = False) -> None:
     """Print calendar as a table with appropriate spacing.
 
     Input Arguments: `data: dict` from URL request., language flag.
     Returns: None.
```

### Comparing `pollenflug-0.1.1/pollenflug` & `pollenflug-0.2.1/pollenflug/pollenflug.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from pathlib import Path
 
 # HTTP requests and parsing
 from datetime import datetime
 import requests
 
 # local
-from lib.functions import loadconfig, print_calendar, print_help
-from lib.consts import LONG_OPT, SHORT_OPT, REQ_URL
-from lib.color import Color
+from .lib.functions import loadconfig, print_calendar, print_help
+from .lib.consts import LONG_OPT, SHORT_OPT, REQ_URL
+from .lib.color import Color
 
 # Config absolute directory
 CONFIG_LOCATION = str(Path.home()) + "/.pollenflug.ini"
 
 
 def main() -> None:
     """main() function, parse arguments and call functions
@@ -37,16 +37,15 @@
     # Load config, with default values
     plz, use_eng, debug = loadconfig(CONFIG_LOCATION)
 
     # Check CLI options, exit if undefined
     try:
         arguments, _val = getopt.getopt(arg_list, SHORT_OPT, LONG_OPT)
     except getopt.error as exp:
-        print(Color.format_color("Error", Color.RED) +
-              ": Invalid input arguments!")
+        print(Color.format_color("Error", Color.RED) + ": Invalid input arguments!")
         if debug:
             print(exp)
         print_help()
         sys.exit(os.EX_USAGE)
 
     # Set CLI arguments.
     for arg, val in arguments:
@@ -63,30 +62,31 @@
         elif arg in ("-e", "--english"):
             use_eng = True
 
     req_load = {"datum": date, "plz": plz, "historie": history}
 
     # Get data from HEXAL, exception if error
     try:
-        request = requests.post(REQ_URL,  params=req_load)
+        request = requests.post(REQ_URL, params=req_load, timeout=2)
     except requests.exceptions.RequestException as exp:
-        print(Color.format_color("Error", Color.RED) +
-              ": Failed sending request.")
+        print(Color.format_color("Error", Color.RED) + ": Failed sending request.")
 
         if debug:
             print(exp)
         sys.exit(os.EX_SOFTWARE)
 
     json_data = request.json()
     if json_data["message"] != "success":
-        print(Color.format_color("Error", Color.RED) +
-              ": Server error. Check your arguments?")
+        print(
+            Color.format_color("Error", Color.RED)
+            + ": Server error. Check your arguments?"
+        )
         sys.exit(os.EX_SOFTWARE)
 
     # Print results
     print("Data for " + str(plz) + ", Germany")
     print_calendar(json_data, eng=use_eng)
     sys.exit(os.EX_OK)
 
 
-if __name__ == "__main__":
-    main()
+# if __name__ == "__main__":
+#     main()
```

