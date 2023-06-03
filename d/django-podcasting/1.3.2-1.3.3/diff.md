# Comparing `tmp/django-podcasting-1.3.2.tar.gz` & `tmp/django-podcasting-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-podcasting-1.3.2.tar", last modified: Thu Mar 23 18:53:11 2017, max compression
+gzip compressed data, was "django-podcasting-1.3.3.tar", last modified: Sat Jun  3 03:22:32 2023, max compression
```

## Comparing `django-podcasting-1.3.2.tar` & `django-podcasting-1.3.3.tar`

### file list

```diff
@@ -1,66 +1,61 @@
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/
--rw-r--r--   0 rizumu     (501) staff       (20)      257 2017-03-23 17:24:06.000000 django-podcasting-1.3.2/AUTHORS
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/
--rw-r--r--   0 rizumu     (501) staff       (20)        1 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/dependency_links.txt
--rw-r--r--   0 rizumu     (501) staff       (20)        1 2015-04-03 18:06:16.000000 django-podcasting-1.3.2/django_podcasting.egg-info/not-zip-safe
--rw-r--r--   0 rizumu     (501) staff       (20)       46 2015-04-20 02:40:15.000000 django-podcasting-1.3.2/django_podcasting.egg-info/pbr.json
--rw-r--r--   0 rizumu     (501) staff       (20)     4229 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/PKG-INFO
--rw-r--r--   0 rizumu     (501) staff       (20)       45 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/requires.txt
--rw-r--r--   0 rizumu     (501) staff       (20)     1911 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/SOURCES.txt
--rw-r--r--   0 rizumu     (501) staff       (20)       11 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/django_podcasting.egg-info/top_level.txt
--rw-r--r--   0 rizumu     (501) staff       (20)     5703 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/LICENSE
--rw-r--r--   0 rizumu     (501) staff       (20)      108 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/MANIFEST.in
--rw-r--r--   0 rizumu     (501) staff       (20)     4229 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/PKG-INFO
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/
--rw-r--r--   0 rizumu     (501) staff       (20)      600 2017-03-23 18:52:20.000000 django-podcasting-1.3.2/podcasting/__init__.py
--rw-r--r--   0 rizumu     (501) staff       (20)     2719 2016-12-22 18:16:11.000000 django-podcasting-1.3.2/podcasting/admin.py
--rw-r--r--   0 rizumu     (501) staff       (20)      172 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/conf.py
--rw-r--r--   0 rizumu     (501) staff       (20)    13034 2017-03-23 17:52:55.000000 django-podcasting-1.3.2/podcasting/feeds.py
--rw-r--r--   0 rizumu     (501) staff       (20)    10153 2017-03-23 17:16:10.000000 django-podcasting-1.3.2/podcasting/forms.py
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/locale/
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/locale/es/
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/locale/es/LC_MESSAGES/
--rw-r--r--   0 rizumu     (501) staff       (20)    16908 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rizumu     (501) staff       (20)    20766 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 rizumu     (501) staff       (20)     1037 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/managers.py
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/migrations/
--rw-r--r--   0 rizumu     (501) staff       (20)    17370 2017-03-23 18:51:10.000000 django-podcasting-1.3.2/podcasting/migrations/0001_initial.py
--rw-r--r--   0 rizumu     (501) staff       (20)     3492 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/migrations/0002_auto_20140914_2220.py
--rw-r--r--   0 rizumu     (501) staff       (20)     3251 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/migrations/0003_auto_20160822_2146.py
--rw-r--r--   0 rizumu     (501) staff       (20)      807 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/migrations/0004_auto_20160822_2147.py
--rw-r--r--   0 rizumu     (501) staff       (20)        0 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/migrations/__init__.py
--rw-r--r--   0 rizumu     (501) staff       (20)    25142 2017-03-23 17:53:09.000000 django-podcasting-1.3.2/podcasting/models.py
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/templates/
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/
--rw-r--r--   0 rizumu     (501) staff       (20)     2481 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_current_episode.html
--rw-r--r--   0 rizumu     (501) staff       (20)     1736 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_episode_detail.html
--rw-r--r--   0 rizumu     (501) staff       (20)     2650 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_episode_list.html
--rw-r--r--   0 rizumu     (501) staff       (20)      552 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_feeds.html
--rw-r--r--   0 rizumu     (501) staff       (20)      620 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_show_detail.html
--rw-r--r--   0 rizumu     (501) staff       (20)      695 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/_show_list.html
--rw-r--r--   0 rizumu     (501) staff       (20)      244 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/admin_thumbnail_css.html
--rw-r--r--   0 rizumu     (501) staff       (20)      236 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/admin_thumbnail_easy-thumbnails.html
--rw-r--r--   0 rizumu     (501) staff       (20)       86 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/admin_thumbnail_imagekit.html
--rw-r--r--   0 rizumu     (501) staff       (20)      276 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/admin_thumbnail_sorl.html
--rw-r--r--   0 rizumu     (501) staff       (20)      331 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/current_episode.html
--rw-r--r--   0 rizumu     (501) staff       (20)      249 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/episode_detail.html
--rw-r--r--   0 rizumu     (501) staff       (20)      313 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/episode_list.html
--rw-r--r--   0 rizumu     (501) staff       (20)       31 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/podcasting_base.html
--rw-r--r--   0 rizumu     (501) staff       (20)      288 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/show_detail.html
--rw-r--r--   0 rizumu     (501) staff       (20)      311 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/templates/podcasting/show_list.html
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/tests/
--rw-r--r--   0 rizumu     (501) staff       (20)        0 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/tests/__init__.py
--rw-r--r--   0 rizumu     (501) staff       (20)        0 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/tests/models.py
--rw-r--r--   0 rizumu     (501) staff       (20)     4495 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/tests/tests.py
--rw-r--r--   0 rizumu     (501) staff       (20)      114 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/tests/urls.py
--rw-r--r--   0 rizumu     (501) staff       (20)      561 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/urls.py
--rw-r--r--   0 rizumu     (501) staff       (20)     1045 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/urls_feeds.py
-drwxr-xr-x   0 rizumu     (501) staff       (20)        0 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/podcasting/utils/
--rw-r--r--   0 rizumu     (501) staff       (20)        0 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/utils/__init__.py
--rw-r--r--   0 rizumu     (501) staff       (20)     3044 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/utils/fields.py
--rw-r--r--   0 rizumu     (501) staff       (20)      290 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/utils/twitter.py
--rw-r--r--   0 rizumu     (501) staff       (20)     1874 2015-04-03 17:57:29.000000 django-podcasting-1.3.2/podcasting/utils/widgets.py
--rw-r--r--   0 rizumu     (501) staff       (20)      915 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/podcasting/views.py
--rw-r--r--   0 rizumu     (501) staff       (20)     2607 2016-11-02 15:42:20.000000 django-podcasting-1.3.2/README.rst
--rw-r--r--   0 rizumu     (501) staff       (20)       38 2017-03-23 18:53:11.000000 django-podcasting-1.3.2/setup.cfg
--rw-r--r--   0 rizumu     (501) staff       (20)     1673 2016-11-02 15:30:15.000000 django-podcasting-1.3.2/setup.py
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.632510 django-podcasting-1.3.3/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      257 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/AUTHORS
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     5703 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/LICENSE
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      108 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/MANIFEST.in
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     3626 2023-06-03 03:22:32.632510 django-podcasting-1.3.3/PKG-INFO
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     2607 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/README.rst
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.622510 django-podcasting-1.3.3/django_podcasting.egg-info/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     3626 2023-06-03 03:22:32.000000 django-podcasting-1.3.3/django_podcasting.egg-info/PKG-INFO
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1838 2023-06-03 03:22:32.000000 django-podcasting-1.3.3/django_podcasting.egg-info/SOURCES.txt
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        1 2023-06-03 03:22:32.000000 django-podcasting-1.3.3/django_podcasting.egg-info/dependency_links.txt
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        1 2023-06-03 03:02:11.000000 django-podcasting-1.3.3/django_podcasting.egg-info/not-zip-safe
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)       45 2023-06-03 03:22:32.000000 django-podcasting-1.3.3/django_podcasting.egg-info/requires.txt
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)       11 2023-06-03 03:22:32.000000 django-podcasting-1.3.3/django_podcasting.egg-info/top_level.txt
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.625843 django-podcasting-1.3.3/podcasting/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      600 2023-06-03 02:52:19.000000 django-podcasting-1.3.3/podcasting/__init__.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     2829 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/admin.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      172 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/conf.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)    13034 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/feeds.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)    10916 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/forms.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1037 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/managers.py
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.625843 django-podcasting-1.3.3/podcasting/migrations/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)    29178 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/0001_initial.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     3490 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/0002_auto_20140914_2220.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     3251 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/0003_auto_20160822_2146.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      807 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/0004_auto_20160822_2147.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     5919 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/0005_auto_20190617_1316.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/migrations/__init__.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)    26444 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/models.py
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.622510 django-podcasting-1.3.3/podcasting/templates/
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.629177 django-podcasting-1.3.3/podcasting/templates/podcasting/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     2481 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_current_episode.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1736 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_episode_detail.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     2650 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_episode_list.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      552 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_feeds.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      620 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_show_detail.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      695 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/_show_list.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      244 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/admin_thumbnail_css.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      236 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/admin_thumbnail_easy-thumbnails.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)       86 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/admin_thumbnail_imagekit.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      276 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/admin_thumbnail_sorl.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      331 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/current_episode.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      249 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/episode_detail.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      313 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/episode_list.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)       31 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/podcasting_base.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      288 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/show_detail.html
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      311 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/templates/podcasting/show_list.html
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.629177 django-podcasting-1.3.3/podcasting/tests/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/tests/__init__.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/tests/models.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     4495 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/tests/tests.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      215 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/tests/urls.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      699 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/urls.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1204 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/urls_feeds.py
+drwxr-xr-x   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 03:22:32.632510 django-podcasting-1.3.3/podcasting/utils/
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)        0 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/utils/__init__.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     3044 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/utils/fields.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      290 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/utils/twitter.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1874 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/utils/widgets.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)      915 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/podcasting/views.py
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)       38 2023-06-03 03:22:32.632510 django-podcasting-1.3.3/setup.cfg
+-rw-r--r--   0 rhizom    (1000) rhizom    (1000)     1673 2023-06-03 02:51:20.000000 django-podcasting-1.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-podcasting-1.3.2/django_podcasting.egg-info/PKG-INFO` & `django-podcasting-1.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-podcasting
-Version: 1.3.2
+Version: 1.3.3
 Summary: Audio podcasting functionality for django sites.
 Home-page: http://django-podcasting.readthedocs.org/
 Author: Thomas Schreiber
 Author-email: tom@nillab.com
 License: BSD
