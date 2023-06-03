# Comparing `tmp/mbase-0.0.1.tar.gz` & `tmp/mbase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbase-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mbase-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mbase-0.0.1.tar` & `mbase-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3090 2023-05-29 05:57:47.185851 mbase-0.0.1/.gitignore
--rw-r--r--   0        0        0        4 2023-06-03 20:00:36.415875 mbase-0.0.1/LICENSE
--rw-r--r--   0        0        0     1939 2023-06-03 20:04:57.987030 mbase-0.0.1/Makefile
--rw-r--r--   0        0        0       90 2023-05-29 05:54:55.382142 mbase-0.0.1/README.md
--rw-r--r--   0        0        0        6 2023-05-31 06:00:54.518458 mbase-0.0.1/VERSION
--rw-r--r--   0        0        0     6148 2022-02-16 17:13:36.168907 mbase-0.0.1/docs/.DS_Store
--rw-r--r--   0        0        0      638 2022-02-14 21:51:19.000000 mbase-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2022-02-14 21:51:19.000000 mbase-0.0.1/docs/make.bat
--rw-r--r--   0        0        0     2252 2023-05-30 07:29:16.202817 mbase-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      513 2023-05-30 04:52:49.017528 mbase-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0       89 2023-05-30 04:38:20.375048 mbase-0.0.1/docs/source/mbase/eventlog.rst
--rw-r--r--   0        0        0       80 2023-05-30 04:52:11.924670 mbase-0.0.1/docs/source/mbase/services.rst
--rw-r--r--   0        0        0       65 2023-05-30 04:49:31.167705 mbase-0.0.1/docs/source/mbase/utils.rst
--rw-r--r--   0        0        0        0 2023-05-29 05:54:36.692581 mbase-0.0.1/mbase/__init__.py
--rw-r--r--   0        0        0     7792 2023-05-30 07:32:56.751342 mbase-0.0.1/mbase/eventlog.py
--rw-r--r--   0        0        0      859 2023-05-29 05:54:36.702787 mbase-0.0.1/mbase/exceptions.py
--rw-r--r--   0        0        0    21987 2023-05-29 17:52:37.309182 mbase-0.0.1/mbase/future.py
--rw-r--r--   0        0        0      946 2023-05-31 05:37:13.359364 mbase-0.0.1/mbase/mlogging.py
--rw-r--r--   0        0        0     7302 2023-05-31 06:00:47.348683 mbase-0.0.1/mbase/models.py
--rw-r--r--   0        0        0     3144 2023-05-29 18:02:21.856877 mbase-0.0.1/mbase/services.py
--rw-r--r--   0        0        0    10981 2023-05-31 05:36:39.195619 mbase-0.0.1/mbase/utils.py
--rw-r--r--   0        0        0      663 2023-06-03 19:59:30.720709 mbase-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      201 2023-05-30 04:53:44.125364 mbase-0.0.1/requirements.txt
--rw-r--r--   0        0        0      231 2023-05-30 07:30:16.717215 mbase-0.0.1/settings.py
--rw-r--r--   0        0        0     1395 2023-05-29 18:25:25.194121 mbase-0.0.1/setup.py
--rw-r--r--   0        0        0     1840 2023-05-29 05:54:44.625161 mbase-0.0.1/tests/models_test.py
--rw-r--r--   0        0        0     1491 2023-05-29 18:04:30.312916 mbase-0.0.1/tests/service_test.py
--rw-r--r--   0        0        0     3775 2023-05-29 06:42:45.874857 mbase-0.0.1/tests/utils_test.py
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 mbase-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3090 2023-05-29 05:57:47.185851 mbase-0.0.2/.gitignore
+-rw-r--r--   0        0        0        4 2023-06-03 20:00:36.415875 mbase-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1975 2023-06-03 20:16:15.868357 mbase-0.0.2/Makefile
+-rw-r--r--   0        0        0       90 2023-05-29 05:54:55.382142 mbase-0.0.2/README.md
+-rw-r--r--   0        0        0        6 2023-05-31 06:00:54.518458 mbase-0.0.2/VERSION
+-rw-r--r--   0        0        0     6148 2022-02-16 17:13:36.168907 mbase-0.0.2/docs/.DS_Store
+-rw-r--r--   0        0        0      638 2022-02-14 21:51:19.000000 mbase-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-02-14 21:51:19.000000 mbase-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     2252 2023-05-30 07:29:16.202817 mbase-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      513 2023-05-30 04:52:49.017528 mbase-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0       89 2023-05-30 04:38:20.375048 mbase-0.0.2/docs/source/mbase/eventlog.rst
+-rw-r--r--   0        0        0       80 2023-05-30 04:52:11.924670 mbase-0.0.2/docs/source/mbase/services.rst
+-rw-r--r--   0        0        0       65 2023-05-30 04:49:31.167705 mbase-0.0.2/docs/source/mbase/utils.rst
+-rw-r--r--   0        0        0        0 2023-05-29 05:54:36.692581 mbase-0.0.2/mbase/__init__.py
+-rw-r--r--   0        0        0     7792 2023-05-30 07:32:56.751342 mbase-0.0.2/mbase/eventlog.py
+-rw-r--r--   0        0        0      859 2023-05-29 05:54:36.702787 mbase-0.0.2/mbase/exceptions.py
+-rw-r--r--   0        0        0    21987 2023-05-29 17:52:37.309182 mbase-0.0.2/mbase/future.py
+-rw-r--r--   0        0        0      946 2023-05-31 05:37:13.359364 mbase-0.0.2/mbase/mlogging.py
+-rw-r--r--   0        0        0     7302 2023-05-31 06:00:47.348683 mbase-0.0.2/mbase/models.py
+-rw-r--r--   0        0        0     3144 2023-05-29 18:02:21.856877 mbase-0.0.2/mbase/services.py
+-rw-r--r--   0        0        0    10981 2023-05-31 05:36:39.195619 mbase-0.0.2/mbase/utils.py
+-rw-r--r--   0        0        0      699 2023-06-03 20:14:55.159843 mbase-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-05-30 04:53:44.125364 mbase-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      231 2023-05-30 07:30:16.717215 mbase-0.0.2/settings.py
+-rw-r--r--   0        0        0     1395 2023-05-29 18:25:25.194121 mbase-0.0.2/setup.py
+-rw-r--r--   0        0        0     1840 2023-05-29 05:54:44.625161 mbase-0.0.2/tests/models_test.py
+-rw-r--r--   0        0        0     1491 2023-05-29 18:04:30.312916 mbase-0.0.2/tests/service_test.py
+-rw-r--r--   0        0        0     3775 2023-05-29 06:42:45.874857 mbase-0.0.2/tests/utils_test.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mbase-0.0.2/PKG-INFO
```

### Comparing `mbase-0.0.1/.gitignore` & `mbase-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/Makefile` & `mbase-0.0.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,15 @@
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = docs/source
 BUILDDIR      = docs/build
 
 .PHONY: docs
 docs:  ## Generate documentation
 	@$(SPHINXBUILD) -M html "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(0)
