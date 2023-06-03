# Comparing `tmp/helloPypi-topic-0.0.1.tar.gz` & `tmp/helloPypi-topic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloPypi-topic-0.0.1.tar", last modified: Sat Jun  3 17:52:28 2023, max compression
+gzip compressed data, was "helloPypi-topic-0.0.2.tar", last modified: Sat Jun  3 18:24:38 2023, max compression
```

## Comparing `helloPypi-topic-0.0.1.tar` & `helloPypi-topic-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 17:52:28.123449 helloPypi-topic-0.0.1/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 17:52:28.123449 helloPypi-topic-0.0.1/PKG-INFO
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 17:52:28.123449 helloPypi-topic-0.0.1/helloPypi_topic.egg-info/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 17:52:28.000000 helloPypi-topic-0.0.1/helloPypi_topic.egg-info/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      201 2023-06-03 17:52:28.000000 helloPypi-topic-0.0.1/helloPypi_topic.egg-info/SOURCES.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-03 17:52:28.000000 helloPypi-topic-0.0.1/helloPypi_topic.egg-info/dependency_links.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        8 2023-06-03 17:52:28.000000 helloPypi-topic-0.0.1/helloPypi_topic.egg-info/top_level.txt
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 17:52:28.123449 helloPypi-topic-0.0.1/libname/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       27 2023-06-03 17:31:10.000000 helloPypi-topic-0.0.1/libname/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       40 2023-06-03 17:29:10.000000 helloPypi-topic-0.0.1/libname/hello.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-03 17:52:28.123449 helloPypi-topic-0.0.1/setup.cfg
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      218 2023-06-03 17:51:50.000000 helloPypi-topic-0.0.1/setup.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/PKG-INFO
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      241 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/SOURCES.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/dependency_links.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       15 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/top_level.txt
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/myhellopackage/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:23:37.000000 helloPypi-topic-0.0.2/myhellopackage/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       79 2023-06-03 18:20:29.000000 helloPypi-topic-0.0.2/myhellopackage/channel.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       41 2023-06-03 18:17:55.000000 helloPypi-topic-0.0.2/myhellopackage/hello.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/setup.cfg
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      218 2023-06-03 18:24:29.000000 helloPypi-topic-0.0.2/setup.py
```

