# Comparing `tmp/cs1-0.2.2.tar.gz` & `tmp/cs1-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs1-0.2.2.tar", last modified: Tue Apr  4 07:13:55 2023, max compression
+gzip compressed data, was "cs1-0.2.3.tar", last modified: Sat Jun  3 05:05:21 2023, max compression
```

## Comparing `cs1-0.2.2.tar` & `cs1-0.2.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:55.062221 cs1-0.2.2/
--rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 cs1-0.2.2/LICENCE
--rw-rw-rw-   0        0        0     4983 2023-04-04 07:13:55.063219 cs1-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4344 2023-03-26 02:46:34.000000 cs1-0.2.2/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cs1-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     1015 2023-04-04 07:13:55.065218 cs1-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.202453 cs1-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.453732 cs1-0.2.2/src/cs1/
--rw-rw-rw-   0        0        0    38783 2023-02-24 08:13:59.000000 cs1-0.2.2/src/cs1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.469360 cs1-0.2.2/src/cs1/basis/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.2/src/cs1/basis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.469360 cs1-0.2.2/src/cs1/basis/adaptive/
--rw-rw-rw-   0        0        0     5124 2023-02-21 12:23:56.000000 cs1-0.2.2/src/cs1/basis/adaptive/__init__.py
--rw-rw-rw-   0        0        0    18165 2023-04-04 07:11:28.000000 cs1-0.2.2/src/cs1/basis/adaptive/vae.py
--rw-rw-rw-   0        0        0     7148 2023-01-15 10:21:44.000000 cs1-0.2.2/src/cs1/basis/common.py
--rw-rw-rw-   0        0        0    24299 2023-02-24 10:38:00.000000 cs1-0.2.2/src/cs1/cs.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.484983 cs1-0.2.2/src/cs1/domain/
--rw-rw-rw-   0        0        0      693 2022-10-08 07:15:14.000000 cs1-0.2.2/src/cs1/domain/__init__.py
--rw-rw-rw-   0        0        0     9862 2023-01-08 15:31:23.000000 cs1-0.2.2/src/cs1/domain/audio.py
--rw-rw-rw-   0        0        0    11912 2023-01-15 13:30:15.000000 cs1-0.2.2/src/cs1/domain/image.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.484983 cs1-0.2.2/src/cs1/gui/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.2/src/cs1/gui/__init__.py
--rw-rw-rw-   0        0        0     4433 2023-03-16 02:40:31.000000 cs1-0.2.2/src/cs1/gui/run.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.783201 cs1-0.2.2/src/cs1/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.2/src/cs1/gui/static/__init__.py
--rw-rw-rw-   0        0        0     2518 2022-07-20 15:27:40.000000 cs1-0.2.2/src/cs1/gui/static/bootstrap-dialog.css
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cs1-0.2.2/src/cs1/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cs1-0.2.2/src/cs1/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    37444 2022-11-12 14:05:28.000000 cs1-0.2.2/src/cs1/gui/static/font-awesome.css
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.924207 cs1-0.2.2/src/cs1/gui/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.2/src/cs1/gui/static/fonts/__init__.py
--rw-rw-rw-   0        0        0   165742 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2022-07-20 15:27:41.000000 cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.987122 cs1-0.2.2/src/cs1/gui/static/images/
--rw-rw-rw-   0        0        0    51449 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/BCoT.png
--rw-rw-rw-   0        0        0   111921 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/DCT.png
--rw-rw-rw-   0        0        0    74145 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/DFT.png
--rw-rw-rw-   0        0        0     8052 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/DFT_A.png
--rw-rw-rw-   0        0        0   108584 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/DFT_P.png
--rw-rw-rw-   0        0        0    13354 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/HWT.png
--rw-rw-rw-   0        0        0     1511 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/IDM.png
--rw-rw-rw-   0        0        0    86935 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/SECS.png
--rw-rw-rw-   0        0        0    71199 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/Sensing - clean.png
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.2/src/cs1/gui/static/images/__init__.py
--rw-rw-rw-   0        0        0    80565 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/reconstruction - clean.png
--rw-rw-rw-   0        0        0   264308 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/reconstruction.png
--rw-rw-rw-   0        0        0   152714 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/sensing matrix - clean.png
--rw-rw-rw-   0        0        0   804558 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/sensing matrix.jpeg
--rw-rw-rw-   0        0        0   160937 2022-07-20 15:47:00.000000 cs1-0.2.2/src/cs1/gui/static/images/sensing.png
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cs1-0.2.2/src/cs1/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0   520714 2022-07-20 15:28:09.000000 cs1-0.2.2/src/cs1/gui/static/jquery-ui-1.12.1.js
--rw-rw-rw-   0        0        0    64017 2022-07-20 15:27:42.000000 cs1-0.2.2/src/cs1/gui/static/jquery-ui.css
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cs1-0.2.2/src/cs1/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cs1-0.2.2/src/cs1/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0     8602 2022-07-20 15:28:18.000000 cs1-0.2.2/src/cs1/gui/static/seedrandom.js
--rw-rw-rw-   0        0        0     4727 2022-11-12 02:00:29.000000 cs1-0.2.2/src/cs1/gui/static/utility.chart.js
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:55.056218 cs1-0.2.2/src/cs1/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cs1-0.2.2/src/cs1/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    95318 2022-11-18 14:09:58.000000 cs1-0.2.2/src/cs1/gui/templates/home.html
--rw-rw-rw-   0        0        0    23043 2022-11-18 14:32:23.000000 cs1-0.2.2/src/cs1/gui/templates/receiver.html
--rw-rw-rw-   0        0        0     8549 2022-11-19 14:14:31.000000 cs1-0.2.2/src/cs1/gui/templates/tutorial.html
--rw-rw-rw-   0        0        0     7753 2023-01-15 08:44:54.000000 cs1-0.2.2/src/cs1/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:55.060221 cs1-0.2.2/src/cs1/security/
--rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.2/src/cs1/security/__init__.py
--rw-rw-rw-   0        0        0     4237 2022-10-08 09:28:26.000000 cs1-0.2.2/src/cs1/security/tvsm.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:13:54.469360 cs1-0.2.2/src/cs1.egg-info/
--rw-rw-rw-   0        0        0     4983 2023-04-04 07:13:54.000000 cs1-0.2.2/src/cs1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2317 2023-04-04 07:13:54.000000 cs1-0.2.2/src/cs1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 07:13:54.000000 cs1-0.2.2/src/cs1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-04 07:13:54.000000 cs1-0.2.2/src/cs1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-04 07:13:54.000000 cs1-0.2.2/src/cs1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.716906 cs1-0.2.3/
+-rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 cs1-0.2.3/LICENCE
+-rw-rw-rw-   0        0        0     4998 2023-06-03 05:05:21.716906 cs1-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4359 2023-06-03 02:56:39.000000 cs1-0.2.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cs1-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1015 2023-06-03 05:05:21.724934 cs1-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.591519 cs1-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.605640 cs1-0.2.3/src/cs1/
+-rw-rw-rw-   0        0        0    38783 2023-02-24 08:13:59.000000 cs1-0.2.3/src/cs1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.628652 cs1-0.2.3/src/cs1/basis/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/basis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.631649 cs1-0.2.3/src/cs1/basis/adaptive/
+-rw-rw-rw-   0        0        0     5124 2023-02-21 12:23:56.000000 cs1-0.2.3/src/cs1/basis/adaptive/__init__.py
+-rw-rw-rw-   0        0        0    18165 2023-04-04 07:11:28.000000 cs1-0.2.3/src/cs1/basis/adaptive/vae.py
+-rw-rw-rw-   0        0        0     7148 2023-01-15 10:21:44.000000 cs1-0.2.3/src/cs1/basis/common.py
+-rw-rw-rw-   0        0        0    24696 2023-06-03 03:57:26.000000 cs1-0.2.3/src/cs1/cs.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.635648 cs1-0.2.3/src/cs1/domain/
+-rw-rw-rw-   0        0        0      693 2022-10-08 07:15:14.000000 cs1-0.2.3/src/cs1/domain/__init__.py
+-rw-rw-rw-   0        0        0     9862 2023-01-08 15:31:23.000000 cs1-0.2.3/src/cs1/domain/audio.py
+-rw-rw-rw-   0        0        0    11912 2023-01-15 13:30:15.000000 cs1-0.2.3/src/cs1/domain/image.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.638653 cs1-0.2.3/src/cs1/gui/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/gui/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-03-16 02:40:31.000000 cs1-0.2.3/src/cs1/gui/run.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.658898 cs1-0.2.3/src/cs1/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/__init__.py
+-rw-rw-rw-   0        0        0     2518 2022-07-20 15:27:40.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap-dialog.css
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cs1-0.2.3/src/cs1/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    37444 2022-11-12 14:05:28.000000 cs1-0.2.3/src/cs1/gui/static/font-awesome.css
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.681901 cs1-0.2.3/src/cs1/gui/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/fonts/__init__.py
+-rw-rw-rw-   0        0        0   165742 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2022-07-20 15:27:41.000000 cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.706900 cs1-0.2.3/src/cs1/gui/static/images/
+-rw-rw-rw-   0        0        0    51449 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/BCoT.png
+-rw-rw-rw-   0        0        0   111921 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DCT.png
+-rw-rw-rw-   0        0        0    74145 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT.png
+-rw-rw-rw-   0        0        0     8052 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT_A.png
+-rw-rw-rw-   0        0        0   108584 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/DFT_P.png
+-rw-rw-rw-   0        0        0    13354 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/HWT.png
+-rw-rw-rw-   0        0        0     1511 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/IDM.png
+-rw-rw-rw-   0        0        0    86935 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/SECS.png
+-rw-rw-rw-   0        0        0    71199 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/Sensing - clean.png
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cs1-0.2.3/src/cs1/gui/static/images/__init__.py
+-rw-rw-rw-   0        0        0    80565 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/reconstruction - clean.png
+-rw-rw-rw-   0        0        0   264308 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/reconstruction.png
+-rw-rw-rw-   0        0        0   152714 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing matrix - clean.png
+-rw-rw-rw-   0        0        0   804558 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing matrix.jpeg
+-rw-rw-rw-   0        0        0   160937 2022-07-20 15:47:00.000000 cs1-0.2.3/src/cs1/gui/static/images/sensing.png
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cs1-0.2.3/src/cs1/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0   520714 2022-07-20 15:28:09.000000 cs1-0.2.3/src/cs1/gui/static/jquery-ui-1.12.1.js
+-rw-rw-rw-   0        0        0    64017 2022-07-20 15:27:42.000000 cs1-0.2.3/src/cs1/gui/static/jquery-ui.css
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cs1-0.2.3/src/cs1/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cs1-0.2.3/src/cs1/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0     8602 2022-07-20 15:28:18.000000 cs1-0.2.3/src/cs1/gui/static/seedrandom.js
+-rw-rw-rw-   0        0        0     4727 2022-11-12 02:00:29.000000 cs1-0.2.3/src/cs1/gui/static/utility.chart.js
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.712924 cs1-0.2.3/src/cs1/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cs1-0.2.3/src/cs1/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    95318 2022-11-18 14:09:58.000000 cs1-0.2.3/src/cs1/gui/templates/home.html
+-rw-rw-rw-   0        0        0    23043 2022-11-18 14:32:23.000000 cs1-0.2.3/src/cs1/gui/templates/receiver.html
+-rw-rw-rw-   0        0        0     8549 2022-11-19 14:14:31.000000 cs1-0.2.3/src/cs1/gui/templates/tutorial.html
+-rw-rw-rw-   0        0        0     7753 2023-01-15 08:44:54.000000 cs1-0.2.3/src/cs1/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.715901 cs1-0.2.3/src/cs1/security/
+-rw-rw-rw-   0        0        0        0 2022-10-07 10:23:54.000000 cs1-0.2.3/src/cs1/security/__init__.py
+-rw-rw-rw-   0        0        0     4237 2022-10-08 09:28:26.000000 cs1-0.2.3/src/cs1/security/tvsm.py
+drwxrwxrwx   0        0        0        0 2023-06-03 05:05:21.626648 cs1-0.2.3/src/cs1.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2317 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-03 05:05:21.000000 cs1-0.2.3/src/cs1.egg-info/top_level.txt
```

### Comparing `cs1-0.2.2/PKG-INFO` & `cs1-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs1
-Version: 0.2.2
+Version: 0.2.3
 Summary: Compressed Sensing library for 1D Spectroscopic Profiling Data
 Home-page: https://github.com/zhangys11/cs1
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -94,15 +94,15 @@
 
     # sparsity analysis
     cs1.metrics.analyze_sparsity(x, PSIs)
 
 <img src='sparsity_analysis.png'>
 
     # compare different bases and sampling ratio on a single sample
