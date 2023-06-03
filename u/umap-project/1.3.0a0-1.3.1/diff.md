# Comparing `tmp/umap-project-1.3.0a0.tar.gz` & `tmp/umap-project-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umap-project-1.3.0a0.tar", last modified: Wed May 31 07:43:08 2023, max compression
+gzip compressed data, was "umap-project-1.3.1.tar", last modified: Sat Jun  3 06:30:23 2023, max compression
```

## Comparing `umap-project-1.3.0a0.tar` & `umap-project-1.3.1.tar`

### file list

```diff
@@ -1,535 +1,535 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/LICENSE
--rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2167 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1184 2019-02-22 20:49:23.000000 umap-project-1.3.0a0/README.md
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1395 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/setup.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.531023 umap-project-1.3.0a0/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/admin.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/apps.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.3.0a0/umap/autocomplete.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/bin/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/bin/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/context_processors.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/decorators.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/fields.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2740 2023-05-23 17:05:44.000000 umap-project-1.3.0a0/umap/forms.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/am_ET/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6577 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11035 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ar/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4038 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9743 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ast/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/bg/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7132 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11584 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/ca/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.534356 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7185 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10694 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/cs_CZ/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7364 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10996 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.514356 umap-project-1.3.0a0/umap/locale/da/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6995 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10627 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/de/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7335 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11063 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/el/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10115 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13827 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/en/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7443 2023-05-31 07:12:10.000000 umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/es/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.537689 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7292 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11100 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/et/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6136 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9983 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fa_IR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8955 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12488 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5792 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10408 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/fr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7399 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11327 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/gl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.541023 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7160 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10751 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/he/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11518 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/hr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1777 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8477 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/hu/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7561 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11122 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/id/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/is/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7603 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11110 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.517689 umap-project-1.3.0a0/umap/locale/it/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.544356 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7309 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11188 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ja/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7672 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11240 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ko/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7625 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11132 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/lt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6845 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10659 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ms/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7577 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10506 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/nl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.547689 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6999 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10549 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/no/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7298 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10828 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt_BR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10908 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/pt_PT/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7271 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10843 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ro/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.551023 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/ru/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9228 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12926 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/si_LK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sk_SK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6891 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10730 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6825 2023-05-31 07:14:25.000000 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10538 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8830 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12352 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/sv/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.554356 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6975 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10508 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.521023 umap-project-1.3.0a0/umap/locale/th_TH/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10318 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13772 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/tr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7375 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10952 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/uk_UA/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9429 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12970 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/vi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6064 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10544 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/zh/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.557690 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.524356 umap-project-1.3.0a0/umap/locale/zh_TW/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10562 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/management/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/management/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/management/commands/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.0a0/umap/management/commands/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      839 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/management/commands/anonymous_edit_url.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.3.0a0/umap/management/commands/generate_js_locale.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.3.0a0/umap/management/commands/import_pictograms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/managers.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/middleware.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.561023 umap-project-1.3.0a0/umap/migrations/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0001_initial.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0002_tilelayer_tms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0003_add_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/migrations/0004_add_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.3.0a0/umap/migrations/0005_remove_map_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.3.0a0/umap/migrations/0006_auto_20190407_0719.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/migrations/0007_auto_20190416_1757.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-05-23 16:48:43.000000 umap-project-1.3.0a0/umap/migrations/0008_alter_map_settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/migrations/0009_star.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.3.0a0/umap/migrations/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11456 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/models.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.564356 umap-project-1.3.0a0/umap/settings/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/settings/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7642 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/settings/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.3.0a0/umap/settings/dev.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.564356 umap-project-1.3.0a0/umap/static/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/.gitignore
--rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/favicon.ico
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.574356 umap-project-1.3.0a0/umap/static/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18104 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/base.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/bitbucket.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5858 2023-05-30 06:46:59.000000 umap-project-1.3.0a0/umap/static/umap/content.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.577690 umap-project-1.3.0a0/umap/static/umap/font/
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff2
--rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/font.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/github.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.584356 umap-project-1.3.0a0/umap/static/umap/img/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/static/umap/img/16-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/static/umap/img/16-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/16.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19711 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38377 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16878 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    36478 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/24.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/edit-16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      554 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/edit.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/icon-bg.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      327 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/logo.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/img/logo_filigree.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/marker.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      473 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/opensource.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1997 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/img/osm.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/img/search.gif
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.587690 umap-project-1.3.0a0/umap/static/umap/js/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7937 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.autocomplete.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38967 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19966 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.core.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31642 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.features.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27320 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.forms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5762 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.icon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    68708 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33580 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.layer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5809 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.popup.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4421 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.slideshow.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4191 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.tableeditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6872 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.ui.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8711 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/static/umap/js/umap.xhr.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.607690 umap-project-1.3.0a0/umap/static/umap/locale/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27485 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/am_ET.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27414 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/am_ET.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23264 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ar.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23199 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/ar.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ast.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/ast.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26550 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/bg.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26485 2023-05-31 07:14:01.000000 umap-project-1.3.0a0/umap/static/umap/locale/bg.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23646 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ca.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23581 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/ca.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24628 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24557 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23232 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/da.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23167 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/da.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24743 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/de.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24678 2023-05-31 07:14:03.000000 umap-project-1.3.0a0/umap/static/umap/locale/de.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33701 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/el.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33636 2023-05-31 07:14:02.000000 umap-project-1.3.0a0/umap/static/umap/locale/el.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/en.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22732 2023-05-31 07:12:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/en.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22442 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/en_US.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24956 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/es.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24891 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/es.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23050 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/et.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22985 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/et.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30194 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30123 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23862 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23797 2023-05-31 07:14:04.000000 umap-project-1.3.0a0/umap/static/umap/locale/fi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24960 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/fr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24895 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/fr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24456 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/gl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24391 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/gl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26905 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/he.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26840 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/he.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23005 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/hr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22940 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/hr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25810 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/hu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25745 2023-05-31 07:14:05.000000 umap-project-1.3.0a0/umap/static/umap/locale/hu.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22795 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/id.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/id.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24377 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/is.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24312 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/is.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24474 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/it.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24409 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/it.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25895 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ja.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25830 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/ja.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23023 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ko.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22958 2023-05-31 07:14:06.000000 umap-project-1.3.0a0/umap/static/umap/locale/ko.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23762 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/lt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23697 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/lt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23906 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23841 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/ms.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24414 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/nl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24349 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/nl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/no.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/no.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24276 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24211 2023-05-31 07:14:08.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pl_PL.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24433 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24368 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24422 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24351 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24432 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24361 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22856 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ro.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22791 2023-05-31 07:14:09.000000 umap-project-1.3.0a0/umap/static/umap/locale/ro.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31470 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/ru.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31405 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/ru.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/si_LK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/si_LK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24310 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24239 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24157 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24092 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27557 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27492 2023-05-31 07:14:10.000000 umap-project-1.3.0a0/umap/static/umap/locale/sr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24031 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/sv.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23966 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/sv.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/th_TH.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/th_TH.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24649 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/tr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24584 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/tr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31037 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30966 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23174 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23109 2023-05-31 07:14:12.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/vi_VN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22421 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22356 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_CN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.Big5.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22410 2023-05-31 07:43:07.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22339 2023-05-31 07:14:13.000000 umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31816 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/map.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/nav.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/openstreetmap.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.617690 umap-project-1.3.0a0/umap/static/umap/test/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/static/umap/test/.eslintrc
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1665 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11544 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/DataLayer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9423 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Feature.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16802 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Map.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3318 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Marker.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2314 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/Permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12614 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/test/Polygon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13986 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/static/umap/test/Polyline.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3216 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/TableEditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14080 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/test/Util.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9840 2023-05-30 15:52:32.000000 umap-project-1.3.0a0/umap/static/umap/test/_pre.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5318 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/static/umap/test/index.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.3.0a0/umap/static/umap/theme.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/static/umap/twitter.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.527689 umap-project-1.3.0a0/umap/static/umap/vendors/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/csv2geojson.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/index.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    62738 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/purify.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/editable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editable/Leaflet.Editable.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editable/Path.Drag.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.621023 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3340 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/edit-in-osm.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/fullscreen.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/hash/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/hash/leaflet-hash.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/heat/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/heat/leaflet-heat.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.624357 umap-project-1.3.0a0/umap/static/umap/vendors/i18n/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/i18n/Leaflet.i18n.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-shadow.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/loading/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-05-31 07:42:57.000000 umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-05-31 07:42:57.000000 umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.631023 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-05-31 07:42:54.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-05-31 07:42:55.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-05-31 07:42:56.000000 umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.svg
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.634357 umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/photon/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/photon/leaflet.photon.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/print/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/togeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/togpx/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/togpx/togpx.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.637690 umap-project-1.3.0a0/umap/static/umap/vendors/tokml/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/tokml/tokml.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-05-31 07:42:58.000000 umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templates/404.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templates/500.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/auth/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/auth/user_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      487 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/templates/auth/user_stars.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/base.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.641023 umap-project-1.3.0a0/umap/templates/registration/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.3.0a0/umap/templates/registration/login.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/templates/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/about.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1897 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/about_summary.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2857 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/content.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/content_footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1309 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/templates/umap/css.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      631 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/home.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3155 2023-05-30 19:49:34.000000 umap-project-1.3.0a0/umap/templates/umap/js.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2023-05-30 19:46:43.000000 umap-project-1.3.0a0/umap/templates/umap/locale.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      629 2023-05-30 06:46:59.000000 umap-project-1.3.0a0/umap/templates/umap/login_popup_end.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.3.0a0/umap/templates/umap/map_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/map_fragment.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/map_init.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/map_list.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/map_messages.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1125 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/templates/umap/navigation.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/password_change.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/password_change_done.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templates/umap/search.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.3.0a0/umap/templates/umap/search_bar.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/templates/umap/success.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/templatetags/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.0a0/umap/templatetags/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/templatetags/umap_tags.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.647690 umap-project-1.3.0a0/umap/tests/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/tests/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/conftest.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      360 2023-05-05 17:42:43.000000 umap-project-1.3.0a0/umap/tests/settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.3.0a0/umap/tests/test_datalayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7173 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_datalayer_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/test_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.3.0a0/umap/tests/test_map.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    20902 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_map_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.3.0a0/umap/tests/test_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      407 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/tests/test_utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5822 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/tests/test_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5304 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/urls.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-05-30 13:55:57.000000 umap-project-1.3.0a0/umap/utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    28421 2023-05-31 07:12:01.000000 umap-project-1.3.0a0/umap/views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.3.0a0/umap/wsgi.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-31 07:43:08.651023 umap-project-1.3.0a0/umap_project.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2167 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14363 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      263 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-05-31 07:43:08.000000 umap-project-1.3.0a0/umap_project.egg-info/top_level.txt
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.275781 umap-project-1.3.1/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.3.1/LICENSE
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.3.1/MANIFEST.in
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2003 2023-06-03 06:30:23.275781 umap-project-1.3.1/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1022 2023-06-02 15:29:26.000000 umap-project-1.3.1/README.md
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1389 2023-06-03 06:30:23.275781 umap-project-1.3.1/setup.cfg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-23 16:48:43.000000 umap-project-1.3.1/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.112443 umap-project-1.3.1/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-23 16:48:43.000000 umap-project-1.3.1/umap/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-06-02 15:27:32.000000 umap-project-1.3.1/umap/admin.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-06-02 15:27:32.000000 umap-project-1.3.1/umap/apps.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.3.1/umap/autocomplete.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.112443 umap-project-1.3.1/umap/bin/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.3.1/umap/bin/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/context_processors.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/decorators.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-06-02 15:27:32.000000 umap-project-1.3.1/umap/fields.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2731 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/forms.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/am_ET/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.112443 umap-project-1.3.1/umap/locale/am_ET/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6577 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11035 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/am_ET/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/ar/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.112443 umap-project-1.3.1/umap/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4038 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9743 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/ast/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.112443 umap-project-1.3.1/umap/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/ast/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/bg/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7132 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11584 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/ca/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7185 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10694 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/cs_CZ/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7364 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10996 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/da/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/da/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6995 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10627 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/de/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7335 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11063 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.065775 umap-project-1.3.1/umap/locale/el/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/el/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10115 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13827 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/en/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/en/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-06-03 06:28:05.000000 umap-project-1.3.1/umap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7443 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/es/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.115777 umap-project-1.3.1/umap/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7292 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11100 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/et/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.119110 umap-project-1.3.1/umap/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6136 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9983 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/fa_IR/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.119110 umap-project-1.3.1/umap/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8955 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12488 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/fa_IR/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/fi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.119110 umap-project-1.3.1/umap/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5792 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10408 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/fr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.119110 umap-project-1.3.1/umap/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7904 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11039 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/gl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.125777 umap-project-1.3.1/umap/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7160 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10751 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/he/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.125777 umap-project-1.3.1/umap/locale/he/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11518 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.069109 umap-project-1.3.1/umap/locale/hr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.125777 umap-project-1.3.1/umap/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1777 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8477 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/hu/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7561 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11122 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/id/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/is/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/is/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7603 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11110 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/it/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7309 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11188 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/ja/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7672 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11240 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.072442 umap-project-1.3.1/umap/locale/ko/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.129110 umap-project-1.3.1/umap/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7625 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11132 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/lt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6845 2023-06-03 06:28:05.000000 umap-project-1.3.1/umap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10659 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/ms/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7577 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/ms/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10506 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/nl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6999 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10549 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/no/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/no/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/pl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7298 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/pt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.132444 umap-project-1.3.1/umap/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10828 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/pt_BR/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.135777 umap-project-1.3.1/umap/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10908 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/pt_PT/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.135777 umap-project-1.3.1/umap/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7271 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10843 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/ro/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.135777 umap-project-1.3.1/umap/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/ru/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.135777 umap-project-1.3.1/umap/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9228 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12926 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/si_LK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.135777 umap-project-1.3.1/umap/locale/si_LK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/si_LK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/si_LK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/sk_SK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.139111 umap-project-1.3.1/umap/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6891 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10730 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.075776 umap-project-1.3.1/umap/locale/sl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.139111 umap-project-1.3.1/umap/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6825 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10538 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.079109 umap-project-1.3.1/umap/locale/sr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.142444 umap-project-1.3.1/umap/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8830 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12352 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.079109 umap-project-1.3.1/umap/locale/sv/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.142444 umap-project-1.3.1/umap/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6975 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10508 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/th_TH/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.142444 umap-project-1.3.1/umap/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10318 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13772 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/tr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.142444 umap-project-1.3.1/umap/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7375 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10952 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/uk_UA/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.142444 umap-project-1.3.1/umap/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9429 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12970 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/uk_UA/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/vi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.145778 umap-project-1.3.1/umap/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6064 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10544 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/zh/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.145778 umap-project-1.3.1/umap/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.082442 umap-project-1.3.1/umap/locale/zh_TW/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.152444 umap-project-1.3.1/umap/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-06-03 06:28:05.000000 umap-project-1.3.1/umap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10562 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.155778 umap-project-1.3.1/umap/management/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.1/umap/management/__init__.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.155778 umap-project-1.3.1/umap/management/commands/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.1/umap/management/commands/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      786 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/management/commands/anonymous_edit_url.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.3.1/umap/management/commands/generate_js_locale.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.3.1/umap/management/commands/import_pictograms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/managers.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/middleware.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.159111 umap-project-1.3.1/umap/migrations/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/migrations/0001_initial.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/migrations/0002_tilelayer_tms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/migrations/0003_add_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/migrations/0004_add_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.3.1/umap/migrations/0005_remove_map_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.3.1/umap/migrations/0006_auto_20190407_0719.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/migrations/0007_auto_20190416_1757.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/migrations/0008_alter_map_settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/migrations/0009_star.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.3.1/umap/migrations/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11496 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/models.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.162445 umap-project-1.3.1/umap/settings/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/settings/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7726 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/settings/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.3.1/umap/settings/dev.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.162445 umap-project-1.3.1/umap/static/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/.gitignore
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/favicon.ico
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.165778 umap-project-1.3.1/umap/static/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18168 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/static/umap/base.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/umap/bitbucket.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5858 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/content.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.169112 umap-project-1.3.1/umap/static/umap/font/
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-Light.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-Light.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-LightItalic.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-LightItalic.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-SemiBold.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.3.1/umap/static/umap/font/FiraSans-SemiBold.woff2
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/font.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/umap/github.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.175778 umap-project-1.3.1/umap/static/umap/img/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/static/umap/img/16-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/static/umap/img/16-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/16.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19711 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/img/24-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38377 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/img/24-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16878 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/img/24.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    36478 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/img/24.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/edit-16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      554 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/static/umap/img/edit.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/icon-bg.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      327 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/static/umap/img/logo.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/umap/img/logo_filigree.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/marker.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      473 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/static/umap/img/opensource.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1997 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/static/umap/img/osm.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/img/search.gif
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.182445 umap-project-1.3.1/umap/static/umap/js/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7937 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.autocomplete.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38965 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19966 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.core.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31642 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.features.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27320 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.forms.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5762 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.icon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    70995 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/static/umap/js/umap.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33580 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.layer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5809 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.popup.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4421 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.slideshow.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4191 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.tableeditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7099 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/static/umap/js/umap.ui.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8711 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/js/umap.xhr.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.222446 umap-project-1.3.1/umap/static/umap/locale/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27485 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/am_ET.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27414 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/am_ET.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23264 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ar.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23199 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ar.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ast.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ast.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26550 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/bg.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26485 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/bg.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23646 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ca.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23581 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ca.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24628 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/cs_CZ.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24557 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/cs_CZ.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23232 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/da.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23167 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/da.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24743 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/de.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24678 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/de.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33701 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/el.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33636 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/el.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22797 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/en.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22732 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/en.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22442 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/en_US.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24956 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/es.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24891 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/es.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23050 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/et.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22985 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/et.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30194 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/fa_IR.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30123 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/fa_IR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23862 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/fi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23797 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/fi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24960 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/fr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24895 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/fr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24456 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/gl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24391 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/gl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26905 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/he.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26840 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/he.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23005 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/hr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22940 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/hr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25810 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/hu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25745 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/hu.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22795 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/id.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/id.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24377 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/is.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24312 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/is.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24474 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/it.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24409 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/it.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25895 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ja.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25830 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ja.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23023 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ko.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22958 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ko.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23762 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/lt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23697 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/lt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23906 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ms.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23841 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ms.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24414 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/nl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24349 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/nl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/no.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/no.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24276 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/pl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24211 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/pl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/pl_PL.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24433 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/pt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24368 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/pt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24422 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/pt_BR.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24351 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/pt_BR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24432 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/pt_PT.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24361 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/pt_PT.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22856 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ro.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22791 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ro.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31470 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/ru.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31405 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/ru.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/si_LK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/si_LK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24310 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/sk_SK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24239 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/sk_SK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24157 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/sl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24092 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/sl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27557 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/sr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27492 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/sr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24031 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/sv.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23966 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/sv.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22801 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/th_TH.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/th_TH.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24649 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/tr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24584 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/tr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31037 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/uk_UA.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30966 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/uk_UA.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23174 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/vi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23109 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/vi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/vi_VN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22421 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/zh.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22356 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/zh.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/zh_CN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22730 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/zh_TW.Big5.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22410 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap/static/umap/locale/zh_TW.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22339 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/locale/zh_TW.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31986 2023-06-02 19:23:59.000000 umap-project-1.3.1/umap/static/umap/map.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/nav.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/umap/openstreetmap.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.225780 umap-project-1.3.1/umap/static/umap/test/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/static/umap/test/.eslintrc
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1665 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11544 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/DataLayer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9423 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Feature.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16802 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Map.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3318 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Marker.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2314 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12614 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Polygon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13986 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Polyline.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3216 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/TableEditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14080 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/Util.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9840 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/_pre.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5318 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/static/umap/test/index.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.3.1/umap/static/umap/theme.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/static/umap/twitter.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.089109 umap-project-1.3.1/umap/static/umap/vendors/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/contextmenu/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/csv2geojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/csv2geojson/csv2geojson.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/csv2geojson/index.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/dompurify/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    62738 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/dompurify/purify.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/editable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/editable/Leaflet.Editable.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/editable/Path.Drag.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/editinosm/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3340 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/editinosm/edit-in-osm.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.229113 umap-project-1.3.1/umap/static/umap/vendors/formbuilder/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.232447 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/fullscreen.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.232447 umap-project-1.3.1/umap/static/umap/vendors/georsstogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.232447 umap-project-1.3.1/umap/static/umap/vendors/hash/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/hash/leaflet-hash.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.232447 umap-project-1.3.1/umap/static/umap/vendors/heat/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/heat/leaflet-heat.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.232447 umap-project-1.3.1/umap/static/umap/vendors/i18n/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/i18n/Leaflet.i18n.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.249114 umap-project-1.3.1/umap/static/umap/vendors/leaflet/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.249114 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/layers-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/layers.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-icon.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-shadow.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.252447 umap-project-1.3.1/umap/static/umap/vendors/loading/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/loading/Control.Loading.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/loading/Control.Loading.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.255781 umap-project-1.3.1/umap/static/umap/vendors/locatecontrol/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/markercluster/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/MarkerCluster.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/measurable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/minimap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/minimap/Control.MiniMap.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/minimap/Control.MiniMap.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/minimap/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/minimap/images/toggle.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/minimap/images/toggle.svg
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/osmtogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.259114 umap-project-1.3.1/umap/static/umap/vendors/photon/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/photon/leaflet.photon.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/static/umap/vendors/print/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.3.1/umap/static/umap/vendors/print/leaflet.browser.print.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.3.1/umap/static/umap/vendors/print/leaflet.browser.print.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/static/umap/vendors/togeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/togeojson/togeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/static/umap/vendors/togpx/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/togpx/togpx.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/static/umap/vendors/tokml/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/tokml/tokml.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/static/umap/vendors/toolbar/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-05-31 08:36:21.000000 umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.262447 umap-project-1.3.1/umap/templates/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/templates/404.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/templates/500.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.265781 umap-project-1.3.1/umap/templates/auth/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/templates/auth/user_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      487 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/auth/user_stars.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/templates/base.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.265781 umap-project-1.3.1/umap/templates/registration/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.3.1/umap/templates/registration/login.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.269114 umap-project-1.3.1/umap/templates/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.3.1/umap/templates/umap/about.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1897 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/about_summary.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2857 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/content.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/templates/umap/content_footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1309 2023-05-30 13:55:57.000000 umap-project-1.3.1/umap/templates/umap/css.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.3.1/umap/templates/umap/footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      631 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/home.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3155 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/js.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/locale.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      629 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/login_popup_end.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.3.1/umap/templates/umap/map_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/templates/umap/map_fragment.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/templates/umap/map_init.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/templates/umap/map_list.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/templates/umap/map_messages.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1125 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/templates/umap/navigation.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.3.1/umap/templates/umap/password_change.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.3.1/umap/templates/umap/password_change_done.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/templates/umap/search.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.3.1/umap/templates/umap/search_bar.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/templates/umap/success.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.269114 umap-project-1.3.1/umap/templatetags/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.1/umap/templatetags/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/templatetags/umap_tags.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.275781 umap-project-1.3.1/umap/tests/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/tests/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.3.1/umap/tests/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-06-02 15:29:26.000000 umap-project-1.3.1/umap/tests/conftest.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      453 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/tests/settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.3.1/umap/tests/test_datalayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7173 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/tests/test_datalayer_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/tests/test_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.3.1/umap/tests/test_map.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21807 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/tests/test_map_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.3.1/umap/tests/test_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      407 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/tests/test_utils.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6177 2023-06-02 20:44:30.000000 umap-project-1.3.1/umap/tests/test_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5538 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/urls.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-06-02 15:27:33.000000 umap-project-1.3.1/umap/utils.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    29216 2023-06-02 21:34:48.000000 umap-project-1.3.1/umap/views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.3.1/umap/wsgi.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-03 06:30:23.275781 umap-project-1.3.1/umap_project.egg-info/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2003 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14363 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/entry_points.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      263 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/requires.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-06-03 06:30:22.000000 umap-project-1.3.1/umap_project.egg-info/top_level.txt
```

### Comparing `umap-project-1.3.0a0/PKG-INFO` & `umap-project-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.3.0a0
+Version: 1.3.1
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
 Author: Yohan Boniface
 Keywords: django leaflet geodjango openstreetmap map
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -28,13 +28,13 @@
 [![Requirements Status](https://requires.io/github/umap-project/umap/requirements.svg?branch=master)](https://requires.io/github/umap-project/umap/requirements/?branch=master)
 [![Join the chat at https://gitter.im/umap-project/umap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/umap-project/umap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Documentation Status](https://readthedocs.org/projects/umap-project/badge/?version=latest)](http://umap-project.readthedocs.io/en/latest/?badge=latest)[![Build Status](https://travis-ci.org/umap-project/umap.svg?branch=master)](https://travis-ci.org/umap-project/umap)
 
 ## About
 
 uMap lets you create maps with OpenStreetMap layers in a minute and embed them in your site.
 *Because we think that the more OSM will be used, the more OSM will be improved.*
-It uses [django-leaflet-storage](https://github.com/umap-project/django-leaflet-storage) and [Leaflet.Storage](https://github.com/umap-project/Leaflet.Storage),  built on top of Django and Leaflet.
+Built on top of Django and Leaflet.
 
 
 ## Installation and configuration
 
 See [developer documentation](https://umap-project.readthedocs.io/en/latest/install/).
```

### Comparing `umap-project-1.3.0a0/README.md` & `umap-project-1.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 [![Requirements Status](https://requires.io/github/umap-project/umap/requirements.svg?branch=master)](https://requires.io/github/umap-project/umap/requirements/?branch=master)
 [![Join the chat at https://gitter.im/umap-project/umap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/umap-project/umap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Documentation Status](https://readthedocs.org/projects/umap-project/badge/?version=latest)](http://umap-project.readthedocs.io/en/latest/?badge=latest)[![Build Status](https://travis-ci.org/umap-project/umap.svg?branch=master)](https://travis-ci.org/umap-project/umap)
 
 ## About
 
 uMap lets you create maps with OpenStreetMap layers in a minute and embed them in your site.
 *Because we think that the more OSM will be used, the more OSM will be improved.*
-It uses [django-leaflet-storage](https://github.com/umap-project/django-leaflet-storage) and [Leaflet.Storage](https://github.com/umap-project/Leaflet.Storage),  built on top of Django and Leaflet.
+Built on top of Django and Leaflet.
 
 
 ## Installation and configuration
 
 See [developer documentation](https://umap-project.readthedocs.io/en/latest/install/).
```

### Comparing `umap-project-1.3.0a0/setup.cfg` & `umap-project-1.3.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = umap-project
-version = 1.3.0.alpha
+version = 1.3.1
 description = Create maps with OpenStreetMap layers in a minute and embed them in your site.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Yohan Boniface
 homepage = https://github.com/umap-project/umap
 keywords = django leaflet geodjango openstreetmap map
 classifiers =
```

### Comparing `umap-project-1.3.0a0/umap/admin.py` & `umap-project-1.3.1/umap/admin.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/autocomplete.py` & `umap-project-1.3.1/umap/autocomplete.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/decorators.py` & `umap-project-1.3.1/umap/decorators.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/fields.py` & `umap-project-1.3.1/umap/fields.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/forms.py` & `umap-project-1.3.1/umap/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,30 @@
 
     def flat(self):
         if not self:
             return u''
         return u' — '.join([e for e in self])
 
 
+class SendLinkForm(forms.Form):
+    email = forms.EmailField()
+
+
 class UpdateMapPermissionsForm(forms.ModelForm):
 
     class Meta:
         model = Map
         fields = ('edit_status', 'editors', 'share_status', 'owner')
 
 
 class AnonymousMapPermissionsForm(forms.ModelForm):
 
     def __init__(self, *args, **kwargs):
         super(AnonymousMapPermissionsForm, self).__init__(*args, **kwargs)
-        full_secret_link = "%s%s" % (settings.SITE_URL, self.instance.get_anonymous_edit_url())
-        help_text = _('Secret edit link is %s') % full_secret_link
+        help_text = _('Secret edit link is %s') % self.instance.get_anonymous_edit_url()
         self.fields['edit_status'].help_text = _(help_text)
 
     STATUS = (
         (Map.ANONYMOUS, _('Everyone can edit')),
         (Map.OWNER, _('Only editable with secret edit link'))
     )
```

### Comparing `umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/am_ET/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/am_ET/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ar/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ast/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/bg/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ca/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/cs_CZ/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/da/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/de/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/el/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/en/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/es/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/et/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/fa_IR/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/fi/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/fr/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,29 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: yohanboniface <yohanboniface@free.fr>, 2014,2016\n"
+"Last-Translator: yohanboniface <yohanboniface@free.fr>, "
+"2013-2014,2018-2019,2023\n"
 "Language-Team: French (http://app.transifex.com/openstreetmap/umap/language/"
 "fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "%(current_user)s has no maps."
 msgstr "%(current_user)s n'a aucune carte."
 
+msgid "%(current_user)s has no starred maps yet."
+msgstr "%(current_user)s n'a aucune carte favorite."
+
 msgid "About"
 msgstr "À propos"
 
 msgid "Add POIs: markers, lines, polygons..."
 msgstr "Ajouter des points d'intérêt : marqueurs, lignes, polygones..."
 
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
@@ -27,14 +31,17 @@
 
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
 msgstr "Import des données géographiques en masse (geojson, gpx, kml, osm...)"
 
 msgid "Browse %(current_user)s's maps"
 msgstr "Consulter les cartes de %(current_user)s"
 
+msgid "Browse %(current_user)s's starred maps"
+msgstr "Consulter les cartes favorites de %(current_user)s"
+
 msgid "Change my password"
 msgstr "Changer de mot de passe"
 
 msgid "Change password"
 msgstr "Changer le mot de passe"
 
 msgid "Choose the layers of your map"
@@ -176,18 +183,28 @@
 
 msgid "Sign in"
 msgstr "Créer un compte"
 
 msgid "Site is readonly for maintenance"
 msgstr "Le site est en lecture seule pour maintenance."
 
+msgid "Starred maps"
+msgstr "Favoris"
+
 msgid "Take me to the home page"
 msgstr "Retour à la page d'accueil"
 
 msgid ""
+"This instance of uMap is currently in read only mode, no creation/edit is "
+"allowed."
+msgstr ""
+"uMap est actuelle en mode lecture seule, aucune création ou modification "
+"n'est possible."
+
+msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
 msgstr ""
 "Il s'agit d'un site de démonstration, utilisé pour les tests et validation "
 "avant diffusion. Si vous avez besoin d'une version stable, utilisez plutôt "
```

### Comparing `umap-project-1.3.0a0/umap/locale/fr/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/pt/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,391 +1,378 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Antonin Del Fabbro, 2023
-# bagage <gautier.pelloux@gmail.com>, 2021
-# Buggi, 2013
-# Buggi, 2013
-# Buggi, 2013
-# Philippe Verdy, 2017
-# severin.menard <severin.menard@protonmail.com>, 2014
-# severin.menard <severin.menard@protonmail.com>, 2014
-# severin.menard <severin.menard@protonmail.com>, 2014
-# spf, 2019
-# spf, 2019
-# Philippe Verdy, 2017
-# yohanboniface <yohanboniface@free.fr>, 2013-2014,2018-2019,2023
-# YOHAN BONIFACE <yb@enix.org>, 2012
-# yohanboniface <yohanboniface@free.fr>, 2014,2016
+# Joao Ponce de Leao Paulouro <joao.ponceleao@gmail.com>, 2014
+# Rui <xymarior@yandex.com>, 2016,2018-2019
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-21 20:50+0000\n"
+"POT-Creation-Date: 2023-02-27 12:54+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: yohanboniface <yohanboniface@free.fr>, 2014,2016\n"
-"Language-Team: French (http://app.transifex.com/openstreetmap/umap/language/fr/)\n"
+"Last-Translator: Rui <xymarior@yandex.com>, 2016,2018-2019\n"
+"Language-Team: Portuguese (http://www.transifex.com/openstreetmap/umap/language/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
+"Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: tmp/framacarte/templates/umap/home.html:8 umap/templates/umap/home.html:9
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Il s'agit d'un site de démonstration, utilisé pour les tests et validation avant diffusion. Si vous avez besoin d'une version stable, utilisez plutôt <a href=\"%(stable_url)s\">%(stable_url)s</a>. Vous pouvez aussi mettre en place votre propre version, c'est <a href=\"%(repo_url)s\">open source</a>!"
+msgstr "Esta é uma versão de demonstração, utilizada para testes e pré-lançamentos. Se precisar de uma versão estável, por favor utilize <a href=\"%(stable_url)s\">%(stable_url)s</a>. Pode também alojar a sua própria instância, e é em <a href=\"%(repo_url)s\">código aberto</a>!"
 
 #: tmp/framacarte/templates/umap/home.html:83
 #: tmp/framacarte/templates/umap/navigation.html:14
 #: umap/templates/umap/about_summary.html:33
 #: umap/templates/umap/navigation.html:26
 msgid "Create a map"
-msgstr "Créer une carte"
+msgstr "Criar um mapa"
 
 #: tmp/framacarte/templates/umap/navigation.html:7
 #: umap/templates/umap/navigation.html:10
 msgid "My maps"
-msgstr "Mes cartes"
+msgstr "Os meus mapas"
 
 #: tmp/framacarte/templates/umap/navigation.html:9
 #: umap/templates/umap/navigation.html:12
 msgid "Log in"
-msgstr "Connexion"
+msgstr "Entrar"
 
 #: tmp/framacarte/templates/umap/navigation.html:9
 #: umap/templates/umap/navigation.html:12
 msgid "Sign in"
-msgstr "Créer un compte"
+msgstr "Criar conta"
 
 #: tmp/framacarte/templates/umap/navigation.html:12
 #: umap/templates/umap/navigation.html:20
 msgid "Log out"
-msgstr "Déconnexion"
+msgstr "Sair"
 
 #: tmp/framacarte/templates/umap/search_bar.html:6
 #: umap/templates/umap/search_bar.html:6
 msgid "Search maps"
-msgstr "Chercher des cartes"
+msgstr "Procurar mapas"
 
 #: tmp/framacarte/templates/umap/search_bar.html:10
 #: tmp/framacarte/templates/umap/search_bar.html:13
 #: umap/templates/umap/search_bar.html:9
 msgid "Search"
-msgstr "Chercher"
+msgstr "Procurar"
 
 #: umap/forms.py:40
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Lien de modification secret : %s"
+msgstr "Link secreto para edição é %s"
 
 #: umap/forms.py:44 umap/models.py:114
 msgid "Everyone can edit"
-msgstr "Tout le monde peut modifier"
+msgstr "Todos podem editar"
 
 #: umap/forms.py:45
 msgid "Only editable with secret edit link"
-msgstr "Modifiable seulement avec le lien de modification secret"
+msgstr "Unicamente editável através de link secreto"
 
 #: umap/middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr "Le site est en lecture seule pour maintenance."
+msgstr "O site está em modo de leitura para manutenção"
 
 #: umap/models.py:16
 msgid "name"
-msgstr "nom"
+msgstr "nome"
 
 #: umap/models.py:47
 msgid "details"
-msgstr "détails"
+msgstr "detalhes"
 
 #: umap/models.py:48
 msgid "Link to a page where the licence is detailed."
-msgstr "Lien vers une page détaillant la licence."
+msgstr "Link para uma página detalhando a licença."
 
 #: umap/models.py:62
 msgid "URL template using OSM tile format"
-msgstr "Modèle d'URL au format des tuiles OSM"
+msgstr "Modelo de URL no formato de telas OSM"
 
 #: umap/models.py:70
 msgid "Order of the tilelayers in the edit box"
-msgstr "Ordre des calques de tuiles dans le panneau de modification"
+msgstr "Ordem das camadas na caixa de edição"
 
 #: umap/models.py:115
 msgid "Only editors can edit"
-msgstr "Seuls les éditeurs peuvent modifier"
+msgstr "Só editores podem editar"
 
 #: umap/models.py:116
 msgid "Only owner can edit"
-msgstr "Seul le créateur peut modifier"
+msgstr "Só o proprietário pode editar"
 
 #: umap/models.py:119
 msgid "everyone (public)"
-msgstr "tout le monde (public)"
+msgstr "todos (público)"
 
 #: umap/models.py:120
 msgid "anyone with link"
-msgstr "quiconque a le lien"
+msgstr "qualquer um com o link"
 
 #: umap/models.py:121
 msgid "editors only"
-msgstr "seulement les modificateurs"
+msgstr "só editores"
 
 #: umap/models.py:122
 msgid "blocked"
-msgstr "Bloquée"
+msgstr "bloqueado"
 
 #: umap/models.py:125 umap/models.py:255
 msgid "description"
-msgstr "description"
+msgstr "descrição"
 
 #: umap/models.py:126
 msgid "center"
-msgstr "centre"
+msgstr "centro"
 
 #: umap/models.py:127
 msgid "zoom"
 msgstr "zoom"
 
 #: umap/models.py:128
 msgid "locate"
-msgstr "géolocaliser"
+msgstr "localizar"
 
 #: umap/models.py:128
 msgid "Locate user on load?"
-msgstr "Géolocaliser l'utilisateur au chargement ?"
+msgstr "Localizar utilizador no início?"
 
 #: umap/models.py:131
 msgid "Choose the map licence."
-msgstr "Choisir une licence pour la carte"
+msgstr "Escolha uma licença para o mapa."
 
 #: umap/models.py:132
 msgid "licence"
-msgstr "licence"
+msgstr "licença"
 
 #: umap/models.py:137
 msgid "owner"
-msgstr "créateur"
+msgstr "proprietário"
 
 #: umap/models.py:138
 msgid "editors"
-msgstr "éditeurs"
+msgstr "editores"
 
 #: umap/models.py:139
 msgid "edit status"
-msgstr "statut de modification"
+msgstr "editar estado"
 
 #: umap/models.py:140
 msgid "share status"
-msgstr "qui a accès"
+msgstr "partilhar estado"
 
 #: umap/models.py:141
 msgid "settings"
-msgstr "réglages"
+msgstr "parâmetros"
 
 #: umap/models.py:209
 msgid "Clone of"
 msgstr "Clone de"
 
 #: umap/models.py:260
 msgid "display on load"
-msgstr "afficher au chargement."
+msgstr "mostrar no início"
 
 #: umap/models.py:261
 msgid "Display this layer on load."
-msgstr "Afficher ce calque au chargement."
+msgstr "Apresentar esta camada ao carregar."
 
 #: umap/templates/404.html:7
 msgid "Take me to the home page"
-msgstr "Retour à la page d'accueil"
+msgstr "Ir para a página principal"
 
 #: umap/templates/auth/user_detail.html:7
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Consulter les cartes de %(current_user)s"
+msgstr "Consulte os mapas de %(current_user)s"
 
 #: umap/templates/auth/user_detail.html:15
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s n'a aucune carte."
+msgstr "%(current_user)s não tem mapas."
 
 #: umap/templates/registration/login.html:4
 msgid "Please log in with your account"
-msgstr "Identifiez-vous"
+msgstr "Por favor entre na sua conta"
 
 #: umap/templates/registration/login.html:18
 msgid "Username"
-msgstr "Nom d'utilisateur"
+msgstr "Nome de utilizador"
 
 #: umap/templates/registration/login.html:20
 msgid "Password"
-msgstr "Mot de passe"
+msgstr "Palavra-passe"
 
 #: umap/templates/registration/login.html:21
 msgid "Login"
-msgstr "Connexion"
+msgstr "Entrar"
 
 #: umap/templates/registration/login.html:27
 msgid "Please choose a provider"
-msgstr "Merci de choisir un fournisseur"
+msgstr "Por favor escolha um fornecedor"
 
 #: umap/templates/umap/about_summary.html:6
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr "uMap permet de créer des cartes personnalisées sur des fonds <a href=\"%(osm_url)s\" />OpenStreetMap</a> en un instant et les afficher dans votre site."
+msgstr "O uMap permite criar mapas através de camadas do <a href=\"%(osm_url)s\" />OpenStreetMap</a> num minuto e mostrá-los no seu site."
 
 #: umap/templates/umap/about_summary.html:11
 msgid "Choose the layers of your map"
-msgstr "Choisir les fonds pour votre carte"
+msgstr "Escolha as camadas do mapa"
 
 #: umap/templates/umap/about_summary.html:12
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Ajouter des points d'intérêt : marqueurs, lignes, polygones..."
+msgstr "Adicionar POIs: marcadores, linhas, polígonos..."
 
 #: umap/templates/umap/about_summary.html:13
 msgid "Manage POIs colours and icons"
-msgstr "Choisir la couleur et les icônes"
+msgstr "Gerir as cores dos POI e ícones"
 
 #: umap/templates/umap/about_summary.html:14
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Gérer les options de la carte : afficher une minicarte, géolocaliser l'utilisateur..."
+msgstr "Gerir diversas opções: mostrar um minimapa, localizar o utilizador ao carregar..."
 
 #: umap/templates/umap/about_summary.html:15
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Import des données géographiques en masse (geojson, gpx, kml, osm...)"
+msgstr "Importação em massa de dados geográficos (geojson, gpx, kml, osm...)"
 
 #: umap/templates/umap/about_summary.html:16
 msgid "Choose the license for your data"
-msgstr "Choisir la licence de vos données"
+msgstr "Escolha uma licença para os seus dados"
 
 #: umap/templates/umap/about_summary.html:17
 msgid "Embed and share your map"
-msgstr "Exporter et partager votre carte"
+msgstr "Exportar e partilhar o seu mapa"
 
 #: umap/templates/umap/about_summary.html:23
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Et c'est <a href=\"%(repo_url)s\">open source</a>!"
+msgstr "E está disponível em <a href=\"%(repo_url)s\">código aberto</a>!"
 
 #: umap/templates/umap/about_summary.html:35
 msgid "Play with the demo"
-msgstr "Tester la démo"
+msgstr "Testar a demo"
 
 #: umap/templates/umap/home.html:17
 msgid "Map of the uMaps"
-msgstr "La carte des uMaps"
+msgstr "Mapa dos uMaps"
 
 #: umap/templates/umap/home.html:24
 msgid "Get inspired, browse maps"
-msgstr "Naviguer dans les cartes"
+msgstr "Inspire-se, explore os mapas"
 
 #: umap/templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Vous êtes maintenant identifié. Merci de patienter..."
+msgstr "Sucesso na identificação. Continuando..."
 
-#: umap/templates/umap/map_list.html:7 umap/views.py:226
+#: umap/templates/umap/map_list.html:7 umap/views.py:227
 msgid "by"
-msgstr "par"
+msgstr "por"
 
 #: umap/templates/umap/map_list.html:11
 msgid "More"
-msgstr "Plus"
+msgstr "Mais"
 
 #: umap/templates/umap/navigation.html:14
 msgid "About"
-msgstr "À propos"
+msgstr "Sobre"
 
 #: umap/templates/umap/navigation.html:15
 msgid "Help"
-msgstr "Aide"
+msgstr ""
 
 #: umap/templates/umap/navigation.html:18
 msgid "Change password"
-msgstr "Changer le mot de passe"
+msgstr "Alterar palavra-passe"
 
 #: umap/templates/umap/password_change.html:6
 msgid "Password change"
-msgstr "Changer le mot de passe"
+msgstr "Alterar palavra-passe"
 
 #: umap/templates/umap/password_change.html:7
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr "Merci de renseigner votre mot de passe actuel, puis deux fois le nouveau."
+msgstr "Por favor introduza a sua palavra-passe antiga, por motivos de segurança, e então introduza a sua nova palavra-passe 2 vezes para que possamos verificar se a digitou corretamente."
 
 #: umap/templates/umap/password_change.html:12
 msgid "Old password"
-msgstr "Ancien mot de passe"
+msgstr "Palavra-passe antiga"
 
 #: umap/templates/umap/password_change.html:14
 msgid "New password"
-msgstr "Nouveau mot de passe"
+msgstr "Nova palavra-passe"
 
 #: umap/templates/umap/password_change.html:16
 msgid "New password confirmation"
-msgstr "Confirmation du nouveau mot de passe"
+msgstr "Confirmação da palavra-passe"
 
 #: umap/templates/umap/password_change.html:18
 msgid "Change my password"
-msgstr "Changer de mot de passe"
+msgstr "Alterar a minha palavra-passe"
 
 #: umap/templates/umap/password_change_done.html:6
 msgid "Password change successful"
-msgstr "Le mot de passe a été modifié"
+msgstr "Alteração da palavra-passe bem sucedida"
 
 #: umap/templates/umap/password_change_done.html:7
 msgid "Your password was changed."
-msgstr "Votre mot de passe a été modifié"
+msgstr "A sua palavra-passe foi alterada"
 
 #: umap/templates/umap/search.html:13
 msgid "Not map found."
-msgstr "Aucune carte trouvée."
+msgstr "Nenhum mapa encontrado."
 
-#: umap/views.py:231
+#: umap/views.py:232
 msgid "View the map"
-msgstr "Voir la carte"
+msgstr "Ver o mapa"
 
-#: umap/views.py:519
+#: umap/views.py:529
 #, python-format
 msgid ""
 "Your map has been created! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Votre carte a été créée ! Si vous souhaitez la modifier depuis un autre ordinateur, veuillez utiliser ce lien : %(anonymous_url)s"
+msgstr "O seu mapa foi criado! Se quiser editar este mapa noutro computador, por favor utilize este link: %(anonymous_url)s"
 
-#: umap/views.py:524
+#: umap/views.py:534
 msgid "Congratulations, your map has been created!"
-msgstr "Félicitations, votre carte a bien été créée !"
+msgstr "Parabéns, o seu mapa foi criado!"
 
-#: umap/views.py:554
+#: umap/views.py:564
 msgid "Map has been updated!"
-msgstr "La carte a été mise à jour !"
+msgstr "O mapa foi atualizado!"
 
-#: umap/views.py:579
+#: umap/views.py:589
 msgid "Map editors updated with success!"
-msgstr "Éditeurs de la carte mis à jour !"
+msgstr "Os editores do mapa foram atualizados com sucesso!"
 
-#: umap/views.py:604
+#: umap/views.py:614
 msgid "Only its owner can delete the map."
-msgstr "Seul le créateur de la carte peut la supprimer."
+msgstr "Só o proprietário pode eliminar o mapa."
 
-#: umap/views.py:627
+#: umap/views.py:637
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Votre carte a été dupliquée ! Si vous souhaitez la modifier depuis un autre ordinateur, veuillez utiliser ce lien : %(anonymous_url)s"
+msgstr "O seu mapa foi clonado! Se quiser editar este mapa noutro computador, por favor utilize este link: %(anonymous_url)s"
 
-#: umap/views.py:632
+#: umap/views.py:642
 msgid "Congratulations, your map has been cloned!"
-msgstr "Votre carte a été dupliquée !"
+msgstr "Parabéns, o seu mapa foi clonado!"
 
-#: umap/views.py:787
+#: umap/views.py:793
 msgid "Layer successfully deleted."
-msgstr "Calque supprimé."
+msgstr "Camada eliminada com sucesso."
```

### Comparing `umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/gl/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/he/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/hr/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/hu/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/id/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/is/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/it/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ja/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ko/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/lt/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ms/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ms/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/nl/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/no/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pl/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pt/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-27 12:54+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
 "Last-Translator: Rui <xymarior@yandex.com>, 2016,2018-2019\n"
-"Language-Team: Portuguese (http://www.transifex.com/openstreetmap/umap/language/pt/)\n"
+"Language-Team: Portuguese (Portugal) (http://www.transifex.com/openstreetmap/umap/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt\n"
+"Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: tmp/framacarte/templates/umap/home.html:8 umap/templates/umap/home.html:9
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
@@ -141,15 +141,15 @@
 
 #: umap/models.py:128
 msgid "locate"
 msgstr "localizar"
 
 #: umap/models.py:128
 msgid "Locate user on load?"
-msgstr "Localizar utilizador no início?"
+msgstr "Localizar usuário no início?"
 
 #: umap/models.py:131
 msgid "Choose the map licence."
 msgstr "Escolha uma licença para o mapa."
 
 #: umap/models.py:132
 msgid "licence"
```

### Comparing `umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pt_BR/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/pt_PT/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,378 +1,383 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Joao Ponce de Leao Paulouro <joao.ponceleao@gmail.com>, 2014
-# Rui <xymarior@yandex.com>, 2016,2018-2019
+# Supaplex <bejokeup@gmail.com>, 2019
+# Chia-liang Kao <clkao@clkao.org>, 2014
+# coop.shen <coop.shen@gmail.com>, 2014
+# Hsin-lin Cheng (lancetw) <lancetw@gmail.com>, 2014
+# Sean Young <assanges@icloud.com>, 2016,2018
+# Supaplex <bejokeup@gmail.com>, 2014
+# Yuan CHAO <yuanchao@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-27 12:54+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: Rui <xymarior@yandex.com>, 2016,2018-2019\n"
-"Language-Team: Portuguese (Portugal) (http://www.transifex.com/openstreetmap/umap/language/pt_PT/)\n"
+"Last-Translator: Supaplex <bejokeup@gmail.com>, 2019\n"
+"Language-Team: Chinese (Taiwan) (http://www.transifex.com/openstreetmap/umap/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_PT\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: tmp/framacarte/templates/umap/home.html:8 umap/templates/umap/home.html:9
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Esta é uma versão de demonstração, utilizada para testes e pré-lançamentos. Se precisar de uma versão estável, por favor utilize <a href=\"%(stable_url)s\">%(stable_url)s</a>. Pode também alojar a sua própria instância, e é em <a href=\"%(repo_url)s\">código aberto</a>!"
+msgstr "這是範例服務﹐提供測試與正式版發行前驗證使用。如果您需要穩定的服務，請使用 <a href=\"%(stable_url)s\">%(stable_url)s</a>。您也可以自行架設服務﹐完全是 <a href=\"%(repo_url)s\">開放原始碼</a> 的！"
 
 #: tmp/framacarte/templates/umap/home.html:83
 #: tmp/framacarte/templates/umap/navigation.html:14
 #: umap/templates/umap/about_summary.html:33
 #: umap/templates/umap/navigation.html:26
 msgid "Create a map"
-msgstr "Criar um mapa"
+msgstr "建立地圖"
 
 #: tmp/framacarte/templates/umap/navigation.html:7
 #: umap/templates/umap/navigation.html:10
 msgid "My maps"
-msgstr "Os meus mapas"
+msgstr "我的地圖"
 
 #: tmp/framacarte/templates/umap/navigation.html:9
 #: umap/templates/umap/navigation.html:12
 msgid "Log in"
-msgstr "Entrar"
+msgstr "登入"
 
 #: tmp/framacarte/templates/umap/navigation.html:9
 #: umap/templates/umap/navigation.html:12
 msgid "Sign in"
-msgstr "Criar conta"
+msgstr "註冊"
 
 #: tmp/framacarte/templates/umap/navigation.html:12
 #: umap/templates/umap/navigation.html:20
 msgid "Log out"
-msgstr "Sair"
+msgstr "登出"
 
 #: tmp/framacarte/templates/umap/search_bar.html:6
 #: umap/templates/umap/search_bar.html:6
 msgid "Search maps"
-msgstr "Procurar mapas"
+msgstr "搜尋地圖"
 
 #: tmp/framacarte/templates/umap/search_bar.html:10
 #: tmp/framacarte/templates/umap/search_bar.html:13
 #: umap/templates/umap/search_bar.html:9
 msgid "Search"
-msgstr "Procurar"
+msgstr "搜尋"
 
 #: umap/forms.py:40
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Link secreto para edição é %s"
+msgstr "不公開的私密編輯連結 %s"
 
 #: umap/forms.py:44 umap/models.py:114
 msgid "Everyone can edit"
-msgstr "Todos podem editar"
+msgstr "所有人皆可編輯"
 
 #: umap/forms.py:45
 msgid "Only editable with secret edit link"
-msgstr "Unicamente editável através de link secreto"
+msgstr "僅能由私密連結編輯"
 
 #: umap/middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr "O site está em modo de leitura para manutenção"
+msgstr "網站目前因維護中設定為唯讀狀態"
 
 #: umap/models.py:16
 msgid "name"
-msgstr "nome"
+msgstr "名稱"
 
 #: umap/models.py:47
 msgid "details"
-msgstr "detalhes"
+msgstr "詳情"
 
 #: umap/models.py:48
 msgid "Link to a page where the licence is detailed."
-msgstr "Link para uma página detalhando a licença."
+msgstr "連結至授權條款說明網址"
 
 #: umap/models.py:62
 msgid "URL template using OSM tile format"
-msgstr "Modelo de URL no formato de telas OSM"
+msgstr "URL 樣板，使用 OSM 地圖磚格式"
 
 #: umap/models.py:70
 msgid "Order of the tilelayers in the edit box"
-msgstr "Ordem das camadas na caixa de edição"
+msgstr "編輯方塊中地圖磚的圖層順序"
 
 #: umap/models.py:115
 msgid "Only editors can edit"
-msgstr "Só editores podem editar"
+msgstr "僅編輯群可編輯"
 
 #: umap/models.py:116
 msgid "Only owner can edit"
-msgstr "Só o proprietário pode editar"
+msgstr "僅擁有者可編輯"
 
 #: umap/models.py:119
 msgid "everyone (public)"
-msgstr "todos (público)"
+msgstr "所有人（公開）"
 
 #: umap/models.py:120
 msgid "anyone with link"
-msgstr "qualquer um com o link"
+msgstr "任何有連結的人"
 
 #: umap/models.py:121
 msgid "editors only"
-msgstr "só editores"
+msgstr "只有編輯者允許"
 
 #: umap/models.py:122
 msgid "blocked"
-msgstr "bloqueado"
+msgstr "已經封鎖了"
 
 #: umap/models.py:125 umap/models.py:255
 msgid "description"
-msgstr "descrição"
+msgstr "描述"
 
 #: umap/models.py:126
 msgid "center"
-msgstr "centro"
+msgstr "中心"
 
 #: umap/models.py:127
 msgid "zoom"
-msgstr "zoom"
+msgstr "縮放"
 
 #: umap/models.py:128
 msgid "locate"
-msgstr "localizar"
+msgstr "定位"
 
 #: umap/models.py:128
 msgid "Locate user on load?"
-msgstr "Localizar usuário no início?"
+msgstr "載入時使用定位功能？"
 
 #: umap/models.py:131
 msgid "Choose the map licence."
-msgstr "Escolha uma licença para o mapa."
+msgstr "選擇地圖授權"
 
 #: umap/models.py:132
 msgid "licence"
-msgstr "licença"
+msgstr "授權"
 
 #: umap/models.py:137
 msgid "owner"
-msgstr "proprietário"
+msgstr "擁有者"
 
 #: umap/models.py:138
 msgid "editors"
-msgstr "editores"
+msgstr "編輯者"
 
 #: umap/models.py:139
 msgid "edit status"
-msgstr "editar estado"
+msgstr "編輯狀態"
 
 #: umap/models.py:140
 msgid "share status"
-msgstr "partilhar estado"
+msgstr "分享狀態"
 
 #: umap/models.py:141
 msgid "settings"
-msgstr "parâmetros"
+msgstr "設定"
 
 #: umap/models.py:209
 msgid "Clone of"
-msgstr "Clone de"
+msgstr "複製"
 
 #: umap/models.py:260
 msgid "display on load"
-msgstr "mostrar no início"
+msgstr "載入時顯示"
 
 #: umap/models.py:261
 msgid "Display this layer on load."
-msgstr "Apresentar esta camada ao carregar."
+msgstr "載入此圖層時顯示"
 
 #: umap/templates/404.html:7
 msgid "Take me to the home page"
-msgstr "Ir para a página principal"
+msgstr "帶我回主頁"
 
 #: umap/templates/auth/user_detail.html:7
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Consulte os mapas de %(current_user)s"
+msgstr "瀏覽 %(current_user)s 的地圖"
 
 #: umap/templates/auth/user_detail.html:15
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s não tem mapas."
+msgstr "%(current_user)s 沒有任何地圖。"
 
 #: umap/templates/registration/login.html:4
 msgid "Please log in with your account"
-msgstr "Por favor entre na sua conta"
+msgstr "請先登入"
 
 #: umap/templates/registration/login.html:18
 msgid "Username"
-msgstr "Nome de utilizador"
+msgstr "使用者名稱"
 
 #: umap/templates/registration/login.html:20
 msgid "Password"
-msgstr "Palavra-passe"
+msgstr "密碼"
 
 #: umap/templates/registration/login.html:21
 msgid "Login"
-msgstr "Entrar"
+msgstr "登入"
 
 #: umap/templates/registration/login.html:27
 msgid "Please choose a provider"
-msgstr "Por favor escolha um fornecedor"
+msgstr "選擇服務商"
 
 #: umap/templates/umap/about_summary.html:6
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr "O uMap permite criar mapas através de camadas do <a href=\"%(osm_url)s\" />OpenStreetMap</a> num minuto e mostrá-los no seu site."
+msgstr "uMap 讓你在幾分鐘的時間內用 <a href=\"%(osm_url)s\" />開放街圖</a>的圖層創建地圖，並且內嵌到你的網站上。"
 
 #: umap/templates/umap/about_summary.html:11
 msgid "Choose the layers of your map"
-msgstr "Escolha as camadas do mapa"
+msgstr "選擇您地圖的圖層"
 
 #: umap/templates/umap/about_summary.html:12
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Adicionar POIs: marcadores, linhas, polígonos..."
+msgstr "新增景點 POI：標記、線段、多邊形..."
 
 #: umap/templates/umap/about_summary.html:13
 msgid "Manage POIs colours and icons"
-msgstr "Gerir as cores dos POI e ícones"
+msgstr "管理景點 POI 的顏色與圖示"
 
 #: umap/templates/umap/about_summary.html:14
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Gerir diversas opções: mostrar um minimapa, localizar o utilizador ao carregar..."
+msgstr "管理地圖選項：顯示小型地圖﹐設定初始位置..."
 
 #: umap/templates/umap/about_summary.html:15
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Importação em massa de dados geográficos (geojson, gpx, kml, osm...)"
+msgstr "批次匯入地理資訊 (geojson, gpx, kml, osm... )"
 
 #: umap/templates/umap/about_summary.html:16
 msgid "Choose the license for your data"
-msgstr "Escolha uma licença para os seus dados"
+msgstr "選擇您的資料的授權條例"
 
 #: umap/templates/umap/about_summary.html:17
 msgid "Embed and share your map"
-msgstr "Exportar e partilhar o seu mapa"
+msgstr "內嵌並分享您的地圖"
 
 #: umap/templates/umap/about_summary.html:23
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "E está disponível em <a href=\"%(repo_url)s\">código aberto</a>!"
+msgstr "而且是 <a href=\"%(repo_url)s\">開放原始碼</a> 的！"
 
 #: umap/templates/umap/about_summary.html:35
 msgid "Play with the demo"
-msgstr "Testar a demo"
+msgstr "播放展示"
 
 #: umap/templates/umap/home.html:17
 msgid "Map of the uMaps"
-msgstr "Mapa dos uMaps"
+msgstr "uMaps 地圖"
 
 #: umap/templates/umap/home.html:24
 msgid "Get inspired, browse maps"
-msgstr "Inspire-se, explore os mapas"
+msgstr "找點子，瀏覽其他地圖"
 
 #: umap/templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Sucesso na identificação. Continuando..."
+msgstr "您已登入，繼續中..."
 
 #: umap/templates/umap/map_list.html:7 umap/views.py:227
 msgid "by"
-msgstr "por"
+msgstr "由"
 
 #: umap/templates/umap/map_list.html:11
 msgid "More"
-msgstr "Mais"
+msgstr "更多"
 
 #: umap/templates/umap/navigation.html:14
 msgid "About"
-msgstr "Sobre"
+msgstr "關於"
 
 #: umap/templates/umap/navigation.html:15
 msgid "Help"
 msgstr ""
 
 #: umap/templates/umap/navigation.html:18
 msgid "Change password"
-msgstr "Alterar palavra-passe"
+msgstr "更改密碼"
 
 #: umap/templates/umap/password_change.html:6
 msgid "Password change"
-msgstr "Alterar palavra-passe"
+msgstr "密碼變更"
 
 #: umap/templates/umap/password_change.html:7
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr "Por favor introduza a sua palavra-passe antiga, por motivos de segurança, e então introduza a sua nova palavra-passe 2 vezes para que possamos verificar se a digitou corretamente."
+msgstr "為確保賬戸安全，請先輸入你的舊有密碼。然後輸入新密碼兩次，以便確認新密碼輸入正確。"
 
 #: umap/templates/umap/password_change.html:12
 msgid "Old password"
-msgstr "Palavra-passe antiga"
+msgstr "舊密碼"
 
 #: umap/templates/umap/password_change.html:14
 msgid "New password"
-msgstr "Nova palavra-passe"
+msgstr "新密碼"
 
 #: umap/templates/umap/password_change.html:16
 msgid "New password confirmation"
-msgstr "Confirmação da palavra-passe"
+msgstr "再次輸入新密碼"
 
 #: umap/templates/umap/password_change.html:18
 msgid "Change my password"
-msgstr "Alterar a minha palavra-passe"
+msgstr "更改我的密碼"
 
 #: umap/templates/umap/password_change_done.html:6
 msgid "Password change successful"
-msgstr "Alteração da palavra-passe bem sucedida"
+msgstr "成功更改密碼"
 
 #: umap/templates/umap/password_change_done.html:7
 msgid "Your password was changed."
-msgstr "A sua palavra-passe foi alterada"
+msgstr "你的密碼已更改。"
 
 #: umap/templates/umap/search.html:13
 msgid "Not map found."
-msgstr "Nenhum mapa encontrado."
+msgstr "找不到地圖。"
 
 #: umap/views.py:232
 msgid "View the map"
-msgstr "Ver o mapa"
+msgstr "檢視地圖"
 
 #: umap/views.py:529
 #, python-format
 msgid ""
 "Your map has been created! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "O seu mapa foi criado! Se quiser editar este mapa noutro computador, por favor utilize este link: %(anonymous_url)s"
+msgstr "您的地圖已建立完成！如果您想在不同的機器編輯這個地圖，請使用這個連結：%(anonymous_url)s"
 
 #: umap/views.py:534
 msgid "Congratulations, your map has been created!"
-msgstr "Parabéns, o seu mapa foi criado!"
+msgstr "恭喜您的地圖已經新增完成"
 
 #: umap/views.py:564
 msgid "Map has been updated!"
-msgstr "O mapa foi atualizado!"
+msgstr "地圖已經更新"
 
 #: umap/views.py:589
 msgid "Map editors updated with success!"
-msgstr "Os editores do mapa foram atualizados com sucesso!"
+msgstr "地圖編輯者更新完成"
 
 #: umap/views.py:614
 msgid "Only its owner can delete the map."
-msgstr "Só o proprietário pode eliminar o mapa."
+msgstr "只有擁有者可以刪除此地圖"
 
 #: umap/views.py:637
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "O seu mapa foi clonado! Se quiser editar este mapa noutro computador, por favor utilize este link: %(anonymous_url)s"
+msgstr "您的地圖已複製完成！如果您想在不同的機器編輯這個地圖，請使用這個連結：%(anonymous_url)s"
 
 #: umap/views.py:642
 msgid "Congratulations, your map has been cloned!"
-msgstr "Parabéns, o seu mapa foi clonado!"
+msgstr "恭喜，您的地圖已被複製！"
 
 #: umap/views.py:793
 msgid "Layer successfully deleted."
-msgstr "Camada eliminada com sucesso."
+msgstr "圖層已刪除"
```

### Comparing `umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ro/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/ru/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/si_LK/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/si_LK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sk_SK/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sl/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sr/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/sv/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/th_TH/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/tr/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/uk_UA/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/vi/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/zh/LC_MESSAGES/django.po` & `umap-project-1.3.1/umap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/locale/zh_TW/LC_MESSAGES/django.mo` & `umap-project-1.3.1/umap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/management/commands/anonymous_edit_url.py` & `umap-project-1.3.1/umap/management/commands/anonymous_edit_url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 
 from django.core.management.base import BaseCommand
-from django.conf import settings
 
 from umap.models import Map
 
 
 class Command(BaseCommand):
     help = ('Retrieve anonymous edit url of a map. '
             'Eg.: python manage.py anonymous_edit_url 1234')
@@ -21,8 +20,8 @@
         pk = options['pk']
         try:
             map_ = Map.objects.get(pk=pk)
         except Map.DoesNotExist:
             self.abort('Map with pk {} not found'.format(pk))
         if map_.owner:
             self.abort('Map is not anonymous (owner: {})'.format(map_.owner))
-        print(settings.SITE_URL + map_.get_anonymous_edit_url())
+        print(map_.get_anonymous_edit_url())
```

### Comparing `umap-project-1.3.0a0/umap/management/commands/generate_js_locale.py` & `umap-project-1.3.1/umap/management/commands/generate_js_locale.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/management/commands/import_pictograms.py` & `umap-project-1.3.1/umap/management/commands/import_pictograms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/middleware.py` & `umap-project-1.3.1/umap/middleware.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/migrations/0001_initial.py` & `umap-project-1.3.1/umap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/migrations/0003_add_tilelayer.py` & `umap-project-1.3.1/umap/migrations/0003_add_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/migrations/0004_add_licence.py` & `umap-project-1.3.1/umap/migrations/0004_add_licence.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/migrations/0007_auto_20190416_1757.py` & `umap-project-1.3.1/umap/migrations/0007_auto_20190416_1757.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/migrations/0009_star.py` & `umap-project-1.3.1/umap/migrations/0009_star.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/models.py` & `umap-project-1.3.1/umap/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,16 @@
 
     def get_absolute_url(self):
         return reverse("map", kwargs={"slug": self.slug or "map", "pk": self.pk})
 
     def get_anonymous_edit_url(self):
         signer = Signer()
         signature = signer.sign(self.pk)
-        return reverse("map_anonymous_edit_url", kwargs={"signature": signature})
+        path = reverse("map_anonymous_edit_url", kwargs={"signature": signature})
+        return settings.SITE_URL + path
 
     def is_anonymous_owner(self, request):
         if self.owner:
             # edit cookies are only valid while map hasn't owner
             return False
         key, value = self.signed_cookie_elements
         try:
```

### Comparing `umap-project-1.3.0a0/umap/settings/__init__.py` & `umap-project-1.3.1/umap/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/settings/base.py` & `umap-project-1.3.1/umap/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
     # See https://github.com/peopledoc/django-agnocomplete/commit/26eda2dfa4a2f8a805ca2ea19a0c504b9d773a1c
     # Django does not find the app config in the default place, so the app is not loaded
     # so the "autodiscover" is not run.
     'agnocomplete.app.AgnocompleteConfig',
 )
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 
+EMAIL_BACKEND = "django.core.mail.backends.console.EmailBackend"
+FROM_EMAIL = None
+
 # =============================================================================
 # Calculation of directories relative to the project module location
 # =============================================================================
 
 import os
 import umap as project_module
```

### Comparing `umap-project-1.3.0a0/umap/static/favicon.ico` & `umap-project-1.3.1/umap/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/base.css` & `umap-project-1.3.1/umap/static/umap/base.css`

 * *Files 1% similar despite different names*

```diff
@@ -730,28 +730,32 @@
 .umap-alert #umap-alert-container {
     visibility: visible;
     top: 23px;
 }
 .umap-alert .umap-action {
     margin-left: 10px;
     background-color: #fff;
-    color: #999;
+    color: #000;
     padding: 5px;
     border-radius: 4px;
 }
 .umap-alert .umap-action:hover {
     color: #000;
 }
 .umap-alert .error .umap-action {
     background-color: #666;
     color: #eee;
 }
 .umap-alert .error .umap-action:hover {
     color: #fff;
 }
+.umap-alert input {
+    padding: 5px;
+    border-radius: 4px;
+}
 
 /* *********** */
 /*   Tooltip   */
 /* *********** */
 #umap-tooltip-container {
     line-height: 20px;
     padding: 5px 10px;
```

### Comparing `umap-project-1.3.0a0/umap/static/umap/bitbucket.png` & `umap-project-1.3.1/umap/static/umap/bitbucket.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/content.css` & `umap-project-1.3.1/umap/static/umap/content.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-Light.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-Light.woff2` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-Light.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-LightItalic.woff2` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font/FiraSans-SemiBold.woff2` & `umap-project-1.3.1/umap/static/umap/font/FiraSans-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/font.css` & `umap-project-1.3.1/umap/static/umap/font.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/github.png` & `umap-project-1.3.1/umap/static/umap/github.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/16-white.png` & `umap-project-1.3.1/umap/static/umap/img/16-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/16-white.svg` & `umap-project-1.3.1/umap/static/umap/img/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/16.png` & `umap-project-1.3.1/umap/static/umap/img/16.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/16.svg` & `umap-project-1.3.1/umap/static/umap/img/16.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/24-white.png` & `umap-project-1.3.1/umap/static/umap/img/24-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/24-white.svg` & `umap-project-1.3.1/umap/static/umap/img/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/24.png` & `umap-project-1.3.1/umap/static/umap/img/24.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/24.svg` & `umap-project-1.3.1/umap/static/umap/img/24.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/edit.svg` & `umap-project-1.3.1/umap/static/umap/img/edit.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/logo_filigree.png` & `umap-project-1.3.1/umap/static/umap/img/logo_filigree.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/osm.svg` & `umap-project-1.3.1/umap/static/umap/img/osm.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/img/search.gif` & `umap-project-1.3.1/umap/static/umap/img/search.gif`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.autocomplete.js` & `umap-project-1.3.1/umap/static/umap/js/umap.autocomplete.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.controls.js` & `umap-project-1.3.1/umap/static/umap/js/umap.controls.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1283,15 +1283,15 @@
         }
         const currentView = this.options.currentView ? window.location.hash : ''
         return `${this.baseUrl}?${L.Util.buildQueryString(this.queryString)}${currentView}`
     },
 
     build: function() {
         const iframeUrl = this.buildUrl()
-        const code = `<iframe width="${this.dimensions.width}" height="${this.dimensions.height}" frameborder="0" allowfullscreen allow="geolocation" src="${iframeUrl}"></iframe>`
+        let code = `<iframe width="${this.dimensions.width}" height="${this.dimensions.height}" frameborder="0" allowfullscreen allow="geolocation" src="${iframeUrl}"></iframe>`
         if (this.options.includeFullScreenLink) {
             code += `<p><a href="${this.baseUrl}">${L._('See full screen')}</a></p>`
         }
         return code
     },
 })
```

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.core.js` & `umap-project-1.3.1/umap/static/umap/js/umap.core.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.features.js` & `umap-project-1.3.1/umap/static/umap/js/umap.features.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.forms.js` & `umap-project-1.3.1/umap/static/umap/js/umap.forms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.icon.js` & `umap-project-1.3.1/umap/static/umap/js/umap.icon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.js` & `umap-project-1.3.1/umap/static/umap/js/umap.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1390,48 +1390,117 @@
             properties: this.exportOptions(),
         }
         this.backup()
         const formData = new FormData()
         formData.append('name', this.options.name)
         formData.append('center', JSON.stringify(this.geometry()))
         formData.append('settings', JSON.stringify(geojson))
+
+        function copyToClipboard(textToCopy) {
+            // https://stackoverflow.com/a/65996386
+            // Navigator clipboard api needs a secure context (https)
+            if (navigator.clipboard && window.isSecureContext) {
+                navigator.clipboard.writeText(textToCopy)
+            } else {
+                // Use the 'out of viewport hidden text area' trick
+                const textArea = document.createElement('textarea')
+                textArea.value = textToCopy
+
+                // Move textarea out of the viewport so it's not visible
+                textArea.style.position = 'absolute'
+                textArea.style.left = '-999999px'
+
+                document.body.prepend(textArea)
+                textArea.select()
+
+                try {
+                    document.execCommand('copy')
+                } catch (error) {
+                    console.error(error)
+                } finally {
+                    textArea.remove()
+                }
+            }
+        }
+
         this.post(this.getSaveUrl(), {
             data: formData,
             context: this,
             callback: function(data) {
-                let duration = 3000
+                let duration = 3000,
+                    alert = {
+                        content: L._('Map has been saved!'),
+                        level: 'info'
+                    }
                 if (!this.options.umap_id) {
-                    duration = 100000 // we want a longer message at map creation (TODO UGLY)
+                    alert.content = L._('Congratulations, your map has been created!')
                     this.options.umap_id = data.id
                     this.permissions.setOptions(data.permissions)
+                    if (
+                        data.permissions &&
+                        data.permissions.anonymous_edit_url &&
+                        this.options.urls.map_send_edit_link
+                    ) {
+                        alert.duration = Infinity
+                        alert.content =
+                            L._(
+                                'Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:'
+                            ) + `<br>${data.permissions.anonymous_edit_url}`
+
+                        alert.actions = [{
+                            label: L._('Send me the link'),
+                            input: L._('Email'),
+                            callback: this.sendEditLink,
+                            callbackContext: this,
+                        }, {
+                            label: L._('Copy link'),
+                            callback: () => {
+                                copyToClipboard(data.permissions.anonymous_edit_url)
+                                this.ui.alert({
+                                    content: L._('Secret edit link copied to clipboard!'),
+                                    level: 'info',
+                                })
+                            },
+                            callbackContext: this,
+                        }, ]
+                    }
                 } else if (!this.permissions.isDirty) {
                     // Do not override local changes to permissions,
                     // but update in case some other editors changed them in the meantime.
                     this.permissions.setOptions(data.permissions)
                 }
                 // Update URL in case the name has changed.
                 if (history && history.pushState)
                     history.pushState({}, this.options.name, data.url)
                 else window.location = data.url
-                if (data.info) msg = data.info
-                else msg = L._('Map has been saved!')
+                alert.content = data.info || alert.content
                 this.once('saved', function() {
                     this.isDirty = false
-                    this.ui.alert({
-                        content: msg,
-                        level: 'info',
-                        duration: duration
-                    })
+                    this.ui.alert(alert)
                 })
                 this.ui.closePanel()
                 this.permissions.save()
             },
         })
     },
 
+    sendEditLink: function() {
+        const url = L.Util.template(this.options.urls.map_send_edit_link, {
+                map_id: this.options.umap_id,
+            }),
+            input = this.ui._alert.querySelector('input'),
+            email = input.value
+
+        const formData = new FormData()
+        formData.append('email', email)
+        this.post(url, {
+            data: formData,
+        })
+    },
+
     getEditUrl: function() {
         return L.Util.template(this.options.urls.map_update, {
             map_id: this.options.umap_id,
         })
     },
 
     getCreateUrl: function() {
```

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.layer.js` & `umap-project-1.3.1/umap/static/umap/js/umap.layer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.permissions.js` & `umap-project-1.3.1/umap/static/umap/js/umap.permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.popup.js` & `umap-project-1.3.1/umap/static/umap/js/umap.popup.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.slideshow.js` & `umap-project-1.3.1/umap/static/umap/js/umap.slideshow.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.tableeditor.js` & `umap-project-1.3.1/umap/static/umap/js/umap.tableeditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.ui.js` & `umap-project-1.3.1/umap/static/umap/js/umap.ui.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -71,27 +71,25 @@
 
     alert: function(e) {
         if (L.DomUtil.hasClass(this.parent, 'umap-alert')) this.ALERTS.push(e)
         else this.popAlert(e)
     },
 
     popAlert: function(e) {
-        const self = this
         if (!e) {
             if (this.ALERTS.length) e = this.ALERTS.pop()
             else return
         }
         let timeoutID
         const level_class = e.level && e.level == 'info' ? 'info' : 'error'
         this._alert.innerHTML = ''
         L.DomUtil.addClass(this.parent, 'umap-alert')
         L.DomUtil.addClass(this._alert, level_class)
-
-        function close() {
-            if (timeoutID !== this.ALERT_ID) {
+        const close = () => {
+            if (timeoutID && timeoutID !== this.ALERT_ID) {
                 return
             } // Another alert has been forced
             this._alert.innerHTML = ''
             L.DomUtil.removeClass(this.parent, 'umap-alert')
             L.DomUtil.removeClass(this._alert, level_class)
             if (timeoutID) window.clearTimeout(timeoutID)
             this.popAlert()
@@ -105,36 +103,44 @@
             closeLink,
             'click',
             close,
             this
         )
         L.DomUtil.add('div', '', this._alert, e.content)
         if (e.actions) {
-            let action, el
+            let action, el, input
             for (let i = 0; i < e.actions.length; i++) {
                 action = e.actions[i]
+                if (action.input) {
+                    input = L.DomUtil.element(
+                        'input', {
+                            className: 'umap-alert-input',
+                            placeholder: action.input
+                        },
+                        this._alert
+                    )
+                }
                 el = L.DomUtil.element('a', {
                     className: 'umap-action'
                 }, this._alert)
                 el.href = '#'
                 el.textContent = action.label
-                L.DomEvent.on(el, 'click', L.DomEvent.stop).on(el, 'click', close, this)
-                if (action.callback)
-                    L.DomEvent.on(
-                        el,
-                        'click',
-                        action.callback,
-                        action.callbackContext || this.map
-                    )
+                L.DomEvent.on(el, 'click', L.DomEvent.stop)
+                if (action.callback) {
+                    L.DomEvent.on(el, 'click', action.callback, action.callbackContext || this.map)
+                }
+                L.DomEvent.on(el, 'click', close, this)
             }
         }
-        self.ALERT_ID = timeoutID = window.setTimeout(
-            L.bind(close, this),
-            e.duration || 3000
-        )
+        if (e.duration !== Infinity) {
+            this.ALERT_ID = timeoutID = window.setTimeout(
+                L.bind(close, this),
+                e.duration || 3000
+            )
+        }
     },
 
     tooltip: function(e) {
         this.TOOLTIP_ID = Math.random()
         const id = this.TOOLTIP_ID
         L.DomUtil.addClass(this.parent, 'umap-tooltip')
         if (e.anchor && e.position === 'top') this.anchorTooltipTop(e.anchor)
```

### Comparing `umap-project-1.3.0a0/umap/static/umap/js/umap.xhr.js` & `umap-project-1.3.1/umap/static/umap/js/umap.xhr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/am_ET.js` & `umap-project-1.3.1/umap/static/umap/locale/am_ET.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/am_ET.json` & `umap-project-1.3.1/umap/static/umap/locale/am_ET.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ar.js` & `umap-project-1.3.1/umap/static/umap/locale/ar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ar.json` & `umap-project-1.3.1/umap/static/umap/locale/ar.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ast.js` & `umap-project-1.3.1/umap/static/umap/locale/ast.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ast.json` & `umap-project-1.3.1/umap/static/umap/locale/ast.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/bg.js` & `umap-project-1.3.1/umap/static/umap/locale/bg.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/bg.json` & `umap-project-1.3.1/umap/static/umap/locale/bg.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ca.js` & `umap-project-1.3.1/umap/static/umap/locale/ca.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ca.json` & `umap-project-1.3.1/umap/static/umap/locale/ca.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.js` & `umap-project-1.3.1/umap/static/umap/locale/cs_CZ.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/cs_CZ.json` & `umap-project-1.3.1/umap/static/umap/locale/cs_CZ.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/da.js` & `umap-project-1.3.1/umap/static/umap/locale/da.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/da.json` & `umap-project-1.3.1/umap/static/umap/locale/da.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/de.js` & `umap-project-1.3.1/umap/static/umap/locale/de.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/de.json` & `umap-project-1.3.1/umap/static/umap/locale/de.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/el.js` & `umap-project-1.3.1/umap/static/umap/locale/el.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/el.json` & `umap-project-1.3.1/umap/static/umap/locale/el.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/en.js` & `umap-project-1.3.1/umap/static/umap/locale/en.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/en.json` & `umap-project-1.3.1/umap/static/umap/locale/en.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/en_US.json` & `umap-project-1.3.1/umap/static/umap/locale/en_US.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/es.js` & `umap-project-1.3.1/umap/static/umap/locale/es.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/es.json` & `umap-project-1.3.1/umap/static/umap/locale/es.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/et.js` & `umap-project-1.3.1/umap/static/umap/locale/et.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/et.json` & `umap-project-1.3.1/umap/static/umap/locale/et.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.js` & `umap-project-1.3.1/umap/static/umap/locale/fa_IR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fa_IR.json` & `umap-project-1.3.1/umap/static/umap/locale/fa_IR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fi.js` & `umap-project-1.3.1/umap/static/umap/locale/fi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fi.json` & `umap-project-1.3.1/umap/static/umap/locale/fi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fr.js` & `umap-project-1.3.1/umap/static/umap/locale/fr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/fr.json` & `umap-project-1.3.1/umap/static/umap/locale/fr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/gl.js` & `umap-project-1.3.1/umap/static/umap/locale/gl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/gl.json` & `umap-project-1.3.1/umap/static/umap/locale/gl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/he.js` & `umap-project-1.3.1/umap/static/umap/locale/he.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/he.json` & `umap-project-1.3.1/umap/static/umap/locale/he.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/hr.js` & `umap-project-1.3.1/umap/static/umap/locale/hr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/hr.json` & `umap-project-1.3.1/umap/static/umap/locale/hr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/hu.js` & `umap-project-1.3.1/umap/static/umap/locale/hu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/hu.json` & `umap-project-1.3.1/umap/static/umap/locale/hu.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/id.js` & `umap-project-1.3.1/umap/static/umap/locale/id.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/id.json` & `umap-project-1.3.1/umap/static/umap/locale/id.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/is.js` & `umap-project-1.3.1/umap/static/umap/locale/is.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/is.json` & `umap-project-1.3.1/umap/static/umap/locale/is.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/it.js` & `umap-project-1.3.1/umap/static/umap/locale/it.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/it.json` & `umap-project-1.3.1/umap/static/umap/locale/it.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ja.js` & `umap-project-1.3.1/umap/static/umap/locale/ja.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ja.json` & `umap-project-1.3.1/umap/static/umap/locale/ja.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ko.js` & `umap-project-1.3.1/umap/static/umap/locale/ko.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ko.json` & `umap-project-1.3.1/umap/static/umap/locale/ko.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/lt.js` & `umap-project-1.3.1/umap/static/umap/locale/lt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/lt.json` & `umap-project-1.3.1/umap/static/umap/locale/lt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ms.js` & `umap-project-1.3.1/umap/static/umap/locale/ms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ms.json` & `umap-project-1.3.1/umap/static/umap/locale/ms.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/nl.js` & `umap-project-1.3.1/umap/static/umap/locale/nl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/nl.json` & `umap-project-1.3.1/umap/static/umap/locale/nl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/no.js` & `umap-project-1.3.1/umap/static/umap/locale/no.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/no.json` & `umap-project-1.3.1/umap/static/umap/locale/no.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pl.js` & `umap-project-1.3.1/umap/static/umap/locale/pl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pl.json` & `umap-project-1.3.1/umap/static/umap/locale/pl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pl_PL.json` & `umap-project-1.3.1/umap/static/umap/locale/pl_PL.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt.js` & `umap-project-1.3.1/umap/static/umap/locale/pt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt.json` & `umap-project-1.3.1/umap/static/umap/locale/pt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.js` & `umap-project-1.3.1/umap/static/umap/locale/pt_BR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt_BR.json` & `umap-project-1.3.1/umap/static/umap/locale/pt_BR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.js` & `umap-project-1.3.1/umap/static/umap/locale/pt_PT.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/pt_PT.json` & `umap-project-1.3.1/umap/static/umap/locale/pt_PT.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ro.js` & `umap-project-1.3.1/umap/static/umap/locale/ro.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ro.json` & `umap-project-1.3.1/umap/static/umap/locale/ro.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ru.js` & `umap-project-1.3.1/umap/static/umap/locale/ru.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/ru.json` & `umap-project-1.3.1/umap/static/umap/locale/ru.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/si_LK.js` & `umap-project-1.3.1/umap/static/umap/locale/si_LK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/si_LK.json` & `umap-project-1.3.1/umap/static/umap/locale/si_LK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.js` & `umap-project-1.3.1/umap/static/umap/locale/sk_SK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sk_SK.json` & `umap-project-1.3.1/umap/static/umap/locale/sk_SK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sl.js` & `umap-project-1.3.1/umap/static/umap/locale/sl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sl.json` & `umap-project-1.3.1/umap/static/umap/locale/sl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sr.js` & `umap-project-1.3.1/umap/static/umap/locale/sr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sr.json` & `umap-project-1.3.1/umap/static/umap/locale/sr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sv.js` & `umap-project-1.3.1/umap/static/umap/locale/sv.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/sv.json` & `umap-project-1.3.1/umap/static/umap/locale/sv.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/th_TH.js` & `umap-project-1.3.1/umap/static/umap/locale/th_TH.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/th_TH.json` & `umap-project-1.3.1/umap/static/umap/locale/th_TH.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/tr.js` & `umap-project-1.3.1/umap/static/umap/locale/tr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/tr.json` & `umap-project-1.3.1/umap/static/umap/locale/tr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.js` & `umap-project-1.3.1/umap/static/umap/locale/uk_UA.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/uk_UA.json` & `umap-project-1.3.1/umap/static/umap/locale/uk_UA.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/vi.js` & `umap-project-1.3.1/umap/static/umap/locale/vi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/vi.json` & `umap-project-1.3.1/umap/static/umap/locale/vi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/vi_VN.json` & `umap-project-1.3.1/umap/static/umap/locale/vi_VN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh.js` & `umap-project-1.3.1/umap/static/umap/locale/zh.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh.json` & `umap-project-1.3.1/umap/static/umap/locale/zh.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh_CN.json` & `umap-project-1.3.1/umap/static/umap/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.Big5.json` & `umap-project-1.3.1/umap/static/umap/locale/zh_TW.Big5.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.js` & `umap-project-1.3.1/umap/static/umap/locale/zh_TW.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/locale/zh_TW.json` & `umap-project-1.3.1/umap/static/umap/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/map.css` & `umap-project-1.3.1/umap/static/umap/map.css`

 * *Files 0% similar despite different names*

```diff
@@ -1314,18 +1314,27 @@
     display: flex;
     flex-direction: column;
 }
 .umap-popup-content iframe {
     min-width: 310px;
     max-width: 100%;
 }
-.umap-popup-content th,
+.umap-popup-content tr:nth-child(odd) {
+   background-color: #f6f6f6;
+}
+.umap-popup-content th {
+    text-align: left;
+}
 .umap-popup-content td {
     word-break: break-word;
 }
+.umap-popup-content th,
+.umap-popup-content td {
+    padding: 1px 3px;
+}
 .umap-popup-container {
     flex-grow: 1;
     padding: 0 10px;
     word-break: break-word;
 }
 .leaflet-popup-content h3 {
     margin-bottom: 0;
```

### Comparing `umap-project-1.3.0a0/umap/static/umap/nav.css` & `umap-project-1.3.1/umap/static/umap/nav.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/openstreetmap.png` & `umap-project-1.3.1/umap/static/umap/openstreetmap.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Controls.js` & `umap-project-1.3.1/umap/static/umap/test/Controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/DataLayer.js` & `umap-project-1.3.1/umap/static/umap/test/DataLayer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Feature.js` & `umap-project-1.3.1/umap/static/umap/test/Feature.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Map.js` & `umap-project-1.3.1/umap/static/umap/test/Map.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Marker.js` & `umap-project-1.3.1/umap/static/umap/test/Marker.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Permissions.js` & `umap-project-1.3.1/umap/static/umap/test/Permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Polygon.js` & `umap-project-1.3.1/umap/static/umap/test/Polygon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Polyline.js` & `umap-project-1.3.1/umap/static/umap/test/Polyline.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/TableEditor.js` & `umap-project-1.3.1/umap/static/umap/test/TableEditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/Util.js` & `umap-project-1.3.1/umap/static/umap/test/Util.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/_pre.js` & `umap-project-1.3.1/umap/static/umap/test/_pre.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/test/index.html` & `umap-project-1.3.1/umap/static/umap/test/index.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/twitter.png` & `umap-project-1.3.1/umap/static/umap/twitter.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css` & `umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js` & `umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css` & `umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js` & `umap-project-1.3.1/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/csv2geojson.js` & `umap-project-1.3.1/umap/static/umap/vendors/csv2geojson/csv2geojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/csv2geojson/index.js` & `umap-project-1.3.1/umap/static/umap/vendors/csv2geojson/index.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/dompurify/purify.js` & `umap-project-1.3.1/umap/static/umap/vendors/dompurify/purify.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/editable/Leaflet.Editable.js` & `umap-project-1.3.1/umap/static/umap/vendors/editable/Leaflet.Editable.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/editable/Path.Drag.js` & `umap-project-1.3.1/umap/static/umap/vendors/editable/Path.Drag.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css` & `umap-project-1.3.1/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js` & `umap-project-1.3.1/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/editinosm/edit-in-osm.png` & `umap-project-1.3.1/umap/static/umap/vendors/editinosm/edit-in-osm.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js` & `umap-project-1.3.1/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js` & `umap-project-1.3.1/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js` & `umap-project-1.3.1/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css` & `umap-project-1.3.1/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js` & `umap-project-1.3.1/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/hash/leaflet-hash.js` & `umap-project-1.3.1/umap/static/umap/vendors/hash/leaflet-hash.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/heat/leaflet-heat.js` & `umap-project-1.3.1/umap/static/umap/vendors/heat/leaflet-heat.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/i18n/Leaflet.i18n.js` & `umap-project-1.3.1/umap/static/umap/vendors/i18n/Leaflet.i18n.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers-2x.png` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/layers.png` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-icon.png` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/images/marker-shadow.png` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet-src.js.map` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.css` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/leaflet/leaflet.js.map` & `umap-project-1.3.1/umap/static/umap/vendors/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.css` & `umap-project-1.3.1/umap/static/umap/vendors/loading/Control.Loading.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/loading/Control.Loading.js` & `umap-project-1.3.1/umap/static/umap/vendors/loading/Control.Loading.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css` & `umap-project-1.3.1/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js` & `umap-project-1.3.1/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/MarkerCluster.css` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map` & `umap-project-1.3.1/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.css` & `umap-project-1.3.1/umap/static/umap/vendors/measurable/Leaflet.Measurable.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/measurable/Leaflet.Measurable.js` & `umap-project-1.3.1/umap/static/umap/vendors/measurable/Leaflet.Measurable.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.css` & `umap-project-1.3.1/umap/static/umap/vendors/minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/Control.MiniMap.js` & `umap-project-1.3.1/umap/static/umap/vendors/minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/minimap/images/toggle.svg` & `umap-project-1.3.1/umap/static/umap/vendors/minimap/images/toggle.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js` & `umap-project-1.3.1/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/photon/leaflet.photon.js` & `umap-project-1.3.1/umap/static/umap/vendors/photon/leaflet.photon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.js` & `umap-project-1.3.1/umap/static/umap/vendors/print/leaflet.browser.print.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/print/leaflet.browser.print.min.js` & `umap-project-1.3.1/umap/static/umap/vendors/print/leaflet.browser.print.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/togeojson/togeojson.js` & `umap-project-1.3.1/umap/static/umap/vendors/togeojson/togeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/togpx/togpx.js` & `umap-project-1.3.1/umap/static/umap/vendors/togpx/togpx.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/tokml/tokml.js` & `umap-project-1.3.1/umap/static/umap/vendors/tokml/tokml.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css` & `umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js` & `umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.css` & `umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/static/umap/vendors/toolbar/leaflet.toolbar.js` & `umap-project-1.3.1/umap/static/umap/vendors/toolbar/leaflet.toolbar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/500.html` & `umap-project-1.3.1/umap/templates/500.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/base.html` & `umap-project-1.3.1/umap/templates/base.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/registration/login.html` & `umap-project-1.3.1/umap/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/about_summary.html` & `umap-project-1.3.1/umap/templates/umap/about_summary.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/content.html` & `umap-project-1.3.1/umap/templates/umap/content.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/content_footer.html` & `umap-project-1.3.1/umap/templates/umap/content_footer.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/css.html` & `umap-project-1.3.1/umap/templates/umap/css.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/home.html` & `umap-project-1.3.1/umap/templates/umap/home.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/js.html` & `umap-project-1.3.1/umap/templates/umap/js.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/login_popup_end.html` & `umap-project-1.3.1/umap/templates/umap/login_popup_end.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/map_detail.html` & `umap-project-1.3.1/umap/templates/umap/map_detail.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/map_list.html` & `umap-project-1.3.1/umap/templates/umap/map_list.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/navigation.html` & `umap-project-1.3.1/umap/templates/umap/navigation.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templates/umap/password_change.html` & `umap-project-1.3.1/umap/templates/umap/password_change.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/templatetags/umap_tags.py` & `umap-project-1.3.1/umap/templatetags/umap_tags.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/base.py` & `umap-project-1.3.1/umap/tests/base.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/conftest.py` & `umap-project-1.3.1/umap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/test_datalayer.py` & `umap-project-1.3.1/umap/tests/test_datalayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/test_datalayer_views.py` & `umap-project-1.3.1/umap/tests/test_datalayer_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/test_map.py` & `umap-project-1.3.1/umap/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/test_map_views.py` & `umap-project-1.3.1/umap/tests/test_map_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 import json
 
 import pytest
 from django.contrib.auth import get_user_model
+from django.core import mail
 from django.urls import reverse
-
 from django.core.signing import Signer
+
 from umap.models import DataLayer, Map, Star
 
 from .base import login_required
 
 pytestmark = pytest.mark.django_db
 User = get_user_model()
 
 
 @pytest.fixture
 def post_data():
     return {
-        'name': 'name',
-        'center': '{"type":"Point","coordinates":[13.447265624999998,48.94415123418794]}',  # noqa
-        'settings': '{"type":"Feature","geometry":{"type":"Point","coordinates":[5.0592041015625,52.05924589011585]},"properties":{"tilelayer":{"maxZoom":20,"url_template":"http://{s}.tile.openstreetmap.fr/hot/{z}/{x}/{y}.png","minZoom":0,"attribution":"HOT and friends"},"licence":"","description":"","name":"test enrhûmé","tilelayersControl":true,"displayDataBrowserOnLoad":false,"displayPopupFooter":true,"displayCaptionOnLoad":false,"miniMap":true,"moreControl":true,"scaleControl":true,"zoomControl":true,"datalayersControl":true,"zoom":8}}'  # noqa
+        "name": "name",
+        "center": '{"type":"Point","coordinates":[13.447265624999998,48.94415123418794]}',  # noqa
+        "settings": '{"type":"Feature","geometry":{"type":"Point","coordinates":[5.0592041015625,52.05924589011585]},"properties":{"tilelayer":{"maxZoom":20,"url_template":"http://{s}.tile.openstreetmap.fr/hot/{z}/{x}/{y}.png","minZoom":0,"attribution":"HOT and friends"},"licence":"","description":"","name":"test enrhûmé","tilelayersControl":true,"displayDataBrowserOnLoad":false,"displayPopupFooter":true,"displayCaptionOnLoad":false,"miniMap":true,"moreControl":true,"scaleControl":true,"zoomControl":true,"datalayersControl":true,"zoom":8}}',  # noqa
     }
 
 
 def test_create(client, user, post_data):
-    url = reverse('map_create')
+    url = reverse("map_create")
     # POST only mendatory fields
-    name = 'test-map-with-new-name'
-    post_data['name'] = name
+    name = "test-map-with-new-name"
+    post_data["name"] = name
     client.login(username=user.username, password="123123")
     response = client.post(url, post_data)
     assert response.status_code == 200
     j = json.loads(response.content.decode())
-    created_map = Map.objects.latest('pk')
-    assert j['id'] == created_map.pk
+    created_map = Map.objects.latest("pk")
+    assert j["id"] == created_map.pk
     assert created_map.name == name
     assert created_map.center.x == 13.447265624999998
     assert created_map.center.y == 48.94415123418794
-    assert j['permissions'] == {
-        'edit_status': 3,
-        'share_status': 1,
-        'owner': {
-            'id': user.pk,
-            'name': 'Joe',
-            'url': '/en/user/Joe/'
-        },
-        'editors': [],
-        'anonymous_edit_url': ('http://umap.org'
-                               + created_map.get_anonymous_edit_url())
+    assert j["permissions"] == {
+        "edit_status": 3,
+        "share_status": 1,
+        "owner": {"id": user.pk, "name": "Joe", "url": "/en/user/Joe/"},
+        "editors": [],
+        "anonymous_edit_url": created_map.get_anonymous_edit_url(),
     }
 
 
 def test_map_create_permissions(client, settings):
     settings.UMAP_ALLOW_ANONYMOUS = False
-    url = reverse('map_create')
+    url = reverse("map_create")
     # POST anonymous
     response = client.post(url, {})
     assert login_required(response)
 
 
 def test_map_update_access(client, map, user):
-    url = reverse('map_update', kwargs={'map_id': map.pk})
+    url = reverse("map_update", kwargs={"map_id": map.pk})
     # GET anonymous
     response = client.get(url)
     assert login_required(response)
     # POST anonymous
     response = client.post(url, {})
     assert login_required(response)
     # GET with wrong permissions
@@ -73,15 +69,15 @@
     # POST with wrong permissions
     client.login(username=user.username, password="123123")
     response = client.post(url, {})
     assert response.status_code == 403
 
 
 def test_map_update_permissions_access(client, map, user):
-    url = reverse('map_update_permissions', kwargs={'map_id': map.pk})
+    url = reverse("map_update_permissions", kwargs={"map_id": map.pk})
     # GET anonymous
     response = client.get(url)
     assert login_required(response)
     # POST anonymous
     response = client.post(url, {})
     assert login_required(response)
     # GET with wrong permissions
@@ -91,94 +87,91 @@
     # POST with wrong permissions
     client.login(username=user.username, password="123123")
     response = client.post(url, {})
     assert response.status_code == 403
 
 
 def test_update(client, map, post_data):
-    url = reverse('map_update', kwargs={'map_id': map.pk})
+    url = reverse("map_update", kwargs={"map_id": map.pk})
     # POST only mendatory fields
-    name = 'new map name'
-    post_data['name'] = name
+    name = "new map name"
+    post_data["name"] = name
     client.login(username=map.owner.username, password="123123")
     response = client.post(url, post_data)
     assert response.status_code == 200
     j = json.loads(response.content.decode())
-    assert 'html' not in j
+    assert "html" not in j
     updated_map = Map.objects.get(pk=map.pk)
-    assert j['id'] == updated_map.pk
+    assert j["id"] == updated_map.pk
     assert updated_map.name == name
 
 
 def test_delete(client, map, datalayer):
-    url = reverse('map_delete', args=(map.pk, ))
+    url = reverse("map_delete", args=(map.pk,))
     client.login(username=map.owner.username, password="123123")
     response = client.post(url, {}, follow=True)
     assert response.status_code == 200
     assert not Map.objects.filter(pk=map.pk).exists()
     assert not DataLayer.objects.filter(pk=datalayer.pk).exists()
     # Check that user has not been impacted
     assert User.objects.filter(pk=map.owner.pk).exists()
     # Test response is a json
     j = json.loads(response.content.decode())
-    assert 'redirect' in j
+    assert "redirect" in j
 
 
 def test_wrong_slug_should_redirect_to_canonical(client, map):
-    url = reverse('map', kwargs={'pk': map.pk, 'slug': 'wrong-slug'})
-    canonical = reverse('map', kwargs={'pk': map.pk,
-                                       'slug': map.slug})
+    url = reverse("map", kwargs={"pk": map.pk, "slug": "wrong-slug"})
+    canonical = reverse("map", kwargs={"pk": map.pk, "slug": map.slug})
     response = client.get(url)
     assert response.status_code == 301
-    assert response['Location'] == canonical
+    assert response["Location"] == canonical
 
 
 def test_wrong_slug_should_redirect_with_query_string(client, map):
-    url = reverse('map', kwargs={'pk': map.pk, 'slug': 'wrong-slug'})
+    url = reverse("map", kwargs={"pk": map.pk, "slug": "wrong-slug"})
     url = "{}?allowEdit=0".format(url)
-    canonical = reverse('map', kwargs={'pk': map.pk,
-                                       'slug': map.slug})
+    canonical = reverse("map", kwargs={"pk": map.pk, "slug": map.slug})
     canonical = "{}?allowEdit=0".format(canonical)
     response = client.get(url)
     assert response.status_code == 301
-    assert response['Location'] == canonical
+    assert response["Location"] == canonical
 
 
 def test_should_not_consider_the_query_string_for_canonical_check(client, map):
-    url = reverse('map', kwargs={'pk': map.pk, 'slug': map.slug})
+    url = reverse("map", kwargs={"pk": map.pk, "slug": map.slug})
     url = "{}?allowEdit=0".format(url)
     response = client.get(url)
     assert response.status_code == 200
 
 
 def test_short_url_should_redirect_to_canonical(client, map):
-    url = reverse('map_short_url', kwargs={'pk': map.pk})
-    canonical = reverse('map', kwargs={'pk': map.pk,
-                                       'slug': map.slug})
+    url = reverse("map_short_url", kwargs={"pk": map.pk})
+    canonical = reverse("map", kwargs={"pk": map.pk, "slug": map.slug})
     response = client.get(url)
     assert response.status_code == 301
-    assert response['Location'] == canonical
+    assert response["Location"] == canonical
 
 
 def test_clone_map_should_create_a_new_instance(client, map):
     assert Map.objects.count() == 1
-    url = reverse('map_clone', kwargs={'map_id': map.pk})
+    url = reverse("map_clone", kwargs={"map_id": map.pk})
     client.login(username=map.owner.username, password="123123")
     response = client.post(url)
     assert response.status_code == 200
     assert Map.objects.count() == 2
-    clone = Map.objects.latest('pk')
+    clone = Map.objects.latest("pk")
     assert clone.pk != map.pk
-    assert clone.name == u"Clone of " + map.name
+    assert clone.name == "Clone of " + map.name
 
 
 def test_user_not_allowed_should_not_clone_map(client, map, user, settings):
     settings.UMAP_ALLOW_ANONYMOUS = False
     assert Map.objects.count() == 1
-    url = reverse('map_clone', kwargs={'map_id': map.pk})
+    url = reverse("map_clone", kwargs={"map_id": map.pk})
     map.edit_status = map.OWNER
     map.save()
     response = client.post(url)
     assert login_required(response)
     client.login(username=user.username, password="123123")
     response = client.post(url)
     assert response.status_code == 403
@@ -187,324 +180,330 @@
     client.logout()
     response = client.post(url)
     assert response.status_code == 403
     assert Map.objects.count() == 1
 
 
 def test_clone_should_set_cloner_as_owner(client, map, user):
-    url = reverse('map_clone', kwargs={'map_id': map.pk})
+    url = reverse("map_clone", kwargs={"map_id": map.pk})
     map.edit_status = map.EDITORS
     map.editors.add(user)
     map.save()
     client.login(username=user.username, password="123123")
     response = client.post(url)
     assert response.status_code == 200
     assert Map.objects.count() == 2
-    clone = Map.objects.latest('pk')
+    clone = Map.objects.latest("pk")
     assert clone.pk != map.pk
-    assert clone.name == u"Clone of " + map.name
+    assert clone.name == "Clone of " + map.name
     assert clone.owner == user
 
 
 def test_map_creation_should_allow_unicode_names(client, map, post_data):
-    url = reverse('map_create')
+    url = reverse("map_create")
     # POST only mendatory fields
-    name = u'Академический'
-    post_data['name'] = name
+    name = "Академический"
+    post_data["name"] = name
     client.login(username=map.owner.username, password="123123")
     response = client.post(url, post_data)
     assert response.status_code == 200
     j = json.loads(response.content.decode())
-    created_map = Map.objects.latest('pk')
-    assert j['id'] == created_map.pk
+    created_map = Map.objects.latest("pk")
+    assert j["id"] == created_map.pk
     assert created_map.name == name
     # Lower case of the russian original name
     # self.assertEqual(created_map.slug, u"академический")
     # for now we fallback to "map", see unicode_name branch
-    assert created_map.slug == 'map'
+    assert created_map.slug == "map"
 
 
 def test_anonymous_can_access_map_with_share_status_public(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.PUBLIC
     map.save()
     response = client.get(url)
     assert response.status_code == 200
 
 
 def test_anonymous_can_access_map_with_share_status_open(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.OPEN
     map.save()
     response = client.get(url)
     assert response.status_code == 200
 
 
 def test_anonymous_cannot_access_map_with_share_status_private(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.PRIVATE
     map.save()
     response = client.get(url)
     assert response.status_code == 403
 
 
 def test_owner_can_access_map_with_share_status_private(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.PRIVATE
     map.save()
     client.login(username=map.owner.username, password="123123")
     response = client.get(url)
     assert response.status_code == 200
 
 
 def test_editors_can_access_map_with_share_status_private(client, map, user):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.PRIVATE
     map.editors.add(user)
     map.save()
     client.login(username=user.username, password="123123")
     response = client.get(url)
     assert response.status_code == 200
 
 
 def test_anonymous_cannot_access_map_with_share_status_blocked(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.BLOCKED
     map.save()
     response = client.get(url)
     assert response.status_code == 403
 
 
 def test_owner_cannot_access_map_with_share_status_blocked(client, map):
-    url = reverse('map', args=(map.slug, map.pk))
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.BLOCKED
     map.save()
     client.login(username=map.owner.username, password="123123")
     response = client.get(url)
     assert response.status_code == 403
 
 
-def test_non_editor_cannot_access_map_if_share_status_private(client, map, user):  # noqa
-    url = reverse('map', args=(map.slug, map.pk))
+def test_non_editor_cannot_access_map_if_share_status_private(
+    client, map, user
+):  # noqa
+    url = reverse("map", args=(map.slug, map.pk))
     map.share_status = map.PRIVATE
     map.save()
     client.login(username=user.username, password="123123")
     response = client.get(url)
     assert response.status_code == 403
 
 
 def test_map_geojson_view(client, map):
-    url = reverse('map_geojson', args=(map.pk, ))
+    url = reverse("map_geojson", args=(map.pk,))
     response = client.get(url)
     j = json.loads(response.content.decode())
-    assert 'json' in response['content-type']
-    assert 'type' in j
+    assert "json" in response["content-type"]
+    assert "type" in j
 
 
 def test_only_owner_can_delete(client, map, user):
     map.editors.add(user)
-    url = reverse('map_delete', kwargs={'map_id': map.pk})
+    url = reverse("map_delete", kwargs={"map_id": map.pk})
     client.login(username=user.username, password="123123")
     response = client.post(url, {}, follow=True)
     assert response.status_code == 403
 
 
 def test_map_editors_do_not_see_owner_change_input(client, map, user):
     map.editors.add(user)
     map.edit_status = map.EDITORS
     map.save()
-    url = reverse('map_update_permissions', kwargs={'map_id': map.pk})
+    url = reverse("map_update_permissions", kwargs={"map_id": map.pk})
     client.login(username=user.username, password="123123")
     response = client.get(url)
-    assert 'id_owner' not in response
+    assert "id_owner" not in response
 
 
 def test_logged_in_user_can_edit_map_editable_by_anonymous(client, map, user):
     map.owner = None
     map.edit_status = map.ANONYMOUS
     map.save()
     client.login(username=user.username, password="123123")
-    url = reverse('map_update', kwargs={'map_id': map.pk})
-    new_name = 'this is my new name'
+    url = reverse("map_update", kwargs={"map_id": map.pk})
+    new_name = "this is my new name"
     data = {
-        'center': '{"type":"Point","coordinates":[13.447265624999998,48.94415123418794]}',  # noqa
-        'name': new_name
+        "center": '{"type":"Point","coordinates":[13.447265624999998,48.94415123418794]}',  # noqa
+        "name": new_name,
     }
     response = client.post(url, data)
     assert response.status_code == 200
     assert Map.objects.get(pk=map.pk).name == new_name
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_anonymous_create(cookieclient, post_data):
-    url = reverse('map_create')
+    url = reverse("map_create")
     # POST only mendatory fields
-    name = 'test-map-with-new-name'
-    post_data['name'] = name
+    name = "test-map-with-new-name"
+    post_data["name"] = name
     response = cookieclient.post(url, post_data)
     assert response.status_code == 200
     j = json.loads(response.content.decode())
-    created_map = Map.objects.latest('pk')
-    assert j['id'] == created_map.pk
-    assert (created_map.get_anonymous_edit_url()
-            in j['permissions']['anonymous_edit_url'])
+    created_map = Map.objects.latest("pk")
+    assert j["id"] == created_map.pk
+    assert (
+        created_map.get_anonymous_edit_url() in j["permissions"]["anonymous_edit_url"]
+    )
     assert created_map.name == name
     key, value = created_map.signed_cookie_elements
     assert key in cookieclient.cookies
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_anonymous_update_without_cookie_fails(client, anonymap, post_data):  # noqa
-    url = reverse('map_update', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_update", kwargs={"map_id": anonymap.pk})
     response = client.post(url, post_data)
     assert response.status_code == 403
 
 
-@pytest.mark.usefixtures('allow_anonymous')
-def test_anonymous_update_with_cookie_should_work(cookieclient, anonymap, post_data):  # noqa
-    url = reverse('map_update', kwargs={'map_id': anonymap.pk})
+@pytest.mark.usefixtures("allow_anonymous")
+def test_anonymous_update_with_cookie_should_work(
+    cookieclient, anonymap, post_data
+):  # noqa
+    url = reverse("map_update", kwargs={"map_id": anonymap.pk})
     # POST only mendatory fields
-    name = 'new map name'
-    post_data['name'] = name
+    name = "new map name"
+    post_data["name"] = name
     response = cookieclient.post(url, post_data)
     assert response.status_code == 200
     j = json.loads(response.content.decode())
     updated_map = Map.objects.get(pk=anonymap.pk)
-    assert j['id'] == updated_map.pk
+    assert j["id"] == updated_map.pk
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_anonymous_delete(cookieclient, anonymap):
-    url = reverse('map_delete', args=(anonymap.pk, ))
+    url = reverse("map_delete", args=(anonymap.pk,))
     response = cookieclient.post(url, {}, follow=True)
     assert response.status_code == 200
     assert not Map.objects.filter(pk=anonymap.pk).count()
     # Test response is a json
     j = json.loads(response.content.decode())
-    assert 'redirect' in j
+    assert "redirect" in j
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_no_cookie_cant_delete(client, anonymap):
-    url = reverse('map_delete', args=(anonymap.pk, ))
+    url = reverse("map_delete", args=(anonymap.pk,))
     response = client.post(url, {}, follow=True)
     assert response.status_code == 403
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_anonymous_edit_url(cookieclient, anonymap):
     url = anonymap.get_anonymous_edit_url()
-    canonical = reverse('map', kwargs={'pk': anonymap.pk,
-                                       'slug': anonymap.slug})
+    canonical = reverse("map", kwargs={"pk": anonymap.pk, "slug": anonymap.slug})
     response = cookieclient.get(url)
     assert response.status_code == 302
-    assert response['Location'] == canonical
+    assert response["Location"] == canonical
     key, value = anonymap.signed_cookie_elements
     assert key in cookieclient.cookies
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_sha1_anonymous_edit_url(cookieclient, anonymap):
-    signer = Signer(algorithm='sha1')
+    signer = Signer(algorithm="sha1")
     signature = signer.sign(anonymap.pk)
-    url = reverse('map_anonymous_edit_url', kwargs={'signature': signature})
-    canonical = reverse('map', kwargs={'pk': anonymap.pk,
-                                       'slug': anonymap.slug})
+    url = reverse("map_anonymous_edit_url", kwargs={"signature": signature})
+    canonical = reverse("map", kwargs={"pk": anonymap.pk, "slug": anonymap.slug})
     response = cookieclient.get(url)
     assert response.status_code == 302
-    assert response['Location'] == canonical
+    assert response["Location"] == canonical
     key, value = anonymap.signed_cookie_elements
     assert key in cookieclient.cookies
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_bad_anonymous_edit_url_should_return_403(cookieclient, anonymap):
     url = anonymap.get_anonymous_edit_url()
     url = reverse(
-        'map_anonymous_edit_url',
-        kwargs={'signature': "%s:badsignature" % anonymap.pk}
+        "map_anonymous_edit_url", kwargs={"signature": "%s:badsignature" % anonymap.pk}
     )
     response = cookieclient.get(url)
     assert response.status_code == 403
 
 
-@pytest.mark.usefixtures('allow_anonymous')
-def test_clone_anonymous_map_should_not_be_possible_if_user_is_not_allowed(client, anonymap, user):  # noqa
+@pytest.mark.usefixtures("allow_anonymous")
+def test_clone_anonymous_map_should_not_be_possible_if_user_is_not_allowed(
+    client, anonymap, user
+):  # noqa
     assert Map.objects.count() == 1
-    url = reverse('map_clone', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_clone", kwargs={"map_id": anonymap.pk})
     anonymap.edit_status = anonymap.OWNER
     anonymap.save()
     response = client.post(url)
     assert response.status_code == 403
     client.login(username=user.username, password="123123")
     response = client.post(url)
     assert response.status_code == 403
     assert Map.objects.count() == 1
 
 
-@pytest.mark.usefixtures('allow_anonymous')
-def test_clone_map_should_be_possible_if_edit_status_is_anonymous(client, anonymap):  # noqa
+@pytest.mark.usefixtures("allow_anonymous")
+def test_clone_map_should_be_possible_if_edit_status_is_anonymous(
+    client, anonymap
+):  # noqa
     assert Map.objects.count() == 1
-    url = reverse('map_clone', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_clone", kwargs={"map_id": anonymap.pk})
     anonymap.edit_status = anonymap.ANONYMOUS
     anonymap.save()
     response = client.post(url)
     assert response.status_code == 200
     assert Map.objects.count() == 2
-    clone = Map.objects.latest('pk')
+    clone = Map.objects.latest("pk")
     assert clone.pk != anonymap.pk
-    assert clone.name == 'Clone of ' + anonymap.name
+    assert clone.name == "Clone of " + anonymap.name
     assert clone.owner is None
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_anyone_can_access_anonymous_map(cookieclient, anonymap):
-    url = reverse('map', args=(anonymap.slug, anonymap.pk))
+    url = reverse("map", args=(anonymap.slug, anonymap.pk))
     anonymap.share_status = anonymap.PUBLIC
     response = cookieclient.get(url)
     assert response.status_code == 200
     anonymap.share_status = anonymap.OPEN
     response = cookieclient.get(url)
     assert response.status_code == 200
     anonymap.share_status = anonymap.PRIVATE
     response = cookieclient.get(url)
     assert response.status_code == 200
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_map_attach_owner(cookieclient, anonymap, user):
-    url = reverse('map_attach_owner', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_attach_owner", kwargs={"map_id": anonymap.pk})
     cookieclient.login(username=user.username, password="123123")
     assert anonymap.owner is None
     response = cookieclient.post(url)
     assert response.status_code == 200
     map = Map.objects.get(pk=anonymap.pk)
     assert map.owner == user
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_map_attach_owner_not_logged_in(cookieclient, anonymap, user):
-    url = reverse('map_attach_owner', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_attach_owner", kwargs={"map_id": anonymap.pk})
     assert anonymap.owner is None
     response = cookieclient.post(url)
     assert response.status_code == 403
 
 
-@pytest.mark.usefixtures('allow_anonymous')
+@pytest.mark.usefixtures("allow_anonymous")
 def test_map_attach_owner_with_already_an_owner(cookieclient, map, user):
-    url = reverse('map_attach_owner', kwargs={'map_id': map.pk})
+    url = reverse("map_attach_owner", kwargs={"map_id": map.pk})
     cookieclient.login(username=user.username, password="123123")
     assert map.owner
     assert map.owner != user
     response = cookieclient.post(url)
     assert response.status_code == 403
 
 
 def test_map_attach_owner_anonymous_not_allowed(cookieclient, anonymap, user):
-    url = reverse('map_attach_owner', kwargs={'map_id': anonymap.pk})
+    url = reverse("map_attach_owner", kwargs={"map_id": anonymap.pk})
     cookieclient.login(username=user.username, password="123123")
     assert anonymap.owner is None
     response = cookieclient.post(url)
     assert response.status_code == 403
 
     # # GET anonymous
     # response = client.get(url)
@@ -520,52 +519,81 @@
     # client.login(username=user.username, password="123123")
     # response = client.post(url, {})
     # assert response.status_code == 403
 
 
 def test_create_readonly(client, user, post_data, settings):
     settings.UMAP_READONLY = True
-    url = reverse('map_create')
+    url = reverse("map_create")
     client.login(username=user.username, password="123123")
     response = client.post(url, post_data)
     assert response.status_code == 403
-    assert response.content == b'Site is readonly for maintenance'
+    assert response.content == b"Site is readonly for maintenance"
 
 
 def test_search(client, map):
     # Very basic search, that do not deal with accent nor case.
     # See install.md for how to have a smarter dict + index.
     map.name = "Blé dur"
     map.save()
     url = reverse("search")
     response = client.get(url + "?q=Blé")
     assert "Blé dur" in response.content.decode()
 
 
 def test_authenticated_user_can_star_map(client, map, user):
-    url = reverse('map_star', args=(map.pk,))
+    url = reverse("map_star", args=(map.pk,))
     client.login(username=user.username, password="123123")
     assert Star.objects.filter(by=user).count() == 0
     response = client.post(url)
     assert response.status_code == 200
     assert Star.objects.filter(by=user).count() == 1
 
 
 def test_anonymous_cannot_star_map(client, map):
-    url = reverse('map_star', args=(map.pk,))
+    url = reverse("map_star", args=(map.pk,))
     assert Star.objects.count() == 0
     response = client.post(url)
     assert response.status_code == 302
     assert "login" in response["Location"]
     assert Star.objects.count() == 0
 
 
 def test_user_can_see_their_star(client, map, user):
-    url = reverse('map_star', args=(map.pk,))
+    url = reverse("map_star", args=(map.pk,))
     client.login(username=user.username, password="123123")
     assert Star.objects.filter(by=user).count() == 0
     response = client.post(url)
     assert response.status_code == 200
-    url = reverse('user_stars', args=(user.username,))
+    url = reverse("user_stars", args=(user.username,))
     response = client.get(url)
     assert response.status_code == 200
     assert map.name in response.content.decode()
+
+
+@pytest.mark.usefixtures("allow_anonymous")
+def test_cannot_send_link_on_owned_map(client, map):
+    assert len(mail.outbox) == 0
+    url = reverse("map_send_edit_link", args=(map.pk,))
+    resp = client.post(url, {"email": "foo@bar.org"})
+    assert resp.status_code == 200
+    assert json.loads(resp.content.decode()) == {"login_required": "/en/login/"}
+    assert len(mail.outbox) == 0
+
+
+@pytest.mark.usefixtures("allow_anonymous")
+def test_cannot_send_link_on_anonymous_map_without_cookie(client, anonymap):
+    assert len(mail.outbox) == 0
+    url = reverse("map_send_edit_link", args=(anonymap.pk,))
+    resp = client.post(url, {"email": "foo@bar.org"})
+    assert resp.status_code == 403
+    assert len(mail.outbox) == 0
+
+
+@pytest.mark.usefixtures("allow_anonymous")
+def test_can_send_link_on_anonymous_map_with_cookie(cookieclient, anonymap):
+    assert len(mail.outbox) == 0
+    url = reverse("map_send_edit_link", args=(anonymap.pk,))
+    resp = cookieclient.post(url, {"email": "foo@bar.org"})
+    assert resp.status_code == 200
+    assert len(mail.outbox) == 1
+    assert mail.outbox[0].subject == "The uMap edit link for your map: test map"
```

### Comparing `umap-project-1.3.0a0/umap/tests/test_tilelayer.py` & `umap-project-1.3.1/umap/tests/test_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/tests/test_views.py` & `umap-project-1.3.1/umap/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,25 @@
     response = client.get(url, params, **headers)
     assert response.status_code == 200
     assert "Example Domain" in response.content.decode()
     assert "Cookie" not in response["Vary"]
     assert "X-Accel-Expires" not in response
 
 
+def test_invalid_proxy_url_should_return_400(client):
+    url = reverse("ajax-proxy")
+    params = {"url": "http://example.org/a space is invalid"}
+    headers = {
+        "HTTP_X_REQUESTED_WITH": "XMLHttpRequest",
+        "HTTP_REFERER": settings.SITE_URL,
+    }
+    response = client.get(url, params, **headers)
+    assert response.status_code == 400
+
+
 @pytest.mark.django_db
 def test_login_does_not_contain_form_if_not_enabled(client, settings):
     settings.ENABLE_ACCOUNT_LOGIN = False
     response = client.get(reverse("login"))
     assert "username" not in response.content.decode()
```

### Comparing `umap-project-1.3.0a0/umap/urls.py` & `umap-project-1.3.1/umap/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,15 @@
     [login_required],
     re_path(
         r"^map/(?P<map_id>[\d]+)/star/$",
         views.ToggleMapStarStatus.as_view(),
         name="map_star",
     ),
 )
-i18n_urls += decorated_patterns(
-    [map_permissions_check, never_cache],
+map_urls = [
     re_path(
         r"^map/(?P<map_id>[\d]+)/update/settings/$",
         views.MapUpdate.as_view(),
         name="map_update",
     ),
     re_path(
         r"^map/(?P<map_id>[\d]+)/update/permissions/$",
@@ -137,15 +136,24 @@
         name="datalayer_update",
     ),
     re_path(
         r"^map/(?P<map_id>[\d]+)/datalayer/delete/(?P<pk>\d+)/$",
         views.DataLayerDelete.as_view(),
         name="datalayer_delete",
     ),
-)
+]
+if settings.FROM_EMAIL:
+    map_urls.append(
+        re_path(
+            r"^map/(?P<map_id>[\d]+)/send-edit-link/$",
+            views.SendEditLink.as_view(),
+            name="map_send_edit_link",
+        )
+    )
+i18n_urls += decorated_patterns([map_permissions_check, never_cache], *map_urls)
 urlpatterns += i18n_patterns(
     re_path(r"^$", views.home, name="home"),
     re_path(
         r"^showcase/$", cache_page(24 * 60 * 60)(views.showcase), name="maps_showcase"
     ),
     re_path(r"^search/$", views.search, name="search"),
     re_path(r"^about/$", views.about, name="about"),
```

### Comparing `umap-project-1.3.0a0/umap/utils.py` & `umap-project-1.3.1/umap/utils.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap/views.py` & `umap-project-1.3.1/umap/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import mimetypes
 import os
 import re
 import socket
 from datetime import date, timedelta
+from http.client import InvalidURL
 from pathlib import Path
+from urllib.error import URLError
 
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth import logout as do_logout
 from django.contrib.auth import get_user_model
 from django.contrib.gis.measure import D
 from django.contrib.postgres.search import SearchQuery, SearchVector
+from django.core.mail import send_mail
 from django.core.paginator import EmptyPage, PageNotAnInteger, Paginator
 from django.core.signing import BadSignature, Signer
 from django.core.validators import URLValidator, ValidationError
 from django.db.models import Q
 from django.http import (
     HttpResponse,
     HttpResponseBadRequest,
@@ -29,25 +32,26 @@
 from django.utils.encoding import smart_bytes
 from django.utils.http import http_date
 from django.utils.translation import gettext as _
 from django.utils.translation import to_locale
 from django.views.generic import DetailView, TemplateView, View
 from django.views.generic.base import RedirectView
 from django.views.generic.detail import BaseDetailView
-from django.views.generic.edit import CreateView, DeleteView, UpdateView
+from django.views.generic.edit import CreateView, DeleteView, FormView, UpdateView
 from django.views.generic.list import ListView
 
 from .forms import (
     DEFAULT_LATITUDE,
     DEFAULT_LONGITUDE,
     DEFAULT_CENTER,
     AnonymousMapPermissionsForm,
     DataLayerForm,
     FlatErrorList,
     MapSettingsForm,
+    SendLinkForm,
     UpdateMapPermissionsForm,
 )
 from .models import DataLayer, Licence, Map, Pictogram, Star, TileLayer
 from .utils import get_uri_template, gzip_file, is_ajax
 
 try:
     # python3
@@ -299,14 +303,18 @@
         headers = {"User-Agent": "uMapProxy +http://wiki.openstreetmap.org/wiki/UMap"}
         request = Request(url, headers=headers)
         opener = build_opener()
         try:
             proxied_request = opener.open(request)
         except HTTPError as e:
             return HttpResponse(e.msg, status=e.code, content_type="text/plain")
+        except URLError:
+            return HttpResponseBadRequest("URL error")
+        except InvalidURL:
+            return HttpResponseBadRequest("Invalid URL")
         else:
             status_code = proxied_request.code
             mimetype = proxied_request.headers.get(
                 "Content-Type"
             ) or mimetypes.guess_type(
                 url
             )  # noqa
@@ -462,21 +470,17 @@
                 {
                     "id": editor.pk,
                     "name": editor.get_username(),
                 }
                 for editor in self.object.editors.all()
             ]
         if not self.object.owner and self.object.is_anonymous_owner(self.request):
-            permissions["anonymous_edit_url"] = self.get_anonymous_edit_url()
+            permissions["anonymous_edit_url"] = self.object.get_anonymous_edit_url()
         return permissions
 
-    def get_anonymous_edit_url(self):
-        anonymous_url = self.object.get_anonymous_edit_url()
-        return settings.SITE_URL + anonymous_url
-
 
 class MapView(MapDetailMixin, PermissionsMixin, DetailView):
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
         canonical = self.get_canonical_url()
         if not request.path == canonical:
             if request.META.get("QUERY_STRING"):
@@ -537,31 +541,22 @@
     model = Map
     form_class = MapSettingsForm
 
     def form_valid(self, form):
         if self.request.user.is_authenticated:
             form.instance.owner = self.request.user
         self.object = form.save()
-        anonymous_url = self.get_anonymous_edit_url()
-        if not self.request.user.is_authenticated:
-            msg = _(
-                "Your map has been created! If you want to edit this map from "
-                "another computer, please use this link: %(anonymous_url)s"
-                % {"anonymous_url": anonymous_url}
-            )
-        else:
-            msg = _("Congratulations, your map has been created!")
+        anonymous_url = self.object.get_anonymous_edit_url()
         permissions = self.get_permissions()
         # User does not have the cookie yet.
         permissions["anonymous_edit_url"] = anonymous_url
         response = simple_json_response(
             id=self.object.pk,
             url=self.object.get_absolute_url(),
             permissions=permissions,
-            info=msg,
         )
         if not self.request.user.is_authenticated:
             key, value = self.object.signed_cookie_elements
             response.set_signed_cookie(
                 key=key, value=value, max_age=ANONYMOUS_COOKIE_MAX_AGE
             )
         return response
@@ -618,14 +613,44 @@
         ):
             return HttpResponseForbidden()
         self.object.owner = self.request.user
         self.object.save()
         return simple_json_response()
 
 
+class SendEditLink(FormLessEditMixin, FormView):
+    form_class = SendLinkForm
+
+    def post(self, form, **kwargs):
+        self.object = kwargs["map_inst"]
+        if (
+            self.object.owner
+            or not self.object.is_anonymous_owner(self.request)
+            or not self.object.can_edit(self.request.user, self.request)
+        ):
+            return HttpResponseForbidden()
+        form = self.get_form()
+        if form.is_valid():
+            email = form.cleaned_data["email"]
+        else:
+            return HttpResponseBadRequest("Invalid")
+        link = self.object.get_anonymous_edit_url()
+
+        send_mail(
+            _("The uMap edit link for your map: %(map_name)s" % {"map_name": self.object.name}),
+            _("Here is your secret edit link: %(link)s" % {"link": link}),
+            settings.FROM_EMAIL,
+            [email],
+            fail_silently=False,
+        )
+        return simple_json_response(
+            info=_("Email sent to %(email)s" % {"email": email})
+        )
+
+
 class MapDelete(DeleteView):
     model = Map
     pk_url_kwarg = "map_id"
 
     def form_valid(self, form):
         self.object = self.get_object()
         if self.object.owner and self.request.user != self.object.owner:
@@ -650,15 +675,15 @@
             key, value = self.object.signed_cookie_elements
             response.set_signed_cookie(
                 key=key, value=value, max_age=ANONYMOUS_COOKIE_MAX_AGE
             )
             msg = _(
                 "Your map has been cloned! If you want to edit this map from "
                 "another computer, please use this link: %(anonymous_url)s"
-                % {"anonymous_url": self.get_anonymous_edit_url()}
+                % {"anonymous_url": self.object.get_anonymous_edit_url()}
             )
         else:
             msg = _("Congratulations, your map has been cloned!")
         messages.info(self.request, msg)
         return response
```

### Comparing `umap-project-1.3.0a0/umap/wsgi.py` & `umap-project-1.3.1/umap/wsgi.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.0a0/umap_project.egg-info/PKG-INFO` & `umap-project-1.3.1/umap_project.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.3.0a0
+Version: 1.3.1
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
 Author: Yohan Boniface
 Keywords: django leaflet geodjango openstreetmap map
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -28,13 +28,13 @@
 [![Requirements Status](https://requires.io/github/umap-project/umap/requirements.svg?branch=master)](https://requires.io/github/umap-project/umap/requirements/?branch=master)
 [![Join the chat at https://gitter.im/umap-project/umap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/umap-project/umap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Documentation Status](https://readthedocs.org/projects/umap-project/badge/?version=latest)](http://umap-project.readthedocs.io/en/latest/?badge=latest)[![Build Status](https://travis-ci.org/umap-project/umap.svg?branch=master)](https://travis-ci.org/umap-project/umap)
 
 ## About
 
 uMap lets you create maps with OpenStreetMap layers in a minute and embed them in your site.
 *Because we think that the more OSM will be used, the more OSM will be improved.*
-It uses [django-leaflet-storage](https://github.com/umap-project/django-leaflet-storage) and [Leaflet.Storage](https://github.com/umap-project/Leaflet.Storage),  built on top of Django and Leaflet.
+Built on top of Django and Leaflet.
 
 
 ## Installation and configuration
 
 See [developer documentation](https://umap-project.readthedocs.io/en/latest/install/).
```

### Comparing `umap-project-1.3.0a0/umap_project.egg-info/SOURCES.txt` & `umap-project-1.3.1/umap_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

