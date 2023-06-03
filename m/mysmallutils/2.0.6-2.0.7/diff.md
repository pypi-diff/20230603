# Comparing `tmp/mysmallutils-2.0.6.tar.gz` & `tmp/mysmallutils-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysmallutils-2.0.6.tar", last modified: Wed May 24 14:00:25 2023, max compression
+gzip compressed data, was "mysmallutils-2.0.7.tar", last modified: Sat Jun  3 12:55:30 2023, max compression
```

## Comparing `mysmallutils-2.0.6.tar` & `mysmallutils-2.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:00:25.345986 mysmallutils-2.0.6/
--rw-rw-rw-   0        0        0    59126 2023-05-24 14:00:25.344534 mysmallutils-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    58644 2023-05-24 12:29:20.000000 mysmallutils-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 14:00:25.292193 mysmallutils-2.0.6/mysmallutils.egg-info/
--rw-rw-rw-   0        0        0    59126 2023-05-24 14:00:25.000000 mysmallutils-2.0.6/mysmallutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-24 14:00:25.000000 mysmallutils-2.0.6/mysmallutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:00:25.000000 mysmallutils-2.0.6/mysmallutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 14:00:25.000000 mysmallutils-2.0.6/mysmallutils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 14:00:25.341232 mysmallutils-2.0.6/mysutils/
--rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/__init__.py
--rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.6/mysutils/collections.py
--rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/command.py
--rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/config.py
--rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/fastapi.py
--rw-rw-rw-   0        0        0    25877 2023-02-13 14:44:23.000000 mysmallutils-2.0.6/mysutils/file.py
--rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/logging.py
--rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/method.py
--rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/misc.py
--rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/request.py
--rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/service.py
--rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.6/mysutils/tar.py
--rw-rw-rw-   0        0        0    10658 2023-05-24 13:57:24.000000 mysmallutils-2.0.6/mysutils/text.py
--rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.6/mysutils/tmp.py
--rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/unittest.py
--rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.6/mysutils/web.py
--rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.6/mysutils/yaml.py
--rw-rw-rw-   0        0        0       42 2023-05-24 14:00:25.345986 mysmallutils-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1711 2023-05-24 12:54:23.000000 mysmallutils-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.182975 mysmallutils-2.0.7/
+-rw-rw-rw-   0        0        0    59645 2023-06-03 12:55:30.181975 mysmallutils-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    59163 2023-06-03 12:54:04.000000 mysmallutils-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.096162 mysmallutils-2.0.7/mysmallutils.egg-info/
+-rw-rw-rw-   0        0        0    59645 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.178658 mysmallutils-2.0.7/mysutils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/__init__.py
+-rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.7/mysutils/collections.py
+-rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/command.py
+-rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/config.py
+-rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/fastapi.py
+-rw-rw-rw-   0        0        0    26268 2023-06-03 12:41:08.000000 mysmallutils-2.0.7/mysutils/file.py
+-rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/logging.py
+-rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/method.py
+-rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/misc.py
+-rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/request.py
+-rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/service.py
+-rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.7/mysutils/tar.py
+-rw-rw-rw-   0        0        0    10988 2023-06-03 12:53:32.000000 mysmallutils-2.0.7/mysutils/text.py
+-rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.7/mysutils/tmp.py
+-rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/unittest.py
+-rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/web.py
+-rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.7/mysutils/yaml.py
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:55:30.183969 mysmallutils-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1711 2023-05-24 14:01:37.000000 mysmallutils-2.0.7/setup.py
```

### Comparing `mysmallutils-2.0.6/PKG-INFO` & `mysmallutils-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.6
+Version: 2.0.7
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -797,14 +797,25 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
+## Hash a text
+
+An very easy way to hash a text.
+
+```python
+from mysutils.text import hash_text
+
+# Print the SHA256 hash of that text
+print(hash_text('This is a text'))
+```
+
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
 ```python
 from mysutils.file import open_file, force_open
@@ -1255,14 +1266,27 @@
 
 # Create 4 files with different extensions
 touch('1.txt', '2.txt', '3.json', '4.yaml')
 # Return ['1.txt', '2.txt', '4.yaml']
 expand_wildcards('*.txt', '*.yaml')
 ```
 
+## Text to filename
+
+Convert a text into a filename, removing unsupported characters.
+
+```python
+from mysutils.file import to_filename
+
+# Print "Hello World_ How are you_"
+print(to_filename('Hello World! How are you?'))
+
+# Print "Hello World_ How are you_.srt"
+print(to_filename('Hello World! How are you?', '.srt'))
+```
 
 # Removable files<a id="removable-files"></a>
 Many times it is necessary to remove temporal files after their use, even if there are any problem with the process.
 These classes and functions allow you to self-removable files, temporally or not.
 
 For example, with removable_tmp() function you can do:
 ```python
```

### Comparing `mysmallutils-2.0.6/README.md` & `mysmallutils-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -783,14 +783,25 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
+## Hash a text
+
+An very easy way to hash a text.
+
+```python
+from mysutils.text import hash_text
+
+# Print the SHA256 hash of that text
+print(hash_text('This is a text'))
+```
+
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
 ```python
 from mysutils.file import open_file, force_open
@@ -1241,14 +1252,27 @@
 
 # Create 4 files with different extensions
 touch('1.txt', '2.txt', '3.json', '4.yaml')
 # Return ['1.txt', '2.txt', '4.yaml']
 expand_wildcards('*.txt', '*.yaml')
 ```
 