-    rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns relative MSEs
+    mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns MSEs and relative MSEs
 
 <img src='grid_search.png'>
 
 # low-level cs functions
     
     from cs1.basis.common import *
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cs1 Version: 0.2.2 Summary: Compressed Sensing
+Metadata-Version: 2.1 Name: cs1 Version: 0.2.3 Summary: Compressed Sensing
 library for 1D Spectroscopic Profiling Data Home-page: https://github.com/
 zhangys11/cs1 Author: Yinsheng Zhang (Ph.D.) Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Operating
 System :: OS Independent Classifier: Topic :: Scientific/Engineering ::
 Mathematics Requires-Python: >=3.6 Description-Content-Type: text/markdown
@@ -41,20 +41,21 @@
 pip install cs1 # A simple startup import cs1 # Generate common non-adaptive
 bases and save to a local pickle file. # The generation process can be very
 slow, so save it for future use. cs1.basis.common.Generate_PSIs(n, savepath =
 'PSIs_' + str(n) + '.pkl') # n is the data/signal dimensionality # load back
 bases file = open('PSIs_' + str(n) + '.pkl','rb') PSIs = pickle.load(file)
 file.close() # sparsity analysis cs1.metrics.analyze_sparsity(x, PSIs)
 [sparsity_analysis.png] # compare different bases and sampling ratio on a
