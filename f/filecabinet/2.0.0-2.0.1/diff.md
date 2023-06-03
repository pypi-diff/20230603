# Comparing `tmp/filecabinet-2.0.0.tar.gz` & `tmp/filecabinet-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filecabinet-2.0.0.tar", last modified: Fri May 19 11:51:20 2023, max compression
+gzip compressed data, was "filecabinet-2.0.1.tar", last modified: Sat Jun  3 09:11:58 2023, max compression
```

## Comparing `filecabinet-2.0.0.tar` & `filecabinet-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 11:51:20.500508 filecabinet-2.0.0/
--rw-r--r--   0 robert    (1000) robert    (1000)     1500 2022-02-26 07:52:08.000000 filecabinet-2.0.0/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)       92 2023-05-19 11:48:32.000000 filecabinet-2.0.0/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-05-19 11:51:20.500508 filecabinet-2.0.0/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     6252 2023-05-19 11:42:35.000000 filecabinet-2.0.0/README.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1334 2023-05-19 11:48:39.000000 filecabinet-2.0.0/example.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 11:51:20.500508 filecabinet-2.0.0/filecabinet/
--rw-r--r--   0 robert    (1000) robert    (1000)       62 2022-02-26 07:52:09.000000 filecabinet-2.0.0/filecabinet/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10047 2023-05-19 11:33:18.000000 filecabinet-2.0.0/filecabinet/cabinet.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3247 2023-05-19 11:33:18.000000 filecabinet-2.0.0/filecabinet/configuration.py
--rw-r--r--   0 robert    (1000) robert    (1000)     9911 2023-05-19 11:33:18.000000 filecabinet-2.0.0/filecabinet/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7889 2023-05-19 11:33:18.000000 filecabinet-2.0.0/filecabinet/manager.py
--rw-r--r--   0 robert    (1000) robert    (1000)      313 2022-02-26 07:52:09.000000 filecabinet-2.0.0/filecabinet/meta.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8605 2023-05-19 11:38:06.000000 filecabinet-2.0.0/filecabinet/shell.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6415 2023-05-19 11:33:18.000000 filecabinet-2.0.0/filecabinet/utils.py
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2023-05-19 11:33:30.000000 filecabinet-2.0.0/filecabinet/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 11:51:20.500508 filecabinet-2.0.0/filecabinet.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)      509 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       53 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       37 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       12 2023-05-19 11:51:20.000000 filecabinet-2.0.0/filecabinet.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       22 2022-02-26 07:52:09.000000 filecabinet-2.0.0/requirements.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-19 11:51:20.500508 filecabinet-2.0.0/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     1059 2023-05-19 11:51:11.000000 filecabinet-2.0.0/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-19 11:51:20.500508 filecabinet-2.0.0/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     5290 2022-02-26 07:52:09.000000 filecabinet-2.0.0/tests/test_processing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/
+-rw-r--r--   0 robert    (1000) robert    (1000)      461 2023-06-03 09:07:55.000000 filecabinet-2.0.1/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1500 2022-02-26 07:52:08.000000 filecabinet-2.0.1/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      113 2023-06-03 09:08:18.000000 filecabinet-2.0.1/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-06-03 09:11:58.613384 filecabinet-2.0.1/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     6252 2023-05-19 11:42:35.000000 filecabinet-2.0.1/README.md
+-rw-r--r--   0 robert    (1000) robert    (1000)      754 2023-06-03 09:11:05.000000 filecabinet-2.0.1/example.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/filecabinet/
+-rw-r--r--   0 robert    (1000) robert    (1000)       62 2022-02-26 07:52:09.000000 filecabinet-2.0.1/filecabinet/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10047 2023-06-03 08:59:25.000000 filecabinet-2.0.1/filecabinet/cabinet.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3247 2023-05-19 11:33:18.000000 filecabinet-2.0.1/filecabinet/configuration.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9911 2023-05-27 07:35:00.000000 filecabinet-2.0.1/filecabinet/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7892 2023-06-03 08:49:18.000000 filecabinet-2.0.1/filecabinet/manager.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      313 2022-02-26 07:52:09.000000 filecabinet-2.0.1/filecabinet/meta.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8605 2023-05-19 11:38:06.000000 filecabinet-2.0.1/filecabinet/shell.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4058 2023-05-28 07:40:25.000000 filecabinet-2.0.1/filecabinet/utils.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2023-06-03 09:06:34.000000 filecabinet-2.0.1/filecabinet/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/filecabinet.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      522 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       53 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       37 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       12 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       22 2022-02-26 07:52:09.000000 filecabinet-2.0.1/requirements.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-03 09:11:58.613384 filecabinet-2.0.1/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     1059 2023-06-03 09:05:46.000000 filecabinet-2.0.1/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     5290 2022-02-26 07:52:09.000000 filecabinet-2.0.1/tests/test_processing.py
```

### Comparing `filecabinet-2.0.0/LICENSE` & `filecabinet-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/PKG-INFO` & `filecabinet-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filecabinet
-Version: 2.0.0
+Version: 2.0.1
 Summary: A local, offline document archive
 Home-page: https://vonshednob.cc/filecabinet
 Author: R
 Author-email: dev+filecabinet-this-is-spam@vonshednob.cc
 License: Copyright 2019 Robert Labudda All Rights Reserved.
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
            * Redistribution of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `filecabinet-2.0.0/README.md` & `filecabinet-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/filecabinet/cabinet.py` & `filecabinet-2.0.1/filecabinet/cabinet.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/filecabinet/configuration.py` & `filecabinet-2.0.1/filecabinet/configuration.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/filecabinet/main.py` & `filecabinet-2.0.1/filecabinet/main.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/filecabinet/manager.py` & `filecabinet-2.0.1/filecabinet/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,25 +52,25 @@
         self.manager = manager
 
     def reduce(self, entry):
         for key in set(entry.metadata.keys()):
             values = entry.metadata[key]
             skey = None
 
-            if key in self.config.synonymized and any(len(v.raw_value) > 0 for v in values):
+            if key in self.config.synonymized and any(len(str(v.raw_value)) > 0 for v in values):
                 skey = 'extra.' + self.config.synonymized[key]
             elif key.startswith('extra.'):
                 skey = key.lower()
             elif key.startswith('rules.') and len(key.strip()) > 6:
                 skey = 'extra.' + key.strip()[6:]
 
             if skey is not None:
                 if skey not in entry.metadata:
                     entry.metadata[skey] = []
-                entry.metadata[skey] = list(set(entry.metadata[skey] + [v for v in values if len(v.raw_value) > 0]))
+                entry.metadata[skey] = list(set(entry.metadata[skey] + [v for v in values if len(str(v.raw_value)) > 0]))
 
             if key != skey:
                 del entry.metadata[key]
 
         return entry
 
     def find(self, *args, **kwargs):
@@ -98,15 +98,15 @@
             self.ocr = shutil.which('tesseract')
 
         # create the metaindex configuration, overwrite existing ones
         cachepath = self.config.path('General', 'database')
         rules = []
         if 'Rules' in self.config:
             rules = [f"{k} = {self.config.get('Rules', k)}" for k in self.config['Rules']]
-        self.miconfig = cachepath.parent / 'metaindex.conf'
+        self.miconfig = cachepath / 'metaindex.conf'
         if not self.miconfig.is_file() or (self.config.filepath is not None
            and self.config.filepath.is_file() and
            metaindex.shared.get_last_modified(self.config.filepath) > metaindex.shared.get_last_modified(self.miconfig)):
             cachepath.mkdir(parents=True, exist_ok=True)
             self.miconfig.parent.mkdir(parents=True, exist_ok=True)
             socketpath = self.miconfig.parent / 'metaindex.sock'
             logfile = self.miconfig.parent / 'metaindex.log'
```

