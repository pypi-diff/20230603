# Comparing `tmp/pyhop-0.0.4.tar.gz` & `tmp/pyhop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhop-0.0.4.tar", last modified: Sat Jun  3 12:25:54 2023, max compression
+gzip compressed data, was "pyhop-0.0.5.tar", last modified: Sat Jun  3 12:45:21 2023, max compression
```

## Comparing `pyhop-0.0.4.tar` & `pyhop-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:25:54.705323 pyhop-0.0.4/
--rw-rw-rw-   0        0        0     1362 2023-06-03 12:25:54.704324 pyhop-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 12:25:54.687283 pyhop-0.0.4/pyhop/
--rw-rw-rw-   0        0        0       30 2023-06-03 12:06:40.000000 pyhop-0.0.4/pyhop/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-06-03 11:48:43.000000 pyhop-0.0.4/pyhop/main.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:25:54.703321 pyhop-0.0.4/pyhop.egg-info/
--rw-rw-rw-   0        0        0     1362 2023-06-03 12:25:54.000000 pyhop-0.0.4/pyhop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-06-03 12:25:54.000000 pyhop-0.0.4/pyhop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:25:54.000000 pyhop-0.0.4/pyhop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 12:25:54.000000 pyhop-0.0.4/pyhop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:25:54.706328 pyhop-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-06-03 12:25:46.000000 pyhop-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:45:21.713601 pyhop-0.0.5/
+-rw-rw-rw-   0        0        0     1362 2023-06-03 12:45:21.712605 pyhop-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 12:45:21.687604 pyhop-0.0.5/pyhop/
+-rw-rw-rw-   0        0        0       30 2023-06-03 12:06:40.000000 pyhop-0.0.5/pyhop/__init__.py
+-rw-rw-rw-   0        0        0     2267 2023-06-03 12:45:00.000000 pyhop-0.0.5/pyhop/main.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:45:21.709601 pyhop-0.0.5/pyhop.egg-info/
+-rw-rw-rw-   0        0        0     1362 2023-06-03 12:45:21.000000 pyhop-0.0.5/pyhop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-06-03 12:45:21.000000 pyhop-0.0.5/pyhop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:45:21.000000 pyhop-0.0.5/pyhop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 12:45:21.000000 pyhop-0.0.5/pyhop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:45:21.713601 pyhop-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-06-03 12:45:09.000000 pyhop-0.0.5/setup.py
```

### Comparing `pyhop-0.0.4/PKG-INFO` & `pyhop-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhop
-Version: 0.0.4
+Version: 0.0.5
 Summary: This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses
 Author: Sarthak
 Author-email: <waliasarthak@gmail.com>
 Keywords: python,traceroute,tracert,hops,ip address,server hops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyhop-0.0.4/pyhop.egg-info/PKG-INFO` & `pyhop-0.0.5/pyhop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhop
-Version: 0.0.4
+Version: 0.0.5
 Summary: This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses
 Author: Sarthak
 Author-email: <waliasarthak@gmail.com>
 Keywords: python,traceroute,tracert,hops,ip address,server hops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyhop-0.0.4/setup.py` & `pyhop-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses'
 LONG_DESCRIPTION = '''
 pyhop is a Python package that simplifies the process of performing traceroutes by utilizing the built-in trace tools, tracert for Windows and traceroute for Linux. This package provides a consistent interface and reliable results across different platforms, allowing network administrators, developers, and users to diagnose network issues and optimize performance with ease. 
 
 With pyhop, you can effortlessly trace the path of packets from your device to a destination host, gaining valuable insights into network connectivity.
 
 Usage Example:
```

