# Comparing `tmp/py-cone-1.0.9.tar.gz` & `tmp/py-cone-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-cone-1.0.9.tar", last modified: Wed May 31 09:37:26 2023, max compression
+gzip compressed data, was "py-cone-1.1.0.tar", last modified: Sat Jun  3 03:47:50 2023, max compression
```

## Comparing `py-cone-1.0.9.tar` & `py-cone-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.304181 py-cone-1.0.9/
--rw-rw-rw-   0        0        0     1085 2023-02-21 05:25:29.000000 py-cone-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      220 2023-05-31 09:37:26.303677 py-cone-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-21 05:25:29.000000 py-cone-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.178447 py-cone-1.0.9/cone/
--rw-rw-rw-   0        0        0      105 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.196213 py-cone-1.0.9/cone/communication/
--rw-rw-rw-   0        0        0      141 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/ding_talk.py
--rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/communication/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.199216 py-cone-1.0.9/cone/crypto/
--rw-rw-rw-   0        0        0      123 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/__init__.py
--rw-rw-rw-   0        0        0     1196 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/aes.py
--rw-rw-rw-   0        0        0      238 2023-03-13 01:28:44.000000 py-cone-1.0.9/cone/crypto/md5.py
--rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/crypto/rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.202829 py-cone-1.0.9/cone/hooks/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/__init__.py
--rw-rw-rw-   0        0        0      364 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/exception.py
--rw-rw-rw-   0        0        0     1643 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/lib.py
--rw-rw-rw-   0        0        0      234 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/hooks/signal.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.214168 py-cone-1.0.9/cone/patterns/
--rw-rw-rw-   0        0        0      201 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/__init__.py
--rw-rw-rw-   0        0        0      393 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/instance.py
--rw-rw-rw-   0        0        0      767 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/patterns/singleton.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.237456 py-cone-1.0.9/cone/utils/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/__init__.py
--rw-rw-rw-   0        0        0     6590 2023-03-15 08:06:02.000000 py-cone-1.0.9/cone/utils/classes.py
--rw-rw-rw-   0        0        0     4520 2023-02-21 08:39:35.000000 py-cone-1.0.9/cone/utils/config.py
--rw-rw-rw-   0        0        0     2704 2023-03-10 01:39:26.000000 py-cone-1.0.9/cone/utils/db_utils.py
--rw-rw-rw-   0        0        0    15011 2023-05-31 09:36:43.000000 py-cone-1.0.9/cone/utils/functional.py
--rw-rw-rw-   0        0        0     2310 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/log.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.245093 py-cone-1.0.9/cone/utils/network/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/curl.py
--rw-rw-rw-   0        0        0      814 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/network/url.py
--rw-rw-rw-   0        0        0     1003 2023-02-21 05:25:29.000000 py-cone-1.0.9/cone/utils/os.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.254597 py-cone-1.0.9/py_cone.egg-info/
--rw-rw-rw-   0        0        0      220 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 09:37:26.000000 py-cone-1.0.9/py_cone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 09:37:26.304181 py-cone-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-05-31 09:36:24.000000 py-cone-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:37:26.302360 py-cone-1.0.9/tests/
--rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0      608 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/communication.py
--rw-rw-rw-   0        0        0     2051 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/curl.py
--rw-rw-rw-   0        0        0      499 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/exception.py
--rw-rw-rw-   0        0        0     1114 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/functional.py
--rw-rw-rw-   0        0        0      923 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/hook.py
--rw-rw-rw-   0        0        0      476 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/interrupt.py
--rw-rw-rw-   0        0        0      996 2023-02-21 05:25:29.000000 py-cone-1.0.9/tests/pattern.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.296902 py-cone-1.1.0/
+-rw-rw-rw-   0        0        0     1085 2023-02-21 05:25:29.000000 py-cone-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      220 2023-06-03 03:47:50.296902 py-cone-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-21 05:25:29.000000 py-cone-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.268366 py-cone-1.1.0/cone/
+-rw-rw-rw-   0        0        0      105 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.270365 py-cone-1.1.0/cone/communication/
+-rw-rw-rw-   0        0        0      141 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/communication/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/communication/ding_talk.py
+-rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/communication/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.272365 py-cone-1.1.0/cone/crypto/
+-rw-rw-rw-   0        0        0      123 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-06-03 03:37:21.000000 py-cone-1.1.0/cone/crypto/aes.py
+-rw-rw-rw-   0        0        0      238 2023-03-13 01:28:44.000000 py-cone-1.1.0/cone/crypto/md5.py
+-rw-rw-rw-   0        0        0       99 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/crypto/rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.274365 py-cone-1.1.0/cone/hooks/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/hooks/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/hooks/exception.py
+-rw-rw-rw-   0        0        0     1643 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/hooks/lib.py
+-rw-rw-rw-   0        0        0      234 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/hooks/signal.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.275365 py-cone-1.1.0/cone/patterns/
+-rw-rw-rw-   0        0        0      201 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/patterns/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/patterns/instance.py
+-rw-rw-rw-   0        0        0      767 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/patterns/singleton.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.279883 py-cone-1.1.0/cone/utils/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/__init__.py
+-rw-rw-rw-   0        0        0     6590 2023-03-15 08:06:02.000000 py-cone-1.1.0/cone/utils/classes.py
+-rw-rw-rw-   0        0        0     4520 2023-02-21 08:39:35.000000 py-cone-1.1.0/cone/utils/config.py
+-rw-rw-rw-   0        0        0     2704 2023-03-10 01:39:26.000000 py-cone-1.1.0/cone/utils/db_utils.py
+-rw-rw-rw-   0        0        0    15011 2023-05-31 09:36:43.000000 py-cone-1.1.0/cone/utils/functional.py
+-rw-rw-rw-   0        0        0     2310 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/log.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.281882 py-cone-1.1.0/cone/utils/network/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/network/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/network/curl.py
+-rw-rw-rw-   0        0        0      814 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/network/url.py
+-rw-rw-rw-   0        0        0     1003 2023-02-21 05:25:29.000000 py-cone-1.1.0/cone/utils/os.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.290903 py-cone-1.1.0/py_cone.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-06-03 03:47:50.000000 py-cone-1.1.0/py_cone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-06-03 03:47:50.000000 py-cone-1.1.0/py_cone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:47:50.000000 py-cone-1.1.0/py_cone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 03:47:50.000000 py-cone-1.1.0/py_cone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:47:50.296902 py-cone-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-06-03 03:37:32.000000 py-cone-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:47:50.295912 py-cone-1.1.0/tests/
+-rw-rw-rw-   0        0        0      109 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/communication.py
+-rw-rw-rw-   0        0        0     2051 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/curl.py
+-rw-rw-rw-   0        0        0      499 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/exception.py
+-rw-rw-rw-   0        0        0     1114 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/functional.py
+-rw-rw-rw-   0        0        0      923 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/hook.py
+-rw-rw-rw-   0        0        0      476 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/interrupt.py
+-rw-rw-rw-   0        0        0      996 2023-02-21 05:25:29.000000 py-cone-1.1.0/tests/pattern.py
```

### Comparing `py-cone-1.0.9/LICENSE` & `py-cone-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/communication/ding_talk.py` & `py-cone-1.1.0/cone/communication/ding_talk.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/hooks/lib.py` & `py-cone-1.1.0/cone/hooks/lib.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/patterns/singleton.py` & `py-cone-1.1.0/cone/patterns/singleton.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/classes.py` & `py-cone-1.1.0/cone/utils/classes.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/config.py` & `py-cone-1.1.0/cone/utils/config.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/db_utils.py` & `py-cone-1.1.0/cone/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/functional.py` & `py-cone-1.1.0/cone/utils/functional.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/log.py` & `py-cone-1.1.0/cone/utils/log.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/network/curl.py` & `py-cone-1.1.0/cone/utils/network/curl.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/network/url.py` & `py-cone-1.1.0/cone/utils/network/url.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/cone/utils/os.py` & `py-cone-1.1.0/cone/utils/os.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/py_cone.egg-info/SOURCES.txt` & `py-cone-1.1.0/py_cone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/tests/communication.py` & `py-cone-1.1.0/tests/communication.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/tests/curl.py` & `py-cone-1.1.0/tests/curl.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/tests/functional.py` & `py-cone-1.1.0/tests/functional.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/tests/hook.py` & `py-cone-1.1.0/tests/hook.py`

 * *Files identical despite different names*

### Comparing `py-cone-1.0.9/tests/pattern.py` & `py-cone-1.1.0/tests/pattern.py`

 * *Files identical despite different names*

