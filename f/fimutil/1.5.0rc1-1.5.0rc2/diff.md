# Comparing `tmp/fimutil-1.5.0rc1.tar.gz` & `tmp/fimutil-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fimutil-1.5.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fimutil-1.5.0rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fimutil-1.5.0rc1.tar` & `fimutil-1.5.0rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fimutil-1.5.0rc1/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fimutil-1.5.0rc1/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fimutil-1.5.0rc1/MANIFEST.in
--rw-r--r--   0        0        0     7321 2023-02-02 01:14:34.889369 fimutil-1.5.0rc1/README.md
--rw-r--r--   0        0        0      159 2023-06-02 21:57:29.787572 fimutil-1.5.0rc1/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fimutil-1.5.0rc1/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fimutil-1.5.0rc1/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fimutil-1.5.0rc1/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fimutil-1.5.0rc1/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fimutil-1.5.0rc1/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fimutil-1.5.0rc1/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fimutil-1.5.0rc1/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fimutil-1.5.0rc1/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fimutil-1.5.0rc1/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fimutil-1.5.0rc1/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fimutil-1.5.0rc1/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fimutil-1.5.0rc1/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21981 2023-06-02 21:31:39.454775 fimutil-1.5.0rc1/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fimutil-1.5.0rc1/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fimutil-1.5.0rc1/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fimutil-1.5.0rc1/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fimutil-1.5.0rc1/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fimutil-1.5.0rc1/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fimutil-1.5.0rc1/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fimutil-1.5.0rc1/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fimutil-1.5.0rc1/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fimutil-1.5.0rc1/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fimutil-1.5.0rc1/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1718 2023-06-02 21:57:17.454940 fimutil-1.5.0rc1/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fimutil-1.5.0rc1/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fimutil-1.5.0rc1/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fimutil-1.5.0rc1/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0      826 2023-06-02 21:57:04.938167 fimutil-1.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0      462 2023-06-01 15:50:15.617615 fimutil-1.5.0rc1/requirements.txt
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fimutil-1.5.0rc1/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fimutil-1.5.0rc1/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fimutil-1.5.0rc1/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fimutil-1.5.0rc1/test/ralph_test.py
--rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 fimutil-1.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fimutil-1.5.0rc2/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fimutil-1.5.0rc2/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fimutil-1.5.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     7321 2023-02-02 01:14:34.889369 fimutil-1.5.0rc2/README.md
+-rw-r--r--   0        0        0      159 2023-06-02 22:03:12.616693 fimutil-1.5.0rc2/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fimutil-1.5.0rc2/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fimutil-1.5.0rc2/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fimutil-1.5.0rc2/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fimutil-1.5.0rc2/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fimutil-1.5.0rc2/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fimutil-1.5.0rc2/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fimutil-1.5.0rc2/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fimutil-1.5.0rc2/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fimutil-1.5.0rc2/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fimutil-1.5.0rc2/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fimutil-1.5.0rc2/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fimutil-1.5.0rc2/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21981 2023-06-02 21:31:39.454775 fimutil-1.5.0rc2/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fimutil-1.5.0rc2/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fimutil-1.5.0rc2/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fimutil-1.5.0rc2/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fimutil-1.5.0rc2/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fimutil-1.5.0rc2/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fimutil-1.5.0rc2/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fimutil-1.5.0rc2/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fimutil-1.5.0rc2/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fimutil-1.5.0rc2/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fimutil-1.5.0rc2/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-02 22:02:16.828125 fimutil-1.5.0rc2/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fimutil-1.5.0rc2/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fimutil-1.5.0rc2/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fimutil-1.5.0rc2/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0      826 2023-06-02 21:57:04.938167 fimutil-1.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-06-01 15:50:15.617615 fimutil-1.5.0rc2/requirements.txt
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fimutil-1.5.0rc2/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fimutil-1.5.0rc2/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fimutil-1.5.0rc2/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fimutil-1.5.0rc2/test/ralph_test.py
+-rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 fimutil-1.5.0rc2/PKG-INFO
```

### Comparing `fimutil-1.5.0rc1/.gitignore` & `fimutil-1.5.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/LICENSE` & `fimutil-1.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/README.md` & `fimutil-1.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/al2s/arm.py` & `fimutil-1.5.0rc2/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/al2s/cloud_cfg.py` & `fimutil-1.5.0rc2/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/al2s/oess.py` & `fimutil-1.5.0rc2/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/netam/arm.py` & `fimutil-1.5.0rc2/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/netam/nso.py` & `fimutil-1.5.0rc2/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/netam/sr_pce.py` & `fimutil-1.5.0rc2/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/asset.py` & `fimutil-1.5.0rc2/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/dp_switch.py` & `fimutil-1.5.0rc2/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/ethernetport.py` & `fimutil-1.5.0rc2/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/fim_helper.py` & `fimutil-1.5.0rc2/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/fpga.py` & `fimutil-1.5.0rc2/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/gpu.py` & `fimutil-1.5.0rc2/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/model.py` & `fimutil-1.5.0rc2/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/nvme.py` & `fimutil-1.5.0rc2/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/ralph_uri.py` & `fimutil-1.5.0rc2/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/site.py` & `fimutil-1.5.0rc2/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/storage.py` & `fimutil-1.5.0rc2/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/ralph/worker_node.py` & `fimutil-1.5.0rc2/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/utilities/generate_instance_flavors.py` & `fimutil-1.5.0rc2/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/utilities/scan_net.py` & `fimutil-1.5.0rc2/fimutil/utilities/scan_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import logging
 import sys
 
 from fimutil.netam.arm import NetworkARM
 
 
-def main()::
+def main():
     parser = argparse.ArgumentParser()
     # split into different mutually exclusive operations
 
     parser.add_argument("-c", "--config", action="store",
                         help="config file")
     parser.add_argument("-d", "--debug", action="count",
                         help="Turn on debugging")
```

### Comparing `fimutil-1.5.0rc1/fimutil/utilities/scan_oess.py` & `fimutil-1.5.0rc2/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/utilities/scan_site.py` & `fimutil-1.5.0rc2/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/fimutil/utilities/scan_worker.py` & `fimutil-1.5.0rc2/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/pyproject.toml` & `fimutil-1.5.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/setup.py` & `fimutil-1.5.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/test/netam_test.py` & `fimutil-1.5.0rc2/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fimutil-1.5.0rc1/PKG-INFO` & `fimutil-1.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fimutil
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

