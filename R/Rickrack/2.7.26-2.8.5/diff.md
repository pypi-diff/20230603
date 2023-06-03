# Comparing `tmp/Rickrack-2.7.26.tar.gz` & `tmp/Rickrack-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Rickrack-2.7.26.tar", last modified: Sun Apr  9 10:14:15 2023, max compression
+gzip compressed data, was "dist\Rickrack-2.8.5.tar", last modified: Sat Jun  3 16:03:49 2023, max compression
```

## Comparing `Rickrack-2.7.26.tar` & `Rickrack-2.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/
--rw-rw-rw-   0        0        0       30 2023-04-09 10:14:14.000000 Rickrack-2.7.26/MANIFEST.in
--rw-rw-rw-   0        0        0    16391 2023-04-09 10:14:15.000000 Rickrack-2.7.26/PKG-INFO
--rw-rw-rw-   0        0        0    13401 2023-04-09 10:14:14.000000 Rickrack-2.7.26/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/rickrack/
--rw-rw-rw-   0        0        0    33878 2023-04-09 10:14:14.000000 Rickrack-2.7.26/rickrack/color.py
--rw-rw-rw-   0        0        0     9994 2023-04-07 06:01:22.000000 Rickrack-2.7.26/rickrack/result.py
--rw-rw-rw-   0        0        0    34745 2023-04-07 13:03:47.000000 Rickrack-2.7.26/rickrack/rickrack.py
--rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.7.26/rickrack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    16391 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 10:14:15.000000 Rickrack-2.7.26/setup.cfg
--rw-rw-rw-   0        0        0     2076 2023-04-09 10:14:14.000000 Rickrack-2.7.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/
+-rw-rw-rw-   0        0        0       30 2023-06-03 16:03:48.000000 Rickrack-2.8.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    30704 2023-06-03 16:03:49.000000 Rickrack-2.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0    26627 2023-06-03 16:03:48.000000 Rickrack-2.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/rickrack/
+-rw-rw-rw-   0        0        0    35477 2023-06-03 16:03:48.000000 Rickrack-2.8.5/rickrack/color.py
+-rw-rw-rw-   0        0        0     9994 2023-04-07 06:01:22.000000 Rickrack-2.8.5/rickrack/result.py
+-rw-rw-rw-   0        0        0    32826 2023-06-03 14:03:45.000000 Rickrack-2.8.5/rickrack/rickrack.py
+-rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.8.5/rickrack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    30704 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 16:03:49.000000 Rickrack-2.8.5/Rickrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 16:03:49.000000 Rickrack-2.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     2075 2023-06-03 16:03:48.000000 Rickrack-2.8.5/setup.py
```

### Comparing `Rickrack-2.7.26/rickrack/color.py` & `Rickrack-2.8.5/rickrack/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Please visit https://github.com/eigenmiao/DigitalPalette for more 
 infomation about DigitalPalette.
 
 Copyright (c) 2019-2021 by Eigenmiao. All Rights Reserved.
 """
 
+import re
 import unittest
 import numpy as np
 
 
 class FakeColor(object):
     """
     FakeColor object. Storing rgb, hsv and hex code (hec) color without functional methods.
@@ -540,26 +541,21 @@
         Args:
             hec (str): color item to be formated.
 
         Returns:
             standard hex code (hec) color.
         """
 
-        if not isinstance(hec, str):
-            raise ValueError("expect hex code (hec) in str type: {}.".format(hec))
+        _hec = re.match(r"[0-9A-F]+", str(hec).upper())
 
-        if len(hec) == 6:
-            for stri in hec.upper():
-                if stri not in ("0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F"):
-                    raise ValueError("expect code in hex type: {}.".format(hec))
+        if _hec and len(_hec[0]) == 6:
+            return _hec[0]
 
         else:
-            raise ValueError("expect hex code (hec) in length 6: {}.".format(hec))
-
-        return hec.upper()
+            raise ValueError("expect hec color in hex type and length 6: {}.".format(hec))
 
     @classmethod
     def fmt_lab(cls, lab):
         """
         Class method. Format item to standard lab color.
 
         Args:
@@ -605,14 +601,81 @@
 
             return _cmyk.astype(np.float32)
 
         else:
             raise ValueError("expect cmyk color in length 4 and float: {}.".format(cmyk))
 
     @classmethod
