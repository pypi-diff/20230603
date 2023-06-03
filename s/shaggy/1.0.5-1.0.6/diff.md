# Comparing `tmp/shaggy-1.0.5.tar.gz` & `tmp/shaggy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaggy-1.0.5.tar", last modified: Sat Jun  3 06:34:40 2023, max compression
+gzip compressed data, was "shaggy-1.0.6.tar", last modified: Sat Jun  3 06:54:27 2023, max compression
```

## Comparing `shaggy-1.0.5.tar` & `shaggy-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.548852 shaggy-1.0.5/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-01 10:20:38.000000 shaggy-1.0.5/.gitignore
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1071 2023-05-31 17:40:10.000000 shaggy-1.0.5/LICENSE
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:34:40.548852 shaggy-1.0.5/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.5/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       54 2023-06-03 06:31:03.000000 shaggy-1.0.5/publish.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-05-31 18:26:53.000000 shaggy-1.0.5/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:34:40.548852 shaggy-1.0.5/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2023-06-03 06:34:05.000000 shaggy-1.0.5/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.544852 shaggy-1.0.5/shaggy/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4185 2023-06-03 06:34:14.000000 shaggy-1.0.5/shaggy/hunt.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/output.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4088 2023-06-03 06:14:32.000000 shaggy-1.0.5/shaggy/sources.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:34:40.544852 shaggy-1.0.5/shaggy.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      316 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:34:40.000000 shaggy-1.0.5/shaggy.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:54:27.792991 shaggy-1.0.6/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:54:27.792991 shaggy-1.0.6/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.6/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:54:27.792991 shaggy-1.0.6/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1203 2023-06-03 06:53:47.000000 shaggy-1.0.6/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:54:27.792991 shaggy-1.0.6/shaggy/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.6/shaggy/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4228 2023-06-03 06:48:55.000000 shaggy-1.0.6/shaggy/hunt.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.6/shaggy/output.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4110 2023-06-03 06:53:34.000000 shaggy-1.0.6/shaggy/sources.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:54:27.792991 shaggy-1.0.6/shaggy.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3324 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      269 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:54:27.000000 shaggy-1.0.6/shaggy.egg-info/top_level.txt
```

### Comparing `shaggy-1.0.5/PKG-INFO` & `shaggy-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
 Description: # Shaggy
```

### Comparing `shaggy-1.0.5/README.md` & `shaggy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.5/setup.py` & `shaggy-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='shaggy',
-    version='1.0.5',
+    version='1.0.6',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mauro Baladés',
     author_email='mauro.balades@tutanota.com',
     description='Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.',
     url='https://github.com/mauro-balades/shaggy',
     packages=["shaggy"],
```

### Comparing `shaggy-1.0.5/shaggy/__init__.py` & `shaggy-1.0.6/shaggy/__init__.py`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.5/shaggy/hunt.py` & `shaggy-1.0.6/shaggy/hunt.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 
             try:
                 # Send a GET request to the URL, if there's an exception,
                 # we just go to the next source
                 response = requests.get(
                     url, headers={**headers, **source.get("headers", {})}
                 )
+
+                print(response.content)
             except requests.exceptions.RequestException:
                 continue
 
             # Create a dictionary to store the source name and URL
             data = {"name": i, "url": source["url"].format(name)}
 
             # Check the conditions for a valid social media account based on the source 
@@ -92,15 +94,15 @@
     p=mp.Pool(len(names))
     p.map(hunt_user,names)
     p.close()
     p.join()
 
     # Print a message indicating the number of found social media accounts
     print(
-        f"[🌐] Found {colored(len(found), 'green', attrs=['bold'])} social media accounts for {colored(niceNames, 'green', attrs=['bold'])} on the following platforms:\n"
+        f"\n[🌐] Found {colored(len(found), 'green', attrs=['bold'])} social media accounts for {colored(niceNames, 'green', attrs=['bold'])} on the following platforms:\n"
     )
 
     # Iterate through the found social media accounts and print their names and URLs
     for user in found:
         print(
             f"[{colored('✓', 'green', attrs=['bold'])}] {colored(user['name'], 'green', attrs=['bold'])}: {user['url']}"
         )
```

### Comparing `shaggy-1.0.5/shaggy/sources.py` & `shaggy-1.0.6/shaggy/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 sources = {
     "Telegram": {
-        "errorMsg": 'If you have <strong>Telegram',
-        "url": "https://t.me/{}",
+        "errorMsg": '<meta property="og:description" content="">',
+        "url": "https://telegram.me/{}",
     },
     "Instagram": {
          "errorMsg": "Sorry, this page isn't available",
          "url": "https://www.instagram.com/{}",
     },
     "Facebook": {
         "url": "https://www.facebook.com/{}",
```

### Comparing `shaggy-1.0.5/shaggy.egg-info/PKG-INFO` & `shaggy-1.0.6/shaggy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 License: MIT
 Description: # Shaggy
```

