# Comparing `tmp/libretrofuzz-2.8.2.tar.gz` & `tmp/libretrofuzz-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.8.2.tar", max compression
+gzip compressed data, was "libretrofuzz-2.8.3.tar", max compression
```

## Comparing `libretrofuzz-2.8.2.tar` & `libretrofuzz-2.8.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-03 18:04:27.749655 libretrofuzz-2.8.2/LICENSE
--rw-r--r--   0        0        0     7166 2023-06-03 18:04:27.749655 libretrofuzz-2.8.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-03 18:04:27.749655 libretrofuzz-2.8.2/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    47734 2023-06-03 18:04:27.749655 libretrofuzz-2.8.2/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      952 2023-06-03 18:04:27.753655 libretrofuzz-2.8.2/pyproject.toml
--rw-r--r--   0        0        0     8328 2023-06-03 18:04:36.912572 libretrofuzz-2.8.2/setup.py
--rw-r--r--   0        0        0     8310 2023-06-03 18:04:36.913553 libretrofuzz-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-03 21:28:03.640685 libretrofuzz-2.8.3/LICENSE
+-rw-r--r--   0        0        0     7166 2023-06-03 21:28:03.640685 libretrofuzz-2.8.3/README.rst
+-rw-r--r--   0        0        0       22 2023-06-03 21:28:03.640685 libretrofuzz-2.8.3/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    47084 2023-06-03 21:28:03.640685 libretrofuzz-2.8.3/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      952 2023-06-03 21:28:03.640685 libretrofuzz-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0     8328 2023-06-03 21:28:18.602472 libretrofuzz-2.8.3/setup.py
+-rw-r--r--   0        0        0     8310 2023-06-03 21:28:18.603587 libretrofuzz-2.8.3/PKG-INFO
```

### Comparing `libretrofuzz-2.8.2/LICENSE` & `libretrofuzz-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.8.2/README.rst` & `libretrofuzz-2.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.8.2/libretrofuzz/__main__.py` & `libretrofuzz-2.8.3/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,93 +229,73 @@
     if not hack:
         t = removeparenthesis(t,'[',']')
     #change all common ascci symbol characters we aren't going to use after this (, and ')
     t = replacemany(t, '_()[]{}-.!?#"', ' ')
     #strips just because the user may have made a mistake naming the source
     #(or the replacement above introduce boundary spaces)
     t = t.strip()
+    #normalize case
+    t = t.lower()
     #beginning and end definite articles in several european languages (people move them)
-    #make sure we're only removing the capitalized start and end forms with spaces
-    t = removefirst(t, ', The')
-    t = removeprefix(t, 'The ')
-    t = removefirst(t, ', Los')
-    t = removeprefix(t, 'Los ')
-    t = removefirst(t, ', Las')
-    t = removeprefix(t, 'Las ')
-    t = removefirst(t, ', Les')
-    t = removeprefix(t, 'Les ')
-    t = removefirst(t, ', Le')
-    t = removeprefix(t, 'Le ')
-    t = removefirst(t, ', La')
-    t = removeprefix(t, 'La ')
-    t = removefirst(t, ', L\'')
+    #make sure we're only removing the start and end forms with spaces
+    t = removefirst(t, ', the')
+    t = removeprefix(t, 'the ')
+    t = removefirst(t, ', los')
+    t = removeprefix(t, 'los ')
+    t = removefirst(t, ', las')
+    t = removeprefix(t, 'las ')
+    t = removefirst(t, ', les')
+    t = removeprefix(t, 'les ')
+    t = removefirst(t, ', le')
+    t = removeprefix(t, 'le ')
+    t = removefirst(t, ', la')
+    t = removeprefix(t, 'la ')
+    t = removefirst(t, ', l\'')
     #L' sometimes ommits the space so always remove L' at the start even without space
-    t = removeprefix(t, 'L\'')  #if there is a extra space the next join will remove it
-    t = removefirst(t, ', Der')
-    t = removeprefix(t, 'Der ')
-    t = removefirst(t, ', Die')
-    t = removeprefix(t, 'Die ')
-    t = removefirst(t, ', Das')
-    t = removeprefix(t, 'Das ')
-    t = removefirst(t, ', El')
-    t = removeprefix(t, 'El ')
-    t = removefirst(t, ', Os')
-    t = removeprefix(t, 'Os ')
-    t = removefirst(t, ', As')
-    t = removeprefix(t, 'As ')
-    t = removefirst(t, ', O')
-    t = removeprefix(t, 'O ')
-    t = removefirst(t, ', A')
-    t = removeprefix(t, 'A ')
+    t = removeprefix(t, 'l\'')  #if there is a extra space the next join will remove it
+    t = removefirst(t, ', der')
+    t = removeprefix(t, 'der ')
+    t = removefirst(t, ', die')
+    t = removeprefix(t, 'die ')
+    t = removefirst(t, ', das')
+    t = removeprefix(t, 'das ')
+    t = removefirst(t, ', el')
+    t = removeprefix(t, 'el ')
+    t = removefirst(t, ', os')
+    t = removeprefix(t, 'os ')
+    t = removefirst(t, ', as')
+    t = removeprefix(t, 'as ')
+    t = removefirst(t, ', o')
+    t = removeprefix(t, 'o ')
+    t = removefirst(t, ', a')
+    t = removeprefix(t, 'a ')
+    #remove the symbols used in the definite article normalization
+    t = replacemany(t, ',\'', '')
     #Tries to make roman numerals in the range 1-20 equivalent to normal numbers (to handle names that change it).
     #If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