-Description: Django Podcasting
-        =================
-        
-        Django Podcasting is a reusable application which provides audio
-        podcasting functionality for websites running on the Django Web
-        framework.
-        
-        |docs|_
-        |build|_
-        |coverage|_
-        |requires|_
-        
-        More documentation about the usage and installation of Django Podcasting
-        can be found on `django-podcasting.readthedocs.org`_.
-        
-        The source code for Django Podcasting can be found and contributed to on
-        `github.com/rizumu/django-podcasting`_. There you can also `file issues`_.
-        
-        To find out what's new in this version of django-podcasting, please see
-        `the changelog`_
-        
-        
-        Quick Installation Guide
-        ========================
-        
-        Please visit `django-podcasting.readthedocs.org`_ for the full
-        installation guide including optional thumbnailing, tagging and
-        twitter support.
-        
-        
-        * Tested against Django 1.8 and greater.
-        
-        
-        * Install Django Podcasting with your favorite Python package manager::
-        
-            pip install django-podcasting
-        
-        
-        * Add ``"podcasting"``, ``"django.contrib.sites"``,
-          and the optional apps of your choice to the ``INSTALLED_APPS`` setting
-          in your ``settings.py``::
-        
-            INSTALLED_APPS = (
-                ...
-                "django.contrib.admin",
-                "django.contrib.sites",
-                ...
-                "podcasting",
-                ...
-            )
-        
-        
-        * Include ``podcasting.urls`` and ``podcasting.urls_feeds`` in your urls definition::
-        
-            url(r"^podcasts/", include("podcasting.urls")),
-            url(r"^feeds/podcasts/", include("podcasting.urls_feeds")),
-        
-        
-        * To run the test suite::
-        
-            ./runtests.sh
-        
-        
-        .. _github.com/rizumu/django-podcasting: https://github.com/rizumu/django-podcasting/
-        .. _django-podcasting.readthedocs.org: http://django-podcasting.readthedocs.org/
-        .. _file issues: https://github.com/rizumu/django-podcasting/issues/
-        .. _in-development version: https://github.com/rizumu/django-podcasting/tarball/master#egg=django-podcasting-dev
-        .. _the changelog: http://django-podcasting.readthedocs.org/en/latest/changelog.html
-        
-        .. |build| image:: https://secure.travis-ci.org/rizumu/django-podcasting.png?branch=master
-        .. _build: http://travis-ci.org/#!/rizumu/django-podcasting
-        .. |coverage| image:: https://coveralls.io/repos/rizumu/django-podcasting/badge.png?branch=master
-        .. _coverage: https://coveralls.io/r/rizumu/django-podcasting
-        .. |requires| image:: https://requires.io/github/rizumu/django-podcasting/requirements.png?branch=master
-        .. _requires: https://requires.io/github/rizumu/django-podcasting/requirements/?branch=master
-        .. |docs| image:: https://readthedocs.org/projects/django-podcasting/badge/?version=latest
-        .. _docs: https://readthedocs.org/projects/django-podcasting/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -96,7 +17,87 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+Django Podcasting
+=================
+
+Django Podcasting is a reusable application which provides audio
+podcasting functionality for websites running on the Django Web
+framework.
+
+|docs|_
+|build|_
+|coverage|_
+|requires|_
+
+More documentation about the usage and installation of Django Podcasting
+can be found on `django-podcasting.readthedocs.org`_.
+
+The source code for Django Podcasting can be found and contributed to on
+`github.com/rizumu/django-podcasting`_. There you can also `file issues`_.
+
+To find out what's new in this version of django-podcasting, please see
+`the changelog`_
+
+
+Quick Installation Guide
+========================
+
+Please visit `django-podcasting.readthedocs.org`_ for the full
+installation guide including optional thumbnailing, tagging and
+twitter support.
+
+
+* Tested against Django 1.8 and greater.
+
+
+* Install Django Podcasting with your favorite Python package manager::
+
+    pip install django-podcasting
+
+
+* Add ``"podcasting"``, ``"django.contrib.sites"``,
+  and the optional apps of your choice to the ``INSTALLED_APPS`` setting
+  in your ``settings.py``::
+
+    INSTALLED_APPS = (
+        ...
+        "django.contrib.admin",
+        "django.contrib.sites",
+        ...
+        "podcasting",
+        ...
+    )
+
+
+* Include ``podcasting.urls`` and ``podcasting.urls_feeds`` in your urls definition::
+
+    url(r"^podcasts/", include("podcasting.urls")),
+    url(r"^feeds/podcasts/", include("podcasting.urls_feeds")),
+
+
+* To run the test suite::
+
+    ./runtests.sh
+
+
+.. _github.com/rizumu/django-podcasting: https://github.com/rizumu/django-podcasting/
+.. _django-podcasting.readthedocs.org: http://django-podcasting.readthedocs.org/
+.. _file issues: https://github.com/rizumu/django-podcasting/issues/
+.. _in-development version: https://github.com/rizumu/django-podcasting/tarball/master#egg=django-podcasting-dev
+.. _the changelog: http://django-podcasting.readthedocs.org/en/latest/changelog.html
+
+.. |build| image:: https://secure.travis-ci.org/rizumu/django-podcasting.png?branch=master
+.. _build: http://travis-ci.org/#!/rizumu/django-podcasting
+.. |coverage| image:: https://coveralls.io/repos/rizumu/django-podcasting/badge.png?branch=master
+.. _coverage: https://coveralls.io/r/rizumu/django-podcasting
+.. |requires| image:: https://requires.io/github/rizumu/django-podcasting/requirements.png?branch=master
+.. _requires: https://requires.io/github/rizumu/django-podcasting/requirements/?branch=master
+.. |docs| image:: https://readthedocs.org/projects/django-podcasting/badge/?version=latest
+.. _docs: https://readthedocs.org/projects/django-podcasting/?badge=latest
```

### Comparing `django-podcasting-1.3.2/django_podcasting.egg-info/SOURCES.txt` & `django-podcasting-1.3.3/django_podcasting.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 MANIFEST.in
 README.rst
 setup.py
 django_podcasting.egg-info/PKG-INFO
 django_podcasting.egg-info/SOURCES.txt
 django_podcasting.egg-info/dependency_links.txt
 django_podcasting.egg-info/not-zip-safe
-django_podcasting.egg-info/pbr.json
 django_podcasting.egg-info/requires.txt
 django_podcasting.egg-info/top_level.txt
 podcasting/__init__.py
 podcasting/admin.py
 podcasting/conf.py
 podcasting/feeds.py
 podcasting/forms.py
 podcasting/managers.py
 podcasting/models.py
 podcasting/urls.py
 podcasting/urls_feeds.py
 podcasting/views.py
-podcasting/locale/es/LC_MESSAGES/django.mo
-podcasting/locale/es/LC_MESSAGES/django.po
 podcasting/migrations/0001_initial.py
 podcasting/migrations/0002_auto_20140914_2220.py
 podcasting/migrations/0003_auto_20160822_2146.py
 podcasting/migrations/0004_auto_20160822_2147.py
+podcasting/migrations/0005_auto_20190617_1316.py
 podcasting/migrations/__init__.py
 podcasting/templates/podcasting/_current_episode.html
 podcasting/templates/podcasting/_episode_detail.html
 podcasting/templates/podcasting/_episode_list.html
 podcasting/templates/podcasting/_feeds.html
 podcasting/templates/podcasting/_show_detail.html
 podcasting/templates/podcasting/_show_list.html
```

### Comparing `django-podcasting-1.3.2/LICENSE` & `django-podcasting-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/PKG-INFO` & `django-podcasting-1.3.3/django_podcasting.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-podcasting
-Version: 1.3.2
+Version: 1.3.3
 Summary: Audio podcasting functionality for django sites.
 Home-page: http://django-podcasting.readthedocs.org/
 Author: Thomas Schreiber
 Author-email: tom@nillab.com
 License: BSD
