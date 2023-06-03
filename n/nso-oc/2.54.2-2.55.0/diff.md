# Comparing `tmp/nso-oc-2.54.2.tar.gz` & `tmp/nso-oc-2.55.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.54.2.tar", last modified: Fri Jun  2 23:11:05 2023, max compression
+gzip compressed data, was "nso-oc-2.55.0.tar", last modified: Sat Jun  3 17:00:44 2023, max compression
```

## Comparing `nso-oc-2.54.2.tar` & `nso-oc-2.55.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-02 23:10:35.000000 nso-oc-2.54.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 23:10:35.000000 nso-oc-2.54.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 23:11:05.664108 nso-oc-2.54.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 23:10:35.000000 nso-oc-2.54.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 23:11:05.000000 nso-oc-2.54.2/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:11:05.664108 nso-oc-2.54.2/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-02 23:10:35.000000 nso-oc-2.54.2/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-02 23:10:35.000000 nso-oc-2.54.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 23:11:05.668108 nso-oc-2.54.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-02 23:10:35.000000 nso-oc-2.54.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:44.722680 nso-oc-2.55.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-03 17:00:14.000000 nso-oc-2.55.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 17:00:14.000000 nso-oc-2.55.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-03 17:00:44.722680 nso-oc-2.55.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-03 17:00:14.000000 nso-oc-2.55.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:44.718680 nso-oc-2.55.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 17:00:44.000000 nso-oc-2.55.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:44.718680 nso-oc-2.55.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:44.722680 nso-oc-2.55.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42335 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:00:44.722680 nso-oc-2.55.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-03 17:00:14.000000 nso-oc-2.55.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-03 17:00:14.000000 nso-oc-2.55.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 17:00:44.722680 nso-oc-2.55.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-03 17:00:14.000000 nso-oc-2.55.0/setup.py
```

### Comparing `nso-oc-2.54.2/LICENSE` & `nso-oc-2.55.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/PKG-INFO` & `nso-oc-2.55.0/package_nso_to_oc/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nso-oc
-Version: 2.54.2
-Summary: Cisco NSO OpenConfig Tools
-Home-page: https://github.com/model-driven-devops/nso-oc-services
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## NSO NED device configuration to OpenConfig
 
 This python package will read in a json configuration for a device and translate to OpenConfig
 
 ### Usage
 1. Decide whether pulling configuration from NSO or reading from file and set the appropriate envars
    - For NSO
@@ -32,8 +24,8 @@
    ```
 3. The below files will be placed in a new directory names "output_data"
    - device_name.json = the full configuration is pulled from NSO
    - device_name_notes.txt = notes resulting from converting NSO config to OpenConfig
    - device_name_openconfig.json = New OpenConfig config
    - device_name_remaining.json = Remaining configuration from NSO
 
-Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
+Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
```

### Comparing `nso-oc-2.54.2/README.md` & `nso-oc-2.55.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.55.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.54.2
+Version: 2.55.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.54.2/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.55.0/nso_oc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 package_nso_to_oc/main.py
 package_nso_to_oc/xe/__init__.py
 package_nso_to_oc/xe/common_xe.py
 package_nso_to_oc/xe/main_xe.py
 package_nso_to_oc/xe/xe_acls.py
 package_nso_to_oc/xe/xe_bgp.py
 package_nso_to_oc/xe/xe_interfaces.py
+package_nso_to_oc/xe/xe_mpls.py
 package_nso_to_oc/xe/xe_network_instances.py
 package_nso_to_oc/xe/xe_ospfv2.py
 package_nso_to_oc/xe/xe_routing_policy.py
 package_nso_to_oc/xe/xe_static_route.py
 package_nso_to_oc/xe/xe_stp.py
 package_nso_to_oc/xe/xe_system.py
 package_nso_to_oc/xe/xe_vlans.py
```

### Comparing `nso-oc-2.54.2/package_nso_to_oc/README.md` & `nso-oc-2.55.0/nso_oc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nso-oc
+Version: 2.55.0
+Summary: Cisco NSO OpenConfig Tools
+Home-page: https://github.com/model-driven-devops/nso-oc-services
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## NSO NED device configuration to OpenConfig
 
 This python package will read in a json configuration for a device and translate to OpenConfig
 
 ### Usage
 1. Decide whether pulling configuration from NSO or reading from file and set the appropriate envars
    - For NSO
@@ -24,8 +32,8 @@
    ```
 3. The below files will be placed in a new directory names "output_data"
    - device_name.json = the full configuration is pulled from NSO
    - device_name_notes.txt = notes resulting from converting NSO config to OpenConfig
    - device_name_openconfig.json = New OpenConfig config
    - device_name_remaining.json = Remaining configuration from NSO
 
-Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
+Ideally device_name_openconfig.json + device_name_remaining.json = device_name.json
```

### Comparing `nso-oc-2.54.2/package_nso_to_oc/common.py` & `nso-oc-2.55.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/main.py` & `nso-oc-2.55.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
             vrf_forwarding_list = route_forwarding_list_by_vrf.get(net_inst["openconfig-network-instance:name"])
             xe_static_route.configure_xe_static_routes(net_inst, vrf_forwarding_list, config_leftover,
                                                        network_instances_notes)
         
         xe_ospfv2.configure_xe_ospf_redistribution(net_inst, config_before, config_leftover, router_ospf_by_vrf)
         xe_bgp.configure_xe_bgp(net_inst, config_before, config_leftover, network_instances_notes)
         xe_bgp.configure_xe_bgp_redistribution(net_inst, config_before, config_leftover)
+        xe_mpls.configure_xe_mpls(net_inst, config_before, config_before, network_instances_notes)
 
 
 def configure_network_interfaces(net_inst, interfaces_by_vrf):
     for interface in interfaces_by_vrf.get(net_inst["openconfig-network-instance:name"], []):
         name_split = interface["name"].split(".")
         primary_interface = name_split[0]
         new_interface = {
@@ -800,20 +801,22 @@
     sys.path.append("../../../")
 
     if (find_spec("package_nso_to_oc") is not None):
         from package_nso_to_oc.xe import common_xe
         from package_nso_to_oc.xe import xe_ospfv2
         from package_nso_to_oc.xe import xe_static_route
         from package_nso_to_oc.xe import xe_bgp
+        from package_nso_to_oc.xe import xe_mpls
         from package_nso_to_oc import common
     else:
         import common_xe
         import xe_ospfv2
         import xe_static_route
         import xe_bgp
+        import xe_mpls
         import common
 
     (config_before_dict, config_leftover_dict, interface_ip_dict) = common_xe.init_xe_configs()
     main(config_before_dict, config_leftover_dict)
     config_name = "_network_instances"
     config_remaining_name = "_remaining_network_instances"
     oc_name = "_openconfig_network_instances"
@@ -823,14 +826,16 @@
 else:
     # This is needed for now due to top level __init__.py. We need to determine if contents in __init__.py is still necessary.
     if (find_spec("package_nso_to_oc") is not None):
         from package_nso_to_oc.xe import common_xe
         from package_nso_to_oc.xe import xe_ospfv2
         from package_nso_to_oc.xe import xe_static_route
         from package_nso_to_oc.xe import xe_bgp
+        from package_nso_to_oc.xe import xe_mpls
         from package_nso_to_oc import common
     else:
         from xe import common_xe
         from xe import xe_ospfv2
         from xe import xe_static_route
         from xe import xe_bgp
+        from xe import xe_mpls
         import common
```

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.55.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.55.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.55.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.55.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.55.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.55.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.54.2/setup.py` & `nso-oc-2.55.0/setup.py`

 * *Files identical despite different names*

