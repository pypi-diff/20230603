# Comparing `tmp/ytsaurus-spyt-1.70.1b451.post25341090.dev21.tar.gz` & `tmp/ytsaurus-spyt-1.70.1b451.post5605632.dev23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b451.post25341090.dev21.tar", last modified: Fri Jun  2 00:48:43 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b451.post5605632.dev23.tar", last modified: Fri Jun  2 20:25:31 2023, max compression
```

## Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21.tar` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      323 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/PKG-INFO
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798377 2023-06-02 00:48:42.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/jars/spark-yt-submit.jar
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/setup.cfg
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/setup.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      183 2023-06-02 00:47:41.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      323 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-06-02 00:48:43.000000 ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/top_level.txt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      322 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/PKG-INFO
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798377 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/jars/spark-yt-submit.jar
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/setup.cfg
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/setup.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-06-02 20:24:26.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      322 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-06-02 20:25:31.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-06-02 20:25:30.000000 ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/top_level.txt
```

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/setup.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/setup.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/client.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/common.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/conf.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/enabler.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/standalone.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/standalone.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/submit.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/types.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/spyt/utils.py` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b451.post25341090.dev21/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.70.1b451.post5605632.dev23/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