-Description: Django Podcasting
-        =================
-        
-        Django Podcasting is a reusable application which provides audio
-        podcasting functionality for websites running on the Django Web
-        framework.
-        
-        |docs|_
-        |build|_
-        |coverage|_
-        |requires|_
-        
-        More documentation about the usage and installation of Django Podcasting
-        can be found on `django-podcasting.readthedocs.org`_.
-        
-        The source code for Django Podcasting can be found and contributed to on
-        `github.com/rizumu/django-podcasting`_. There you can also `file issues`_.
-        
-        To find out what's new in this version of django-podcasting, please see
-        `the changelog`_
-        
-        
-        Quick Installation Guide
-        ========================
-        
-        Please visit `django-podcasting.readthedocs.org`_ for the full
-        installation guide including optional thumbnailing, tagging and
-        twitter support.
-        
-        
-        * Tested against Django 1.8 and greater.
-        
-        
-        * Install Django Podcasting with your favorite Python package manager::
-        
-            pip install django-podcasting
-        
-        
-        * Add ``"podcasting"``, ``"django.contrib.sites"``,
-          and the optional apps of your choice to the ``INSTALLED_APPS`` setting
-          in your ``settings.py``::
-        
-            INSTALLED_APPS = (
-                ...
-                "django.contrib.admin",
-                "django.contrib.sites",
-                ...
-                "podcasting",
-                ...
-            )
-        
-        
-        * Include ``podcasting.urls`` and ``podcasting.urls_feeds`` in your urls definition::
-        
-            url(r"^podcasts/", include("podcasting.urls")),
-            url(r"^feeds/podcasts/", include("podcasting.urls_feeds")),
-        
-        
-        * To run the test suite::
-        
-            ./runtests.sh
-        
-        
-        .. _github.com/rizumu/django-podcasting: https://github.com/rizumu/django-podcasting/
-        .. _django-podcasting.readthedocs.org: http://django-podcasting.readthedocs.org/
-        .. _file issues: https://github.com/rizumu/django-podcasting/issues/
-        .. _in-development version: https://github.com/rizumu/django-podcasting/tarball/master#egg=django-podcasting-dev
-        .. _the changelog: http://django-podcasting.readthedocs.org/en/latest/changelog.html
-        
-        .. |build| image:: https://secure.travis-ci.org/rizumu/django-podcasting.png?branch=master
-        .. _build: http://travis-ci.org/#!/rizumu/django-podcasting
-        .. |coverage| image:: https://coveralls.io/repos/rizumu/django-podcasting/badge.png?branch=master
-        .. _coverage: https://coveralls.io/r/rizumu/django-podcasting
-        .. |requires| image:: https://requires.io/github/rizumu/django-podcasting/requirements.png?branch=master
-        .. _requires: https://requires.io/github/rizumu/django-podcasting/requirements/?branch=master
-        .. |docs| image:: https://readthedocs.org/projects/django-podcasting/badge/?version=latest
-        .. _docs: https://readthedocs.org/projects/django-podcasting/?badge=latest
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -96,7 +17,87 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+Django Podcasting
+=================
+
+Django Podcasting is a reusable application which provides audio
+podcasting functionality for websites running on the Django Web
+framework.
+
+|docs|_
+|build|_
+|coverage|_
+|requires|_
+
+More documentation about the usage and installation of Django Podcasting
+can be found on `django-podcasting.readthedocs.org`_.
+
+The source code for Django Podcasting can be found and contributed to on
+`github.com/rizumu/django-podcasting`_. There you can also `file issues`_.
+
+To find out what's new in this version of django-podcasting, please see
+`the changelog`_
+
+
+Quick Installation Guide
+========================
+
+Please visit `django-podcasting.readthedocs.org`_ for the full
+installation guide including optional thumbnailing, tagging and
+twitter support.
+
+
+* Tested against Django 1.8 and greater.
+
+
+* Install Django Podcasting with your favorite Python package manager::
+
+    pip install django-podcasting
+
+
+* Add ``"podcasting"``, ``"django.contrib.sites"``,
+  and the optional apps of your choice to the ``INSTALLED_APPS`` setting
+  in your ``settings.py``::
+
+    INSTALLED_APPS = (
+        ...
+        "django.contrib.admin",
+        "django.contrib.sites",
+        ...
+        "podcasting",
+        ...
+    )
+
+
+* Include ``podcasting.urls`` and ``podcasting.urls_feeds`` in your urls definition::
+
+    url(r"^podcasts/", include("podcasting.urls")),
+    url(r"^feeds/podcasts/", include("podcasting.urls_feeds")),
+
+
+* To run the test suite::
+
+    ./runtests.sh
+
+
+.. _github.com/rizumu/django-podcasting: https://github.com/rizumu/django-podcasting/
+.. _django-podcasting.readthedocs.org: http://django-podcasting.readthedocs.org/
+.. _file issues: https://github.com/rizumu/django-podcasting/issues/
+.. _in-development version: https://github.com/rizumu/django-podcasting/tarball/master#egg=django-podcasting-dev
+.. _the changelog: http://django-podcasting.readthedocs.org/en/latest/changelog.html
+
+.. |build| image:: https://secure.travis-ci.org/rizumu/django-podcasting.png?branch=master
+.. _build: http://travis-ci.org/#!/rizumu/django-podcasting
+.. |coverage| image:: https://coveralls.io/repos/rizumu/django-podcasting/badge.png?branch=master
+.. _coverage: https://coveralls.io/r/rizumu/django-podcasting
+.. |requires| image:: https://requires.io/github/rizumu/django-podcasting/requirements.png?branch=master
+.. _requires: https://requires.io/github/rizumu/django-podcasting/requirements/?branch=master
+.. |docs| image:: https://readthedocs.org/projects/django-podcasting/badge/?version=latest
+.. _docs: https://readthedocs.org/projects/django-podcasting/?badge=latest
```

### Comparing `django-podcasting-1.3.2/podcasting/__init__.py` & `django-podcasting-1.3.3/podcasting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # If you change this version, change it also in docs/conf.py
 # Packging guide: http://guide.python-distribute.org/quickstart.html
 __version_info__ = {
     "major": 1,
     "minor": 3,
-    "micro": 2,
+    "micro": 3,
     "releaselevel": "final",
     "serial": 0,
 }
 
 
 def get_version():
     vers = ["{major}.{minor}".format(**__version_info__)]
```

### Comparing `django-podcasting-1.3.2/podcasting/admin.py` & `django-podcasting-1.3.3/podcasting/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-from django.utils.translation import ugettext_lazy as _
+try:
+    from django.utils.translation import gettext_lazy as _
+except ImportError:
+    from django.utils.translation import ugettext_lazy as _
 
 from django.contrib import admin
 
 try:
     from imagekit.admin import AdminThumbnail
 except ImportError:
     AdminThumbnail = None
 
-from podcasting.forms import AdminShowForm, AdminEpisodeForm, EnclosureForm as AdminEnclosureForm
+from podcasting.forms import (
+    AdminShowForm,
+    AdminEpisodeForm,
+    EnclosureForm as AdminEnclosureForm,
+)
 from podcasting.models import Show, Episode, Enclosure, EmbedMedia
 from podcasting.utils.twitter import can_tweet
 
 
 class ShowAdmin(admin.ModelAdmin):
     form = AdminShowForm
 
@@ -22,19 +29,21 @@
         admin_thumbnail = AdminThumbnail(image_field="admin_thumb_sm")
 
     if can_tweet():
         fields.append("tweet_text")  # noqa
 
     def published_flag(self, obj):
         return bool(obj.published)
+
     published_flag.short_description = _("Published")
     published_flag.boolean = True
 
     def show_sites(self, obj):
-        return ', '.join([site.name for site in obj.sites.all()])
+        return ", ".join([site.name for site in obj.sites.all()])
+
     show_sites.short_description = "Sites"
 
 
 class EpisodeAdmin(admin.ModelAdmin):
     form = AdminEpisodeForm
 
     list_display = ["title", "episode_shows", "slug", "episode_sites", "published_flag"]
@@ -44,28 +53,31 @@
         admin_thumbnail = AdminThumbnail(image_field="admin_thumb_sm")
 
     if can_tweet():
         readonly_fields = ("tweet_text",)
 
     def published_flag(self, obj):
         return bool(obj.published)
+
     published_flag.short_description = _("Published")
     published_flag.boolean = True
 
     def episode_shows(self, obj):
-        return ', '.join([show.title for show in obj.shows.all()])
+        return ", ".join([show.title for show in obj.shows.all()])
+
     episode_shows.short_description = "Shows"
 
     def episode_sites(self, obj):
         sites = list()
         for show in obj.shows.all():
             for site in show.sites.all():
                 if site not in sites:
                     sites.append(site)
-        return ', '.join([site.name for site in sites])
+        return ", ".join([site.name for site in sites])
+
     episode_sites.short_description = "Sites"
 
     def save_form(self, request, form, change):
         # this is done for explicitness that we want form.save to commit
         # form.save doesn't take a commit kwarg for this reason
         return form.save()
```

### Comparing `django-podcasting-1.3.2/podcasting/feeds.py` & `django-podcasting-1.3.3/podcasting/feeds.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/forms.py` & `django-podcasting-1.3.3/podcasting/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,75 @@
 try:
     from django.utils.timezone import now
 except ImportError:
     from datetime.datetime import now  # noqa
 
+try:
+    from django.utils.translation import gettext_lazy as _
+except ImportError:
+    from django.utils.translation import ugettext_lazy as _
+
 from django import forms
 from django.conf import settings
-from django.utils.translation import ugettext_lazy as _
+
 from django.core.exceptions import ObjectDoesNotExist
 
 from podcasting.utils.twitter import can_tweet
 from podcasting.utils.widgets import CustomAdminThumbnailWidget
 from podcasting.models import Enclosure, Episode, Show
 
 
 class BaseShowForm(forms.ModelForm):
 