+## Text to filename
+
+Convert a text into a filename, removing unsupported characters.
+
+```python
+from mysutils.file import to_filename
+
+# Print "Hello World_ How are you_"
+print(to_filename('Hello World! How are you?'))
+
+# Print "Hello World_ How are you_.srt"
+print(to_filename('Hello World! How are you?', '.srt'))
+```
 
 # Removable files<a id="removable-files"></a>
 Many times it is necessary to remove temporal files after their use, even if there are any problem with the process.
 These classes and functions allow you to self-removable files, temporally or not.
 
 For example, with removable_tmp() function you can do:
 ```python
```

### Comparing `mysmallutils-2.0.6/mysmallutils.egg-info/PKG-INFO` & `mysmallutils-2.0.7/mysmallutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.6
+Version: 2.0.7
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -797,14 +797,25 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
+## Hash a text
+
+An very easy way to hash a text.
+
+```python
+from mysutils.text import hash_text
+
+# Print the SHA256 hash of that text
+print(hash_text('This is a text'))
+```
+
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
 ```python
 from mysutils.file import open_file, force_open
@@ -1255,14 +1266,27 @@
 
 # Create 4 files with different extensions
 touch('1.txt', '2.txt', '3.json', '4.yaml')
 # Return ['1.txt', '2.txt', '4.yaml']
 expand_wildcards('*.txt', '*.yaml')
 ```
 
+## Text to filename
+
+Convert a text into a filename, removing unsupported characters.
+
+```python
+from mysutils.file import to_filename
+
+# Print "Hello World_ How are you_"
+print(to_filename('Hello World! How are you?'))
+
+# Print "Hello World_ How are you_.srt"
+print(to_filename('Hello World! How are you?', '.srt'))
+```
 
 # Removable files<a id="removable-files"></a>
 Many times it is necessary to remove temporal files after their use, even if there are any problem with the process.
 These classes and functions allow you to self-removable files, temporally or not.
 
 For example, with removable_tmp() function you can do:
 ```python
```

### Comparing `mysmallutils-2.0.6/mysutils/collections.py` & `mysmallutils-2.0.7/mysutils/collections.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/command.py` & `mysmallutils-2.0.7/mysutils/command.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/config.py` & `mysmallutils-2.0.7/mysutils/config.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/fastapi.py` & `mysmallutils-2.0.7/mysutils/fastapi.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/file.py` & `mysmallutils-2.0.7/mysutils/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from os import makedirs, remove, rmdir, scandir, PathLike
 from os.path import exists, dirname, join, basename, isdir
 from shutil import copyfile, rmtree
 from sys import stdout
 from shutil import move
 from typing import Union, Optional, TextIO, Any, List, Tuple, IO
 import glob
+from string import ascii_letters, digits
 
 
 def expand_wildcards(*filenames: Union[PathLike, str, bytes]) -> List[str]:
     """ Expand a list of files if they have wildcards.
     :param filenames: List of filenames to expand.
     :return: List of expanded filenames.
     """
@@ -560,7 +561,17 @@
     """
     try:
         with codecs.open(file, 'r', encoding=encoding) as fh:
             fh.readlines()
     except UnicodeDecodeError:
         return False
     return True
+
+
+def to_filename(text: str, ext: str = '') -> str:
+    """ Convert a string to a valid filename.
+    :param text: The string to convert.
+    :param ext: The file extension.
+    :return: The converted string.
+    """
+    valid_chars = f'-_.() {ascii_letters}{digits}'
+    return ''.join(c if c in valid_chars else '_' for c in text) + ext
```

### Comparing `mysmallutils-2.0.6/mysutils/logging.py` & `mysmallutils-2.0.7/mysutils/logging.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/method.py` & `mysmallutils-2.0.7/mysutils/method.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/request.py` & `mysmallutils-2.0.7/mysutils/request.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/service.py` & `mysmallutils-2.0.7/mysutils/service.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/tar.py` & `mysmallutils-2.0.7/mysutils/tar.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/text.py` & `mysmallutils-2.0.7/mysutils/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from enum import Enum, unique
+from hashlib import sha256
 from re import Match
 from typing import Union, Iterator, List
 
 PROTOCOL_PATTERN = r'[\w\+]+://'
 DOMAIN_PATTERN = r'\w[\w%@:\-_]+(\.\w[\w%@:\-_]*)+/?'
 PATH_PATTERN = r'([\w%@\.\-_]+/?)*'
 QUERY_PATTERN = r'(\?[\w%\-_&=]*)?'
@@ -271,7 +272,16 @@
 
 def is_color(color_code: str) -> bool:
     """ Check if a color code is a valid ANSI color code.
     :param color_code: The color code to evaluate.
     :return: True if the color is valid, False otherwise.
     """
     return bool(re.match(r'^\033\[(([3-4][0-7]|39|49|59)|(38|48|58);(5;[0-9]+|2;[0-9]+;[0-9]+;[0-9]+))m$', color_code))
+
+
+def hash_text(text: str, encoding='utf-8') -> str:
+    """ Hash the text with SHA256.
+    :param text: The text to hash.
+    :param encoding: The encoding to convert to bytes.
+    :return: A SHA256 hash that represents that text.
+    """
+    return sha256(text.encode(encoding)).hexdigest()
```

### Comparing `mysmallutils-2.0.6/mysutils/tmp.py` & `mysmallutils-2.0.7/mysutils/tmp.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/unittest.py` & `mysmallutils-2.0.7/mysutils/unittest.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/web.py` & `mysmallutils-2.0.7/mysutils/web.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/mysutils/yaml.py` & `mysmallutils-2.0.7/mysutils/yaml.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.6/setup.py` & `mysmallutils-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 setuptools.setup(
     cmdclass={
         'clean': CleanCommand,
         'prepublish': PrepublishCommand,
     },
     name='mysmallutils',
-    version='2.0.6',
+    version='2.0.7',
     url='https://github.com/jmgomezsoriano/mysmallutils',
     license='LGPL2',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Small Python utils to do life easier.',
```