+    def findall_hec_lst(cls, hec):
+        """
+        Class method. Format item to standard hex code (hec) color.
+
+        Args:
+            hec (str): color item to be formated.
+
+        Returns:
+            standard hex code (hec) color.
+        """
+
+        _hec = re.findall(r"[0-9A-F]+", str(hec).upper())
+        _hec = ["" if len(i) < 6 else i[:6] for i in _hec]
+
+        while "" in _hec:
+            _hec.remove("")
+
+        return _hec
+
+    @classmethod
+    def stri2color(cls, stri):
+        """
+        Find the first possible color in string.
+
+        Args:
+            stri (str): rgb, hsv or hec color string.
+
+        Returns:
+            color.
+        """
+
+        _stri = re.findall(r"[0-9A-F\.]+", str(stri).upper())
+
+        if len(_stri) > 2:
+            _num = re.findall(r"[0-9\.]+", str(stri))
+
+            if len(_num) > 2:
+                _a, _b, _c = _num[:3]
+                _a = float(".".join(_a.split(".")[:2])) if "." in _a else int(_a)
+                _b = float(".".join(_b.split(".")[:2])) if "." in _b else int(_b)
+                _c = float(".".join(_c.split(".")[:2])) if "." in _c else int(_c)
+
+                if _a > 255:
+                    return Color((_a, _b, _c), tp="hsv")
+
+                elif _b > 1.0 or _c > 1.0:
+                    return Color((_a, _b, _c), tp="rgb")
+
+                elif isinstance(_a, float) or isinstance(_b, float) or isinstance(_c, float):
+                    return Color((_a, _b, _c), tp="hsv")
+
+                else:
+                    return Color((_a, _b, _c), tp="rgb")
+
+            else:
+                return None
+
+        elif len(_stri) > 0:
+            if len(_stri[0]) > 5:
+                return Color(Color.fmt_hec(_stri[0]), tp="hec")
+
+            return None
+
+        else:
+            return None
+
+    @classmethod
     def rgb2hsv(cls, rgb):
         """
         Translate rgb color into hsv color.
 
         Args:
             rgb (tuple or list): rgb color.
 
@@ -970,19 +1033,19 @@
             lab (tuple or list): lab color.
             white_ref (tuple or list): xyz (Tristimulus) Reference values of a perfect reflecting diffuser. default: value of standard "D65, 2Ang".
 
         Returns:
             rgb color.
         """
 
-        lab = cls.fmt_lab(lab)
+        l, a, b = cls.fmt_lab(lab)
 