-single sample rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver =
-'LASSO') # returns relative MSEs [grid_search.png] # low-level cs functions
-from cs1.basis.common import * dftmtx() dctmtx() hwtmtx() from cs1.cs import *
-sensing() recovery() from cs1.metrics import * mutual_coherence() ... # singal
-processing functions for audio / image domains from cs1.domain.audio import *
-simulate_ECG() dct_lossy_signal_compression() dft_lossy_signal_compression()
-from cs1.domain.image import * img_dct() img_dft() dct_lossy_image_compression
-() dft_lossy_image_compression() # adaptive cs bases from cs1.basis.adaptive
-import * PSI, _ = EBP(X) # X is a m-by-n training dataset. PSI is the EBP basis
-PSI, _, _ = LDA(X, y, display = True) # X and y are training dataset. PSI is
-the LDA basis. # run as a local web server `python -m cs1.gui.run` You can then
-access the web GUI at the 5006 port: [src/cs1/gui/static/images/Sensing -
-clean.png] [src/cs1/gui/static/images/reconstruction - clean.png]
+single sample mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs,
+solver = 'LASSO') # returns MSEs and relative MSEs [grid_search.png] # low-
+level cs functions from cs1.basis.common import * dftmtx() dctmtx() hwtmtx()
+from cs1.cs import * sensing() recovery() from cs1.metrics import *
+mutual_coherence() ... # singal processing functions for audio / image domains
+from cs1.domain.audio import * simulate_ECG() dct_lossy_signal_compression()
+dft_lossy_signal_compression() from cs1.domain.image import * img_dct() img_dft
+() dct_lossy_image_compression() dft_lossy_image_compression() # adaptive cs
+bases from cs1.basis.adaptive import * PSI, _ = EBP(X) # X is a m-by-n training
+dataset. PSI is the EBP basis PSI, _, _ = LDA(X, y, display = True) # X and y
+are training dataset. PSI is the LDA basis. # run as a local web server `python
+-m cs1.gui.run` You can then access the web GUI at the 5006 port: [src/cs1/gui/
+static/images/Sensing - clean.png] [src/cs1/gui/static/images/reconstruction -
+clean.png]
```

