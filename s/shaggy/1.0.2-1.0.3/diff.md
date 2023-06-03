# Comparing `tmp/shaggy-1.0.2.tar.gz` & `tmp/shaggy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaggy-1.0.2.tar", last modified: Fri Jun  2 16:55:46 2023, max compression
+gzip compressed data, was "shaggy-1.0.3.tar", last modified: Sat Jun  3 06:27:18 2023, max compression
```

## Comparing `shaggy-1.0.2.tar` & `shaggy-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 16:55:46.317046 shaggy-1.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-05-31 11:30:02.000000 shaggy-1.0.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 16:55:46.317046 shaggy-1.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2264 2023-06-02 12:57:10.000000 shaggy-1.0.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-02 16:55:46.317046 shaggy-1.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      693 2023-06-02 16:55:31.000000 shaggy-1.0.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 16:55:46.313046 shaggy-1.0.2/shaggy.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:27:18.457062 shaggy-1.0.3/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-01 10:20:38.000000 shaggy-1.0.3/.gitignore
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1071 2023-05-31 17:40:10.000000 shaggy-1.0.3/LICENSE
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-03 06:27:18.457062 shaggy-1.0.3/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2264 2023-06-03 06:14:32.000000 shaggy-1.0.3/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       55 2023-06-03 06:27:17.000000 shaggy-1.0.3/publish.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       62 2023-05-31 18:26:53.000000 shaggy-1.0.3/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       38 2023-06-03 06:27:18.457062 shaggy-1.0.3/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1212 2023-06-03 06:27:15.000000 shaggy-1.0.3/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:27:18.453062 shaggy-1.0.3/shaggy/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4870 2023-06-03 06:14:32.000000 shaggy-1.0.3/shaggy/__init__py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4190 2023-06-03 06:14:32.000000 shaggy-1.0.3/shaggy/hunt.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      337 2023-06-03 06:14:32.000000 shaggy-1.0.3/shaggy/output.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4088 2023-06-03 06:14:32.000000 shaggy-1.0.3/shaggy/sources.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-03 06:27:18.457062 shaggy-1.0.3/shaggy.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3087 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      315 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       49 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-03 06:27:18.000000 shaggy-1.0.3/shaggy.egg-info/top_level.txt
```

### Comparing `shaggy-1.0.2/LICENSE` & `shaggy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.2/PKG-INFO` & `shaggy-1.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: shaggy
-Version: 1.0.2
-Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
-Home-page: https://github.com/mauro-balades/shaggy
-Author: Mauro Baladés
-Author-email: mauro.balades@tutanota.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shaggy
 
 Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 
 As you know sherlock's devs don't really care about the **important** websites, so we came and cut the **bs** to make your lifes easier. May the [shaggy](https://www.youtube.com/watch?v=6qQJvUfBDOQ) supremacy beggin.
 
 ~ **Sherlock, but better**
```

