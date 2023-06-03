# Comparing `tmp/funtoo-metatools-1.3.0.tar.gz` & `tmp/funtoo-metatools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-metatools-1.3.0.tar", last modified: Tue May 30 01:30:24 2023, max compression
+gzip compressed data, was "funtoo-metatools-1.3.1.tar", last modified: Sat Jun  3 19:14:46 2023, max compression
```

## Comparing `funtoo-metatools-1.3.0.tar` & `funtoo-metatools-1.3.1.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6778 2023-05-30 01:28:18.000000 funtoo-metatools-1.3.0/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-05-30 01:28:36.000000 funtoo-metatools-1.3.0/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.967848 funtoo-metatools-1.3.0/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.0/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-09-27 00:51:20.000000 funtoo-metatools-1.3.0/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.0/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.967848 funtoo-metatools-1.3.0/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.0/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23260 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-05-10 22:44:54.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2007 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      511 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/blos.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5547 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8854 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27038 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21741 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11361 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-05-30 01:30:21.000000 funtoo-metatools-1.3.0/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/yaml_util.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/zmq/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/app_core.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/key_monkey.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_breezyops.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-05-30 01:30:21.000000 funtoo-metatools-1.3.0/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.0/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7697 2023-06-03 19:14:17.000000 funtoo-metatools-1.3.1/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-06-03 19:09:39.000000 funtoo-metatools-1.3.1/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.263907 funtoo-metatools-1.3.1/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.1/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-09-27 00:51:20.000000 funtoo-metatools-1.3.1/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.1/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.1/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.263907 funtoo-metatools-1.3.1/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.1/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23260 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-05-10 22:44:54.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.267907 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2033 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-06-03 19:14:46.000000 funtoo-metatools-1.3.1/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-03 19:14:35.000000 funtoo-metatools-1.3.1/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/blos.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5547 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.1/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8854 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27038 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21741 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11722 2023-06-03 19:10:01.000000 funtoo-metatools-1.3.1/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-06-03 19:14:42.000000 funtoo-metatools-1.3.1/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/metatools/zmq/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:08:14.000000 funtoo-metatools-1.3.1/metatools/zmq/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-06-03 19:14:46.271907 funtoo-metatools-1.3.1/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-06-03 19:14:42.000000 funtoo-metatools-1.3.1/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.1/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.1/subpop.yaml
```

### Comparing `funtoo-metatools-1.3.0/.pre-commit-config.yaml` & `funtoo-metatools-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/ChangeLog.rst` & `funtoo-metatools-1.3.1/ChangeLog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+metatools 1.3.1
+===============
+
+Released on June 3, 2023.
+
+This is a bugfix release.
+
+* Add a missing __init__.py to ``metatools/zmq`` so that these
+  source files get included in the distribution. This fixes a
+  traceback due to these missing files which prevented the 
+  distributed PyPi source from working.
+* If ``doit`` was interrupted, it could write incomplete JSON
+  to disk using ``FileStorageBackend``. In this case, the JSON
+  will be corrupt and the retrieved data will be invalid, and
+  there was no obvious way to clear out this corrupt data.
+  This would result in cached JSON data from ``get_page()``
+  being invalid and re-running ``doit`` would not fix this.
+  So a fix was added so that any corrupt entries in
+  ``FileStorageBackend`` will be treated as if they don't exist
+  (returning a ``CacheMiss()``) which will allow ``doit`` to
+  overwite these corrupt entries with new, corrected entries.
+
 metatools 1.3.0
 ===============
 
 Released on May 29, 2023.
 
 This is a feature release containing a number of new capabilities
 and improvements.
@@ -126,8 +148,8 @@
   restarted to append the contents of the new download at the end of
   the aborted file. This now works properly.
 * Fix ``bin/merge-gentoo-staging`` (FL-10850: thanks: borisp)
 * Minor fix to .zst archive handling for dynamic archives.
 * Rework of error handling, fixes related to aggregating errors (FL-10556)
 * Add GitHub tag pagination using async generators (thanks: invakid404)
 * Allow ``create_branches=True`` with a GitTree to create missing branches
