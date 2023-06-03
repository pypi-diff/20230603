# Comparing `tmp/pinit-0.0.3.tar.gz` & `tmp/pinit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinit-0.0.3.tar", max compression
+gzip compressed data, was "pinit-0.0.4.tar", max compression
```

## Comparing `pinit-0.0.3.tar` & `pinit-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      334 2023-01-23 13:45:53.635214 pinit-0.0.3/README.md
--rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.3/pinit/.pinit/install.py
--rw-r--r--   0        0        0     2445 2023-03-27 12:20:43.105475 pinit-0.0.3/pinit/.pinit/main.py
--rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.3/pinit/.pinit/pinit.svg
--rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.3/pinit/.pinit/requirements.txt
--rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.3/pinit/.pinit/shortcut.py
--rw-r--r--   0        0        0   378236 2023-03-27 12:12:41.420434 pinit-0.0.3/pinit/.pinit/ui/assets/index-4bfb2d27.css
--rw-r--r--   0        0        0  1118350 2023-03-27 12:12:41.422433 pinit-0.0.3/pinit/.pinit/ui/assets/index-c123fd1d.js
--rw-r--r--   0        0        0   128352 2023-03-27 12:12:41.413433 pinit-0.0.3/pinit/.pinit/ui/assets/w1-8265f647.woff2
--rw-r--r--   0        0        0   155276 2023-03-27 12:12:41.409433 pinit-0.0.3/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
--rwxr-xr-x   0        0        0     2210 2023-03-27 12:12:40.759433 pinit-0.0.3/pinit/.pinit/ui/icon.svg
--rw-r--r--   0        0        0      614 2023-03-27 12:12:41.420434 pinit-0.0.3/pinit/.pinit/ui/index.html
--rw-r--r--   0        0        0      115 2023-01-06 18:08:51.599138 pinit-0.0.3/pinit/.pinit/uninstall.py
--rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.3/pinit/.pinit/upgrade.py
--rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.3/pinit/__init__.py
--rw-r--r--   0        0        0     2203 2023-01-20 07:49:54.642473 pinit-0.0.3/pinit/main.py
--rw-r--r--   0        0        0      457 2023-03-27 12:25:24.103499 pinit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 pinit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.4/README.md
+-rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.4/pinit/.pinit/install.py
+-rw-r--r--   0        0        0     6929 2023-06-03 08:04:59.494226 pinit-0.0.4/pinit/.pinit/main.py
+-rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.4/pinit/.pinit/pinit.svg
+-rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.4/pinit/.pinit/requirements.txt
+-rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.4/pinit/.pinit/shortcut.py
+-rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.4/pinit/.pinit/ui/assets/index-88a0609b.css
+-rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.4/pinit/.pinit/ui/assets/index-a407b3b0.js
+-rw-r--r--   0        0        0   128352 2023-06-03 10:08:22.907252 pinit-0.0.4/pinit/.pinit/ui/assets/w1-8265f647.woff2
+-rw-r--r--   0        0        0   155276 2023-06-03 10:08:22.909252 pinit-0.0.4/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
+-rwxr-xr-x   0        0        0     2210 2023-06-03 10:08:22.437250 pinit-0.0.4/pinit/.pinit/ui/icon.svg
+-rw-r--r--   0        0        0      899 2023-06-03 10:08:22.909252 pinit-0.0.4/pinit/.pinit/ui/index.html
+-rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.4/pinit/.pinit/uninstall.py
+-rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.4/pinit/.pinit/upgrade.py
+-rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.4/pinit/__init__.py
+-rw-r--r--   0        0        0     2203 2023-01-20 07:49:54.642473 pinit-0.0.4/pinit/main.py
+-rw-r--r--   0        0        0      457 2023-06-03 10:26:35.399003 pinit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.4/PKG-INFO
```

### Comparing `pinit-0.0.3/pinit/.pinit/pinit.svg` & `pinit-0.0.4/pinit/.pinit/pinit.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/pinit/.pinit/shortcut.py` & `pinit-0.0.4/pinit/.pinit/shortcut.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/pinit/.pinit/ui/assets/w1-8265f647.woff2` & `pinit-0.0.4/pinit/.pinit/ui/assets/w1-8265f647.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/pinit/.pinit/ui/assets/w2-35dca8a7.woff2` & `pinit-0.0.4/pinit/.pinit/ui/assets/w2-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/pinit/.pinit/ui/icon.svg` & `pinit-0.0.4/pinit/.pinit/ui/icon.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/pinit/.pinit/ui/index.html` & `pinit-0.0.4/pinit/.pinit/ui/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <link rel="icon" href="/icon.svg">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>pinit</title>
     
+    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;900&display=swap" rel="stylesheet">
+	
     <!-- <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;900&display=swap" rel="stylesheet"> -->
+    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
     <script type="text/javascript" src="/eel.js"></script>
-    <script type="module" crossorigin src="/assets/index-c123fd1d.js"></script>
-    <link rel="stylesheet" href="/assets/index-4bfb2d27.css">
+
+
+
+
+
+    <script type="module" crossorigin src="/assets/index-a407b3b0.js"></script>
+    <link rel="stylesheet" href="/assets/index-88a0609b.css">
   </head>
   <body>
     <div id="app"></div>
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
 
 
 
+
```

### Comparing `pinit-0.0.3/pinit/main.py` & `pinit-0.0.4/pinit/main.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.3/PKG-INFO` & `pinit-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinit
-Version: 0.0.3
+Version: 0.0.4
 Summary: an application for creating shortcut for apps and scripts in linux
 Home-page: https://github.com/rraammiinn/pinit.git
 License: MIT
 Author: ramin
 Author-email: ramin.kishani.farahani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,19 +14,26 @@
 Project-URL: Repository, https://github.com/rraammiinn/pinit.git
 Description-Content-Type: text/markdown
 
 # pinit
 ## an application for creating shortcut for apps and scripts ( only for linux )
 ## installation
 - using pip :
-run this two commands in terminal
-1. pip install pinit
-2. pinit
-- appimage :
-just download pinit.AppImage file and run it
+run this two commands in terminal :
+```bash
+pip install pinit
+pinit install
+```
+
+or run :
+```bash
+pip install pinit && pinit install
+```
+<!-- - appimage : -->
+<!-- just download pinit.AppImage file and run it -->
 ## commands
 - pinit
 - pinit install
 - pinit uninstall
 - pinit upgrade
 - pinit upgrade --force
```

