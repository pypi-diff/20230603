# Comparing `tmp/pinit-0.0.5.tar.gz` & `tmp/pinit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinit-0.0.5.tar", max compression
+gzip compressed data, was "pinit-0.0.6.tar", max compression
```

## Comparing `pinit-0.0.5.tar` & `pinit-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.5/README.md
--rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.5/pinit/.pinit/install.py
--rw-r--r--   0        0        0     6929 2023-06-03 08:04:59.494226 pinit-0.0.5/pinit/.pinit/main.py
--rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.5/pinit/.pinit/pinit.svg
--rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.5/pinit/.pinit/requirements.txt
--rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.5/pinit/.pinit/shortcut.py
--rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.5/pinit/.pinit/ui/assets/index-88a0609b.css
--rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.5/pinit/.pinit/ui/assets/index-a407b3b0.js
--rw-r--r--   0        0        0   128352 2023-06-03 10:08:22.907252 pinit-0.0.5/pinit/.pinit/ui/assets/w1-8265f647.woff2
--rw-r--r--   0        0        0   155276 2023-06-03 10:08:22.909252 pinit-0.0.5/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
--rwxr-xr-x   0        0        0     2210 2023-06-03 10:08:22.437250 pinit-0.0.5/pinit/.pinit/ui/icon.svg
--rw-r--r--   0        0        0      899 2023-06-03 10:08:22.909252 pinit-0.0.5/pinit/.pinit/ui/index.html
--rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.5/pinit/.pinit/uninstall.py
--rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.5/pinit/.pinit/upgrade.py
--rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.5/pinit/__init__.py
--rw-r--r--   0        0        0     2203 2023-01-20 07:49:54.642473 pinit-0.0.5/pinit/main.py
--rw-r--r--   0        0        0      457 2023-06-03 13:02:58.666852 pinit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.6/README.md
+-rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.6/pinit/.pinit/install.py
+-rw-r--r--   0        0        0     6929 2023-06-03 08:04:59.494226 pinit-0.0.6/pinit/.pinit/main.py
+-rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.6/pinit/.pinit/pinit.svg
+-rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.6/pinit/.pinit/requirements.txt
+-rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.6/pinit/.pinit/shortcut.py
+-rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.6/pinit/.pinit/ui/assets/index-88a0609b.css
+-rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.6/pinit/.pinit/ui/assets/index-a407b3b0.js
+-rw-r--r--   0        0        0   128352 2023-06-03 10:08:22.907252 pinit-0.0.6/pinit/.pinit/ui/assets/w1-8265f647.woff2
+-rw-r--r--   0        0        0   155276 2023-06-03 10:08:22.909252 pinit-0.0.6/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
+-rwxr-xr-x   0        0        0     2210 2023-06-03 10:08:22.437250 pinit-0.0.6/pinit/.pinit/ui/icon.svg
+-rw-r--r--   0        0        0      899 2023-06-03 10:08:22.909252 pinit-0.0.6/pinit/.pinit/ui/index.html
+-rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.6/pinit/.pinit/uninstall.py
+-rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.6/pinit/.pinit/upgrade.py
+-rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.6/pinit/__init__.py
+-rw-r--r--   0        0        0     2338 2023-06-03 13:16:45.028043 pinit-0.0.6/pinit/main.py
+-rw-r--r--   0        0        0      457 2023-06-03 13:17:21.306187 pinit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.6/PKG-INFO
```

### Comparing `pinit-0.0.5/pinit/.pinit/main.py` & `pinit-0.0.6/pinit/.pinit/main.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/pinit.svg` & `pinit-0.0.6/pinit/.pinit/pinit.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/shortcut.py` & `pinit-0.0.6/pinit/.pinit/shortcut.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/assets/index-88a0609b.css` & `pinit-0.0.6/pinit/.pinit/ui/assets/index-88a0609b.css`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/assets/index-a407b3b0.js` & `pinit-0.0.6/pinit/.pinit/ui/assets/index-a407b3b0.js`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/assets/w1-8265f647.woff2` & `pinit-0.0.6/pinit/.pinit/ui/assets/w1-8265f647.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/assets/w2-35dca8a7.woff2` & `pinit-0.0.6/pinit/.pinit/ui/assets/w2-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/icon.svg` & `pinit-0.0.6/pinit/.pinit/ui/icon.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/.pinit/ui/index.html` & `pinit-0.0.6/pinit/.pinit/ui/index.html`

 * *Files identical despite different names*

### Comparing `pinit-0.0.5/pinit/main.py` & `pinit-0.0.6/pinit/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,19 @@
             shutil.rmtree(dist)
         finally:
             shutil.copytree(src, dist)
             os.chdir(dist)
             subprocess.run(['python','-m','venv','venv'])
             subprocess.run(['venv/bin/python','-m','pip','install','-r','requirements.txt'])
             subprocess.run(['venv/bin/python', 'install.py'])
+        try:
+            os.makedirs(f'{dist}'/ui/desktop)
+            os.makedirs(f'{dist}'/ui/menu)
+        except:
+            pass
 
 
 
 def upgrade():
     if '--force' in sys.argv or '-f' in sys.argv:
         subprocess.run(['pip', 'install', '--upgrade', 'pinit'])
         install()
```

### Comparing `pinit-0.0.5/PKG-INFO` & `pinit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinit
-Version: 0.0.5
+Version: 0.0.6
 Summary: an application for creating shortcut for apps and scripts in linux
 Home-page: https://github.com/rraammiinn/pinit.git
 License: MIT
 Author: ramin
 Author-email: ramin.kishani.farahani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