-  even in prod mode.
+  even in prod mode.
```

### Comparing `funtoo-metatools-1.3.0/PKG-INFO` & `funtoo-metatools-1.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.0
+Version: 1.3.1
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.0/README.rst` & `funtoo-metatools-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/blos` & `funtoo-metatools-1.3.1/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/deepdive` & `funtoo-metatools-1.3.1/bin/deepdive`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/deepquery` & `funtoo-metatools-1.3.1/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/distfile-kit-fetch` & `funtoo-metatools-1.3.1/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/distfile-stats` & `funtoo-metatools-1.3.1/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/doit` & `funtoo-metatools-1.3.1/bin/doit`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/fastpull-daemon` & `funtoo-metatools-1.3.1/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/fastpull-daemon-ng` & `funtoo-metatools-1.3.1/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/fastpull-fixer` & `funtoo-metatools-1.3.1/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/fetch` & `funtoo-metatools-1.3.1/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/interkit-links` & `funtoo-metatools-1.3.1/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/list-kits` & `funtoo-metatools-1.3.1/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/mcafee-tool` & `funtoo-metatools-1.3.1/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/merge-gentoo-staging` & `funtoo-metatools-1.3.1/bin/merge-gentoo-staging`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/merge-kits` & `funtoo-metatools-1.3.1/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/missing-links` & `funtoo-metatools-1.3.1/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/release-yaml-test` & `funtoo-metatools-1.3.1/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/reposcan` & `funtoo-metatools-1.3.1/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/storage-test` & `funtoo-metatools-1.3.1/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/bin/test-metadata-extract` & `funtoo-metatools-1.3.1/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/deprecated/mongo_backends.py` & `funtoo-metatools-1.3.1/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/Makefile` & `funtoo-metatools-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.3.1/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.3.1/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/autogen-dev.rst` & `funtoo-metatools-1.3.1/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/autogen.rst` & `funtoo-metatools-1.3.1/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/conf.py` & `funtoo-metatools-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.3.1/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.3.1/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.3.1/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/index.rst` & `funtoo-metatools-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/install.rst` & `funtoo-metatools-1.3.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/intro.rst` & `funtoo-metatools-1.3.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/docs/meta-repo.rst` & `funtoo-metatools-1.3.1/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/ebuild.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/fetch.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/fetch.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/github.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/github.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/golang.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/golang.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/http.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/http.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo/pkgtools/rust.py` & `funtoo-metatools-1.3.1/funtoo/pkgtools/rust.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.3.1/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.0
+Version: 1.3.1
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.0/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.3.1/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,11 +81,12 @@
 metatools/config/autogen.py
 metatools/config/base.py
 metatools/config/merge.py
 metatools/config/mongodb.py
 metatools/fastpull/__init__.py
 metatools/fastpull/core.py
 metatools/fastpull/spider.py
+metatools/zmq/__init__.py
 metatools/zmq/app_core.py
 metatools/zmq/key_monkey.py
 metatools/zmq/zmq_msg_breezyops.py
 metatools/zmq/zmq_msg_core.py
```

### Comparing `funtoo-metatools-1.3.0/metatools/blos.py` & `funtoo-metatools-1.3.1/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/config/autogen.py` & `funtoo-metatools-1.3.1/metatools/config/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/config/base.py` & `funtoo-metatools-1.3.1/metatools/config/base.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/config/merge.py` & `funtoo-metatools-1.3.1/metatools/config/merge.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/context.py` & `funtoo-metatools-1.3.1/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/fastpull/core.py` & `funtoo-metatools-1.3.1/metatools/fastpull/core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/fastpull/spider.py` & `funtoo-metatools-1.3.1/metatools/fastpull/spider.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/fetch_cache.py` & `funtoo-metatools-1.3.1/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/hashutils.py` & `funtoo-metatools-1.3.1/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/kit.py` & `funtoo-metatools-1.3.1/metatools/kit.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/kit_cache.py` & `funtoo-metatools-1.3.1/metatools/kit_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/metadata.py` & `funtoo-metatools-1.3.1/metatools/metadata.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/model.py` & `funtoo-metatools-1.3.1/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/pretty_logging.py` & `funtoo-metatools-1.3.1/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/steps.py` & `funtoo-metatools-1.3.1/metatools/steps.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/store.py` & `funtoo-metatools-1.3.1/metatools/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import hashlib
+import json
 import os
 from collections import OrderedDict
 from typing import Mapping, Optional
 
 from bson import UuidRepresentation
 from bson.codec_options import TypeRegistry
 from bson.json_util import dumps, JSONOptions, loads
 