-    if 'photologue' in settings.INSTALLED_APPS:
+    if "photologue" in settings.INSTALLED_APPS:
         original_image = forms.ImageField(
             widget=CustomAdminThumbnailWidget,
-            help_text=Show._meta.get_field("original_image").help_text)
+            help_text=Show._meta.get_field("original_image").help_text,
+        )
 
     publish = forms.BooleanField(
         required=False,
-        help_text=_("Checking this will publish this show on the site, no turning back."),
+        help_text=_(
+            "Checking this will publish this show on the site, no turning back."
+        ),
     )
 
     class Meta:
         model = Show
         fields = [
             "original_image",
             "author_text",
             "owner",
             "editor_email",
             "webmaster_email",
-            "title", "subtitle", "description",
+            "title",
+            "subtitle",
+            "description",
             "twitter_tweet_prefix",
-            "feedburner", "itunes",
-            "keywords", "organization", "license",
-            "explicit", "link",
+            "feedburner",
+            "itunes",
+            "keywords",
+            "organization",
+            "license",
+            "explicit",
+            "link",
             "on_itunes",
             "publish",
         ]
         if "taggit" in settings.INSTALLED_APPS:
             fields.append("tags")
 
 
 class ShowAddForm(BaseShowForm):
-
     def clean_publish(self):
         if self.cleaned_data["publish"]:
             self.instance.published = now()
 
 
 class ShowChangeForm(BaseShowForm):
-
     def __init__(self, *args, **kwargs):
         super(ShowChangeForm, self).__init__(*args, **kwargs)
         self.fields["publish"].initial = bool(self.instance.published)
 
     def clean_publish(self):
         # clean_publish is called twice, skip the first time when instance is unset
         if not self.instance.pk:
@@ -67,38 +79,45 @@
             return
         if self.cleaned_data["publish"]:
             self.instance.published = now()
 
 
 class BaseEpisodeForm(forms.ModelForm):
 
-    if 'photologue' in settings.INSTALLED_APPS:
+    if "photologue" in settings.INSTALLED_APPS:
         original_image = forms.ImageField(
             widget=CustomAdminThumbnailWidget,
-            help_text=Episode._meta.get_field("original_image").help_text)
+            help_text=Episode._meta.get_field("original_image").help_text,
+        )
 
     publish = forms.BooleanField(
         required=False,
-        help_text=_("Checking this will publish this episode on the site, no turning back."),
+        help_text=_(
+            "Checking this will publish this episode on the site, no turning back."
+        ),
     )
 
     if can_tweet():
         tweet = forms.BooleanField(
             required=False,
-            help_text=_("Checking this will send out a tweet announcing the episode."))
+            help_text=_("Checking this will send out a tweet announcing the episode."),
+        )
 
     class Meta:
         model = Episode
         fields = [
             "original_image",
             "author_text",
-            "title", "subtitle",
+            "title",
+            "subtitle",
             "description",
             "tracklist",
-            "hours", "minutes", "seconds",
+            "hours",
+            "minutes",
+            "seconds",
             "publish",
         ]
         if "taggit" in settings.INSTALLED_APPS:
             fields.append("tags")
         extra_fields_itunes = [
             "keywords",
             "explicit",
@@ -118,25 +137,32 @@
 
         if can_tweet() and self.cleaned_data["tweet"]:
             instance.tweet()
 
         return instance
 
     def validate_published(self):
-        if not self.instance.enclosure_set.count() or not self.instance.embedmedia_set.count():
+        if (
+            not self.instance.enclosure_set.count()
+            or not self.instance.embedmedia_set.count()
+        ):
             raise forms.ValidationError(
-                _("An episode must have at least one enclosure or media file before publishing.\n "
-                  "Uncheck, save this episode, and add an encoslure before publishing."))
+                _(
+                    "An episode must have at least one enclosure or media file before publishing.\n "
+                    "Uncheck, save this episode, and add an encoslure before publishing."
+                )
+            )
         elif not self.instance.is_show_published:
-            raise forms.ValidationError(_("The show for this episode is not yet published"))
+            raise forms.ValidationError(
+                _("The show for this episode is not yet published")
+            )
         self.instance.published = now()
 
 
 class EpisodeChangeForm(BaseEpisodeForm):
-
     def __init__(self, *args, **kwargs):
         super(EpisodeChangeForm, self).__init__(*args, **kwargs)
         self.fields["publish"].initial = bool(self.instance.published)
 
     def clean_publish(self):
         # clean_publish is called twice, skip the first time when instance is unset
         if not self.instance.pk:
@@ -151,19 +177,20 @@
 class EpisodeITunesChangeForm(EpisodeChangeForm):
     def __init__(self, *args, **kwargs):
         super(EpisodeITunesChangeForm, self).__init__(*args, **kwargs)
         for key in self.Meta.required_fields_itunes:
             self.fields[key].required = True
 
     class Meta(EpisodeChangeForm.Meta):
-        fields = EpisodeChangeForm.Meta.fields + EpisodeChangeForm.Meta.extra_fields_itunes
+        fields = (
+            EpisodeChangeForm.Meta.fields + EpisodeChangeForm.Meta.extra_fields_itunes
+        )
 
 
 class EpisodeAddForm(BaseEpisodeForm):
-
     def clean_publish(self):
         if self.cleaned_data["publish"]:
             self.validate_published()
 
 
 class EpisodeITunesAddForm(EpisodeAddForm):
     def __init__(self, *args, **kwargs):
@@ -172,15 +199,14 @@
             self.fields[key].required = True
 
     class Meta(EpisodeAddForm.Meta):
         fields = EpisodeAddForm.Meta.fields + EpisodeAddForm.Meta.extra_fields_itunes
 
 
 class EnclosureForm(forms.ModelForm):
-
     class Meta:
         model = Enclosure
         fields = [
             "episodes",
             "url",
             "mime",
             "size",
@@ -188,21 +214,24 @@
             "sample",
             "channel",
             "duration",
         ]
 
     def clean(self):
         cleaned_data = super(EnclosureForm, self).clean()
-        for episode in cleaned_data.get('episodes'):
+        for episode in cleaned_data.get("episodes"):
             try:
-                episode.enclosure_set.get(mime=cleaned_data.get('mime'))
+                episode.enclosure_set.get(mime=cleaned_data.get("mime"))
                 raise forms.ValidationError(
-                    _("An episode can only have one enclosure of a specific mimetype. \n "
-                      "Episode '%(item)s' already has an enclosure of mimetype %(mimetype)s"),
-                    params={'item': episode, 'mimetype': cleaned_data.get('mime')})
+                    _(
+                        "An episode can only have one enclosure of a specific mimetype. \n "
+                        "Episode '%(item)s' already has an enclosure of mimetype %(mimetype)s"
+                    ),
+                    params={"item": episode, "mimetype": cleaned_data.get("mime")},
+                )
             except ObjectDoesNotExist:
                 pass
 
     def validate_unique(self):
         exclude = self._get_validation_exclusions()
 
         try:
@@ -212,31 +241,39 @@
 
 
 class AdminShowForm(forms.ModelForm):
 
     publish = forms.BooleanField(
         label=_("publish"),
         required=False,
-        help_text=_("Checking this will publish this show on the site, no turning back."),
+        help_text=_(
+            "Checking this will publish this show on the site, no turning back."
+        ),
     )
 
     class Meta:
         model = Show
         fields = [
             "sites",
             "original_image",
             "author_text",
             "owner",
             "editor_email",
             "webmaster_email",
-            "title", "subtitle", "description",
+            "title",
+            "subtitle",
+            "description",
             "twitter_tweet_prefix",
-            "feedburner", "itunes",
-            "keywords", "organization", "license",
-            "explicit", "link",
+            "feedburner",
+            "itunes",
+            "keywords",
+            "organization",
+            "license",
+            "explicit",
+            "link",
             "on_itunes",
             "publish",
         ]
         if "taggit" in settings.INSTALLED_APPS:
             fields.append("tags")
 
     def __init__(self, *args, **kwargs):
@@ -255,50 +292,65 @@
 
 
 class AdminEpisodeForm(forms.ModelForm):
 
     publish = forms.BooleanField(
         label=_("publish"),
         required=False,
-        help_text=_("Checking this will publish this episode on the site, no turning back."))
+        help_text=_(
+            "Checking this will publish this episode on the site, no turning back."
+        ),
+    )
 
     if can_tweet():
         tweet = forms.BooleanField(
             required=False,
-            help_text=_("Checking this will send out a tweet announcing the episode."))
+            help_text=_("Checking this will send out a tweet announcing the episode."),
+        )
 
     class Meta:
         model = Episode
         fields = [
             "shows",
             "original_image",
             "author_text",
-            "title", "subtitle",
+            "title",
+            "subtitle",
             "description",
             "tracklist",
-            "hours", "minutes", "seconds",
+            "hours",
+            "minutes",
+            "seconds",
             "publish",
             "keywords",
             "explicit",
             "block",
         ]
         if "taggit" in settings.INSTALLED_APPS:
             fields.append("tags")
 
     def __init__(self, *args, **kwargs):
         super(AdminEpisodeForm, self).__init__(*args, **kwargs)
         self.fields["publish"].initial = bool(self.instance.published)
 
     def validate_published(self):
-        if not self.instance.enclosure_set.count() and not self.instance.embedmedia_set.count():
+        if (
+            not self.instance.enclosure_set.count()
+            and not self.instance.embedmedia_set.count()
+        ):
             raise forms.ValidationError(
-                _("An episode must have at least one enclosure or media file before publishing.\n "
-                  "Uncheck, save this episode, and add an encoslure before publishing."))
+                _(
+                    "An episode must have at least one enclosure or media file before publishing.\n "
+                    "Uncheck, save this episode, and add an encoslure before publishing."
+                )
+            )
         elif not self.instance.is_show_published:
-            raise forms.ValidationError(_("The show for this episode is not yet published"))
+            raise forms.ValidationError(
+                _("The show for this episode is not yet published")
+            )
         self.instance.published = now()
 
     def clean_publish(self):
         # clean_publish is called twice, skip the first time when instance is unset
         if not self.instance.pk:
             return
         # do nothing if already published
```

### Comparing `django-podcasting-1.3.2/podcasting/managers.py` & `django-podcasting-1.3.3/podcasting/managers.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/migrations/0002_auto_20140914_2220.py` & `django-podcasting-1.3.3/podcasting/migrations/0002_auto_20140914_2220.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         migrations.AlterUniqueTogether(
             name='enclosure',
             unique_together=None,
         ),
         migrations.AlterField(
             model_name='episode',
             name='slug',
-            field=AutoSlugField(verbose_name='slug', unique=b'True', editable=False),
+            field=AutoSlugField(verbose_name='slug', unique='True', editable=False),
         ),
         migrations.AlterField(
             model_name='show',
             name='slug',
-            field=AutoSlugField(verbose_name='slug', unique=b'True', editable=False),
+            field=AutoSlugField(verbose_name='slug', unique='True', editable=False),
         ),
 
         migrations.RunPython(move_enclosure_episode),
 
         migrations.RunPython(move_show_site),
 
         migrations.RunPython(move_episode_show),
```

### Comparing `django-podcasting-1.3.2/podcasting/migrations/0003_auto_20160822_2146.py` & `django-podcasting-1.3.3/podcasting/migrations/0003_auto_20160822_2146.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/migrations/0004_auto_20160822_2147.py` & `django-podcasting-1.3.3/podcasting/migrations/0004_auto_20160822_2147.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/models.py` & `django-podcasting-1.3.3/podcasting/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 try:
     from urllib2 import urlopen
 except ImportError:
     from urllib.request import urlopen
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
+
 try:
     from django.urls import reverse
 except ImportError:
     from django.core.urlresolvers import reverse
 from django.db import models
 from django.template.defaultfilters import slugify
-from django.utils.encoding import python_2_unicode_compatible
-from django.utils.translation import ugettext_lazy as _
+
+try:
+    from django.utils.translation import gettext_lazy as _
+except ImportError:
+    from django.utils.translation import ugettext_lazy as _
 
 from django.contrib.sites.models import Site
 
 from autoslug import AutoSlugField
 
 from podcasting.managers import EpisodeQuerySet, ShowQuerySet
 from podcasting.utils.fields import UUIDField
@@ -37,40 +41,46 @@
     from imagekit.models import ImageSpecField
     from imagekit.processors import ResizeToFill
 except ImportError:
     ResizeToFill = ImageSpecField = None
 
 try:
     from easy_thumbnails.fields import ThumbnailerImageField as ImageField
+
     custom_image_field = True
 except ImportError:
     custom_image_field = False
 
 try:
     from photologue.models import Photo
+
     custom_image_field = True
 except ImportError:
     custom_image_field = False
 
 if not custom_image_field:
     try:
         from sorl.thumbnail import ImageField  # noqa
+
         custom_image_field = True
     except ImportError:
         custom_image_field = False
 
 if not custom_image_field:
     # image-kit uses the standard ImageField as well
     from django.db.models import ImageField  # noqa
 
 if "taggit" in settings.INSTALLED_APPS:
     from taggit.managers import TaggableManager
 else:
+
     def TaggableManager(blank=True):  # noqa
         return None
+
+
 try:
     import twitter
 except ImportError:
     twitter = None  # noqa
 
 try:
     from embed_video.fields import EmbedVideoField
@@ -87,421 +97,594 @@
 
 
 def get_episode_upload_folder(instance, pathname):
     "A standardized pathname for uploaded files and images."
     root, ext = os.path.splitext(pathname)
     if instance.shows.count() == 1:
         return "{0}/podcasts/{1}/episodes/{2}{3}".format(
-            settings.PODCASTING_IMG_PATH, instance.shows.all()[0].slug, slugify(root), ext
+            settings.PODCASTING_IMG_PATH,
+            instance.shows.all()[0].slug,
+            slugify(root),
+            ext,
         )
     else:
         return "{0}/podcasts/episodes/{1}/{2}{3}".format(
             settings.PODCASTING_IMG_PATH, instance.slug, slugify(root), ext
         )
 
 
-@python_2_unicode_compatible
 class Show(models.Model):
     """
     A podcast show, which has many episodes.
     """
+
     EXPLICIT_CHOICES = (
         (1, _("yes")),
         (2, _("no")),
         (3, _("clean")),
     )
     uuid = UUIDField(_("id"), unique=True)
 
     created = models.DateTimeField(_("created"), auto_now_add=True, editable=False)
     updated = models.DateTimeField(_("updated"), auto_now=True, editable=False)
-    published = models.DateTimeField(_("published"), null=True, blank=True, editable=False)
+    published = models.DateTimeField(
+        _("published"), null=True, blank=True, editable=False
+    )
 
-    sites = models.ManyToManyField(Site, verbose_name=_('Sites'))
+    sites = models.ManyToManyField(Site, verbose_name=_("Sites"))
 
     ttl = models.PositiveIntegerField(
-        _("ttl"), default=1440,
-        help_text=_("""``Time to Live,`` the number of minutes a channel can be
-        cached before refreshing."""))
+        _("ttl"),
+        default=1440,
+        help_text=_(
+            """``Time to Live,`` the number of minutes a channel can be
+        cached before refreshing."""
+        ),
+    )
 
     owner = models.ForeignKey(
-        settings.AUTH_USER_MODEL, related_name="podcast_shows",
+        settings.AUTH_USER_MODEL,
+        related_name="podcast_shows",
         verbose_name=_("owner"),
-        help_text=_("""Make certain the user account has a name and e-mail address."""))
+        on_delete=models.PROTECT,
+        help_text=_("""Make certain the user account has a name and e-mail address."""),
+    )
 
     editor_email = models.EmailField(
-        _("editor email"), blank=True,
-        help_text=_("Email address of the person responsible for the feed's content."))
+        _("editor email"),
+        blank=True,
+        help_text=_("Email address of the person responsible for the feed's content."),
+    )
     webmaster_email = models.EmailField(
-        _("webmaster email"), blank=True,
-        help_text=_("Email address of the person responsible for channel publishing."))
+        _("webmaster email"),
+        blank=True,
+        help_text=_("Email address of the person responsible for channel publishing."),
+    )
 
-    if 'licenses' in settings.INSTALLED_APPS:
+    if "licenses" in settings.INSTALLED_APPS:
         license = models.ForeignKey(License, verbose_name=_("license"))
     else:
         license = models.CharField(
-            _("license"), max_length=255,
-            help_text=_("To publish a podcast to iTunes it is required to set a license type."))
+            _("license"),
+            max_length=255,
+            help_text=_(
+                "To publish a podcast to iTunes it is required to set a license type."
+            ),
+        )
 
     organization = models.CharField(
-        _("organization"), max_length=255,
-        help_text=_("Name of the organization, company or Web site producing the podcast."))
-    link = models.URLField(_("link"), help_text=_("""URL of either the main website or the
-        podcast section of the main website."""))
+        _("organization"),
+        max_length=255,
+        help_text=_(
+            "Name of the organization, company or Web site producing the podcast."
+        ),
+    )
+    link = models.URLField(
+        _("link"),
+        help_text=_(
+            """URL of either the main website or the
+        podcast section of the main website."""
+        ),
+    )
 
     enable_comments = models.BooleanField(default=True)
 
     author_text = models.CharField(
-        _("author text"), max_length=255, help_text=_("""
+        _("author text"),
+        max_length=255,
+        help_text=_(
+            """
             This tag contains the name of the person or company that is most
             widely attributed to publishing the Podcast and will be
             displayed immediately underneath the title of the Podcast.
             The suggested format is: 'email@example.com (Full Name)'
             but 'Full Name' only, is acceptable. Multiple authors
-            should be comma separated."""))
+            should be comma separated."""
+        ),
+    )
 
     title = models.CharField(_("title"), max_length=255)
     slug = AutoSlugField(_("slug"), populate_from="title", unique="True")
 
     subtitle = models.CharField(
-        _("subtitle"), max_length=255,
-        help_text=_("Looks best if only a few words, like a tagline."))
+        _("subtitle"),
+        max_length=255,
+        help_text=_("Looks best if only a few words, like a tagline."),
+    )
 
     # If the show is not on iTunes, many fields may be ignored in your user forms
     on_itunes = models.BooleanField(
-        _("iTunes"), default=True,
-        help_text=_("Checked if the podcast is submitted to iTunes"))
+        _("iTunes"),
+        default=True,
+        help_text=_("Checked if the podcast is submitted to iTunes"),
+    )
 
     description_pretty = models.TextField(
-        _("pretty description"), blank=True,
-        help_text="May be longer than 4000 characters and contain HTML tags and styling.")
+        _("pretty description"),
+        blank=True,
+        help_text="May be longer than 4000 characters and contain HTML tags and styling.",
+    )
 
     description = models.TextField(
-        _("description"), max_length=4000, help_text=_("""
+        _("description"),
+        max_length=4000,
+        help_text=_(
+            """
             This is your chance to tell potential subscribers all about your
             podcast. Describe your subject matter, media format,
             episode schedule, and other relevant info so that they
             know what they'll be getting when they subscribe. In
             addition, make a list of the most relevant search terms
             that you want yourp podcast to match, then build them into
             your description. Note that iTunes removes podcasts that
             include lists of irrelevant words in the itunes:summary,
             description, or itunes:keywords tags. This field can be up
-            to 4000 characters."""))
+            to 4000 characters."""
+        ),
+    )
 
