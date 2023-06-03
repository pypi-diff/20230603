# Comparing `tmp/object-serialization-0.1.0.tar.gz` & `tmp/object-serialization-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object-serialization-0.1.0.tar", last modified: Sat Jun  3 12:49:53 2023, max compression
+gzip compressed data, was "object-serialization-0.1.1.tar", last modified: Sat Jun  3 14:43:36 2023, max compression
```

## Comparing `object-serialization-0.1.0.tar` & `object-serialization-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:49:53.031830 object-serialization-0.1.0/
--rw-rw-rw-   0        0        0      125 2023-06-03 12:49:53.030832 object-serialization-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 12:49:53.029831 object-serialization-0.1.0/object_serialization.egg-info/
--rw-rw-rw-   0        0        0      125 2023-06-03 12:49:52.000000 object-serialization-0.1.0/object_serialization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-06-03 12:49:52.000000 object-serialization-0.1.0/object_serialization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:49:52.000000 object-serialization-0.1.0/object_serialization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:49:52.000000 object-serialization-0.1.0/object_serialization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:49:53.031830 object-serialization-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      239 2023-06-03 12:49:11.000000 object-serialization-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 14:43:36.660755 object-serialization-0.1.1/
+-rw-rw-rw-   0        0        0      647 2023-06-01 06:55:56.000000 object-serialization-0.1.1/MySerializer.py
+-rw-rw-rw-   0        0        0      125 2023-06-03 14:43:36.660755 object-serialization-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 14:43:36.659767 object-serialization-0.1.1/object_serialization.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-06-03 14:43:36.000000 object-serialization-0.1.1/object_serialization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-06-03 14:43:36.000000 object-serialization-0.1.1/object_serialization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 14:43:36.000000 object-serialization-0.1.1/object_serialization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 14:43:36.000000 object-serialization-0.1.1/object_serialization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 14:43:36.661756 object-serialization-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      273 2023-06-03 14:43:29.000000 object-serialization-0.1.1/setup.py
```