### Comparing `cs1-0.2.2/README.md` & `cs1-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     # sparsity analysis
     cs1.metrics.analyze_sparsity(x, PSIs)
 
 <img src='sparsity_analysis.png'>
 
     # compare different bases and sampling ratio on a single sample
-    rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns relative MSEs
+    mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns MSEs and relative MSEs
 
 <img src='grid_search.png'>
 
 # low-level cs functions
     
     from cs1.basis.common import *
```

#### html2text {}

```diff
@@ -33,20 +33,21 @@
 pip install cs1 # A simple startup import cs1 # Generate common non-adaptive
 bases and save to a local pickle file. # The generation process can be very
 slow, so save it for future use. cs1.basis.common.Generate_PSIs(n, savepath =
 'PSIs_' + str(n) + '.pkl') # n is the data/signal dimensionality # load back
 bases file = open('PSIs_' + str(n) + '.pkl','rb') PSIs = pickle.load(file)
 file.close() # sparsity analysis cs1.metrics.analyze_sparsity(x, PSIs)
 [sparsity_analysis.png] # compare different bases and sampling ratio on a
-single sample rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver =
-'LASSO') # returns relative MSEs [grid_search.png] # low-level cs functions
-from cs1.basis.common import * dftmtx() dctmtx() hwtmtx() from cs1.cs import *
-sensing() recovery() from cs1.metrics import * mutual_coherence() ... # singal
-processing functions for audio / image domains from cs1.domain.audio import *
-simulate_ECG() dct_lossy_signal_compression() dft_lossy_signal_compression()
-from cs1.domain.image import * img_dct() img_dft() dct_lossy_image_compression
-() dft_lossy_image_compression() # adaptive cs bases from cs1.basis.adaptive
-import * PSI, _ = EBP(X) # X is a m-by-n training dataset. PSI is the EBP basis
-PSI, _, _ = LDA(X, y, display = True) # X and y are training dataset. PSI is
-the LDA basis. # run as a local web server `python -m cs1.gui.run` You can then
-access the web GUI at the 5006 port: [src/cs1/gui/static/images/Sensing -
-clean.png] [src/cs1/gui/static/images/reconstruction - clean.png]
+single sample mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs,
+solver = 'LASSO') # returns MSEs and relative MSEs [grid_search.png] # low-
+level cs functions from cs1.basis.common import * dftmtx() dctmtx() hwtmtx()
+from cs1.cs import * sensing() recovery() from cs1.metrics import *
+mutual_coherence() ... # singal processing functions for audio / image domains
+from cs1.domain.audio import * simulate_ECG() dct_lossy_signal_compression()
+dft_lossy_signal_compression() from cs1.domain.image import * img_dct() img_dft
+() dct_lossy_image_compression() dft_lossy_image_compression() # adaptive cs
+bases from cs1.basis.adaptive import * PSI, _ = EBP(X) # X is a m-by-n training
+dataset. PSI is the EBP basis PSI, _, _ = LDA(X, y, display = True) # X and y
+are training dataset. PSI is the LDA basis. # run as a local web server `python
+-m cs1.gui.run` You can then access the web GUI at the 5006 port: [src/cs1/gui/
+static/images/Sensing - clean.png] [src/cs1/gui/static/images/reconstruction -
+clean.png]
```