-    if 'photologue' in settings.INSTALLED_APPS:
-        original_image = models.ForeignKey(Photo, verbose_name=_("image"), default=None, null=True, blank=True, help_text=_("""
+    if "photologue" in settings.INSTALLED_APPS:
+        original_image = models.ForeignKey(
+            Photo,
+            verbose_name=_("image"),
+            default=None,
+            null=True,
+            blank=True,
+            on_delete=models.SET_NULL,
+            help_text=_(
+                """
                 A podcast must have 1400 x 1400 pixel cover art in JPG or PNG
                 format using RGB color space. See our technical spec for
                 details. To be eligible for featuring on iTunes Stores,
                 choose an attractive, original, and square JPEG (.jpg) or
                 PNG (.png) image at a size of 1400x1400 pixels. The image
                 will be scaled down to 50x50 pixels at smallest in iTunes.
                 For reference see the <a
                 href="http://www.apple.com/itunes/podcasts/specs.html#metadata">iTunes
                 Podcast specs</a>.<br /><br /> For episode artwork to
                 display in iTunes, image must be <a
                 href="http://answers.yahoo.com/question/index?qid=20080501164348AAjvBvQ">
                 saved to file's <strong>metadata</strong></a> before
-                enclosure uploading!"""))
+                enclosure uploading!"""
+            ),
+        )
     else:
         original_image = ImageField(
-            _("image"), upload_to=get_show_upload_folder, blank=True, help_text=_("""
+            _("image"),
+            upload_to=get_show_upload_folder,
+            blank=True,
+            help_text=_(
+                """
                 A podcast must have 1400 x 1400 pixel cover art in JPG or PNG
                 format using RGB color space. See our technical spec for
                 details. To be eligible for featuring on iTunes Stores,
                 choose an attractive, original, and square JPEG (.jpg) or
                 PNG (.png) image at a size of 1400x1400 pixels. The image
                 will be scaled down to 50x50 pixels at smallest in iTunes.
                 For reference see the <a
                 href="http://www.apple.com/itunes/podcasts/specs.html#metadata">iTunes
                 Podcast specs</a>.<br /><br /> For episode artwork to
                 display in iTunes, image must be <a
                 href="http://answers.yahoo.com/question/index?qid=20080501164348AAjvBvQ">
                 saved to file's <strong>metadata</strong></a> before
-                enclosure uploading!"""))
+                enclosure uploading!"""
+            ),
+        )
 
     if ResizeToFill:
-        admin_thumb_sm = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(50, 50)],
-                                        options={"quality": 100})
-        admin_thumb_lg = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(450, 450)],
-                                        options={"quality": 100})
-        img_show_sm = ImageSpecField(source="original_image",
-                                     processors=[ResizeToFill(120, 120)],
-                                     options={"quality": 100})
-        img_show_lg = ImageSpecField(source="original_image",
-                                     processors=[ResizeToFill(550, 550)],
-                                     options={"quality": 100})
-        img_itunes_sm = ImageSpecField(source="original_image",
-                                       processors=[ResizeToFill(144, 144)],
-                                       options={"quality": 100})
-        img_itunes_lg = ImageSpecField(source="original_image",
-                                       processors=[ResizeToFill(1400, 1400)],
-                                       options={"quality": 100})
+        admin_thumb_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(50, 50)],
+            options={"quality": 100},
+        )
+        admin_thumb_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(450, 450)],
+            options={"quality": 100},
+        )
+        img_show_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(120, 120)],
+            options={"quality": 100},
+        )
+        img_show_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(550, 550)],
+            options={"quality": 100},
+        )
+        img_itunes_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(144, 144)],
+            options={"quality": 100},
+        )
+        img_itunes_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(1400, 1400)],
+            options={"quality": 100},
+        )
 
     feedburner = models.URLField(
-        _("feedburner url"), blank=True,
-        help_text=_("""Fill this out after saving this show and at least one
+        _("feedburner url"),
+        blank=True,
+        help_text=_(
+            """Fill this out after saving this show and at least one
             episode. URL should look like "http://feeds.feedburner.com/TitleOfShow".
             See <a href="http://code.google.com/p/django-podcast/">documentation</a>
-            for more. <a href="http://www.feedburner.com/fb/a/ping">Manually ping</a>"""))
+            for more. <a href="http://www.feedburner.com/fb/a/ping">Manually ping</a>"""
+        ),
+    )
 
     # iTunes specific fields
     explicit = models.PositiveSmallIntegerField(
-        _("explicit"), default=1, choices=EXPLICIT_CHOICES,
-        help_text=_("``Clean`` will put the clean iTunes graphic by it."))
+        _("explicit"),
+        default=1,
+        choices=EXPLICIT_CHOICES,
+        help_text=_("``Clean`` will put the clean iTunes graphic by it."),
+    )
     redirect = models.URLField(
-        _("redirect"), blank=True,
-        help_text=_("""The show's new URL feed if changing
+        _("redirect"),
+        blank=True,
+        help_text=_(
+            """The show's new URL feed if changing
             the URL of the current show feed. Must continue old feed for at least
-            two weeks and write a 301 redirect for old feed."""))
+            two weeks and write a 301 redirect for old feed."""
+        ),
+    )
     keywords = models.CharField(
-        _("keywords"), max_length=255, blank=True,
-        help_text=_("""A comma-demlimitedlist of up to 12 words for iTunes
-            searches. Perhaps include misspellings of the title."""))
+        _("keywords"),
+        max_length=255,
+        blank=True,
+        help_text=_(
+            """A comma-demlimitedlist of up to 12 words for iTunes
+            searches. Perhaps include misspellings of the title."""
+        ),
+    )
     itunes = models.URLField(
-        _("itunes store url"), blank=True,
-        help_text=_("""Fill this out after saving this show and at least one
+        _("itunes store url"),
+        blank=True,
+        help_text=_(
+            """Fill this out after saving this show and at least one
             episode. URL should look like:
             "http://phobos.apple.com/WebObjects/MZStore.woa/wa/viewPodcast?id=000000000".
-            See <a href="http://code.google.com/p/django-podcast/">documentation</a> for more."""))
+            See <a href="http://code.google.com/p/django-podcast/">documentation</a> for more."""
+        ),
+    )
 
     twitter_tweet_prefix = models.CharField(
-        _("Twitter tweet prefix"), max_length=80,
-        help_text=_("Enter a short ``tweet_text`` prefix for new episodes on this show."),
-        blank=True)
+        _("Twitter tweet prefix"),
+        max_length=80,
+        help_text=_(
+            "Enter a short ``tweet_text`` prefix for new episodes on this show."
+        ),
+        blank=True,
+    )
 
     objects = ShowQuerySet.as_manager()
     tags = TaggableManager(blank=True)
 
     class Meta:
         verbose_name = _("Show")
         verbose_name_plural = _("Shows")
         ordering = ("organization", "slug")
 
     def __str__(self):
         return self.title
 
     def get_share_url(self):
-        return "http://{0}{1}".format(Site.objects.get_current(), self.get_absolute_url())
+        return "http://{0}{1}".format(
+            Site.objects.get_current(), self.get_absolute_url()
+        )
 
     def get_absolute_url(self):
         return reverse("podcasting_show_detail", kwargs={"slug": self.slug})
 
     @property
     def current_episode(self):
         try:
             return self.episode_set.published().order_by("-published")[0]
         except IndexError:
             return None
 
 
-@python_2_unicode_compatible
 class Episode(models.Model):
     """
     An individual podcast episode and it's unique attributes.
     """
+
     SIXTY_CHOICES = tuple((x, x) for x in range(60))
     uuid = UUIDField("ID", unique=True)
 
     created = models.DateTimeField(_("created"), auto_now_add=True, editable=False)
     updated = models.DateTimeField(_("updated"), auto_now=True, editable=False)
-    published = models.DateTimeField(_("published"), null=True, blank=True, editable=False)
+    published = models.DateTimeField(
+        _("published"), null=True, blank=True, editable=False
+    )
 
     shows = models.ManyToManyField(Show, verbose_name=_("Podcasts"))
 
     enable_comments = models.BooleanField(default=True)
 