+	touch docs
 
-build:  ## Build mbase using flit
+build:  docs ## Build mbase using flit
 	flit build
 
-publish:  ## Publish to PyPI
+publish: mbase   ## Publish to PyPI
     flit publish
+	touch dist
```

### Comparing `mbase-0.0.1/docs/.DS_Store` & `mbase-0.0.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/docs/Makefile` & `mbase-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/docs/make.bat` & `mbase-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/docs/source/conf.py` & `mbase-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/docs/source/index.rst` & `mbase-0.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/eventlog.py` & `mbase-0.0.2/mbase/eventlog.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/exceptions.py` & `mbase-0.0.2/mbase/exceptions.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/future.py` & `mbase-0.0.2/mbase/future.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/mlogging.py` & `mbase-0.0.2/mbase/mlogging.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/models.py` & `mbase-0.0.2/mbase/models.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/services.py` & `mbase-0.0.2/mbase/services.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/mbase/utils.py` & `mbase-0.0.2/mbase/utils.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/setup.py` & `mbase-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/tests/models_test.py` & `mbase-0.0.2/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/tests/service_test.py` & `mbase-0.0.2/tests/service_test.py`

 * *Files identical despite different names*

### Comparing `mbase-0.0.1/tests/utils_test.py` & `mbase-0.0.2/tests/utils_test.py`

 * *Files identical despite different names*