### Comparing `cs1-0.2.2/setup.cfg` & `cs1-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7331 0d0a 7665 7273 696f 6e20   = cs1..version 
-00000020: 3d20 302e 322e 320d 0a61 7574 686f 7220  = 0.2.2..author 
+00000020: 3d20 302e 322e 330d 0a61 7574 686f 7220  = 0.2.3..author 
 00000030: 3d20 5969 6e73 6865 6e67 205a 6861 6e67  = Yinsheng Zhang
 00000040: 2028 5068 2e44 2e29 0d0a 6175 7468 6f72   (Ph.D.)..author
 00000050: 5f65 6d61 696c 203d 206f 6f40 7a6a 752e  _email = oo@zju.
 00000060: 6564 752e 636e 0d0a 6465 7363 7269 7074  edu.cn..descript
 00000070: 696f 6e20 3d20 436f 6d70 7265 7373 6564  ion = Compressed
 00000080: 2053 656e 7369 6e67 206c 6962 7261 7279   Sensing library
 00000090: 2066 6f72 2031 4420 5370 6563 7472 6f73   for 1D Spectros
```

### Comparing `cs1-0.2.2/src/cs1/__init__.py` & `cs1-0.2.3/src/cs1/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/basis/adaptive/__init__.py` & `cs1-0.2.3/src/cs1/basis/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/basis/adaptive/vae.py` & `cs1-0.2.3/src/cs1/basis/adaptive/vae.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/basis/common.py` & `cs1-0.2.3/src/cs1/basis/common.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/cs.py` & `cs1-0.2.3/src/cs1/cs.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         if  t == PSI_NAMES[5] or t == PSI_LONGNAMES[5] or \
             t == 'DFT' or \
             t == 'DWT' or \
             t == 'LDA':
             alphas = [0.005, 0.0001, 0.00001] # set empirical alpha values. LDA needs smaller alpha
 
         if isinstance(L1, float):
-            lasso = Lasso(alpha=L1, tol = 0.0005)    
+            lasso = Lasso(alpha=L1, tol = 0.0005)
         else:
             lasso = LassoCV(alphas = alphas, selection = 'random', tol = 0.001, n_jobs=-1, verbose = verbose) # ‘random’ often leads to significantly faster convergence especially when tol is higher than 1e-4.
             # 实测并未发现 selction = cyclic / random 两种模式的运行时间差异
         
         lasso.fit(A, xs)
         z = lasso.coef_
 
