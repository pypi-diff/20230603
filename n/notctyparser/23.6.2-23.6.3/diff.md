# Comparing `tmp/notctyparser-23.6.2.tar.gz` & `tmp/notctyparser-23.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notctyparser-23.6.2.tar", last modified: Fri Jun  2 14:22:18 2023, max compression
+gzip compressed data, was "notctyparser-23.6.3.tar", last modified: Sat Jun  3 17:32:33 2023, max compression
```

## Comparing `notctyparser-23.6.2.tar` & `notctyparser-23.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:22:18.981004 notctyparser-23.6.2/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1080 2023-06-01 20:39:35.000000 notctyparser-23.6.2/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1572 2023-06-02 14:22:18.980004 notctyparser-23.6.2/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      808 2023-06-02 14:18:21.000000 notctyparser-23.6.2/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:22:18.979004 notctyparser-23.6.2/docs/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2346 2023-06-01 20:39:35.000000 notctyparser-23.6.2/docs/conf.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:22:18.979004 notctyparser-23.6.2/notctyparser/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      368 2023-06-02 14:16:48.000000 notctyparser-23.6.2/notctyparser/__info__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      251 2023-06-01 20:39:35.000000 notctyparser-23.6.2/notctyparser/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      499 2023-06-01 21:07:38.000000 notctyparser-23.6.2/notctyparser/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10333 2023-06-02 14:10:12.000000 notctyparser-23.6.2/notctyparser/bigcty.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-02 14:22:18.980004 notctyparser-23.6.2/notctyparser.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1572 2023-06-02 14:22:18.000000 notctyparser-23.6.2/notctyparser.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      322 2023-06-02 14:22:18.000000 notctyparser-23.6.2/notctyparser.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-02 14:22:18.000000 notctyparser-23.6.2/notctyparser.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       20 2023-06-02 14:22:18.000000 notctyparser-23.6.2/notctyparser.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       23 2023-06-02 14:22:18.000000 notctyparser-23.6.2/notctyparser.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      908 2023-06-02 14:17:10.000000 notctyparser-23.6.2/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-02 14:22:18.981004 notctyparser-23.6.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.216105 notctyparser-23.6.3/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1080 2023-06-01 20:39:35.000000 notctyparser-23.6.3/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1703 2023-06-03 17:32:33.216105 notctyparser-23.6.3/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      939 2023-06-03 17:30:33.000000 notctyparser-23.6.3/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.211105 notctyparser-23.6.3/docs/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2346 2023-06-01 20:39:35.000000 notctyparser-23.6.3/docs/conf.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.213105 notctyparser-23.6.3/notctyparser/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      368 2023-06-02 14:16:48.000000 notctyparser-23.6.3/notctyparser/__info__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      251 2023-06-01 20:39:35.000000 notctyparser-23.6.3/notctyparser/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      499 2023-06-01 21:07:38.000000 notctyparser-23.6.3/notctyparser/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10663 2023-06-03 17:28:30.000000 notctyparser-23.6.3/notctyparser/bigcty.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.215105 notctyparser-23.6.3/notctyparser.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1703 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      322 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       20 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       23 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      908 2023-06-03 17:18:59.000000 notctyparser-23.6.3/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-03 17:32:33.217105 notctyparser-23.6.3/setup.cfg
```

### Comparing `notctyparser-23.6.2/LICENSE` & `notctyparser-23.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notctyparser-23.6.2/PKG-INFO` & `notctyparser-23.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notctyparser
-Version: 23.6.2
+Version: 23.6.3
 Summary: Just ctyparser with added version check.
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/ctyparser
 Project-URL: Bug Tracker, https://github.com/mbridak/ctyparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -39,12 +39,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
