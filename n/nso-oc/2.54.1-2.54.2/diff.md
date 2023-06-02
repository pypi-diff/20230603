# Comparing `tmp/nso-oc-2.54.1.tar.gz` & `tmp/nso-oc-2.54.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.54.1.tar", last modified: Fri Jun  2 18:53:41 2023, max compression
+gzip compressed data, was "nso-oc-2.54.2.tar", last modified: Fri Jun  2 23:11:05 2023, max compression
```

## Comparing `nso-oc-2.54.1.tar` & `nso-oc-2.54.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:53:41.049604 nso-oc-2.54.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-02 18:53:11.000000 nso-oc-2.54.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 18:53:11.000000 nso-oc-2.54.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 18:53:41.049604 nso-oc-2.54.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 18:53:11.000000 nso-oc-2.54.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:53:41.049604 nso-oc-2.54.1/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 18:53:41.000000 nso-oc-2.54.1/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:53:41.049604 nso-oc-2.54.1/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:53:41.049604 nso-oc-2.54.1/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:53:41.049604 nso-oc-2.54.1/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-02 18:53:11.000000 nso-oc-2.54.1/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-02 18:53:11.000000 nso-oc-2.54.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 18:53:41.053604 nso-oc-2.54.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-02 18:53:11.000000 nso-oc-2.54.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-02 23:10:35.000000 nso-oc-2.54.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 23:10:35.000000 nso-oc-2.54.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 23:11:05.664108 nso-oc-2.54.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 23:10:35.000000 nso-oc-2.54.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-02 23:10:35.000000 nso-oc-2.54.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 23:11:05.668108 nso-oc-2.54.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-02 23:10:35.000000 nso-oc-2.54.2/setup.py
```

### Comparing `nso-oc-2.54.1/LICENSE` & `nso-oc-2.54.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/PKG-INFO` & `nso-oc-2.54.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.54.1
+Version: 2.54.2
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.54.1/README.md` & `nso-oc-2.54.2/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.54.2/nso_oc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.54.1
+Version: 2.54.2
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.54.1/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.54.2/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/README.md` & `nso-oc-2.54.2/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/common.py` & `nso-oc-2.54.2/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/main.py` & `nso-oc-2.54.2/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.54.2/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.54.2/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.54.2/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.54.2/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.54.2/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.54.2/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.1/setup.py` & `nso-oc-2.54.2/setup.py`

 * *Files identical despite different names*