@@ -149,15 +149,15 @@
     elif solver == 'BP':
         
         n = A.shape[1]
         z = cvxpy.Variable(n)
         obj = cvxpy.Minimize(cvxpy.norm(z, 1))
         const = [A @ z == xs]
         prob = cvxpy.Problem(obj,const)
-        _ = prob.solve()       
+        _ = prob.solve()  
         z = z.value
 
     if t == PSI_NAMES[0] or t == PSI_LONGNAMES[0]:
         z = np.linalg.pinv(A) @ xs
         xr = z
     elif  t == PSI_NAMES[1] or t == PSI_LONGNAMES[1]:
         xr = cv2.idct(z)
@@ -232,38 +232,42 @@
     Use grid search strategy to find the best.
 
     Parameters
     ----------
     x : a single data sample (a vector) 
     '''
 
-    def DynamicProperty(RMSES, PSIs, ks, repeat = 1):
+    def DynamicProperty(MSES, RMSES, PSIs, ks):
 
-        assert (len(RMSES) == len(PSIs))
+        assert (len(RMSES) == len(PSIs) and len(MSES) == len(PSIs))
         matplotlib.rcParams.update({'font.size': 16})
         
-        for i, key in enumerate(PSIs):   
+        for metric_name, metric_value in zip(['MSE', 'RMSE'], [MSES, RMSES]):
+            # print(metric_name, metric_value)
+
+            for i, key in enumerate(PSIs):
+                    
+                plt.figure(figsize=(8,6))
                 
-            plt.figure(figsize=(8,6))
-            
-            plt.scatter(ks, RMSES[i], c='gray', s = 70, label = key)
-            plt.plot(ks, RMSES[i], c='gray')
-            plt.xlabel('k')
-            plt.ylabel('RMSE')
-            
-            plt.legend()
-            plt.show()
+                plt.scatter(ks, metric_value[i], c='gray', s = 70, label = key)
+                plt.plot(ks, metric_value[i], c='gray')
+                plt.xlabel(r'$k$')
+                plt.ylabel(metric_name)
+                plt.ticklabel_format(style='scientific', axis='y', scilimits=(-4,4), useMathText = True)
+                plt.legend()
+                plt.show()
 
         matplotlib.rcParams.update({'font.size': 12})
 
 
     plt.figure(figsize=(40, len(PSIs)*5))
     rows = len(PSIs) + 1
     matplotlib.rcParams.update({'font.size': 24})    
     COLS = 2 + len(ks)
+    MSES = []
     RMSES = []
 
     for idx, key in enumerate(PSIs):
 
         PSI = PSIs[key]
         
         # padded version
@@ -330,14 +334,15 @@
             plt.title('z (latent space)') # '\n'+psi_name + 
         if psi_name == 'EBP':
             pylab.ylim([-abs(max(z,key=abs)), abs(max(z,key=abs))])
         plt.xticks([])
         plt.yticks([])
         # plt.axis('off')
         
+        mses = []
         rmses = []
         
         for kidx, k in enumerate(ks):
         
             ########## sensing #############
 
             # either works fine
@@ -362,41 +367,43 @@
 
             else:
                 A = MeasurementMatrix(len(xe), pidx, psi_name)
                 W = None
 
             z, xr = Recovery (A, xs, psi_name, display = False, PSI = W, solver = solver) # lower k needs bigger L1. k 0.1 - L1 0.1, k 0.01, L1 - 10
             
-            _, _, rmse = calculate_recon_error(xe.reshape(1, -1), xr.reshape(1, -1)) #(np.matrix(xe), np.matrix(xr))        
+            mse, _, rmse = calculate_recon_error(xe.reshape(1, -1), xr.reshape(1, -1)) #(np.matrix(xe), np.matrix(xr))        
+            mses.append(mse)
             rmses.append(rmse)
             
             plt.subplot(rows,COLS,COLS*idx+2+1+kidx)
             plt.plot(xr[:len(x)], label = 'RMSE ' + str( round(rmse, 3) ), color='gray') # cut the first n points, as in HWT, xr is padded.
             if idx == 0:
                 plt.title('$x_r$ ($k$=' + str(round(k, 2)) + ', $n_s$=' + str(len(xs)) + ')')
             plt.xticks([])
             plt.yticks([])
             # plt.legend()
             
+        MSES.append(mses)
         RMSES.append(rmses)
         
         #plt.subplot(rows,3,3*idx+3)
         #plt.scatter(thresholds, rs, color='gray')
         #plt.title('\nAUC = ' + str(round(auc,3)) + ', s = ' + str(round(r,3))) # $s_{2\%}$ 
         #pylab.xlim([0,0.002])
         #pylab.ylim([0,1.0])
         #plt.xticks(np.arange(0.0, 0.0021, 0.0005))
         
         #plt.subplots_adjust(top=1., left=0., right=1., bottom=0.)
 
     matplotlib.rcParams.update({'font.size': 12})
 
     print('\n-------------\nThe following are dynamic properties of each PSI:')
-    DynamicProperty(RMSES, PSIs, np.round(ks,2))
-    return RMSES
+    DynamicProperty(MSES, RMSES, PSIs, np.round(ks,2))
+    return MSES, RMSES
 
 
 def Dataset_Sensing_n_Recovery (X, y = None, k = 0.2, t = 'DCT', solver = 'LASSO', L1 = 0.005, display = 'all'):
     '''
     Provide a complete pipeline for an entire dataset. 
     PCA 2D visualization and multivariate KLD are evaluated.