+from metatools.model import get_model
+
+model = get_model("metatools")
+
 # Notes:
 #
 # So far, what I have for a FileStore works great, as long as the process/thread has exclusive access
 # to the underlying data since there is no locking.
 #
 # To work around the locking issue, one possibility is to have every datastore fronted by a separate
 # process or distinct, dedicated thread that implements a ZeroMQ protocol that others can connect to
@@ -239,15 +244,19 @@
 	def encode_data(self, data) -> bytes:
 		# We sort the keys so we always have a consistent representation of dictionary keys on disk.
 		return dumps(data, json_options=JSON_OPTIONS, sort_keys=True).encode('utf-8')
 
 	def decode_data(self, path) -> OrderedDict:
 		with open(path, "rb") as f:
 			in_string = f.read().decode("utf-8")
-			return loads(in_string, json_options=JSON_OPTIONS)
+			try:
+				return loads(in_string, json_options=JSON_OPTIONS)
+			except json.decoder.JSONDecodeError as je:
+				model.log.error("!!! Invalid JSON in FileStorageBackend (will be ignored so it can be repaired)", exc_info=je)
+				raise NotFoundError()
 
 	def write(self, data, blob_path=None) -> Optional[StoreObject]:
 		sha = self.store.key_spec.data_as_hash(data)
 		dir_index = f"{sha[0:2]}/{sha[2:4]}/{sha[4:6]}"
 		out_path = f"{self.root}/{dir_index}/{sha}"
 		os.makedirs(os.path.dirname(out_path), exist_ok=True)
 		return self._write_phase2(out_path, data, blob_path)
@@ -281,15 +290,19 @@
 	def read(self, spec_dict) -> Optional[StoreObject]:
 		sha = self.store.key_spec.specdict_as_hash(spec_dict)
 		dir_index = f"{sha[0:2]}/{sha[2:4]}/{sha[4:6]}"
 		in_path = f"{self.root}/{dir_index}/{sha}"
 		if not os.path.exists(in_path):
 			return None
 		blob_path = in_path + ".blob"
-		return StoreObject(data=self.decode_data(in_path), blob_path=blob_path if os.path.exists(blob_path) else None)
+		try:
+			data = self.decode_data(in_path)
+		except json.decoder.JSONDecodeError as je:
+			return None
+		return StoreObject(data=data, blob_path=blob_path if os.path.exists(blob_path) else None)
 
 	def delete(self, spec_dict) -> None:
 		sha = self.store.key_spec.specdict_as_hash(spec_dict)
 		dir_index = f"{sha[0:2]}/{sha[2:4]}/{sha[4:6]}"
 		in_path = f"{self.root}/{dir_index}/{sha}"
 		if os.path.exists(in_path):
 			os.unlink(in_path)
```

### Comparing `funtoo-metatools-1.3.0/metatools/tree.py` & `funtoo-metatools-1.3.1/metatools/tree.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/yaml_util.py` & `funtoo-metatools-1.3.1/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/zmq/app_core.py` & `funtoo-metatools-1.3.1/metatools/zmq/app_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/zmq/key_monkey.py` & `funtoo-metatools-1.3.1/metatools/zmq/key_monkey.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_breezyops.py` & `funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_breezyops.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_core.py` & `funtoo-metatools-1.3.1/metatools/zmq/zmq_msg_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.0/setup.py` & `funtoo-metatools-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.3.0",
+	version="1.3.1",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
```

### Comparing `funtoo-metatools-1.3.0/setup.py.in` & `funtoo-metatools-1.3.1/setup.py.in`

 * *Files identical despite different names*