-        y = (lab[0] + 16) / 116
-        x = lab[1] / 500 + y
-        z = y - lab[2] / 200
+        y = (l + 16) / 116
+        x = a / 500 + y
+        z = y - b / 200
 
         normed_xyz = [i ** 3 if i > 0.008856 else (i - 16 / 116) / 7.787 for i in (x, y, z)]
         xyz = np.array(normed_xyz) * white_ref / 100.0
 
         normed_rgb = np.array([
             [ 3.24048134, -1.53715152, -0.49853633],
             [-0.96925495,  1.87599   ,  0.04155593],
```

### Comparing `Rickrack-2.7.26/rickrack/result.py` & `Rickrack-2.8.5/rickrack/result.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.7.26/rickrack/rickrack.py` & `Rickrack-2.8.5/rickrack/rickrack.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 """
 
 __WEBSITE__ = """
 https://github.com/eigenmiao/Rickrack
 """
 
 __VERSION__ = """
-v2.7.26-x2d3s3-stable
+v2.8.5-x2d3s3-pre
 """
 
 __AUTHOR__ = """
 Eigenmiao (eigenmiao@outlook.com)
 """
 
 __DATE__ = """
-April 9, 2023
+May 21, 2023
 """
 
 __HELP__ = """
 INTRODUCTION:
   Rickrack-Startup provides the ability to operate Rickrack from the 
   command line or through Python code, allowing you to start it, close it, 
   and obtain color results from Rickrack.
@@ -783,21 +783,15 @@
             return
 
         if dp_proj:
             dirname, basename = para_dir(dp_proj)
 
         elif os.path.isfile(os.sep.join([os.path.abspath(os.path.dirname(__file__)), "data.json"])):
             with open(os.sep.join([os.path.abspath(os.path.dirname(__file__)), "data.json"]), "r", encoding="utf-8") as f:
-                try:
-                    data = json.load(f)
-
-                except Exception as err:
-                    print("Load project data faild:\n{}".format(err))
-
-                    data = {}
+                data = json.load(f)
 
             if "dp_proj" in data and data["dp_proj"]:
                 dirname, basename = para_dir(data["dp_proj"])
 
             else:
                 dirname, basename = None, None
 
@@ -811,20 +805,16 @@
             print("\n+" + "-" * 30 + " Rickrack-Startup " + "-" * 30 + "+")
             print(__HELP__)
             print(__ERROR__)
             sys.exit()
 
         os.chdir(dirname)
 
-        try:
-            with open(os.sep.join([os.path.abspath(os.path.dirname(__file__)), "data.json"]), "w", encoding="utf-8") as f:
-                json.dump({"dp_proj": dirname, "dp_exec": basename}, f, indent=4, ensure_ascii=False)
-
-        except Exception as err:
-            print("Dump project data faild:\n{}".format(err))
+        with open(os.sep.join([os.path.abspath(os.path.dirname(__file__)), "data.json"]), "w", encoding="utf-8") as f:
+            json.dump({"dp_proj": dirname, "dp_exec": basename}, f, indent=4, ensure_ascii=False)
 
         # run project.
         sdp_argv = dict()
 
         if dp_argv:
             if isinstance(dp_argv, dict):
                 sdp_argv = dp_argv.copy()
@@ -1013,52 +1003,34 @@
                 # Color Grid ...
                 if para_color_grid:
                     if line[2] == " ":
                         color_line = line[4:].split(" ")
                         rt_gcol = len(color_line)
 
                         for i in range(len(color_line)):
-                            try:
-                                color_line[i] = Color.fmt_hec(color_line[i])
-
-                            except Exception as err:
-                                print("Parse colors in grid faild:\n{}".format(color_line[i]))
-
-                                color_line[i] = self._default_color
+                            color_line[i] = Color.fmt_hec(color_line[i])
 
                         rt_cgrd += color_line
 
                 # Full Colors
                 elif para_full_colors:
                     if line[2] == " ":
                         color_line = line[4:].split(" ")
 
                         for i in range(len(color_line)):
-                            try:
-                                color_line[i] = Color.fmt_hec(color_line[i])
-
-                            except Exception as err:
-                                print("Parse colors in grid faild:\n{}".format(color_line[i]))
-
-                                color_line[i] = self._default_color
+                            color_line[i] = Color.fmt_hec(color_line[i])
 
                         rt_refs = color_line
 
                 else:
                     if line[4] in [str(i) for i in range(5)]:
                         if line[2] == "*":
                             rt_cidx = int(line[4])
 
-                        try:
-                            rt_cset[int(line[4])] = Color.fmt_hec(line[3:].split()[7])
-
-                        except Exception as err:
-                            print("Parse colors for id {} faild:\n{}".format(line[4], err))
-
-                            rt_cset[int(line[4])] = self._default_color
+                        rt_cset[int(line[4])] = Color.fmt_hec(line[3:].split()[7])
 
                     elif line[4:8] == "Rule":
                         rt_rule = line[10:].lstrip().rstrip()
 
                         if rt_rule not in ("Analogous", "Monochromatic", "Triad", "Tetrad", "Pentad", "Complementary", "Shades", "Custom"):
                             rt_rule = "Custom"
 
@@ -1080,44 +1052,24 @@
                     data_grid = data_grid.split(" ")
                     data_grid_name = data_grid_name.lstrip().rstrip()
 
                     if data_grid_name:
                         data_grid_name = data_grid_name[1:-1].split('" "')
 
                     for i in range(5):
-                        try:
-                            rt_cset[(2, 1, 0, 3, 4)[i]] = Color.fmt_hec(data_set[i])
-
-                        except Exception as err:
-                            print("Parse colors for id {} faild:\n{}".format(i, err))
-
-                            rt_cset[i] = self._default_color
+                        rt_cset[(2, 1, 0, 3, 4)[i]] = Color.fmt_hec(data_set[i])
 
                     for i in range(len(data_set) - 6):
-                        try:
-                            rt_refs.append(Color.fmt_hec(data_set[i + 6]))
-
-                        except Exception as err:
-                            print("Parse ref colors for id {} faild:\n{}".format(i, err))
-
-                            rt_refs.append(self._default_color)
-                            rt_refs_name.append("RR")
+                        rt_refs.append(Color.fmt_hec(data_set[i + 6]))
 
                     for i in range(len(data_grid)):
-                        try:
-                            rt_cgrd.append(Color.fmt_hec(data_grid[i]))
-
-                            if data_grid_name:
-                                rt_cgrd_name.append(data_grid_name[i])
-
-                        except Exception as err:
-                            print("Parse color grid for id {} faild:\n{}".format(i, err))
+                        rt_cgrd.append(Color.fmt_hec(data_grid[i]))
 
-                            rt_cgrd.append(self._default_color)
-                            rt_cgrd_name.append("RR")
+                        if data_grid_name:
+                            rt_cgrd_name.append(data_grid_name[i])
 
         rt_cset = Grid(rt_cset, rt_cset_name, 5)
         rt_refs = Grid(rt_refs, rt_refs_name, len(rt_refs))
         rt_cgrd = Grid(rt_cgrd, rt_cgrd_name, (rt_gcol, rt_gcol))
 
         result = {"rule": str(rt_rule), "index": int(rt_cidx), "colors": rt_cset, "refs": rt_refs, "grid": rt_cgrd}
         result = Result(result)
```

### Comparing `Rickrack-2.7.26/rickrack/__init__.py` & `Rickrack-2.8.5/rickrack/__init__.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.7.26/setup.py` & `Rickrack-2.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from setuptools import setup
 
 
 setup(
     name="Rickrack",
-    version="2.7.26",
+    version="2.8.5",
     author="Eigenmiao",
     author_email="eigenmiao@outlook.com",
     description="Generate harmonious colors freely.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://eigenmiao.github.io/rickrack/",
     classifiers=[
```

