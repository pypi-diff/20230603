# Comparing `tmp/modulegraph-0.9.tar.gz` & `tmp/modulegraph-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modulegraph-0.9.tar", last modified: Tue Mar 29 06:19:24 2011, max compression
+gzip compressed data, was "dist/modulegraph-0.9.1.tar", last modified: Sun Jul 24 12:18:33 2011, max compression
```

## Comparing `modulegraph-0.9.tar` & `modulegraph-0.9.1.tar`

### file list

```diff
@@ -1,203 +1,262 @@
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/
--rw-r--r--   0 ronald     (502) staff       (20)    14614 2010-08-22 12:09:33.000000 modulegraph-0.9/distribute_setup.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/doc/
--rw-r--r--   0 ronald     (502) staff       (20)     2614 2011-03-15 12:05:38.000000 modulegraph-0.9/doc/changelog.rst
--rw-r--r--   0 ronald     (502) staff       (20)      720 2011-03-15 02:29:13.000000 modulegraph-0.9/doc/commandline.rst
--rw-r--r--   0 ronald     (502) staff       (20)     7054 2011-03-29 06:18:26.000000 modulegraph-0.9/doc/conf.py
--rw-r--r--   0 ronald     (502) staff       (20)     2151 2011-03-14 12:08:43.000000 modulegraph-0.9/doc/find_modules.rst
--rw-r--r--   0 ronald     (502) staff       (20)     1033 2011-03-15 19:35:51.000000 modulegraph-0.9/doc/index.rst
--rw-r--r--   0 ronald     (502) staff       (20)      975 2010-09-28 19:33:54.000000 modulegraph-0.9/doc/license.rst
--rw-r--r--   0 ronald     (502) staff       (20)     3130 2010-09-28 19:04:46.000000 modulegraph-0.9/doc/Makefile
--rw-r--r--   0 ronald     (502) staff       (20)    12811 2011-03-19 21:44:46.000000 modulegraph-0.9/doc/modulegraph.rst
--rw-r--r--   0 ronald     (502) staff       (20)      794 2011-03-14 14:26:31.000000 modulegraph-0.9/doc/util.rst
--rw-r--r--   0 ronald     (502) staff       (20)     1839 2011-03-15 19:35:41.000000 modulegraph-0.9/doc/zipio.rst
--rw-r--r--   0 ronald     (502) staff       (20)      170 2011-03-08 08:51:36.000000 modulegraph-0.9/MANIFEST.in
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph/
--rw-r--r--   0 ronald     (502) staff       (20)       84 2010-08-22 12:09:33.000000 modulegraph-0.9/modulegraph/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)      234 2011-02-06 18:58:05.000000 modulegraph-0.9/modulegraph/_compat.py
--rw-r--r--   0 ronald     (502) staff       (20)     8005 2011-03-09 21:56:37.000000 modulegraph-0.9/modulegraph/find_modules.py
--rw-r--r--   0 ronald     (502) staff       (20)    45901 2011-03-19 21:12:52.000000 modulegraph-0.9/modulegraph/modulegraph.py
--rw-r--r--   0 ronald     (502) staff       (20)     2214 2011-03-16 02:07:40.000000 modulegraph-0.9/modulegraph/util.py
--rw-r--r--   0 ronald     (502) staff       (20)     8368 2011-03-16 16:45:01.000000 modulegraph-0.9/modulegraph/zipio.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-29 06:19:23.000000 modulegraph-0.9/modulegraph.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)       66 2011-03-29 06:19:23.000000 modulegraph-0.9/modulegraph.egg-info/entry_points.txt
--rw-r--r--   0 ronald     (502) staff       (20)     4354 2011-03-29 06:19:23.000000 modulegraph-0.9/modulegraph.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)       15 2011-03-29 06:19:23.000000 modulegraph-0.9/modulegraph.egg-info/requires.txt
--rw-r--r--   0 ronald     (502) staff       (20)     8857 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)       12 2011-03-29 06:19:23.000000 modulegraph-0.9/modulegraph.egg-info/top_level.txt
--rw-r--r--   0 ronald     (502) staff       (20)        1 2010-08-22 15:03:54.000000 modulegraph-0.9/modulegraph.egg-info/zip-safe
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/
--rw-r--r--   0 ronald     (502) staff       (20)       26 2011-03-14 21:47:09.000000 modulegraph-0.9/modulegraph_tests/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)     1293 2011-03-15 19:45:17.000000 modulegraph-0.9/modulegraph_tests/test_basic.py
--rw-r--r--   0 ronald     (502) staff       (20)      599 2011-02-06 19:04:55.000000 modulegraph-0.9/modulegraph_tests/test_compat.py
--rw-r--r--   0 ronald     (502) staff       (20)     2887 2011-03-16 17:33:23.000000 modulegraph-0.9/modulegraph_tests/test_implies.py
--rw-r--r--   0 ronald     (502) staff       (20)     7008 2011-03-09 23:23:10.000000 modulegraph-0.9/modulegraph_tests/test_imports.py
--rw-r--r--   0 ronald     (502) staff       (20)    33514 2011-03-19 22:08:47.000000 modulegraph-0.9/modulegraph_tests/test_modulegraph.py
--rw-r--r--   0 ronald     (502) staff       (20)     4378 2011-03-09 23:20:04.000000 modulegraph-0.9/modulegraph_tests/test_setuptools_nspkg.py
--rw-r--r--   0 ronald     (502) staff       (20)     1859 2011-03-09 23:32:49.000000 modulegraph-0.9/modulegraph_tests/test_util.py
--rw-r--r--   0 ronald     (502) staff       (20)     8803 2011-03-16 17:31:22.000000 modulegraph-0.9/modulegraph_tests/test_zipio.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/namedpkg/slave.py
--rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 12:02:02.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg/parent.py
--rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/namedpkg/slave.py
--rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:04.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg/parent.py
--rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:12.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/namedpkg/slave.py
--rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:26.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg/parent.py
--rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5-nspkg.pth
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/top_level.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/build/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/build/lib/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:19:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/slave.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:19:11.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/namedpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/namedpkg/slave.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/top_level.txt
--rw-r--r--   0 ronald     (502) staff       (20)      160 2011-03-16 11:19:23.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/child/setup.py
--rw-r--r--   0 ronald     (502) staff       (20)     1652 2011-03-16 11:52:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/install.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/build/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/build/lib/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:18:18.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/parent.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:18:18.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/parent.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/top_level.txt
--rw-r--r--   0 ronald     (502) staff       (20)      159 2011-03-16 11:17:43.000000 modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/parent/setup.py
--rwxr-xr-x   0 ronald     (502) staff       (20)       54 2011-03-16 19:06:33.000000 modulegraph-0.9/modulegraph_tests/testdata/script
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/subdir/
--rw-r--r--   0 ronald     (502) staff       (20)        2 2011-03-15 18:09:53.000000 modulegraph-0.9/modulegraph_tests/testdata/subdir/file1.txt
--rw-r--r--   0 ronald     (502) staff       (20)        2 2011-03-15 18:09:56.000000 modulegraph-0.9/modulegraph_tests/testdata/subdir/file2.txt
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/
--rw-r--r--   0 ronald     (502) staff       (20)       23 2011-03-19 18:55:54.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/myext.pyd
--rw-r--r--   0 ronald     (502) staff       (20)       20 2011-03-19 18:55:27.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/mymodule.py
--rw-r--r--   0 ronald     (502) staff       (20)       21 2011-03-19 19:07:58.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/mymodule3.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/mypkg/
--rw-r--r--   0 ronald     (502) staff       (20)       21 2011-03-19 18:56:23.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath/mypkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)     2065 2011-03-19 20:51:55.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath.egg
--rw-r--r--   0 ronald     (502) staff       (20)     1825 2011-03-19 19:08:52.000000 modulegraph-0.9/modulegraph_tests/testdata/syspath.zip
--rw-r--r--   0 ronald     (502) staff       (20)      760 2011-03-14 02:46:02.000000 modulegraph-0.9/modulegraph_tests/testdata/test.egg
--rw-r--r--   0 ronald     (502) staff       (20)       17 2011-03-15 17:52:15.000000 modulegraph-0.9/modulegraph_tests/testdata/test.txt
--rw-r--r--   0 ronald     (502) staff       (20)     1627 2011-03-15 18:19:08.000000 modulegraph-0.9/modulegraph_tests/testdata/zipped.egg
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/
--rw-r--r--   0 ronald     (502) staff       (20)       17 2010-08-20 10:37:53.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/main_script.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/pkg/
--rw-r--r--   0 ronald     (502) staff       (20)        0 2010-08-20 10:36:50.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/pkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       15 2010-08-20 10:37:15.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/pkg/a.py
--rw-r--r--   0 ronald     (502) staff       (20)        0 2010-08-20 10:37:22.000000 modulegraph-0.9/modulegraph_tests/testpkg-regr1/pkg/b.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/
--rw-r--r--   0 ronald     (502) staff       (20)       24 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/mod.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/
--rw-r--r--   0 ronald     (502) staff       (20)       18 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       25 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/mod.py
--rw-r--r--   0 ronald     (502) staff       (20)       11 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/oldstyle.py
--rw-r--r--   0 ronald     (502) staff       (20)       57 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/relative.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/sub2/
--rw-r--r--   0 ronald     (502) staff       (20)       17 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/sub2/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/sub2/mod.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/subpkg/
--rw-r--r--   0 ronald     (502) staff       (20)       19 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/subpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)      118 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/subpkg/mod2.py
--rw-r--r--   0 ronald     (502) staff       (20)       86 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/subpkg/relative.py
--rw-r--r--   0 ronald     (502) staff       (20)       50 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/pkg/toplevel.py
--rw-r--r--   0 ronald     (502) staff       (20)      147 2010-09-28 20:15:58.000000 modulegraph-0.9/modulegraph_tests/testpkg-relimport/script.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/
--rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/module.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/
--rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       26 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/sub.py
--rw-r--r--   0 ronald     (502) staff       (20)      221 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/setup.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/
--rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/module.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/
--rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/__init__.py
--rw-r--r--   0 ronald     (502) staff       (20)       26 2010-08-22 12:09:34.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/sub.py
-drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-03-29 06:19:24.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/
--rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-29 05:44:21.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (502) staff       (20)       21 2011-03-29 05:44:21.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/namespace_packages.txt
--rw-r--r--   0 ronald     (502) staff       (20)        1 2010-09-28 19:30:31.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/not-zip-safe
--rw-r--r--   0 ronald     (502) staff       (20)      177 2011-03-29 05:44:21.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-29 05:44:21.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (502) staff       (20)        6 2011-03-29 05:44:21.000000 modulegraph-0.9/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/top_level.txt
--rw-r--r--   0 ronald     (502) staff       (20)     4354 2011-03-29 06:19:24.000000 modulegraph-0.9/PKG-INFO
--rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-19 18:36:03.000000 modulegraph-0.9/README.txt
--rw-r--r--   0 ronald     (502) staff       (20)      865 2011-03-29 06:19:24.000000 modulegraph-0.9/setup.cfg
--rw-r--r--   0 ronald     (502) staff       (20)    13991 2011-03-29 06:15:41.000000 modulegraph-0.9/setup.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/
+-rw-r--r--   0 ronald     (502) staff       (20)    14615 2011-06-14 20:02:45.000000 modulegraph-0.9.1/distribute_setup.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/_build/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/_build/doctrees/
+-rw-r--r--   0 ronald     (502) staff       (20)    20348 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/changelog.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)     7518 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/commandline.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)  1149172 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/environment.pickle
+-rw-r--r--   0 ronald     (502) staff       (20)    18843 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/find_modules.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)     9687 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/index.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)     4908 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/license.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)   140216 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/modulegraph.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)    10748 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/util.doctree
+-rw-r--r--   0 ronald     (502) staff       (20)    22090 2011-03-29 06:19:28.000000 modulegraph-0.9.1/doc/_build/doctrees/zipio.doctree
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/_build/html/
+-rw-r--r--   0 ronald     (502) staff       (20)      230 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/.buildinfo
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/_build/html/_sources/
+-rw-r--r--   0 ronald     (502) staff       (20)     2614 2011-03-15 12:05:38.000000 modulegraph-0.9.1/doc/_build/html/_sources/changelog.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      720 2011-03-15 02:29:13.000000 modulegraph-0.9.1/doc/_build/html/_sources/commandline.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     2151 2011-03-14 12:08:43.000000 modulegraph-0.9.1/doc/_build/html/_sources/find_modules.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     1033 2011-03-15 19:35:51.000000 modulegraph-0.9.1/doc/_build/html/_sources/index.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      975 2010-09-28 19:33:54.000000 modulegraph-0.9.1/doc/_build/html/_sources/license.txt
+-rw-r--r--   0 ronald     (502) staff       (20)    12811 2011-03-19 21:44:46.000000 modulegraph-0.9.1/doc/_build/html/_sources/modulegraph.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      794 2011-03-14 14:26:31.000000 modulegraph-0.9.1/doc/_build/html/_sources/util.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     1839 2011-03-15 19:35:41.000000 modulegraph-0.9.1/doc/_build/html/_sources/zipio.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/doc/_build/html/_static/
+-rw-r--r--   0 ronald     (502) staff       (20)     8270 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/basic.css
+-rw-r--r--   0 ronald     (502) staff       (20)     6871 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 ronald     (502) staff       (20)      392 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/file.png
+-rw-r--r--   0 ronald     (502) staff       (20)    72174 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/jquery.js
+-rw-r--r--   0 ronald     (502) staff       (20)      199 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/minus.png
+-rw-r--r--   0 ronald     (502) staff       (20)     4175 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/_static/nature.css
+-rw-r--r--   0 ronald     (502) staff       (20)      199 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/plus.png
+-rw-r--r--   0 ronald     (502) staff       (20)     3932 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 ronald     (502) staff       (20)    14509 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 ronald     (502) staff       (20)     8205 2011-03-14 13:27:49.000000 modulegraph-0.9.1/doc/_build/html/_static/underscore.js
+-rw-r--r--   0 ronald     (502) staff       (20)     9289 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/changelog.html
+-rw-r--r--   0 ronald     (502) staff       (20)     5871 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/commandline.html
+-rw-r--r--   0 ronald     (502) staff       (20)    10518 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/find_modules.html
+-rw-r--r--   0 ronald     (502) staff       (20)    16138 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/genindex.html
+-rw-r--r--   0 ronald     (502) staff       (20)     6668 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/index.html
+-rw-r--r--   0 ronald     (502) staff       (20)     5509 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/license.html
+-rw-r--r--   0 ronald     (502) staff       (20)    45447 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/modulegraph.html
+-rw-r--r--   0 ronald     (502) staff       (20)      882 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/objects.inv
+-rw-r--r--   0 ronald     (502) staff       (20)     4492 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/py-modindex.html
+-rw-r--r--   0 ronald     (502) staff       (20)     3349 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/search.html
+-rw-r--r--   0 ronald     (502) staff       (20)     8614 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/searchindex.js
+-rw-r--r--   0 ronald     (502) staff       (20)     7071 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/util.html
+-rw-r--r--   0 ronald     (502) staff       (20)     9969 2011-03-29 06:19:29.000000 modulegraph-0.9.1/doc/_build/html/zipio.html
+-rw-r--r--   0 ronald     (502) staff       (20)     3271 2011-05-03 07:05:51.000000 modulegraph-0.9.1/doc/changelog.rst
+-rw-r--r--   0 ronald     (502) staff       (20)      720 2011-03-15 02:29:13.000000 modulegraph-0.9.1/doc/commandline.rst
+-rw-r--r--   0 ronald     (502) staff       (20)     7048 2011-05-01 09:21:35.000000 modulegraph-0.9.1/doc/conf.py
+-rw-r--r--   0 ronald     (502) staff       (20)     2151 2011-03-14 12:08:43.000000 modulegraph-0.9.1/doc/find_modules.rst
+-rw-r--r--   0 ronald     (502) staff       (20)     1033 2011-03-15 19:35:51.000000 modulegraph-0.9.1/doc/index.rst
+-rw-r--r--   0 ronald     (502) staff       (20)      975 2010-09-28 19:33:54.000000 modulegraph-0.9.1/doc/license.rst
+-rw-r--r--   0 ronald     (502) staff       (20)     3130 2010-09-28 19:04:46.000000 modulegraph-0.9.1/doc/Makefile
+-rw-r--r--   0 ronald     (502) staff       (20)    12811 2011-03-19 21:44:46.000000 modulegraph-0.9.1/doc/modulegraph.rst
+-rw-r--r--   0 ronald     (502) staff       (20)      794 2011-03-14 14:26:31.000000 modulegraph-0.9.1/doc/util.rst
+-rw-r--r--   0 ronald     (502) staff       (20)     1839 2011-03-15 19:35:41.000000 modulegraph-0.9.1/doc/zipio.rst
+-rw-r--r--   0 ronald     (502) staff       (20)      170 2011-03-08 08:51:36.000000 modulegraph-0.9.1/MANIFEST.in
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph/
+-rw-r--r--   0 ronald     (502) staff       (20)       84 2010-08-22 12:09:33.000000 modulegraph-0.9.1/modulegraph/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)      234 2011-02-06 18:58:05.000000 modulegraph-0.9.1/modulegraph/_compat.py
+-rw-r--r--   0 ronald     (502) staff       (20)     8005 2011-03-09 21:56:37.000000 modulegraph-0.9.1/modulegraph/find_modules.py
+-rw-r--r--   0 ronald     (502) staff       (20)    46193 2011-05-03 10:28:57.000000 modulegraph-0.9.1/modulegraph/modulegraph.py
+-rw-r--r--   0 ronald     (502) staff       (20)     2214 2011-03-16 02:07:40.000000 modulegraph-0.9.1/modulegraph/util.py
+-rw-r--r--   0 ronald     (502) staff       (20)     8369 2011-05-03 10:25:51.000000 modulegraph-0.9.1/modulegraph/zipio.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-07-24 12:18:31.000000 modulegraph-0.9.1/modulegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)       66 2011-07-24 12:18:31.000000 modulegraph-0.9.1/modulegraph.egg-info/entry_points.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     5180 2011-07-24 12:18:31.000000 modulegraph-0.9.1/modulegraph.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)       15 2011-07-24 12:18:31.000000 modulegraph-0.9.1/modulegraph.egg-info/requires.txt
+-rw-r--r--   0 ronald     (502) staff       (20)    10661 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)       12 2011-07-24 12:18:31.000000 modulegraph-0.9.1/modulegraph.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2010-08-22 15:03:54.000000 modulegraph-0.9.1/modulegraph.egg-info/zip-safe
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/
+-rw-r--r--   0 ronald     (502) staff       (20)       26 2011-03-14 21:47:09.000000 modulegraph-0.9.1/modulegraph_tests/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)     1293 2011-03-15 19:45:17.000000 modulegraph-0.9.1/modulegraph_tests/test_basic.py
+-rw-r--r--   0 ronald     (502) staff       (20)      599 2011-02-06 19:04:55.000000 modulegraph-0.9.1/modulegraph_tests/test_compat.py
+-rw-r--r--   0 ronald     (502) staff       (20)     2887 2011-03-16 17:33:23.000000 modulegraph-0.9.1/modulegraph_tests/test_implies.py
+-rw-r--r--   0 ronald     (502) staff       (20)     9206 2011-07-24 12:17:56.000000 modulegraph-0.9.1/modulegraph_tests/test_imports.py
+-rw-r--r--   0 ronald     (502) staff       (20)    33561 2011-05-03 10:48:30.000000 modulegraph-0.9.1/modulegraph_tests/test_modulegraph.py
+-rw-r--r--   0 ronald     (502) staff       (20)     4378 2011-03-09 23:20:04.000000 modulegraph-0.9.1/modulegraph_tests/test_setuptools_nspkg.py
+-rw-r--r--   0 ronald     (502) staff       (20)     1859 2011-03-09 23:32:49.000000 modulegraph-0.9.1/modulegraph_tests/test_util.py
+-rw-r--r--   0 ronald     (502) staff       (20)     8803 2011-05-03 10:27:00.000000 modulegraph-0.9.1/modulegraph_tests/test_zipio.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/namedpkg/slave.py
+-rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/child/nameduser-1.5-py2.6.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 12:02:02.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg/parent.py
+-rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.10/parent/namedpkg-1.0-py2.6.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/namedpkg/slave.py
+-rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:04.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/child/nameduser-1.5-py2.5.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg/parent.py
+-rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:31:12.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/distribute-0.6.12/parent/namedpkg-1.0-py2.5.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/namedpkg/slave.py
+-rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:26.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/child/nameduser-1.5-py2.5.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg/parent.py
+-rw-r--r--   0 ronald     (502) staff       (20)      305 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5-nspkg.pth
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:30:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/setuptools-0.6c9/parent/namedpkg-1.0-py2.5.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/build/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/build/lib/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:19:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/build/lib/namedpkg/slave.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:19:11.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/namedpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       33 2011-03-16 11:19:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/namedpkg/slave.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      181 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      221 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/nameduser.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      160 2011-03-16 11:19:23.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/child/setup.py
+-rw-r--r--   0 ronald     (502) staff       (20)     1652 2011-03-16 11:52:24.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/install.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/build/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/build/lib/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:18:18.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/build/lib/namedpkg/parent.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       56 2011-03-16 11:18:18.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       35 2011-03-16 11:18:38.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg/parent.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      180 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      217 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        9 2011-03-16 11:50:05.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/namedpkg.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      159 2011-03-16 11:17:43.000000 modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/parent/setup.py
+-rwxr-xr-x   0 ronald     (502) staff       (20)       54 2011-03-16 19:06:33.000000 modulegraph-0.9.1/modulegraph_tests/testdata/script
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/subdir/
+-rw-r--r--   0 ronald     (502) staff       (20)        2 2011-03-15 18:09:53.000000 modulegraph-0.9.1/modulegraph_tests/testdata/subdir/file1.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        2 2011-03-15 18:09:56.000000 modulegraph-0.9.1/modulegraph_tests/testdata/subdir/file2.txt
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/
+-rw-r--r--   0 ronald     (502) staff       (20)       23 2011-03-19 18:55:54.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/myext.pyd
+-rw-r--r--   0 ronald     (502) staff       (20)       20 2011-03-19 18:55:27.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/mymodule.py
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2011-03-19 19:07:58.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/mymodule3.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/mypkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2011-03-19 18:56:23.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath/mypkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)     2065 2011-03-19 20:51:55.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath.egg
+-rw-r--r--   0 ronald     (502) staff       (20)     1825 2011-03-19 19:08:52.000000 modulegraph-0.9.1/modulegraph_tests/testdata/syspath.zip
+-rw-r--r--   0 ronald     (502) staff       (20)      760 2011-03-14 02:46:02.000000 modulegraph-0.9.1/modulegraph_tests/testdata/test.egg
+-rw-r--r--   0 ronald     (502) staff       (20)       17 2011-03-15 17:52:15.000000 modulegraph-0.9.1/modulegraph_tests/testdata/test.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     1627 2011-03-15 18:19:08.000000 modulegraph-0.9.1/modulegraph_tests/testdata/zipped.egg
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/
+-rw-r--r--   0 ronald     (502) staff       (20)       17 2010-08-20 10:37:53.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/main_script.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/pkg/
+-rw-r--r--   0 ronald     (502) staff       (20)        0 2010-08-20 10:36:50.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/pkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       15 2010-08-20 10:37:15.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/pkg/a.py
+-rw-r--r--   0 ronald     (502) staff       (20)        0 2010-08-20 10:37:22.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr1/pkg/b.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/
+-rw-r--r--   0 ronald     (502) staff       (20)       11 2011-05-03 06:46:57.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/main_script.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/pkg/
+-rw-r--r--   0 ronald     (502) staff       (20)      154 2011-05-03 06:51:12.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/pkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2011-05-03 06:44:28.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/pkg/base.py
+-rw-r--r--   0 ronald     (502) staff       (20)       15 2011-05-03 06:44:20.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr2/pkg/pkg.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/mypkg/
+-rw-r--r--   0 ronald     (502) staff       (20)        0 2011-07-24 12:17:56.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/mypkg/__init__.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/mypkg/distutils/
+-rw-r--r--   0 ronald     (502) staff       (20)        0 2011-07-24 12:17:56.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/mypkg/distutils/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       85 2011-07-24 12:17:56.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/mypkg/distutils/ccompiler.py
+-rw-r--r--   0 ronald     (502) staff       (20)       38 2011-07-24 12:17:56.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-regr3/script.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/
+-rw-r--r--   0 ronald     (502) staff       (20)       24 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/mod.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       18 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       25 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/mod.py
+-rw-r--r--   0 ronald     (502) staff       (20)       11 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/oldstyle.py
+-rw-r--r--   0 ronald     (502) staff       (20)       57 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/relative.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/sub2/
+-rw-r--r--   0 ronald     (502) staff       (20)       17 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/sub2/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/sub2/mod.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/subpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)       19 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/subpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)      118 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/subpkg/mod2.py
+-rw-r--r--   0 ronald     (502) staff       (20)       86 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/subpkg/relative.py
+-rw-r--r--   0 ronald     (502) staff       (20)       50 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/pkg/toplevel.py
+-rw-r--r--   0 ronald     (502) staff       (20)      147 2010-09-28 20:15:58.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-relimport/script.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/
+-rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/module.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       26 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/build/lib/nspkg/nssubpkg/sub.py
+-rw-r--r--   0 ronald     (502) staff       (20)      221 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/setup.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/
+-rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/module.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/
+-rw-r--r--   0 ronald     (502) staff       (20)      201 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/__init__.py
+-rw-r--r--   0 ronald     (502) staff       (20)       26 2010-08-22 12:09:34.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg/nssubpkg/sub.py
+drwxr-xr-x   0 ronald     (502) staff       (20)        0 2011-07-24 12:18:32.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2011-07-19 05:37:27.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (502) staff       (20)       21 2011-07-19 05:37:27.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/namespace_packages.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        1 2010-09-28 19:30:31.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/not-zip-safe
+-rw-r--r--   0 ronald     (502) staff       (20)      177 2011-07-19 05:37:27.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      313 2011-07-19 05:37:27.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (502) staff       (20)        6 2011-07-19 05:37:27.000000 modulegraph-0.9.1/modulegraph_tests/testpkg-setuptools-namespace/src/nspkg.egg-info/top_level.txt
+-rw-r--r--   0 ronald     (502) staff       (20)     5180 2011-07-24 12:18:32.000000 modulegraph-0.9.1/PKG-INFO
+-rw-r--r--   0 ronald     (502) staff       (20)      313 2011-03-19 18:36:03.000000 modulegraph-0.9.1/README.txt
+-rw-r--r--   0 ronald     (502) staff       (20)      866 2011-07-24 12:18:32.000000 modulegraph-0.9.1/setup.cfg
+-rw-r--r--   0 ronald     (502) staff       (20)    13991 2011-03-29 06:15:41.000000 modulegraph-0.9.1/setup.py
```

### Comparing `modulegraph-0.9/distribute_setup.py` & `modulegraph-0.9.1/distribute_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             def quote(arg):
                 if ' ' in arg:
                     return '"%s"' % arg
                 return arg
             args = [quote(arg) for arg in args]
         return os.spawnl(os.P_WAIT, sys.executable, *args) == 0
 
