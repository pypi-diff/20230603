# Comparing `tmp/telegramweb-4.4.tar.gz` & `tmp/telegramweb-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-4.4.tar", last modified: Sat Jun  3 13:01:01 2023, max compression
+gzip compressed data, was "dist/telegramweb-4.5.tar", last modified: Sat Jun  3 14:07:21 2023, max compression
```

## Comparing `telegramweb-4.4.tar` & `telegramweb-4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:01.240838 telegramweb-4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 13:00:45.000000 telegramweb-4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 13:00:45.000000 telegramweb-4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-03 13:01:01.240838 telegramweb-4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-03 13:00:45.000000 telegramweb-4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:01:01.240838 telegramweb-4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-03 13:00:45.000000 telegramweb-4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:01.240838 telegramweb-4.4/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:01.240838 telegramweb-4.4/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-03 13:00:45.000000 telegramweb-4.4/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:01.240838 telegramweb-4.4/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-03 13:01:01.000000 telegramweb-4.4/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-03 13:01:01.000000 telegramweb-4.4/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:01:01.000000 telegramweb-4.4/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-03 13:01:01.000000 telegramweb-4.4/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-03 13:01:01.000000 telegramweb-4.4/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:07:21.000000 telegramweb-4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 14:07:04.000000 telegramweb-4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 14:07:04.000000 telegramweb-4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-03 14:07:21.000000 telegramweb-4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-03 14:07:04.000000 telegramweb-4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:07:21.000000 telegramweb-4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-03 14:07:04.000000 telegramweb-4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:07:21.000000 telegramweb-4.5/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:07:21.000000 telegramweb-4.5/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-03 14:07:04.000000 telegramweb-4.5/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-03 14:07:21.000000 telegramweb-4.5/telegramweb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `telegramweb-4.4/LICENSE` & `telegramweb-4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/PKG-INFO` & `telegramweb-4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.4
+Version: 4.5
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 4.4 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 4.5 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

### Comparing `telegramweb-4.4/README.md` & `telegramweb-4.5/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/setup.py` & `telegramweb-4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='4.4',
+    version='4.5',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-4.4/telegram_news/__init__.py` & `telegramweb-4.5/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/telegram_news/constant.py` & `telegramweb-4.5/telegram_news/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 MAX_URL_IMAGE_SIZE = int(5E6)   # (5MB)
 MAX_URL_VIDEO_SIZE = int(20E6)  # (20MB)
 MAX_IMAGE_SIZE = int(10E6)      # (10MB) May be changed in the future.
 MAX_VIDEO_SIZE = int(50E6)      # (50MB) May be changed in the future.
 MAX_PHOTOSIZE_UPLOAD = int(10E6)  # (10MB)
 MAX_VIDEOSIZE_UPLOAD = int(20E6)  # (20MB)
 
-MAX_MESSAGES_PER_SECOND_PER_CHAT = 1
+MAX_MESSAGES_PER_SECOND_PER_CHAT = 5
 MAX_MESSAGES_PER_SECOND = 50
 MAX_MESSAGES_PER_MINUTE_PER_GROUP = 50
 
 MAX_MEDIA_PER_MEDIAGROUP = 10
 
 ALL_METHOD = [
     'getMe',
```

### Comparing `telegramweb-4.4/telegram_news/displaypolicy.py` & `telegramweb-4.5/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/telegram_news/ratelimit.py` & `telegramweb-4.5/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/telegram_news/template/common.py` & `telegramweb-4.5/telegram_news/template/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1125,15 +1125,15 @@
                     print('Get ' + item['id'] + ', but no action!')
                 total += 1
             else:
                 posted += 1
                 # print(item['id'] + 'Posted!')
         return total, posted
 
-    def poll(self, sleep_time=60):
+    def poll(self, sleep_time=10):
         # Thread work function
         def work():
             while True:
                 try:
                     total, posted = self._action()
                     if total is None:
                         print(self._tag + ':' + ' ' * (6 - len(self._tag)) + '\tList not modified! ' +
```

### Comparing `telegramweb-4.4/telegram_news/utils.py` & `telegramweb-4.5/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.4/telegramweb.egg-info/PKG-INFO` & `telegramweb-4.5/telegramweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.4
+Version: 4.5
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Description: <h1 align="center">
           <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: telegramweb Version: 4.4 Summary: Python package
+Metadata-Version: 2.1 Name: telegramweb Version: 4.5 Summary: Python package
 for automatically fetching and pushing news by Telegram. Home-page: https://
 github.com/craziks-creator/telegram-web Author: craziks Author-email:
 chandrashekharpanday07@gmail.com License: MIT Description:
                             ****** [Telegram-news]
                                  Telegram-news
                                      ******
   Python package for automatically fetching and pushing news by Telegram. [!
```