```

### Comparing `cs1-0.2.2/src/cs1/domain/__init__.py` & `cs1-0.2.3/src/cs1/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/domain/audio.py` & `cs1-0.2.3/src/cs1/domain/audio.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/domain/image.py` & `cs1-0.2.3/src/cs1/domain/image.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/run.py` & `cs1-0.2.3/src/cs1/gui/run.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/bootstrap-dialog.css` & `cs1-0.2.3/src/cs1/gui/static/bootstrap-dialog.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/bootstrap.css` & `cs1-0.2.3/src/cs1/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/bootstrap.js` & `cs1-0.2.3/src/cs1/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/font-awesome.css` & `cs1-0.2.3/src/cs1/gui/static/font-awesome.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/FontAwesome.otf` & `cs1-0.2.3/src/cs1/gui/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.eot` & `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.svg` & `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.ttf` & `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.woff` & `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/fontawesome-webfont.woff2` & `cs1-0.2.3/src/cs1/gui/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot` & `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg` & `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf` & `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff` & `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2` & `cs1-0.2.3/src/cs1/gui/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/BCoT.png` & `cs1-0.2.3/src/cs1/gui/static/images/BCoT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/DCT.png` & `cs1-0.2.3/src/cs1/gui/static/images/DCT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/DFT.png` & `cs1-0.2.3/src/cs1/gui/static/images/DFT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/DFT_A.png` & `cs1-0.2.3/src/cs1/gui/static/images/DFT_A.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/DFT_P.png` & `cs1-0.2.3/src/cs1/gui/static/images/DFT_P.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/HWT.png` & `cs1-0.2.3/src/cs1/gui/static/images/HWT.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/IDM.png` & `cs1-0.2.3/src/cs1/gui/static/images/IDM.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/SECS.png` & `cs1-0.2.3/src/cs1/gui/static/images/SECS.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/Sensing - clean.png` & `cs1-0.2.3/src/cs1/gui/static/images/Sensing - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/reconstruction - clean.png` & `cs1-0.2.3/src/cs1/gui/static/images/reconstruction - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/reconstruction.png` & `cs1-0.2.3/src/cs1/gui/static/images/reconstruction.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/sensing matrix - clean.png` & `cs1-0.2.3/src/cs1/gui/static/images/sensing matrix - clean.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/sensing matrix.jpeg` & `cs1-0.2.3/src/cs1/gui/static/images/sensing matrix.jpeg`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/images/sensing.png` & `cs1-0.2.3/src/cs1/gui/static/images/sensing.png`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/jquery-3.3.1.min.js` & `cs1-0.2.3/src/cs1/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/jquery-ui-1.12.1.js` & `cs1-0.2.3/src/cs1/gui/static/jquery-ui-1.12.1.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/jquery-ui.css` & `cs1-0.2.3/src/cs1/gui/static/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/jquery.blockUI.js` & `cs1-0.2.3/src/cs1/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/jquery.form.min.js` & `cs1-0.2.3/src/cs1/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/seedrandom.js` & `cs1-0.2.3/src/cs1/gui/static/seedrandom.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/static/utility.chart.js` & `cs1-0.2.3/src/cs1/gui/static/utility.chart.js`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/templates/home.html` & `cs1-0.2.3/src/cs1/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/templates/receiver.html` & `cs1-0.2.3/src/cs1/gui/templates/receiver.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/gui/templates/tutorial.html` & `cs1-0.2.3/src/cs1/gui/templates/tutorial.html`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/metrics.py` & `cs1-0.2.3/src/cs1/metrics.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1/security/tvsm.py` & `cs1-0.2.3/src/cs1/security/tvsm.py`

 * *Files identical despite different names*

### Comparing `cs1-0.2.2/src/cs1.egg-info/PKG-INFO` & `cs1-0.2.3/src/cs1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs1
-Version: 0.2.2
+Version: 0.2.3
 Summary: Compressed Sensing library for 1D Spectroscopic Profiling Data
 Home-page: https://github.com/zhangys11/cs1
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -94,15 +94,15 @@
 
     # sparsity analysis
     cs1.metrics.analyze_sparsity(x, PSIs)
 
 <img src='sparsity_analysis.png'>
 
     # compare different bases and sampling ratio on a single sample