-    t = t.replace('XVIII', '18')
     t = t.replace('xviii', '18')
-    t = t.replace('XVII',  '17')
     t = t.replace('xvii',  '17')
-    t = t.replace('XVI' ,  '16')
     t = t.replace('xvi' ,  '16')
-    t = t.replace('XIII',  '13')
     t = t.replace('xiii',  '13')
-    t = t.replace('XII' ,  '12')
     t = t.replace('xii' ,  '12')
-    t = t.replace('XIV' ,  '14')
     t = t.replace('xiv' ,  '14')
-    t = t.replace('XV'  ,  '15')
     t = t.replace('xv'  ,  '15')
-    t = t.replace('XIX',   '19')
     t = t.replace('xix',   '19')
-    t = t.replace('XX',   '20')
     t = t.replace('xx',   '20')
-    t = t.replace('XI',   '11')
     t = t.replace('xi',   '11')
-    t = t.replace('VIII', '8')
     t = t.replace('viii', '8')
-    t = t.replace('VII',  '7')
     t = t.replace('vii',  '7')
-    t = t.replace('VI' ,  '6')
     t = t.replace('vi' ,  '6')
-    t = t.replace('III',  '3')
     t = t.replace('iii',  '3')
-    t = t.replace('II' ,  '2')
     t = t.replace('ii' ,  '2')
-    t = t.replace('IV' ,  '4')
     t = t.replace('iv' ,  '4')
-    t = t.replace('V'  ,  '5')
     t = t.replace('v'  ,  '5')
-    t = t.replace('IX',   '9')
     t = t.replace('ix',   '9')
-    t = t.replace('X',   '10')
     t = t.replace('x',   '10')
-    t = t.replace('I',    '1')
     t = t.replace('i',    '1')
-    #remove the symbols used in the definite article normalization
-    t = replacemany(t, ',\'', '')
-    #normalize case
-    t = t.lower()
     #this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
     #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
     t = t.replace(' and ',  '')
     #although all names have spaces (now), the local names may have weird spaces,
     #so to equalize them after the space dependent checks (this also strips)
     t = ''.join(t.split())
     #remove diacritics (does nothing to asian languages diacritics, only for 2 to 1 character combinations)
```

### Comparing `libretrofuzz-2.8.2/pyproject.toml` & `libretrofuzz-2.8.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.8.2"
+version = "2.8.3"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.8.2/setup.py` & `libretrofuzz-2.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.8.2',
+    'version': '2.8.3',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n ``libretro-fuzz --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.\n\nExample:\n  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy\n                        matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails.\n                        If not provided, asked from the user.\n  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.\n                        No-op with --no-image.  [1<=x<=10]\n  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths -\n                        in the playlist, can be used multiple times and\n                        matches reset thumbnails, --filter '\\*' downloads all.\n  --score FUZZ          Download fuzz (less is more fuzz, 100 being average).\n                        No-op with --no-fail.  [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to --score 0.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if\n                        there is at least one in cache to avoid mixing\n                        thumbnails from different server directories on\n                        repeated calls. No-op with --filter.\n  --no-subtitle         Ignores text after last ' - ' or ': '. ':' can't occur\n                        in server names, so if the server has 'Name\\_\n                        subtitle.png' and not 'Name - subtitle.png'\n                        (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false\n                        positives. Forced with --before.\n  --hack                Matches [] delimited metadata and may cause false\n                        positives, Best used if the hack has thumbnails.\n                        Ignored with --before.\n  --before TEXT         Use only the part of the label before TEXT to match.\n                        TEXT may not be inside of brackets of any kind, may\n                        cause false positives but some labels do not have\n                        traditional separators. Forces ignoring metadata.\n  --verbose             Shows the failures, score and normalized local and\n                        server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.8.2/PKG-INFO` & `libretrofuzz-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.8.2
+Version: 2.8.3
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

