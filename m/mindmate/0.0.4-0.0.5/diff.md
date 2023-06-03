# Comparing `tmp/mindmate-0.0.4.tar.gz` & `tmp/mindmate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.0.4.tar", last modified: Sat Jun  3 16:23:23 2023, max compression
+gzip compressed data, was "mindmate-0.0.5.tar", last modified: Sat Jun  3 16:36:08 2023, max compression
```

## Comparing `mindmate-0.0.4.tar` & `mindmate-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.250839 mindmate-0.0.4/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:23:23.247839 mindmate-0.0.4/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      701 2023-06-03 15:12:40.000000 mindmate-0.0.4/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.631647 mindmate-0.0.4/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:21:53.000000 mindmate-0.0.4/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.968992 mindmate-0.0.4/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 15:08:35.000000 mindmate-0.0.4/mindmate/commands/ai.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-05-15 20:38:34.000000 mindmate-0.0.4/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.4/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:17:26.000000 mindmate-0.0.4/mindmate/commands/version.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-03 16:13:11.000000 mindmate-0.0.4/mindmate/meta.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.062337 mindmate-0.0.4/mindmate/services/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:05:22.000000 mindmate-0.0.4/mindmate/services/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 15:10:29.000000 mindmate-0.0.4/mindmate/services/directory.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 15:09:47.000000 mindmate-0.0.4/mindmate/services/models.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.225838 mindmate-0.0.4/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      730 2023-06-03 15:21:23.000000 mindmate-0.0.4/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.4/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.4/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 14:53:12.000000 mindmate-0.0.4/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.813302 mindmate-0.0.4/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-03 16:23:23.251843 mindmate-0.0.4/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:13:54.000000 mindmate-0.0.4/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.626398 mindmate-0.0.5/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:36:08.607854 mindmate-0.0.5/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      701 2023-06-03 16:28:25.000000 mindmate-0.0.5/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:07.990010 mindmate-0.0.5/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.340877 mindmate-0.0.5/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/commands/ai.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-05-15 20:38:34.000000 mindmate-0.0.5/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.5/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/commands/version.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-03 16:34:02.000000 mindmate-0.0.5/mindmate/meta.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.420240 mindmate-0.0.5/mindmate/services/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/services/models.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.582833 mindmate-0.0.5/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.5/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      730 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.5/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.5/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 16:28:25.000000 mindmate-0.0.5/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:36:08.186718 mindmate-0.0.5/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-03 16:36:06.000000 mindmate-0.0.5/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-03 16:36:08.638399 mindmate-0.0.5/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:28:25.000000 mindmate-0.0.5/setup.py
```

### Comparing `mindmate-0.0.4/PKG-INFO` & `mindmate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.0.4
+Version: 0.0.5
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
```

### Comparing `mindmate-0.0.4/README.md` & `mindmate-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/cli.py` & `mindmate-0.0.5/mindmate/cli.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/commands/ai.py` & `mindmate-0.0.5/mindmate/commands/ai.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/commands/chat.py` & `mindmate-0.0.5/mindmate/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/commands/configure.py` & `mindmate-0.0.5/mindmate/commands/configure.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/services/directory.py` & `mindmate-0.0.5/mindmate/services/directory.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/services/models.py` & `mindmate-0.0.5/mindmate/services/models.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/utils/conf.py` & `mindmate-0.0.5/mindmate/utils/conf.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/utils/env.py` & `mindmate-0.0.5/mindmate/utils/env.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate/utils/utils.py` & `mindmate-0.0.5/mindmate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/mindmate.egg-info/PKG-INFO` & `mindmate-0.0.5/mindmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindmate
-Version: 0.0.4
+Version: 0.0.5
 Summary: MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers
 Home-page: https://github.com/yalattas/mindmate
 Author: Yasser Alattas
 Author-email: y.alattas@gmail.com
 License: LGPL-2.1 license
 Download-URL: https://github.com/yalattas/mindmate
 Description: # install package
```

### Comparing `mindmate-0.0.4/mindmate.egg-info/SOURCES.txt` & `mindmate-0.0.5/mindmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.4/setup.py` & `mindmate-0.0.5/setup.py`

 * *Files identical despite different names*