+Used xpath to parse the download link.
+Chose more narrow raised exceptions.
+Specified utf-8 file encoding.
+Made the linter happy.
+
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.2/README.md` & `notctyparser-23.6.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,12 +20,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
+Used xpath to parse the download link.
+Chose more narrow raised exceptions.
+Specified utf-8 file encoding.
+Made the linter happy.
+
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.2/docs/conf.py` & `notctyparser-23.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `notctyparser-23.6.2/notctyparser/bigcty.py` & `notctyparser-23.6.3/notctyparser/bigcty.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import tempfile
 import zipfile
 from datetime import datetime
 from typing import Union
 
 import feedparser
 import requests
+from lxml import html
 
 DEFAULT_FEED = "http://www.country-files.com/category/big-cty/feed/"
 
 
 class BigCty(collections.abc.Mapping):
     """Class representing a BigCTY dataset.
     Can be initialised with data by passing the path to a valid ``cty.json`` file
@@ -63,42 +64,42 @@
         """Loads a ``cty.json`` file into the instance.
 
         :param cty_file: Path to the file to load.
         :type cty_file: str or os.PathLike
         :return: None
         """
         cty_file = pathlib.Path(cty_file)
-        with cty_file.open("r") as file:
+        with cty_file.open("r", encoding="utf-8") as file:
             ctyjson = json.load(file)
             self._version = ctyjson.pop("version", None)
             self._data = ctyjson
 
     def dump(self, cty_file: Union[str, os.PathLike]) -> None:
         """Dumps the data of the instance to a ``cty.json`` file.
 
         :param cty_file: Path to the file to dump to.
         :type cty_file: str or os.PathLike
         :return: None
         """
         cty_file = pathlib.Path(cty_file)
         datadump = self._data.copy()
         datadump["version"] = self._version
-        with cty_file.open("w") as file:
+        with cty_file.open("w", encoding="utf-8") as file:
             json.dump(datadump, file)
 
     def import_dat(self, dat_file: Union[str, os.PathLike]) -> None:
         """Imports CTY data from a ``CTY.DAT`` file.
 
         :param dat_file: Path to the file to import.
         :type dat_file: str or os.PathLike
         :return: None
         """
         dat_file = pathlib.Path(dat_file)
-        with dat_file.open("r") as file:
-            cty_dict = dict()
+        with dat_file.open("r", encoding="utf-8") as file:
+            cty_dict = {}
 
             # get the version from the file
             ver_match = re.search(self.regex_version_entry, file.read())
             self._version = ver_match.group(1) if ver_match is not None else ""
             file.seek(0)
 
             # stores the previous prefix for the next iteration
@@ -134,15 +135,15 @@
                     last = segments[7]
 
                 # check if the line continues a DXCC
                 elif line != "" and line[0].isspace():
                     overrides = line.strip().rstrip(";").rstrip(",").split(",")
 
                     for item in overrides:
-                        if item not in cty_dict.keys():
+                        if item not in cty_dict:
                             # get the already stored data from primary prefix
                             data = copy.deepcopy(cty_dict[last])
                             # apply regex to extract the prefix and overrides
                             match = re.search(self.regex_dat, item)
                             if match is None:
                                 continue
                             if match.group("itu"):
@@ -159,66 +160,72 @@
                             if item.startswith("="):
                                 data["exact_match"] = True
                             prefix = match.group("prefix")
                             cty_dict[prefix] = data
         self._data = cty_dict
 
     def check_update(self) -> bool:
-        """doc"""
+        """Checks if an update exists.
+        :raises AttributeError : If there is no date in the feed.
+        :return: ``True`` if an update is available, otherwise ``False``.
+        :rtype: bool
+        """
         with requests.Session() as session:
             feed = session.get(DEFAULT_FEED)
             parsed_feed = feedparser.parse(feed.content)
             update_url = parsed_feed.entries[0]["link"]
             date_match = re.search(self.regex_feed_date, update_url)
             if date_match is None:
-                raise Exception(
-                    "Error parsing feed: date missing"
-                )  # TODO: Better exception
+                raise AttributeError("Error parsing feed: date missing")
             date_str = date_match.group(1).title()
             update_date = datetime.strftime(
                 datetime.strptime(date_str, "%d-%B-%Y"), "%Y%m%d"
             )
 
             if self._version == update_date:
                 return False
             return True
 
     def update(self) -> bool:
         """Upates the instance's data from the feed.
 
-        :raises Exception: If there is no date in the feed.
+        :raises AttributeError: If there is no date in the feed.
+        :raises ResourceWarning: If unable to download bigcty.
         :return: ``True`` if an update was done, otherwise ``False``.
         :rtype: bool
         """
         with requests.Session() as session:
             feed = session.get(DEFAULT_FEED)
             parsed_feed = feedparser.parse(feed.content)
             update_url = parsed_feed.entries[0]["link"]
             date_match = re.search(self.regex_feed_date, update_url)
             if date_match is None:
-                raise Exception(
-                    "Error parsing feed: date missing"
-                )  # TODO: Better exception
+                raise AttributeError("Error parsing feed: date missing")
             date_str = date_match.group(1).title()
             update_date = datetime.strftime(
                 datetime.strptime(date_str, "%d-%B-%Y"), "%Y%m%d"
             )
 
             if self._version == update_date:
                 return False
 
             with tempfile.TemporaryDirectory() as temp:
                 path = pathlib.PurePath(temp)
-                dl_url = f"http://www.country-files.com/bigcty/download/{update_date[:4]}/bigcty-{update_date}.zip"  # TODO: Issue #10
+                page = session.get(update_url)
+                tree = html.fromstring(page.content)
+                dl_url = tree.xpath("//a[contains(@href,'zip')]/@href")[0]
                 the_request = session.get(dl_url)
                 if the_request.status_code == 404:
-                    dl_url = f"http://www.country-files.com/bigcty/download/bigcty-{update_date}.zip"
+                    dl_url = (
+                        "http://www.country-files.com/bigcty/download/bigcty-"
+                        f"{update_date}.zip"
+                    )
                     the_request = session.get(dl_url)
                     if the_request.status_code != 200:
-                        raise Exception(
+                        raise ResourceWarning(
                             f"Unable to find and download bigcty-{update_date}.zip"
                         )
                 with open(path / "cty.zip", "wb+") as file:
                     file.write(the_request.content)
                     zipfile.ZipFile(file).extract(
                         "cty.dat", path=str(path)
                     )  # Force cast as str because mypy
```

### Comparing `notctyparser-23.6.2/notctyparser.egg-info/PKG-INFO` & `notctyparser-23.6.3/notctyparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notctyparser
-Version: 23.6.2
+Version: 23.6.3
 Summary: Just ctyparser with added version check.
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/ctyparser
 Project-URL: Bug Tracker, https://github.com/mbridak/ctyparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -39,12 +39,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
+Used xpath to parse the download link.
+Chose more narrow raised exceptions.
+Specified utf-8 file encoding.
+Made the linter happy.
+
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.2/pyproject.toml` & `notctyparser-23.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notctyparser" 
-version = "23.6.2"
+version = "23.6.3"
 description = "Just ctyparser with added version check."
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

