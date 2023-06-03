# Comparing `tmp/lishixian-0.2.2.tar.gz` & `tmp/lishixian-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lishixian-0.2.2.tar", last modified: Sun Mar 12 07:30:39 2023, max compression
+gzip compressed data, was "dist\lishixian-0.2.3.tar", last modified: Sat Jun  3 03:21:40 2023, max compression
```

## Comparing `lishixian-0.2.2.tar` & `lishixian-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 07:30:39.000000 lishixian-0.2.2/
--rw-rw-rw-   0        0        0       98 2022-03-17 14:04:28.000000 lishixian-0.2.2/.gitignore
--rwxrwxrwx   0        0        0       32 2022-03-17 14:03:45.000000 lishixian-0.2.2/install.bat
--rw-rw-rw-   0        0        0     1119 2022-03-17 14:04:28.000000 lishixian-0.2.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-03-12 07:30:39.000000 lishixian-0.2.2/lishixian/
--rw-rw-rw-   0        0        0     3131 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/auto.py
--rw-rw-rw-   0        0        0     3446 2022-07-24 01:20:25.000000 lishixian-0.2.2/lishixian/c.py
--rw-rw-rw-   0        0        0     3967 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/cls.py
--rw-rw-rw-   0        0        0     2827 2022-11-25 21:39:08.000000 lishixian-0.2.2/lishixian/dec.py
--rw-rw-rw-   0        0        0     9104 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/doc.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:30:39.000000 lishixian-0.2.2/lishixian/docs/
--rw-rw-rw-   0        0        0     1119 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian/docs/license.txt
--rw-rw-rw-   0        0        0     3699 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian/docs/readme.md
--rw-rw-rw-   0        0        0        5 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian/docs/version.txt
--rw-rw-rw-   0        0        0       59 2022-03-17 14:04:28.000000 lishixian-0.2.2/lishixian/docs/__init__.py
--rw-rw-rw-   0        0        0     2375 2022-03-17 14:04:28.000000 lishixian-0.2.2/lishixian/gui.py
--rw-rw-rw-   0        0        0     1639 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/line.py
--rw-rw-rw-   0        0        0     2460 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/new.py
--rw-rw-rw-   0        0        0      956 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/np.py
--rw-rw-rw-   0        0        0     1264 2022-03-17 14:03:45.000000 lishixian-0.2.2/lishixian/reg.py
--rw-rw-rw-   0        0        0     4867 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/useful.py
--rw-rw-rw-   0        0        0     4131 2022-07-24 01:20:27.000000 lishixian-0.2.2/lishixian/windll.py
--rw-rw-rw-   0        0        0     1791 2023-03-12 07:10:25.000000 lishixian-0.2.2/lishixian/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:30:39.000000 lishixian-0.2.2/lishixian.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4246 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-03-12 07:30:39.000000 lishixian-0.2.2/lishixian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-03-12 07:30:38.000000 lishixian-0.2.2/lishixian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2022-03-17 14:03:45.000000 lishixian-0.2.2/MANIFEST.in
--rwxrwxrwx   0        0        0       57 2022-03-17 14:03:45.000000 lishixian-0.2.2/pip_uninstall.bat
--rw-rw-rw-   0        0        0     4246 2023-03-12 07:30:39.000000 lishixian-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3699 2023-03-12 07:10:25.000000 lishixian-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-12 07:30:39.000000 lishixian-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1250 2022-03-17 14:03:45.000000 lishixian-0.2.2/setup.py
--rw-rw-rw-   0        0        0        5 2023-03-12 07:10:25.000000 lishixian-0.2.2/VERSION.txt
--rwxrwxrwx   0        0        0      289 2022-03-17 14:03:45.000000 lishixian-0.2.2/__local_test.bat
--rwxrwxrwx   0        0        0      208 2022-03-17 14:03:45.000000 lishixian-0.2.2/__pypi_upload.bat
+drwxrwxrwx   0        0        0        0 2023-06-03 03:21:40.000000 lishixian-0.2.3/
+-rw-rw-rw-   0        0        0       98 2022-03-17 14:04:28.000000 lishixian-0.2.3/.gitignore
+-rwxrwxrwx   0        0        0       32 2022-03-17 14:03:45.000000 lishixian-0.2.3/install.bat
+-rw-rw-rw-   0        0        0     1119 2022-03-17 14:04:28.000000 lishixian-0.2.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian/
+-rw-rw-rw-   0        0        0     3131 2023-03-12 07:10:25.000000 lishixian-0.2.3/lishixian/auto.py
+-rw-rw-rw-   0        0        0     3446 2022-07-24 01:20:25.000000 lishixian-0.2.3/lishixian/c.py
+-rw-rw-rw-   0        0        0     3967 2023-03-12 07:10:25.000000 lishixian-0.2.3/lishixian/cls.py
+-rw-rw-rw-   0        0        0     2989 2023-06-03 03:08:08.000000 lishixian-0.2.3/lishixian/dec.py
+-rw-rw-rw-   0        0        0     9104 2023-03-12 07:10:25.000000 lishixian-0.2.3/lishixian/doc.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian/docs/
+-rw-rw-rw-   0        0        0     1119 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian/docs/license.txt
+-rw-rw-rw-   0        0        0     4019 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian/docs/readme.md
+-rw-rw-rw-   0        0        0        5 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian/docs/version.txt
+-rw-rw-rw-   0        0        0       59 2022-03-17 14:04:28.000000 lishixian-0.2.3/lishixian/docs/__init__.py
+-rw-rw-rw-   0        0        0     2375 2022-03-17 14:04:28.000000 lishixian-0.2.3/lishixian/gui.py
+-rw-rw-rw-   0        0        0     1911 2023-06-03 03:06:31.000000 lishixian-0.2.3/lishixian/line.py
+-rw-rw-rw-   0        0        0     2532 2023-06-03 03:06:31.000000 lishixian-0.2.3/lishixian/new.py
+-rw-rw-rw-   0        0        0      956 2023-03-12 07:10:25.000000 lishixian-0.2.3/lishixian/np.py
+-rw-rw-rw-   0        0        0     1264 2022-03-17 14:03:45.000000 lishixian-0.2.3/lishixian/reg.py
+-rw-rw-rw-   0        0        0     5874 2023-06-03 03:08:08.000000 lishixian-0.2.3/lishixian/useful.py
+-rw-rw-rw-   0        0        0     4131 2022-07-24 01:20:27.000000 lishixian-0.2.3/lishixian/windll.py
+-rw-rw-rw-   0        0        0     2300 2023-06-03 03:20:50.000000 lishixian-0.2.3/lishixian/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4572 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 03:21:40.000000 lishixian-0.2.3/lishixian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2022-03-17 14:03:45.000000 lishixian-0.2.3/MANIFEST.in
+-rwxrwxrwx   0        0        0       57 2022-03-17 14:03:45.000000 lishixian-0.2.3/pip_uninstall.bat
+-rw-rw-rw-   0        0        0     4572 2023-06-03 03:21:40.000000 lishixian-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4019 2023-06-03 03:20:50.000000 lishixian-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:21:40.000000 lishixian-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1256 2023-06-03 03:20:50.000000 lishixian-0.2.3/setup.py
+-rw-rw-rw-   0        0        0        5 2023-06-03 03:20:50.000000 lishixian-0.2.3/VERSION.txt
+-rwxrwxrwx   0        0        0      289 2022-03-17 14:03:45.000000 lishixian-0.2.3/__local_test.bat
+-rwxrwxrwx   0        0        0      208 2022-03-17 14:03:45.000000 lishixian-0.2.3/__pypi_upload.bat
```

### Comparing `lishixian-0.2.2/LICENSE.txt` & `lishixian-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/auto.py` & `lishixian-0.2.3/lishixian/auto.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/c.py` & `lishixian-0.2.3/lishixian/c.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/cls.py` & `lishixian-0.2.3/lishixian/cls.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/dec.py` & `lishixian-0.2.3/lishixian/dec.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 
 __all__ = list(globals())
 
 
 def main(f):
     import inspect
     if '__main__' == inspect.currentframe().f_back.f_globals['__name__']:
-        if len(sys.argv) == 1:
-            f()
-        for v in sys.argv[1:]:
-            f(v)
+        try:
+            if len(sys.argv) == 1:
+                f()
+            for v in sys.argv[1:]:
+                f(v)
+        except Exception:
+            import traceback
+            traceback.print_exc()
+        input('Press enter to exit: ')
     return f
 
 
 def timeit(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         s = time.time()
```

### Comparing `lishixian-0.2.2/lishixian/doc.py` & `lishixian-0.2.3/lishixian/doc.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/docs/license.txt` & `lishixian-0.2.3/lishixian/docs/license.txt`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/docs/readme.md` & `lishixian-0.2.3/lishixian/docs/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Lishixian Library
-Contain 111 functions.
+# Lite Software eXtension
+
+Contain 10 modules and 115 functions.
 
 
 ## About
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
 - __Github:__ https://github.com/znsoooo/lishixian
@@ -12,14 +13,21 @@
 
 ## Install
 ```bash
 pip install lishixian --upgrade
 ```
 
 
+## Usage
+```python
+import lishixian as lsx
+lsx.help()
+```
+
+
 ## Modules
 
 ### Top module
 - all()
 - help()
 
 ### Module 'cls'
@@ -34,14 +42,15 @@
 - protect(f)
 - surround(before=(), after=())
 - hotkey(key='F12')
 - threads(cnt)
 
 ### Module 'new'
 - print(*value, file=sys.stdout)
+- time(start=0)
 - infinity = <class 'itertools.count'>
 - makedirs(name, mode=511, *, exist_ok=True)
 - breakpoint()
 - popen(cmd)
 - listdir(*paths)
 - findall(pattern, string, flags=0)
 - split(arr, cols)
@@ -51,47 +60,55 @@
 
 ### Module 'line'
 - s128 = bytes(range(128)).decode()
 - s127 = bytes(range(32, 127)).decode()
 - empty(*v, **kv)
 - freeze(fn, *v, **kv)
 - t(arr)
+- crc(b)
 - md5(b)
 - mask(p)
 - start(func, *args, **kwargs)
 - create(file)
 - pprint(*value, file=sys.stdout)
 - dumps(data)
 - sort_kv(d, reverse=False)
 - sort_key(d, reverse=False)
 - sort_num(s)
 - str2dict(s)
 - tuple2item(item)
 - unique(arr)
+- flatten(arr)
+- reshape(arr, width)
 - pc_ip()
 - pc_mac()
 - pc_user()
 - randombytes(n)
 - join(*s, sp='')
 
 ### Module 'useful'
-- tag()
-- log(*value)
-- check(obj, patt='.*')
+- log(*value, file='log.txt')
+- progress(*value, interval=1)
+- check(obj, patt='.*', stdout=True)
 - fps()
+- stem(p)
 - select(path)
 - path_mark(path, mark='.bak')
-- path_quote(p, repl=None)
+- path_safe(p, repl=None)
 - path_split(p)
 - path_unique(p, dash='-')
+- file_mtime(path)
+- file_ctime(path)
+- file_utime(path, date)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
 - urlopen(url, timeout=5)
+- scan(format, string)
 - findpair(s, p1='(', p2=')', st=0)
 - bytes_format(data, n=16)
 - bytes_print(data, n=16)
 - bytes_hex(data, offset=0, length=-1, slice=-1)
 - install(path, block=False)
 - input_wait(msg)
 - input_default(msg, default)
@@ -107,16 +124,16 @@
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
 - Monitor(func)
 - Recoder(complete=False)
 
 ### Module 'doc'
-- read(file)
-- write(file, data)
+- read(file, encoding='u8')
+- write(file, data, encoding='u8')
 - ReadIni(file, encoding='u8')
 - WriteIni(file, dic, encoding='u8')
 - WriteTxt(file, data, encoding='utf-8-sig')
 - ReadCsv(file, encoding='utf-8-sig')
 - WriteCsv(file, data, encoding='utf-8-sig', errors='ignore')
 - WriteExcel(file, data, new_sheet='sheet1')
 - OpenExcel(file)
@@ -140,13 +157,13 @@
 - EventThread(parent, id, target=<class 'bool'>, *args, **kwargs)
 
 ### Module 'np'
 - imread(file)
 - imwrite(file, im)
 - imshow(img, delay=50, title='')
 - imsave(file)
-- imiter(file_or_id, st=None, ed=None)
+- imiter(file_or_id)
 
 
 ## Comment
 1. Lib `lsx` is same as `lishixian` in `pypi.org`.
 2. If you **really** need domain `lsx` in `pypi.org`, contact me with `Email`.
```

### Comparing `lishixian-0.2.2/lishixian/gui.py` & `lishixian-0.2.3/lishixian/gui.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/line.py` & `lishixian-0.2.3/lishixian/line.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 import sys
 import json
 import uuid
 import random
 import socket
 import getpass
 import hashlib
+import binascii
 from threading import Thread
 
 __all__ = list(globals())
 
 s128 = bytes(range(128)).decode()
 s127 = bytes(range(32, 127)).decode()
 
 empty = lambda *v, **kv: None
 freeze = lambda fn, *v, **kv: (lambda: fn(*v, **kv))
 
 t = lambda arr: list(zip(*arr))
 
-md5 = lambda b: hashlib.md5(b).hexdigest()
+crc = lambda b: '0x%04X' % binascii.crc_hqx(b if isinstance(b, bytes) else open(b, 'rb').read(), 0)
+md5 = lambda b: hashlib.md5(b if isinstance(b, bytes) else open(b, 'rb').read()).hexdigest()
 mask = lambda p: open(p + '.inv', 'wb').write(bytes(255 - b for b in open(p, 'rb').read()))
 start = lambda func, *args, **kwargs: Thread(target=func, args=args, kwargs=kwargs).start()
 create = lambda file: open(file, 'w').close()
 pprint = lambda *value, file=sys.stdout: print(' '.join(map(str, value)) + '\n', end='', file=file)
 
 dumps = lambda data: json.dumps(data, ensure_ascii=False, indent=2)
 
@@ -32,14 +34,16 @@
 sort_key = lambda d, reverse=False: sorted(d, key=d.__getitem__, reverse=reverse)
 sort_num = lambda s: [(s, int(n)) for s, n in re.findall(r'(\D+)(\d+)', 'a%s0' % s)]
 
 str2dict = lambda s: dict(re.findall(r'(.*?):(.*)', s))
 tuple2item = lambda item: item if len(item) > 1 else item[0]
 
 unique = lambda arr: sorted(set(arr), key=arr.index)
+flatten = lambda arr: sum(arr[1:], arr[0])
+reshape = lambda arr, width: list(zip(*[iter(arr)]*width))
 
 pc_ip = lambda: socket.gethostbyname(socket.gethostname())
 pc_mac = lambda: '-'.join(re.findall('..', uuid.uuid1().hex[-12:].upper()))
 pc_user = lambda: getpass.getuser()
 
 randombytes = lambda n: bytes(random.randint(0, 255) for i in range(n))
```

### Comparing `lishixian-0.2.2/lishixian/new.py` & `lishixian-0.2.3/lishixian/new.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import re
 import pdb
 import sys
 import itertools
 import subprocess
 from functools import partial
 from contextlib import suppress
+from time import time as _time
 
 _open = open
 
 
 __all__ = list(globals())
 
 
 _print, print = print, lambda *value, file=sys.stdout: _print(' '.join(map(str, value)) + '\n', end='', file=file)
+time = lambda start=0: _time() - start
 infinity = itertools.count
 makedirs = partial(os.makedirs, exist_ok=True)
 breakpoint = lambda: pdb.set_trace()
 # open = partial(open, encoding='u8')
 popen = lambda cmd: subprocess.Popen(cmd, -1, None, -1, -1, -1, shell=True).stdout
 listdir = lambda *paths: os.listdir(os.path.join(*paths))
 findall = lambda pattern, string, flags=0: [(m.start(), m.end(), m.group()) for m in re.finditer(pattern, string, flags)]
```

### Comparing `lishixian-0.2.2/lishixian/np.py` & `lishixian-0.2.3/lishixian/np.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/reg.py` & `lishixian-0.2.3/lishixian/reg.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian/useful.py` & `lishixian-0.2.3/lishixian/useful.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,42 +3,47 @@
 import os
 import html
 import time
 import traceback
 import urllib.parse
 import urllib.request
 
-# LOG = time.strftime('RECORD_%Y%m%d_%H%M%S.log')
-LOG = time.strftime('LOG_%Y%m%d_%H%M%S.txt')
-
 
 __all__ = list(globals())
 
 
 # ---------------------------------------------------------------------------
 # Debug
 # ---------------------------------------------------------------------------
 
 
-def tag():
-    return time.strftime('[%Y-%m-%d %H:%M:%S] ')
-
+def log(*value, file='log.txt'):
+    string = ' '.join(map(str, value)) + '\n'
+    header = time.strftime('[%Y-%m-%d %H:%M:%S] ')
+    print(string, end='')
+    with open(file, 'a', encoding='u8') as f:
+        f.write(header + string)
+
+
+_last = 0
+def progress(*value, interval=1):
+    global _last
+    now = time.time()
+    if interval == 0 or now - _last > interval:
+        _last = now
+        print(*value)
 
-def log(*value):
-    s = tag() + ' '.join(map(str, value))
-    with open(LOG, 'a', encoding='u8') as f:
-        f.write(s)
 
-
-def check(obj, patt='.*'):
+def check(obj, patt='.*', stdout=True):
     import re
     import sys
     import inspect
     patt = re.compile(patt)
-    print('\nobj:', obj)
+    stdout = {True: sys.stdout, False: sys.stderr}.get(stdout, stdout)
+    print('obj: %r' % obj, end='')
     for key in sorted(dir(obj)):
         attr = getattr(obj, key)
         try:
             key += str(inspect.signature(attr))
         except (TypeError, ValueError):
             pass
         if patt.fullmatch(key):
@@ -48,31 +53,32 @@
                 key += ' = '
             else:
                 try:
                     result = repr(attr())
                     key += ' = '
                 except Exception:
                     result = ''
-            print(key, end='')
-            print(result, file=sys.stderr)
+            print('\n' + key, end='')
+            print(result, file=stdout, end='')
+    print()
 
 
-fps_n = -1
-fps_t1 = 0
+_fps_n = -1
+_fps_t1 = 0
 def fps():
     import time
-    global fps_n, fps_t1
-    fps_n += 1
+    global _fps_n, _fps_t1
+    _fps_n += 1
     fps_t2 = time.time()
-    if fps_t1 == 0:
-        fps_t1 = fps_t2
-    if fps_t2 - fps_t1 > 1:
-        print('fps: %.1f' % (fps_n / (fps_t2 - fps_t1)))
-        fps_t1 = fps_t2
-        fps_n = 0
+    if _fps_t1 == 0:
+        _fps_t1 = fps_t2
+    if fps_t2 - _fps_t1 > 1:
+        print('fps: %.1f' % (_fps_n / (fps_t2 - _fps_t1)))
+        _fps_t1 = fps_t2
+        _fps_n = 0
     return True
 
 
 # ---------------------------------------------------------------------------
 # File system
 # ---------------------------------------------------------------------------
 
@@ -82,19 +88,18 @@
 
 
 def path_mark(path, mark='.bak'):
     root, ext = os.path.splitext(path)
     return root + mark + ext
 
 
-def path_quote(p, repl=None):  # not include path
-    for c in '\r\n\t\\/:*?"<>|':
-        new = repl if repl is not None else urllib.parse.quote_plus(c)
-        p = p.replace(c, new)
-    return p
+def path_safe(p, repl=None):  # not include path
+    from urllib.parse import quote_plus
+    map = {ord(c): quote_plus(c) if repl is None else repl for c in '\r\n\t\\/:*?"<>|'}
+    return p.translate(map)
 
 
 def path_split(p):
     root, file = os.path.split(p)
     name, ext = os.path.splitext(file)
     return root, name, ext
 
@@ -104,14 +109,29 @@
     n = 0
     while os.path.exists(p):
         n += 1
         p = '%s%s%d%s' % (root, dash, n, ext)
     return p
 
 
+def file_mtime(path):
+    mtime = os.stat(path).st_mtime
+    return time.localtime(mtime)[:6]
+
+
+def file_ctime(path):
+    ctime = os.stat(path).st_ctime
+    return time.localtime(ctime)[:6]
+
+
+def file_utime(path, date):
+    mtime = time.mktime((tuple(date) + (0,) * 6)[:9])
+    os.utime(path, (mtime, mtime))
+
+
 # ---------------------------------------------------------------------------
 # Web
 # ---------------------------------------------------------------------------
 
 
 escape = html.escape
 unescape = html.unescape
@@ -126,14 +146,24 @@
 
 
 # ---------------------------------------------------------------------------
 # ...
 # ---------------------------------------------------------------------------
 
 
+def scan(format, string):
+    import re
+    sp = re.split('(%d|%f|%s)', format, flags=re.I)
+    patt = ''.join('(.*)' if i % 2 else re.escape(s) for i, s in enumerate(sp))
+    match = re.fullmatch(patt, string)
+    fun_map = {'%d': int, '%f': float, '%s': str}
+    formats = re.findall('%d|%f|%s', format, flags=re.I)
+    return [fun_map[fmt.lower()](s) for fmt, s in zip(formats, match.groups())]
+
+
 def findpair(s, p1='(', p2=')', st=0):
     n1 = n2 = 0
     for n, c in enumerate(s[st:]):
         n1 += c in p1
         n2 += c in p2
         if n1 and n1 == n2:
             return st + n
```

### Comparing `lishixian-0.2.2/lishixian/windll.py` & `lishixian-0.2.3/lishixian/windll.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/lishixian.egg-info/PKG-INFO` & `lishixian-0.2.3/lishixian.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: lishixian
-Version: 0.2.2
-Summary: lishixian package
+Version: 0.2.3
+Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Lishixian(znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Keywords: lishixian lsx
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Lishixian Library
-Contain 111 functions.
+# Lite Software eXtension
+
+Contain 10 modules and 115 functions.
 
 
 ## About
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
 - __Github:__ https://github.com/znsoooo/lishixian
@@ -29,14 +30,21 @@
 
 ## Install
 ```bash
 pip install lishixian --upgrade
 ```
 
 
+## Usage
+```python
+import lishixian as lsx
+lsx.help()
+```
+
+
 ## Modules
 
 ### Top module
 - all()
 - help()
 
 ### Module 'cls'
@@ -51,14 +59,15 @@
 - protect(f)
 - surround(before=(), after=())
 - hotkey(key='F12')
 - threads(cnt)
 
 ### Module 'new'
 - print(*value, file=sys.stdout)
+- time(start=0)
 - infinity = <class 'itertools.count'>
 - makedirs(name, mode=511, *, exist_ok=True)
 - breakpoint()
 - popen(cmd)
 - listdir(*paths)
 - findall(pattern, string, flags=0)
 - split(arr, cols)
@@ -68,47 +77,55 @@
 
 ### Module 'line'
 - s128 = bytes(range(128)).decode()
 - s127 = bytes(range(32, 127)).decode()
 - empty(*v, **kv)
 - freeze(fn, *v, **kv)
 - t(arr)
+- crc(b)
 - md5(b)
 - mask(p)
 - start(func, *args, **kwargs)
 - create(file)
 - pprint(*value, file=sys.stdout)
 - dumps(data)
 - sort_kv(d, reverse=False)
 - sort_key(d, reverse=False)
 - sort_num(s)
 - str2dict(s)
 - tuple2item(item)
 - unique(arr)
+- flatten(arr)
+- reshape(arr, width)
 - pc_ip()
 - pc_mac()
 - pc_user()
 - randombytes(n)
 - join(*s, sp='')
 
 ### Module 'useful'
-- tag()
-- log(*value)
-- check(obj, patt='.*')
+- log(*value, file='log.txt')
+- progress(*value, interval=1)
+- check(obj, patt='.*', stdout=True)
 - fps()
+- stem(p)
 - select(path)
 - path_mark(path, mark='.bak')
-- path_quote(p, repl=None)
+- path_safe(p, repl=None)
 - path_split(p)
 - path_unique(p, dash='-')
+- file_mtime(path)
+- file_ctime(path)
+- file_utime(path, date)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
 - urlopen(url, timeout=5)
+- scan(format, string)
 - findpair(s, p1='(', p2=')', st=0)
 - bytes_format(data, n=16)
 - bytes_print(data, n=16)
 - bytes_hex(data, offset=0, length=-1, slice=-1)
 - install(path, block=False)
 - input_wait(msg)
 - input_default(msg, default)
@@ -124,16 +141,16 @@
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
 - Monitor(func)
 - Recoder(complete=False)
 
 ### Module 'doc'
-- read(file)
-- write(file, data)
+- read(file, encoding='u8')
+- write(file, data, encoding='u8')
 - ReadIni(file, encoding='u8')
 - WriteIni(file, dic, encoding='u8')
 - WriteTxt(file, data, encoding='utf-8-sig')
 - ReadCsv(file, encoding='utf-8-sig')
 - WriteCsv(file, data, encoding='utf-8-sig', errors='ignore')
 - WriteExcel(file, data, new_sheet='sheet1')
 - OpenExcel(file)
@@ -157,15 +174,15 @@
 - EventThread(parent, id, target=<class 'bool'>, *args, **kwargs)
 
 ### Module 'np'
 - imread(file)
 - imwrite(file, im)
 - imshow(img, delay=50, title='')
 - imsave(file)
-- imiter(file_or_id, st=None, ed=None)
+- imiter(file_or_id)
 
 
 ## Comment
 1. Lib `lsx` is same as `lishixian` in `pypi.org`.
 2. If you **really** need domain `lsx` in `pypi.org`, contact me with `Email`.
```

### Comparing `lishixian-0.2.2/lishixian.egg-info/SOURCES.txt` & `lishixian-0.2.3/lishixian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lishixian-0.2.2/PKG-INFO` & `lishixian-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: lishixian
-Version: 0.2.2
-Summary: lishixian package
+Version: 0.2.3
+Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Lishixian(znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Keywords: lishixian lsx
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Lishixian Library
-Contain 111 functions.
+# Lite Software eXtension
+
+Contain 10 modules and 115 functions.
 
 
 ## About
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
 - __Github:__ https://github.com/znsoooo/lishixian
@@ -29,14 +30,21 @@
 
 ## Install
 ```bash
 pip install lishixian --upgrade
 ```
 
 
+## Usage
+```python
+import lishixian as lsx
+lsx.help()
+```
+
+
 ## Modules
 
 ### Top module
 - all()
 - help()
 
 ### Module 'cls'
@@ -51,14 +59,15 @@
 - protect(f)
 - surround(before=(), after=())
 - hotkey(key='F12')
 - threads(cnt)
 
 ### Module 'new'
 - print(*value, file=sys.stdout)
+- time(start=0)
 - infinity = <class 'itertools.count'>
 - makedirs(name, mode=511, *, exist_ok=True)
 - breakpoint()
 - popen(cmd)
 - listdir(*paths)
 - findall(pattern, string, flags=0)
 - split(arr, cols)
@@ -68,47 +77,55 @@
 
 ### Module 'line'
 - s128 = bytes(range(128)).decode()
 - s127 = bytes(range(32, 127)).decode()
 - empty(*v, **kv)
 - freeze(fn, *v, **kv)
 - t(arr)
+- crc(b)
 - md5(b)
 - mask(p)
 - start(func, *args, **kwargs)
 - create(file)
 - pprint(*value, file=sys.stdout)
 - dumps(data)
 - sort_kv(d, reverse=False)
 - sort_key(d, reverse=False)
 - sort_num(s)
 - str2dict(s)
 - tuple2item(item)
 - unique(arr)
+- flatten(arr)
+- reshape(arr, width)
 - pc_ip()
 - pc_mac()
 - pc_user()
 - randombytes(n)
 - join(*s, sp='')
 
 ### Module 'useful'
-- tag()
-- log(*value)
-- check(obj, patt='.*')
+- log(*value, file='log.txt')
+- progress(*value, interval=1)
+- check(obj, patt='.*', stdout=True)
 - fps()
+- stem(p)
 - select(path)
 - path_mark(path, mark='.bak')
-- path_quote(p, repl=None)
+- path_safe(p, repl=None)
 - path_split(p)
 - path_unique(p, dash='-')
+- file_mtime(path)
+- file_ctime(path)
+- file_utime(path, date)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
 - urlopen(url, timeout=5)
+- scan(format, string)
 - findpair(s, p1='(', p2=')', st=0)
 - bytes_format(data, n=16)
 - bytes_print(data, n=16)
 - bytes_hex(data, offset=0, length=-1, slice=-1)
 - install(path, block=False)
 - input_wait(msg)
 - input_default(msg, default)
@@ -124,16 +141,16 @@
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
 - Monitor(func)
 - Recoder(complete=False)
 
 ### Module 'doc'
-- read(file)
-- write(file, data)
+- read(file, encoding='u8')
+- write(file, data, encoding='u8')
 - ReadIni(file, encoding='u8')
 - WriteIni(file, dic, encoding='u8')
 - WriteTxt(file, data, encoding='utf-8-sig')
 - ReadCsv(file, encoding='utf-8-sig')
 - WriteCsv(file, data, encoding='utf-8-sig', errors='ignore')
 - WriteExcel(file, data, new_sheet='sheet1')
 - OpenExcel(file)
@@ -157,15 +174,15 @@
 - EventThread(parent, id, target=<class 'bool'>, *args, **kwargs)
 
 ### Module 'np'
 - imread(file)
 - imwrite(file, im)
 - imshow(img, delay=50, title='')
 - imsave(file)
-- imiter(file_or_id, st=None, ed=None)
+- imiter(file_or_id)
 
 
 ## Comment
 1. Lib `lsx` is same as `lishixian` in `pypi.org`.
 2. If you **really** need domain `lsx` in `pypi.org`, contact me with `Email`.
```

### Comparing `lishixian-0.2.2/README.md` & `lishixian-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Lishixian Library
-Contain 111 functions.
+# Lite Software eXtension
+
+Contain 10 modules and 115 functions.
 
 
 ## About
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
 - __Github:__ https://github.com/znsoooo/lishixian
@@ -12,14 +13,21 @@
 
 ## Install
 ```bash
 pip install lishixian --upgrade
 ```
 
 
+## Usage
+```python
+import lishixian as lsx
+lsx.help()
+```
+
+
 ## Modules
 
 ### Top module
 - all()
 - help()
 
 ### Module 'cls'
@@ -34,14 +42,15 @@
 - protect(f)
 - surround(before=(), after=())
 - hotkey(key='F12')
 - threads(cnt)
 
 ### Module 'new'
 - print(*value, file=sys.stdout)
+- time(start=0)
 - infinity = <class 'itertools.count'>
 - makedirs(name, mode=511, *, exist_ok=True)
 - breakpoint()
 - popen(cmd)
 - listdir(*paths)
 - findall(pattern, string, flags=0)
 - split(arr, cols)
@@ -51,47 +60,55 @@
 
 ### Module 'line'
 - s128 = bytes(range(128)).decode()
 - s127 = bytes(range(32, 127)).decode()
 - empty(*v, **kv)
 - freeze(fn, *v, **kv)
 - t(arr)
+- crc(b)
 - md5(b)
 - mask(p)
 - start(func, *args, **kwargs)
 - create(file)
 - pprint(*value, file=sys.stdout)
 - dumps(data)
 - sort_kv(d, reverse=False)
 - sort_key(d, reverse=False)
 - sort_num(s)
 - str2dict(s)
 - tuple2item(item)
 - unique(arr)
+- flatten(arr)
+- reshape(arr, width)
 - pc_ip()
 - pc_mac()
 - pc_user()
 - randombytes(n)
 - join(*s, sp='')
 
 ### Module 'useful'
-- tag()
-- log(*value)
-- check(obj, patt='.*')
+- log(*value, file='log.txt')
+- progress(*value, interval=1)
+- check(obj, patt='.*', stdout=True)
 - fps()
+- stem(p)
 - select(path)
 - path_mark(path, mark='.bak')
-- path_quote(p, repl=None)
+- path_safe(p, repl=None)
 - path_split(p)
 - path_unique(p, dash='-')
+- file_mtime(path)
+- file_ctime(path)
+- file_utime(path, date)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
 - urlopen(url, timeout=5)
+- scan(format, string)
 - findpair(s, p1='(', p2=')', st=0)
 - bytes_format(data, n=16)
 - bytes_print(data, n=16)
 - bytes_hex(data, offset=0, length=-1, slice=-1)
 - install(path, block=False)
 - input_wait(msg)
 - input_default(msg, default)
@@ -107,16 +124,16 @@
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
 - Monitor(func)
 - Recoder(complete=False)
 
 ### Module 'doc'
-- read(file)
-- write(file, data)
+- read(file, encoding='u8')
+- write(file, data, encoding='u8')
 - ReadIni(file, encoding='u8')
 - WriteIni(file, dic, encoding='u8')
 - WriteTxt(file, data, encoding='utf-8-sig')
 - ReadCsv(file, encoding='utf-8-sig')
 - WriteCsv(file, data, encoding='utf-8-sig', errors='ignore')
 - WriteExcel(file, data, new_sheet='sheet1')
 - OpenExcel(file)
@@ -140,13 +157,13 @@
 - EventThread(parent, id, target=<class 'bool'>, *args, **kwargs)
 
 ### Module 'np'
 - imread(file)
 - imwrite(file, im)
 - imshow(img, delay=50, title='')
 - imsave(file)
-- imiter(file_or_id, st=None, ed=None)
+- imiter(file_or_id)
 
 
 ## Comment
 1. Lib `lsx` is same as `lishixian` in `pypi.org`.
 2. If you **really** need domain `lsx` in `pypi.org`, contact me with `Email`.
```

### Comparing `lishixian-0.2.2/setup.py` & `lishixian-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_description = f.read()
 
 setuptools.setup(
     name=pkg[0],
     version=version,
     author='Lishixian(znsoooo)',
     author_email='lsx7@sina.com',
-    description='lishixian package',
+    description='Lite Software eXtension',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/znsoooo/lishixian',
     project_urls={
         'Bug Tracker': 'https://github.com/znsoooo/lishixian/issues',
     },
     classifiers=[
```

