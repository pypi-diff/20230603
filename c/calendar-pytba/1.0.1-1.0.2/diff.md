# Comparing `tmp/calendar_pytba-1.0.1.tar.gz` & `tmp/calendar_pytba-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_pytba-1.0.1.tar", max compression
+gzip compressed data, was "calendar_pytba-1.0.2.tar", max compression
```

## Comparing `calendar_pytba-1.0.1.tar` & `calendar_pytba-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/LICENSE
--rw-r--r--   0        0        0       41 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/main.py
--rw-r--r--   0        0        0        0 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/__init__.py
--rw-r--r--   0        0        0     3944 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/handler.py
--rw-r--r--   0        0        0     2315 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/text.py
--rw-r--r--   0        0        0      444 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/types.py
--rw-r--r--   0        0        0      374 2023-06-03 09:21:07.444210 calendar_pytba-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      662 2023-06-03 09:21:07.444210 calendar_pytba-1.0.1/readme.md
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 calendar_pytba-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/LICENSE
+-rw-r--r--   0        0        0       41 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/__init__.py
+-rw-r--r--   0        0        0     6995 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/main.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/__init__.py
+-rw-r--r--   0        0        0     3944 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/handler.py
+-rw-r--r--   0        0        0     2315 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/text.py
+-rw-r--r--   0        0        0      444 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/types.py
+-rw-r--r--   0        0        0      373 2023-06-03 09:27:36.495600 calendar_pytba-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-06-03 09:27:36.495600 calendar_pytba-1.0.2/readme.md
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 calendar_pytba-1.0.2/PKG-INFO
```

### Comparing `calendar_pytba-1.0.1/LICENSE` & `calendar_pytba-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.1/calendar_pytba/main.py` & `calendar_pytba-1.0.2/calendar_pytba/main.py`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.1/calendar_pytba/utils/handler.py` & `calendar_pytba-1.0.2/calendar_pytba/utils/handler.py`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.1/calendar_pytba/utils/text.py` & `calendar_pytba-1.0.2/calendar_pytba/utils/text.py`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.1/readme.md` & `calendar_pytba-1.0.2/readme.md`

 * *Files identical despite different names*