-DEFAULT_VERSION = "0.6.4"
+DEFAULT_VERSION = "0.6.19"
 DEFAULT_URL = "http://pypi.python.org/packages/source/d/distribute/"
 SETUPTOOLS_PKG_INFO = """\
 Metadata-Version: 1.0
 Name: setuptools
 Version: 0.6c9
 Summary: xxxx
 Home-page: xxx
```

### Comparing `modulegraph-0.9/doc/changelog.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/changelog.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/commandline.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/commandline.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/conf.py` & `modulegraph-0.9.1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def get_version():
     fn = os.path.join(
         os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
         'setup.cfg')
     for ln in open(fn):
         if ln.startswith('version'):
-            version = ln.split('=')[-1].strip()[1:-1]
+            version = ln.split('=')[-1].strip()
             return version
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.append(os.path.abspath('.'))
```

### Comparing `modulegraph-0.9/doc/find_modules.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/find_modules.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/index.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/license.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/license.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/Makefile` & `modulegraph-0.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/modulegraph.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/modulegraph.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/util.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/util.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/doc/zipio.rst` & `modulegraph-0.9.1/doc/_build/html/_sources/zipio.txt`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph/find_modules.py` & `modulegraph-0.9.1/modulegraph/find_modules.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph/modulegraph.py` & `modulegraph-0.9.1/modulegraph/modulegraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -850,15 +850,22 @@
 
     def _safe_import_hook(self, name, caller, fromlist, level=-1):
         # wrapper for self.import_hook() that won't raise ImportError
         try:
             mods = self.import_hook(name, caller, level=level)
         except ImportError, msg:
             self.msg(2, "ImportError:", str(msg))
-            m = self.createNode(MissingModule, name)
+
+            # This is a hack, but sadly enough the necessary information
+            # isn't available otherwise.
+            m = re.match('^No module named (\S+)$', str(msg))
+            if m is not None:
+                m = self.createNode(MissingModule, m.group(1))
+            else:
+                m = self.createNode(MissingModule, name)
             self.createReference(caller, m)
         else:
             assert len(mods) == 1
             m = list(mods)[0]
 
         subs = [m]
         for sub in (fromlist or ()):
```

### Comparing `modulegraph-0.9/modulegraph/util.py` & `modulegraph-0.9.1/modulegraph/util.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph/zipio.py` & `modulegraph-0.9.1/modulegraph/zipio.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
                     "No such file or directory")
             
             # Directory exists, but has no entry of its
             # own, fake mtime by using the timestamp of
             # the zipfile itself.
             return _os.path.getmtime(path)
 
-        return _time.mktime(info.date_time + (0, 0, 0))
+        return _time.mktime(info.date_time + (0, 0, -1))
 
     except KeyError:
         if zf is not None:
             zf.close()
         raise IOError(
             _errno.ENOENT, full_path, 
             "No such file or directory")
```

### Comparing `modulegraph-0.9/modulegraph.egg-info/PKG-INFO` & `modulegraph-0.9.1/modulegraph.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.0
 Name: modulegraph
-Version: 0.9
+Version: 0.9.1
 Summary: Python module dependency analysis tool
-Home-page: http://bitbucket.org/ronaldoussoren/modulegraph"
+Home-page: http://bitbucket.org/ronaldoussoren/modulegraph
 Author: Ronald Oussoren
 Author-email: ronaldoussoren@mac.com
 License: MIT
 Download-URL: http://pypi.python.org/pypi/modulegraph
 Description: modulegraph determines a dependency graph between Python modules primarily
         by bytecode analysis for import statements.
         
@@ -14,14 +14,35 @@
         but uses a more flexible internal representation, has more extensive 
         knowledge of special cases, and is extensible.
         
         
         Release history
         ===============
         
+        0.9.1
+        -----
+        
+        This is a bugfix release
+        
+        Bug fixes
+        .........
+        
+        - Fixed the name of nodes imports in packages where the first element of
+          a dotted name can be found but the rest cannot. This used to create
+          a MissingModule node for the dotted name in the global namespace instead
+          of relative to the package.
+        
+          That is, given a package "pkg" with submodule "sub" if the "__init__.py"
+          of "pkg" contains "import sub.nomod" we now create a MissingModule node
+          for "pkg.sub.nomod" instead of "sub.nomod".
+        
+          This fixes an issue with including the crcmod package in application 
+          bundles, first reported on the pythonmac-sig mailinglist by
+          Brendan Simon.
+        
         0.9
         ---
         
         This is a minor feature release
         
         
         Features:
```

### Comparing `modulegraph-0.9/modulegraph_tests/test_basic.py` & `modulegraph-0.9.1/modulegraph_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/test_compat.py` & `modulegraph-0.9.1/modulegraph_tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/test_implies.py` & `modulegraph-0.9.1/modulegraph_tests/test_implies.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/test_imports.py` & `modulegraph-0.9.1/modulegraph_tests/test_imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.assertEqual(m, 'pkg.sub2.mod')
 
 
 class TestModuleGraphImport (unittest.TestCase):
     if not hasattr(unittest.TestCase, 'assertIsInstance'):
         def assertIsInstance(self, value, types):
             if not isinstance(value, types):
-                self.fail("%r is not an instance of %r", value, types)
+                self.fail("%r is not an instance of %r"%(value, types))
 
     def setUp(self):
         root = os.path.join(
                 os.path.dirname(os.path.abspath(__file__)),
                 'testpkg-relimport')
         self.mf = modulegraph.ModuleGraph(path=[ root ] + sys.path)
         #self.mf.debug = 999
@@ -156,15 +156,15 @@
         self.assertIsInstance(node, modulegraph.SourceModule)
         self.assertEqual(node.identifier, 'pkg.subpkg.mod2')
         sub = [ n for n in self.mf.get_edges(node)[0] if n.identifier != '__future__' ][0]
         self.assertIsInstance(sub, modulegraph.SourceModule)
         self.assertEqual(sub.identifier, 'pkg.sub2.mod')
 
 
-class TestRegressions (unittest.TestCase):
+class TestRegressions1 (unittest.TestCase):
     if not hasattr(unittest.TestCase, 'assertIsInstance'):
         def assertIsInstance(self, value, types):
             if not isinstance(value, types):
                 self.fail("%r is not an instance of %r", value, types)
 
     def setUp(self):
         root = os.path.join(
@@ -185,9 +185,59 @@
                 os.path.dirname(os.path.abspath(__file__)),
                 'nosuchdirectory')
         try:
             mf = modulegraph.ModuleGraph(path=[ root ] + sys.path)
         except os.error:
             self.fail('modulegraph initialiser raises os.error')
 
+class TestRegressions2 (unittest.TestCase):
+    if not hasattr(unittest.TestCase, 'assertIsInstance'):
+        def assertIsInstance(self, value, types):
+            if not isinstance(value, types):
+                self.fail("%r is not an instance of %r"%(value, types))
+
+    def setUp(self):
+        root = os.path.join(
+                os.path.dirname(os.path.abspath(__file__)),
+                'testpkg-regr2')
+        self.mf = modulegraph.ModuleGraph(path=[ root ] + sys.path)
+        self.mf.run_script(os.path.join(root, 'main_script.py'))
+
+    def testRegr1(self):
+        node = self.mf.findNode('pkg.base')
+        self.assertIsInstance(node, modulegraph.SourceModule)
+        node = self.mf.findNode('pkg.pkg')
+        self.assertIsInstance(node, modulegraph.SourceModule)
+
+class TestRegressions3 (unittest.TestCase):
+    if not hasattr(unittest.TestCase, 'assertIsInstance'):
+        def assertIsInstance(self, value, types):
+            if not isinstance(value, types):
+                self.fail("%r is not an instance of %r"%(value, types))
+
+    def setUp(self):
+        root = os.path.join(
+                os.path.dirname(os.path.abspath(__file__)),
+                'testpkg-regr3')
+        self.mf = modulegraph.ModuleGraph(path=[ root ] + sys.path)
+        self.mf.run_script(os.path.join(root, 'script.py'))
+
+    def testRegr1(self):
+        node = self.mf.findNode('mypkg.distutils')
+        self.assertIsInstance(node, modulegraph.Package)
+        node = self.mf.findNode('mypkg.distutils.ccompiler')
+        self.assertIsInstance(node, modulegraph.SourceModule)
+        self.assertTrue(node.filename.startswith(os.path.dirname(__file__)))
+
+        import distutils.sysconfig, distutils.ccompiler
+        node = self.mf.findNode('distutils.ccompiler')
+        self.assertIsInstance(node, modulegraph.SourceModule)
+        self.assertEqual(os.path.dirname(node.filename), 
+                os.path.dirname(distutils.ccompiler.__file__))
+
+        node = self.mf.findNode('distutils.sysconfig')
+        self.assertIsInstance(node, modulegraph.SourceModule)
+        self.assertEqual(os.path.dirname(node.filename), 
+                os.path.dirname(distutils.sysconfig.__file__))
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `modulegraph-0.9/modulegraph_tests/test_modulegraph.py` & `modulegraph-0.9.1/modulegraph_tests/test_modulegraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,32 +557,33 @@
     @expectedFailure
     def test_import_hook(self):
         self.fail("import_hook")
 
     def test_determine_parent(self):
         graph = modulegraph.ModuleGraph()
         graph.import_hook('os.path', None)
+        graph.import_hook('idlelib', None)
         
         for node in graph.nodes():
             if isinstance(node, modulegraph.Package):
                 break
         else:
             self.fail("No package located, should have at least 'os'")
 
         self.assertIsInstance(node, modulegraph.Package)
         parent = graph.determine_parent(node)
         self.assertEqual(parent.identifier, node.identifier)
         self.assertEqual(parent, graph.findNode(node.identifier))
         self.assertTrue(isinstance(parent, modulegraph.Package))
 
         # XXX: Might be a usecase for some odd code in determine_parent...
-        node = modulegraph.Package('encodings')
-        node.packagepath = parent.packagepath
-        m = graph.determine_parent(node)
-        self.assertTrue(m is parent)
+        #node = modulegraph.Package('encodings')
+        #node.packagepath = parent.packagepath
+        #m = graph.determine_parent(node)
+        #self.assertTrue(m is parent)
 
         m = graph.findNode('xml')
         self.assertEqual(graph.determine_parent(m), None)
 
         m = graph.findNode('xml.dom')
         self.assertEqual(graph.determine_parent(m), graph.findNode('xml'))
```

### Comparing `modulegraph-0.9/modulegraph_tests/test_setuptools_nspkg.py` & `modulegraph-0.9.1/modulegraph_tests/test_setuptools_nspkg.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/test_util.py` & `modulegraph-0.9.1/modulegraph_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/test_zipio.py` & `modulegraph-0.9.1/modulegraph_tests/test_zipio.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,18 +152,18 @@
         fn = os.path.join(TESTDATA, 'test.txt')
         self.assertEqual(os.path.getmtime(fn), zipio.getmtime(fn))
 
         fn = os.path.join(TESTDATA, 'zipped.egg')
         self.assertEqual(os.path.getmtime(fn), zipio.getmtime(fn))
 
         fn = os.path.join(TESTDATA, 'zipped.egg/test.txt')
-        self.assertEqual(zipio.getmtime(fn), 1300215280.0)
+        self.assertEqual(zipio.getmtime(fn), 1300193680.0)
 
         fn = os.path.join(TESTDATA, 'zipped.egg/subdir')
-        self.assertEqual(zipio.getmtime(fn), 1300215490.0)
+        self.assertEqual(zipio.getmtime(fn), 1300193890.0)
 
         fn = os.path.join(TESTDATA, 'zipped.egg/subdir4')
         self.assertEqual(zipio.getmtime(fn), os.path.getmtime(os.path.join(TESTDATA, 'zipped.egg')))
 
         self.assertRaises(IOError, zipio.getmtime, os.path.join(TESTDATA, 'no-file'))
         self.assertRaises(IOError, zipio.getmtime, os.path.join(TESTDATA, 'zipped.egg/no-file'))
```

### Comparing `modulegraph-0.9/modulegraph_tests/testdata/nspkg/src/install.py` & `modulegraph-0.9.1/modulegraph_tests/testdata/nspkg/src/install.py`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/testdata/syspath.egg` & `modulegraph-0.9.1/modulegraph_tests/testdata/syspath.egg`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/testdata/syspath.zip` & `modulegraph-0.9.1/modulegraph_tests/testdata/syspath.zip`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/testdata/test.egg` & `modulegraph-0.9.1/modulegraph_tests/testdata/test.egg`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/modulegraph_tests/testdata/zipped.egg` & `modulegraph-0.9.1/modulegraph_tests/testdata/zipped.egg`

 * *Files identical despite different names*

### Comparing `modulegraph-0.9/PKG-INFO` & `modulegraph-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.0
 Name: modulegraph
-Version: 0.9
+Version: 0.9.1
 Summary: Python module dependency analysis tool
-Home-page: http://bitbucket.org/ronaldoussoren/modulegraph"
+Home-page: http://bitbucket.org/ronaldoussoren/modulegraph
 Author: Ronald Oussoren
 Author-email: ronaldoussoren@mac.com
 License: MIT
 Download-URL: http://pypi.python.org/pypi/modulegraph
 Description: modulegraph determines a dependency graph between Python modules primarily
         by bytecode analysis for import statements.
         
@@ -14,14 +14,35 @@
         but uses a more flexible internal representation, has more extensive 
         knowledge of special cases, and is extensible.
         
         
         Release history
         ===============
         
+        0.9.1
+        -----
+        
+        This is a bugfix release
+        
+        Bug fixes
+        .........
+        
+        - Fixed the name of nodes imports in packages where the first element of
+          a dotted name can be found but the rest cannot. This used to create
+          a MissingModule node for the dotted name in the global namespace instead
+          of relative to the package.
+        
+          That is, given a package "pkg" with submodule "sub" if the "__init__.py"
+          of "pkg" contains "import sub.nomod" we now create a MissingModule node
+          for "pkg.sub.nomod" instead of "sub.nomod".
+        
+          This fixes an issue with including the crcmod package in application 
+          bundles, first reported on the pythonmac-sig mailinglist by
+          Brendan Simon.
+        
         0.9
         ---
         
         This is a minor feature release
         
         
         Features:
```

### Comparing `modulegraph-0.9/setup.cfg` & `modulegraph-0.9.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = modulegraph
-version = 0.9
+version = 0.9.1
 description = Python module dependency analysis tool
 long_description_file = README.txt doc/changelog.rst
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Software Development :: Build Tools
 maintainer = Ronald Oussoren
 maintainer_email = ronaldoussoren@mac.com
-url = http://bitbucket.org/ronaldoussoren/modulegraph"
+url = http://bitbucket.org/ronaldoussoren/modulegraph
 download_url = http://pypi.python.org/pypi/modulegraph
 license = MIT
 packages = modulegraph
 platforms = any
 install_requires = 
 	altgraph >= 0.9
 zip-safe = yes
```

### Comparing `modulegraph-0.9/setup.py` & `modulegraph-0.9.1/setup.py`

 * *Files identical despite different names*