-    rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns relative MSEs
+    mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver = 'LASSO') # returns MSEs and relative MSEs
 
 <img src='grid_search.png'>
 
 # low-level cs functions
     
     from cs1.basis.common import *
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cs1 Version: 0.2.2 Summary: Compressed Sensing
+Metadata-Version: 2.1 Name: cs1 Version: 0.2.3 Summary: Compressed Sensing
 library for 1D Spectroscopic Profiling Data Home-page: https://github.com/
 zhangys11/cs1 Author: Yinsheng Zhang (Ph.D.) Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/cs1/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Operating
 System :: OS Independent Classifier: Topic :: Scientific/Engineering ::
 Mathematics Requires-Python: >=3.6 Description-Content-Type: text/markdown
@@ -41,20 +41,21 @@
 pip install cs1 # A simple startup import cs1 # Generate common non-adaptive
 bases and save to a local pickle file. # The generation process can be very
 slow, so save it for future use. cs1.basis.common.Generate_PSIs(n, savepath =
 'PSIs_' + str(n) + '.pkl') # n is the data/signal dimensionality # load back
 bases file = open('PSIs_' + str(n) + '.pkl','rb') PSIs = pickle.load(file)
 file.close() # sparsity analysis cs1.metrics.analyze_sparsity(x, PSIs)
 [sparsity_analysis.png] # compare different bases and sampling ratio on a
-single sample rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs, solver =
-'LASSO') # returns relative MSEs [grid_search.png] # low-level cs functions
-from cs1.basis.common import * dftmtx() dctmtx() hwtmtx() from cs1.cs import *
-sensing() recovery() from cs1.metrics import * mutual_coherence() ... # singal
-processing functions for audio / image domains from cs1.domain.audio import *
-simulate_ECG() dct_lossy_signal_compression() dft_lossy_signal_compression()
-from cs1.domain.image import * img_dct() img_dft() dct_lossy_image_compression
-() dft_lossy_image_compression() # adaptive cs bases from cs1.basis.adaptive
-import * PSI, _ = EBP(X) # X is a m-by-n training dataset. PSI is the EBP basis
-PSI, _, _ = LDA(X, y, display = True) # X and y are training dataset. PSI is
-the LDA basis. # run as a local web server `python -m cs1.gui.run` You can then
-access the web GUI at the 5006 port: [src/cs1/gui/static/images/Sensing -
-clean.png] [src/cs1/gui/static/images/reconstruction - clean.png]
+single sample mses, rmses = cs1.cs.GridSearch_Sensing_n_Recovery(x, PSIs,
+solver = 'LASSO') # returns MSEs and relative MSEs [grid_search.png] # low-
+level cs functions from cs1.basis.common import * dftmtx() dctmtx() hwtmtx()
+from cs1.cs import * sensing() recovery() from cs1.metrics import *
+mutual_coherence() ... # singal processing functions for audio / image domains
+from cs1.domain.audio import * simulate_ECG() dct_lossy_signal_compression()
+dft_lossy_signal_compression() from cs1.domain.image import * img_dct() img_dft
+() dct_lossy_image_compression() dft_lossy_image_compression() # adaptive cs
+bases from cs1.basis.adaptive import * PSI, _ = EBP(X) # X is a m-by-n training
+dataset. PSI is the EBP basis PSI, _, _ = LDA(X, y, display = True) # X and y
+are training dataset. PSI is the LDA basis. # run as a local web server `python
+-m cs1.gui.run` You can then access the web GUI at the 5006 port: [src/cs1/gui/
+static/images/Sensing - clean.png] [src/cs1/gui/static/images/reconstruction -
+clean.png]
```

### Comparing `cs1-0.2.2/src/cs1.egg-info/SOURCES.txt` & `cs1-0.2.3/src/cs1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