-    author_text = models.CharField(_("author text"), max_length=255, blank=True, help_text=_("""
+    author_text = models.CharField(
+        _("author text"),
+        max_length=255,
+        blank=True,
+        help_text=_(
+            """
         The person or musician name(s) featured on this specific episode.
         The suggested format is: 'email@example.com (Full Name)' but 'Full Name' only,
-        is acceptable. Multiple authors should be comma separated."""))
+        is acceptable. Multiple authors should be comma separated."""
+        ),
+    )
 
     title = models.CharField(_("title"), max_length=255)
     slug = AutoSlugField(_("slug"), populate_from="title", unique="True")
 
     subtitle = models.CharField(
-        _("subtitle"), max_length=255, blank=True,
-        help_text=_("Looks best if only a few words like a tagline."))
+        _("subtitle"),
+        max_length=255,
+        blank=True,
+        help_text=_("Looks best if only a few words like a tagline."),
+    )
 
     description_pretty = models.TextField(
-        _("pretty description"), blank=True,
-        help_text="May be longer than 4000 characters and contain HTML tags and styling.")
+        _("pretty description"),
+        blank=True,
+        help_text="May be longer than 4000 characters and contain HTML tags and styling.",
+    )
 
     description = models.TextField(
-        _("description"), max_length=4000, blank=True, help_text=_("""
+        _("description"),
+        max_length=4000,
+        blank=True,
+        help_text=_(
+            """
             This is your chance to tell potential subscribers all about your podcast.
             Describe your subject matter, media format, episode schedule, and other
             relevant info so that they know what they'll be getting when they
             subscribe. In addition, make a list of the most relevant search terms
             that you want your podcast to match, then build them into your
             description. Note that iTunes removes podcasts that include lists of
             irrelevant words in the itunes:summary, description, or
             itunes:keywords tags. This field can be up to 4000 plain text characters.
-            No HTML tags or styling allowed."""))
+            No HTML tags or styling allowed."""
+        ),
+    )
 
     tracklist = models.TextField(
-        _("tracklist"), blank=True,
-        help_text=_("""One track per line, machine will automatically add the numbers."""))
+        _("tracklist"),
+        blank=True,
+        help_text=_(
+            """One track per line, machine will automatically add the numbers."""
+        ),
+    )
 
     tweet_text = models.CharField(_("tweet text"), max_length=140, editable=False)
 
-    if 'photologue' in settings.INSTALLED_APPS:
-        original_image = models.ForeignKey(Photo, verbose_name=_("image"), default=None, null=True, blank=True, help_text=_("""
+    if "photologue" in settings.INSTALLED_APPS:
+        original_image = models.ForeignKey(
+            Photo,
+            verbose_name=_("image"),
+            default=None,
+            null=True,
+            blank=True,
+            on_delete=models.PROTECT,
+            help_text=_(
+                """
                 A podcast must have 1400 x 1400 pixel cover art in JPG or PNG
                 format using RGB color space. See our technical spec for
                 details. To be eligible for featuring on iTunes Stores,
                 choose an attractive, original, and square JPEG (.jpg) or
                 PNG (.png) image at a size of 1400x1400 pixels. The image
                 will be scaled down to 50x50 pixels at smallest in iTunes.
                 For reference see the <a
                 href="http://www.apple.com/itunes/podcasts/specs.html#metadata">iTunes
                 Podcast specs</a>.<br /><br /> For episode artwork to
                 display in iTunes, image must be <a
                 href="http://answers.yahoo.com/question/index?qid=20080501164348AAjvBvQ">
                 saved to file's <strong>metadata</strong></a> before
-                enclosure uploading!"""))
+                enclosure uploading!"""
+            ),
+        )
     else:
         original_image = ImageField(
-            _("image"), upload_to=get_episode_upload_folder, blank=True, help_text=_("""
+            _("image"),
+            upload_to=get_episode_upload_folder,
+            blank=True,
+            help_text=_(
+                """
                 A podcast must have 1400 x 1400 pixel cover art in JPG or PNG
                 format using RGB color space. See our technical spec for
                 details. To be eligible for featuring on iTunes Stores,
                 choose an attractive, original, and square JPEG (.jpg) or
                 PNG (.png) image at a size of 1400x1400 pixels. The image
                 will be scaled down to 50x50 pixels at smallest in iTunes.
                 For reference see the <a
                 href="http://www.apple.com/itunes/podcasts/specs.html#metadata">iTunes
                 Podcast specs</a>.<br /><br /> For episode artwork to
                 display in iTunes, image must be <a
                 href="http://answers.yahoo.com/question/index?qid=20080501164348AAjvBvQ">
                 saved to file's <strong>metadata</strong></a> before
-                enclosure uploading!"""))
+                enclosure uploading!"""
+            ),
+        )
 
     if ImageSpecField:
-        admin_thumb_sm = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(50, 50)],
-                                        options={"quality": 100})
-        admin_thumb_lg = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(450, 450)],
-                                        options={"quality": 100})
-        img_episode_sm = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(120, 120)],
-                                        options={"quality": 100})
-        img_episode_lg = ImageSpecField(source="original_image",
-                                        processors=[ResizeToFill(550, 550)],
-                                        options={"quality": 100})
-        img_itunes_sm = ImageSpecField(source="original_image",
-                                       processors=[ResizeToFill(144, 144)],
-                                       options={"quality": 100})
-        img_itunes_lg = ImageSpecField(source="original_image",
-                                       processors=[ResizeToFill(1400, 1400)],
-                                       options={"quality": 100})
+        admin_thumb_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(50, 50)],
+            options={"quality": 100},
+        )
+        admin_thumb_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(450, 450)],
+            options={"quality": 100},
+        )
+        img_episode_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(120, 120)],
+            options={"quality": 100},
+        )
+        img_episode_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(550, 550)],
+            options={"quality": 100},
+        )
+        img_itunes_sm = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(144, 144)],
+            options={"quality": 100},
+        )
+        img_itunes_lg = ImageSpecField(
+            source="original_image",
+            processors=[ResizeToFill(1400, 1400)],
+            options={"quality": 100},
+        )
 
     # iTunes specific fields
     hours = models.SmallIntegerField(_("hours"), default=0)
     minutes = models.SmallIntegerField(_("minutes"), default=0, choices=SIXTY_CHOICES)
     seconds = models.SmallIntegerField(_("seconds"), default=0, choices=SIXTY_CHOICES)
     keywords = models.CharField(
-        _("keywords"), max_length=255, blank=True,
-        help_text=_("A comma-delimited list of words for searches, up to 12; "
-                    "perhaps include misspellings."))
+        _("keywords"),
+        max_length=255,
+        blank=True,
+        help_text=_(
+            "A comma-delimited list of words for searches, up to 12; "
+            "perhaps include misspellings."
+        ),
+    )
     explicit = models.PositiveSmallIntegerField(
-        _("explicit"), choices=Show.EXPLICIT_CHOICES,
-        help_text=_("``Clean`` will put the clean iTunes graphic by it."), default=1)
+        _("explicit"),
+        choices=Show.EXPLICIT_CHOICES,
+        help_text=_("``Clean`` will put the clean iTunes graphic by it."),
+        default=1,
+    )
     block = models.BooleanField(
-        _("block"), default=False,
-        help_text=_("Check to block this episode from iTunes because <br />its "
-                    "content might cause the entire show to be <br />removed from iTunes."""))
+        _("block"),
+        default=False,
+        help_text=_(
+            "Check to block this episode from iTunes because <br />its "
+            "content might cause the entire show to be <br />removed from iTunes."
+            ""
+        ),
+    )
 
     objects = EpisodeQuerySet.as_manager()
     tags = TaggableManager(blank=True)
 
     class Meta:
         verbose_name = _("Episode")
         verbose_name_plural = _("Episodes")
         ordering = ("-published", "slug")
 
     def __str__(self):
         return self.title
 
     def get_absolute_url(self):
-        return reverse("podcasting_episode_detail",
-                       kwargs={"show_slug": self.shows.all()[0].slug, "slug": self.slug})
+        return reverse(
+            "podcasting_episode_detail",
+            kwargs={"show_slug": self.shows.all()[0].slug, "slug": self.slug},
+        )
 
     def get_next(self):
         next = self.__class__.objects.filter(published__gt=self.published)
         try:
             return next[0]
         except IndexError:
             return False
 
     def get_prev(self):
-        prev = self.__class__.objects.filter(published__lt=self.published).order_by("-published")
+        prev = self.__class__.objects.filter(published__lt=self.published).order_by(
+            "-published"
+        )
         try:
             return prev[0]
         except IndexError:
             return False
 
     def as_tweet(self):
         if not self.tweet_text:
             current_site = Site.objects.get_current()
             api_url = "http://api.tr.im/api/trim_url.json"
-            u = urlopen("{0}?url=http://{1}{2}".format(
-                api_url,
-                current_site.domain,
-                self.get_absolute_url(),
-            ))
+            u = urlopen(
+                "{0}?url=http://{1}{2}".format(
+                    api_url,
+                    current_site.domain,
+                    self.get_absolute_url(),
+                )
+            )
             result = json.loads(u.read())
             self.tweet_text = "{0} {1} - {2}".format(
                 self.shows.all()[0].episode_twitter_tweet_prefix,
                 self.title,
                 result["url"],
             )
         return self.tweet_text
 
     def tweet(self):
         if can_tweet():
             account = twitter.Api(
-                username=settings.TWITTER_USERNAME,
-                password=settings.TWITTER_PASSWORD)
+                username=settings.TWITTER_USERNAME, password=settings.TWITTER_PASSWORD
+            )
             account.PostUpdate(self.as_tweet())
         else:
             raise ImproperlyConfigured(
                 "Unable to send tweet due to either "
-                "missing python-twitter or required settings.")
+                "missing python-twitter or required settings."
+            )
 
     def seconds_total(self):
         try:
             return self.minutes * 60 + self.seconds
         except:
             return 0
 
     def get_share_url(self):
-        return "http://{0}{1}".format(Site.objects.get_current(), self.get_absolute_url())
+        return "http://{0}{1}".format(
+            Site.objects.get_current(), self.get_absolute_url()
+        )
 
     def get_share_title(self):
         return self.title
 
     def get_share_description(self):
         return "{0}...".format(self.description[:512])
 
     def is_show_published(self):
         for show in self.shows.all():
             if show.published:
                 return True
         return False
 
 
-@python_2_unicode_compatible
 class Enclosure(models.Model):
     """
     An enclosure is one, of possibly many, files/filetypes of an episode.
     """
