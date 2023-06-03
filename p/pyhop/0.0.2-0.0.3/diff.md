# Comparing `tmp/pyhop-0.0.2.tar.gz` & `tmp/pyhop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhop-0.0.2.tar", last modified: Sat Jun  3 12:19:26 2023, max compression
+gzip compressed data, was "pyhop-0.0.3.tar", last modified: Sat Jun  3 12:21:38 2023, max compression
```

## Comparing `pyhop-0.0.2.tar` & `pyhop-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:19:26.875842 pyhop-0.0.2/
--rw-rw-rw-   0        0        0     1349 2023-06-03 12:19:26.874848 pyhop-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 12:19:26.858172 pyhop-0.0.2/pyhop/
--rw-rw-rw-   0        0        0       30 2023-06-03 12:06:40.000000 pyhop-0.0.2/pyhop/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-06-03 11:48:43.000000 pyhop-0.0.2/pyhop/main.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:19:26.871681 pyhop-0.0.2/pyhop.egg-info/
--rw-rw-rw-   0        0        0     1349 2023-06-03 12:19:26.000000 pyhop-0.0.2/pyhop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-06-03 12:19:26.000000 pyhop-0.0.2/pyhop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:19:26.000000 pyhop-0.0.2/pyhop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-03 12:19:26.000000 pyhop-0.0.2/pyhop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 12:19:26.875842 pyhop-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1674 2023-06-03 12:19:17.000000 pyhop-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:21:38.624372 pyhop-0.0.3/
+-rw-rw-rw-   0        0        0     1351 2023-06-03 12:21:38.623273 pyhop-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 12:21:38.605486 pyhop-0.0.3/pyhop/
+-rw-rw-rw-   0        0        0       30 2023-06-03 12:06:40.000000 pyhop-0.0.3/pyhop/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-06-03 11:48:43.000000 pyhop-0.0.3/pyhop/main.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:21:38.621489 pyhop-0.0.3/pyhop.egg-info/
+-rw-rw-rw-   0        0        0     1351 2023-06-03 12:21:38.000000 pyhop-0.0.3/pyhop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-06-03 12:21:38.000000 pyhop-0.0.3/pyhop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:21:38.000000 pyhop-0.0.3/pyhop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-03 12:21:38.000000 pyhop-0.0.3/pyhop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:21:38.624876 pyhop-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-06-03 12:21:20.000000 pyhop-0.0.3/setup.py
```

### Comparing `pyhop-0.0.2/PKG-INFO` & `pyhop-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhop
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses
 Author: Sarthak
 Author-email: <waliasarthak@gmail.com>
 Keywords: python,traceroute,tracert,hops,ip address,server hops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -16,9 +16,10 @@
 pyhop is a Python package that simplifies the process of performing traceroutes by utilizing the built-in trace tools, tracert for Windows and traceroute for Linux. This package provides a consistent interface and reliable results across different platforms, allowing network administrators, developers, and users to diagnose network issues and optimize performance with ease. 
 
 With pyhop, you can effortlessly trace the path of packets from your device to a destination host, gaining valuable insights into network connectivity.
 
 Usage Example:
 
 from pyhop import pyhop
+
 print(pyhop(example.com))
```

### Comparing `pyhop-0.0.2/pyhop/main.py` & `pyhop-0.0.3/pyhop/main.py`

 * *Files identical despite different names*

### Comparing `pyhop-0.0.2/pyhop.egg-info/PKG-INFO` & `pyhop-0.0.3/pyhop.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhop
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses
 Author: Sarthak
 Author-email: <waliasarthak@gmail.com>
 Keywords: python,traceroute,tracert,hops,ip address,server hops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -16,9 +16,10 @@
 pyhop is a Python package that simplifies the process of performing traceroutes by utilizing the built-in trace tools, tracert for Windows and traceroute for Linux. This package provides a consistent interface and reliable results across different platforms, allowing network administrators, developers, and users to diagnose network issues and optimize performance with ease. 
 
 With pyhop, you can effortlessly trace the path of packets from your device to a destination host, gaining valuable insights into network connectivity.
 
 Usage Example:
 
 from pyhop import pyhop
+
 print(pyhop(example.com))
```

### Comparing `pyhop-0.0.2/setup.py` & `pyhop-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'This project is a Python script that utilizes built-in trace tools like tracert for Windows and traceroute for Linux to perform a traceroute to a given hostname or IP address. It traces the path that packets take from your device to the destination host, providing ip addresses'
 LONG_DESCRIPTION = '''
 pyhop is a Python package that simplifies the process of performing traceroutes by utilizing the built-in trace tools, tracert for Windows and traceroute for Linux. This package provides a consistent interface and reliable results across different platforms, allowing network administrators, developers, and users to diagnose network issues and optimize performance with ease. 
 
 With pyhop, you can effortlessly trace the path of packets from your device to a destination host, gaining valuable insights into network connectivity.
 
 Usage Example:
 
 from pyhop import pyhop
+
 print(pyhop(example.com))
 
 '''
 
 # Setting up
 setup(
     name="pyhop",
```