### Comparing `filecabinet-2.0.0/filecabinet/shell.py` & `filecabinet-2.0.1/filecabinet/shell.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.0/filecabinet.egg-info/PKG-INFO` & `filecabinet-2.0.1/filecabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filecabinet
-Version: 2.0.0
+Version: 2.0.1
 Summary: A local, offline document archive
 Home-page: https://vonshednob.cc/filecabinet
 Author: R
 Author-email: dev+filecabinet-this-is-spam@vonshednob.cc
 License: Copyright 2019 Robert Labudda All Rights Reserved.
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
            * Redistribution of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `filecabinet-2.0.0/setup.py` & `filecabinet-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,13 +20,13 @@
       author_email="dev+filecabinet-this-is-spam@vonshednob.cc",
       license=licensetext,
       entry_points={'console_scripts': ['filecabinet=filecabinet.main:run']},
       packages=['filecabinet',
                 ],
       package_data={},
       data_files=[],
-      install_requires=['pyyaml', 'pypdf', 'Pillow', 'metaindex >= 2.1.1'],
+      install_requires=['pyyaml', 'pypdf', 'Pillow', 'metaindex >= 2.2.2'],
       python_requires='>=3.7',
       classifiers=['Development Status :: 3 - Alpha',
                    'License :: OSI Approved :: BSD License',
                    'Programming Language :: Python :: 3',
                    ])
```

### Comparing `filecabinet-2.0.0/tests/test_processing.py` & `filecabinet-2.0.1/tests/test_processing.py`

 * *Files identical despite different names*