+
     try:
         MIME_CHOICES = settings.PODCASTING_MIME_CHOICES
     except AttributeError:
         MIME_CHOICES = (
             ("aiff", "audio/aiff"),
             ("flac", "audio/flac"),
             ("mp3", "audio/mpeg"),
@@ -511,64 +694,92 @@
             ("wav", "audio/wav"),
         )
 
     episodes = models.ManyToManyField(Episode, verbose_name=_("Episodes"))
 
     url = models.URLField(
         _("url"),
-        help_text=_("""URL of the media file. <br /> It is <strong>very</strong>
+        help_text=_(
+            """URL of the media file. <br /> It is <strong>very</strong>
             important to remember that for episode artwork to display in iTunes, image must be
             <a href="http://answers.yahoo.com/question/index?qid=20080501164348AAjvBvQ">
             saved to file's <strong>metadata</strong></a> before enclosure uploading!<br /><br />
             For best results, choose an attractive, original, and square JPEG (.jpg) or PNG (.png)
             image at a size of 1400x1400 pixels. The image will be
-            scaled down to 50x50 pixels at smallest in iTunes."""))
+            scaled down to 50x50 pixels at smallest in iTunes."""
+        ),
+    )
 
     size = models.PositiveIntegerField(
-        _("size"), help_text=_("The length attribute is the file size in bytes. "
-                               "Find this information in the files properties "
-                               "(on a Mac, ``Get Info`` and refer to the size row)"))
+        _("size"),
+        help_text=_(
+            "The length attribute is the file size in bytes. "
+            "Find this information in the files properties "
+            "(on a Mac, ``Get Info`` and refer to the size row)"
+        ),
+    )
     mime = models.CharField(
-        _("mime format"), max_length=4, choices=MIME_CHOICES,
-        help_text=_("Supports mime types of: {0}".format(
-            ", ".join([mime[0] for mime in MIME_CHOICES]))))
+        _("mime format"),
+        max_length=4,
+        choices=MIME_CHOICES,
+        help_text=_(
+            "Supports mime types of: {0}".format(
+                ", ".join([mime[0] for mime in MIME_CHOICES])
+            )
+        ),
+    )
     bitrate = models.CharField(
-        _("bit rate"), max_length=5, default="192",
-        help_text=_("Measured in kilobits per second (kbps), often 128 or 192."))
+        _("bit rate"),
+        max_length=5,
+        default="192",
+        help_text=_("Measured in kilobits per second (kbps), often 128 or 192."),
+    )
     sample = models.CharField(
-        _("sample rate"), max_length=5, default="44.1",
-        help_text=_("Measured in kilohertz (kHz), often 44.1."))
+        _("sample rate"),
+        max_length=5,
+        default="44.1",
+        help_text=_("Measured in kilohertz (kHz), often 44.1."),
+    )
     channel = models.CharField(
-        _("channel"), max_length=1, default=2,
-        help_text=_("Number of channels; 2 for stereo, 1 for mono."))
+        _("channel"),
+        max_length=1,
+        default=2,
+        help_text=_("Number of channels; 2 for stereo, 1 for mono."),
+    )
     duration = models.IntegerField(
         _("duration"),
-        help_text=_("Duration of the audio file, in seconds (always as integer)."))
+        help_text=_("Duration of the audio file, in seconds (always as integer)."),
+    )
 
     class Meta:
-        ordering = ("url", "mime",)
+        ordering = (
+            "url",
+            "mime",
+        )
         verbose_name = _("Enclosure")
         verbose_name_plural = _("Enclosures")
 
     def __str__(self):
         return "{0} - {1}".format(self.url, self.mime)
 
 
-@python_2_unicode_compatible
 class EmbedMedia(models.Model):
     """
     Associate a media URL to an Episode.
 
     This is *not* a replacement for a video podcast, but simply a way
     to embed content via url in an episode description.
 
     Ideally this will be used with django-embed-video which supports
     easy embeding for YouTube and Vimeo videos and music from SoundCloud.
     """
-    episode = models.ForeignKey(Episode, verbose_name=_("episode"))
+
+    episode = models.ForeignKey(
+        Episode, verbose_name=_("episode"), on_delete=models.PROTECT
+    )
 
     if EmbedVideoField:
         url = EmbedVideoField(_("url"), help_text=_("URL of the media file"))
     else:
         url = models.URLField(_("url"), help_text=_("URL of the media file"))
 
     class Meta:
```

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_current_episode.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_current_episode.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_episode_detail.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_episode_detail.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_episode_list.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_episode_list.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_feeds.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_feeds.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_show_detail.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_show_detail.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/templates/podcasting/_show_list.html` & `django-podcasting-1.3.3/podcasting/templates/podcasting/_show_list.html`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/tests/tests.py` & `django-podcasting-1.3.3/podcasting/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/urls.py` & `django-podcasting-1.3.3/podcasting/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,29 @@
-from django.conf.urls import url
-from podcasting.views import ShowListView, ShowDetailView, EpisodeListView, EpisodeDetailView
+try:
+    from django.urls import re_path as url
+except ImportError:
+    from django.conf.urls import url
+
+from podcasting.views import (
+    ShowListView,
+    ShowDetailView,
+    EpisodeListView,
+    EpisodeDetailView,
+)
 
 
 urlpatterns = [
-    url(r"^$", ShowListView.as_view(),
-        name="podcasting_show_list"),
-    url(r"^(?P<slug>[-\w]+)/$", ShowDetailView.as_view(),
-        name="podcasting_show_detail"),
-    url(r"^(?P<show_slug>[-\w]+)/archive/$", EpisodeListView.as_view(),
-        name="podcasting_episode_list"),
-    url(r"^(?P<show_slug>[-\w]+)/(?P<slug>[-\w]+)/$", EpisodeDetailView.as_view(),
-        name="podcasting_episode_detail"),
+    url(r"^$", ShowListView.as_view(), name="podcasting_show_list"),
+    url(
+        r"^(?P<slug>[-\w]+)/$", ShowDetailView.as_view(), name="podcasting_show_detail"
+    ),
+    url(
+        r"^(?P<show_slug>[-\w]+)/archive/$",
+        EpisodeListView.as_view(),
+        name="podcasting_episode_list",
+    ),
+    url(
+        r"^(?P<show_slug>[-\w]+)/(?P<slug>[-\w]+)/$",
+        EpisodeDetailView.as_view(),
+        name="podcasting_episode_detail",
+    ),
 ]
```

### Comparing `django-podcasting-1.3.2/podcasting/urls_feeds.py` & `django-podcasting-1.3.3/podcasting/urls_feeds.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from django.conf.urls import url
+try:
+    from django.urls import re_path as url
+except ImportError:
+    from django.conf.urls import url
 
 from podcasting.feeds import (
-    RssShowFeed, AtomShowFeed, AtomRedirectView, RssRedirectView)
+    RssShowFeed,
+    AtomShowFeed,
+    AtomRedirectView,
+    RssRedirectView,
+)
 from podcasting.models import Enclosure
 
 
 MIMES = "|".join([enclosure[0] for enclosure in Enclosure.MIME_CHOICES])
 
 
 urlpatterns = [
     # Episode list feed by show (RSS 2.0 and iTunes)
-    url(r"^(?P<show_slug>[-\w]+)/(?P<mime_type>{mimes})/rss/$".format(mimes=MIMES),
-        RssShowFeed(), name="podcasts_show_feed_rss"),
-
+    url(
+        r"^(?P<show_slug>[-\w]+)/(?P<mime_type>{mimes})/rss/$".format(mimes=MIMES),
+        RssShowFeed(),
+        name="podcasts_show_feed_rss",
+    ),
     # Episode list feed by show (Atom)
-    url(r"^(?P<show_slug>[-\w]+)/(?P<mime_type>{mimes})/atom/$".format(mimes=MIMES),
-        AtomShowFeed(), name="podcasts_show_feed_atom"),
-
+    url(
+        r"^(?P<show_slug>[-\w]+)/(?P<mime_type>{mimes})/atom/$".format(mimes=MIMES),
+        AtomShowFeed(),
+        name="podcasts_show_feed_atom",
+    ),
     # Episode list feed by show (Media RSS)
     # TODO upon request
-
     # Previously we had /itunes/ in the feed url.
     # This is now deprecated and redirects to a more general feed url.
-    url(r"^(?P<show_slug>[-\w]+)/itunes/(?P<mime_type>[-\w]+)/rss/$",
-        RssRedirectView.as_view()),
-    url(r"^(?P<show_slug>[-\w]+)/itunes/(?P<mime_type>[-\w]+)/atom/$",
-        AtomRedirectView.as_view()),
+    url(
+        r"^(?P<show_slug>[-\w]+)/itunes/(?P<mime_type>[-\w]+)/rss/$",
+        RssRedirectView.as_view(),
+    ),
+    url(
+        r"^(?P<show_slug>[-\w]+)/itunes/(?P<mime_type>[-\w]+)/atom/$",
+        AtomRedirectView.as_view(),
+    ),
 ]
```

### Comparing `django-podcasting-1.3.2/podcasting/utils/fields.py` & `django-podcasting-1.3.3/podcasting/utils/fields.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/utils/widgets.py` & `django-podcasting-1.3.3/podcasting/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/podcasting/views.py` & `django-podcasting-1.3.3/podcasting/views.py`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/README.rst` & `django-podcasting-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-podcasting-1.3.2/setup.py` & `django-podcasting-1.3.3/setup.py`

 * *Files identical despite different names*

