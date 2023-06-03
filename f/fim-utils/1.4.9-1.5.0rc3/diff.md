# Comparing `tmp/fim_utils-1.4.9.tar.gz` & `tmp/fim_utils-1.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.4.9.tar", last modified: Wed Feb  1 22:52:01 2023, max compression
+gzip compressed data, was "fim_utils-1.5.0rc3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.4.9.tar` & `fim_utils-1.5.0rc3.tar`

### file list

```diff
@@ -1,43 +1,38 @@
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.652475 fim_utils-1.4.9/
--rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2021-03-24 00:22:11.000000 fim_utils-1.4.9/LICENSE
--rw-r--r--   0 ibaldin    (502) staff       (20)      201 2022-08-11 21:42:55.000000 fim_utils-1.4.9/MANIFEST.in
--rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-02-01 22:52:01.652203 fim_utils-1.4.9/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)     7536 2022-11-18 22:04:52.000000 fim_utils-1.4.9/README.md
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.639320 fim_utils-1.4.9/fim_utils.egg-info/
--rw-r--r--   0 ibaldin    (502) staff       (20)      493 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)      809 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)      461 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/requires.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        8 2023-02-01 22:52:01.000000 fim_utils-1.4.9/fim_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.639577 fim_utils-1.4.9/fimutil/
--rw-r--r--   0 ibaldin    (502) staff       (20)       25 2023-02-01 22:51:36.000000 fim_utils-1.4.9/fimutil/__init__.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.641379 fim_utils-1.4.9/fimutil/al2s/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/al2s/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9065 2023-01-17 20:07:11.000000 fim_utils-1.4.9/fimutil/al2s/arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11087 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/al2s/oess.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.644067 fim_utils-1.4.9/fimutil/netam/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2021-10-19 20:02:19.000000 fim_utils-1.4.9/fimutil/netam/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    19470 2023-01-20 02:29:04.000000 fim_utils-1.4.9/fimutil/netam/arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4247 2023-01-08 20:10:10.000000 fim_utils-1.4.9/fimutil/netam/nso.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3439 2021-09-17 00:59:00.000000 fim_utils-1.4.9/fimutil/netam/sr_pce.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.649751 fim_utils-1.4.9/fimutil/ralph/
--rw-r--r--   0 ibaldin    (502) staff       (20)        2 2022-02-22 22:46:07.000000 fim_utils-1.4.9/fimutil/ralph/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3438 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/asset.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2454 2022-11-09 23:04:15.000000 fim_utils-1.4.9/fimutil/ralph/dp_switch.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3835 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/ethernetport.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    20282 2022-11-12 16:12:02.000000 fim_utils-1.4.9/fimutil/ralph/fim_helper.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1075 2021-07-02 19:22:05.000000 fim_utils-1.4.9/fimutil/ralph/gpu.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3307 2022-10-26 01:51:00.000000 fim_utils-1.4.9/fimutil/ralph/model.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1464 2023-02-01 22:45:42.000000 fim_utils-1.4.9/fimutil/ralph/nvme.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1384 2021-09-27 19:32:26.000000 fim_utils-1.4.9/fimutil/ralph/ralph_uri.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4912 2022-11-09 23:04:15.000000 fim_utils-1.4.9/fimutil/ralph/site.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      885 2021-07-02 19:22:05.000000 fim_utils-1.4.9/fimutil/ralph/storage.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9208 2022-11-18 22:04:52.000000 fim_utils-1.4.9/fimutil/ralph/worker_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      462 2022-12-21 02:37:06.000000 fim_utils-1.4.9/requirements.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-02-01 22:52:01.652554 fim_utils-1.4.9/setup.cfg
--rw-r--r--   0 ibaldin    (502) staff       (20)      984 2022-08-11 21:42:55.000000 fim_utils-1.4.9/setup.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-01 22:52:01.651642 fim_utils-1.4.9/utilities/
--rw-r--r--   0 ibaldin    (502) staff       (20)     6183 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/generate_instance_flavors.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1694 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/scan_net.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5482 2022-10-26 01:51:00.000000 fim_utils-1.4.9/utilities/scan_site.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1975 2021-09-27 19:32:26.000000 fim_utils-1.4.9/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fim_utils-1.5.0rc3/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.0rc3/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.0rc3/MANIFEST.in
+-rw-r--r--   0        0        0     7348 2023-06-03 17:33:55.104520 fim_utils-1.5.0rc3/README.md
+-rw-r--r--   0        0        0      159 2023-06-02 22:05:34.391169 fim_utils-1.5.0rc3/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.0rc3/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.0rc3/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.0rc3/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.0rc3/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.0rc3/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fim_utils-1.5.0rc3/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.0rc3/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.0rc3/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.0rc3/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fim_utils-1.5.0rc3/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.0rc3/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fim_utils-1.5.0rc3/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21981 2023-06-02 21:31:39.454775 fim_utils-1.5.0rc3/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fim_utils-1.5.0rc3/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fim_utils-1.5.0rc3/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.0rc3/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fim_utils-1.5.0rc3/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.0rc3/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.0rc3/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.0rc3/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fim_utils-1.5.0rc3/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fim_utils-1.5.0rc3/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fim_utils-1.5.0rc3/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-02 22:02:16.828125 fim_utils-1.5.0rc3/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fim_utils-1.5.0rc3/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fim_utils-1.5.0rc3/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fim_utils-1.5.0rc3/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0      950 2023-06-03 18:07:08.151748 fim_utils-1.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.0rc3/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.0rc3/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.0rc3/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.0rc3/test/ralph_test.py
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 fim_utils-1.5.0rc3/PKG-INFO
```

### Comparing `fim_utils-1.4.9/LICENSE` & `fim_utils-1.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/README.md` & `fim_utils-1.5.0rc3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-[![Requirements Status](https://requires.io/github/fabric-testbed/information-model-utils/requirements.svg?branch=main)](https://requires.io/github/fabric-testbed/information-model-utils/requirements/?branch=main)
-
 [![PyPI](https://img.shields.io/pypi/v/fim-utils?style=plastic)](https://pypi.org/project/fim-utils/)
 
 # Information Model Utilities
 
 There are a number of libraries and utilities in this repo that help convert 
 information from various sources into FABRIC Information Models
 
@@ -168,15 +166,15 @@
 ```
 ## Installation
 
 ### For use
 
 You can use a virtualenv or install directly:
 ```
-$ pip install fim-utils
+$ pip install fimutil
 ```
 
 ### For development
 
 Developed under Python 3.9. Using virtualenv, something like this should work:
 
 ```
@@ -184,14 +182,14 @@
 $ mkvirtualenv -r requirements.txt fim-utils
 $ cd information-model-utils/utilities/
 $ python scan_worker.py <options>
 ```
 Note that to install PyJQ dependency as part of requirements you need to have `automake` installed on your system. So
 `yum install automake` or `brew install automake` or similar. 
 
-### Building and packaging
+### Building and packaging 
 
-Use 
+Use (make sure to `pip install flit` first):
 ```
-$ python -m build
-$ twine upload dist/*
+$ flit build
+$ flit publish
 ```
```

### Comparing `fim_utils-1.4.9/fimutil/al2s/arm.py` & `fim_utils-1.5.0rc3/fimutil/al2s/arm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import fim.user as f
 import fim.slivers.capacities_labels as caplab
 from fim.slivers.interface_info import InterfaceType
 from fim.slivers.network_node import NodeType
 from fim.slivers.network_service import ServiceType
 
 from fimutil.al2s.oess import OessClient
+from fimutil.al2s.cloud_cfg import REGION_NAME_MAP
 from yaml import load as yload
 from yaml import FullLoader
 import os
 import re
 
 
+
 def _update_vlan_label(labs, vlan: str):
     if '-' not in vlan and ',' not in vlan:
         return f.Labels.update(labs, vlan=vlan)
     else:
         try:
             return f.Labels.update(labs, vlan_range=vlan.split(','))
         except caplab.LabelException:
             return labs
 
 
+def _tralsate_cloud_region_name(name: str):
+    if name not in REGION_NAME_MAP.keys():
+        return name
+    return REGION_NAME_MAP[name]
+
+
 class OessARM:
     """
     Generate AL2S AM resources information model.
     """
 
     def __init__(self, *, config_file=None, isis_link_validation=False):
         self.topology = None
@@ -40,15 +48,15 @@
                 if 'AL2S' in sites_metadata:
                     self.site_info = sites_metadata['AL2S']
 
     def build_topology(self) -> None:
         # start topology model
         self.topology = f.SubstrateTopology()
         model_name = 'AL2S OESS'
-        site_name = "Internet2"
+        site_name = "AL2S"
         node_name = "AL2S"
         node_nid = "node+" + node_name
         switch = self.topology.add_node(name=node_name, model=model_name, site=site_name,
                                         node_id=node_nid, ntype=f.NodeType.Switch,
                                         capacities=f.Capacities(unit=1),
                                         labels=f.Labels(local_name=node_name), stitch_node=False)
         # add L2 NetworkService
@@ -75,15 +83,15 @@
             # port_mac = port['phys-address'] # add to port_labs if available
             port_nid = f"port+al2s:{port_name}"
             speed_gbps = int(port['capacity'])
             vlan_range = port['vlan_range']
             # add capabilities
             port_caps = f.Capacities(bw=speed_gbps)
             # add labels
-            port_labs = f.Labels(local_name=port_name)
+            port_labs = f.Labels(device_name=port['device_name'], local_name=port['interface_name'])
             port_labs = _update_vlan_label(port_labs, vlan_range)
 
             # TODO: identify FABRIC facing interface
             #   Add WAN switch node, network_service and ports with stitch_node=True
             #   Add Links with stitch_node=False
             #   ++ The peering WAN site / port IDs will come from config inventory.
             #   ++ Or ask Internet2 to incldue peering into FABRIC entity->interface->description instead
@@ -94,44 +102,49 @@
 
             # add facility_ports based on stitching metadata
             if 'cloud_interconnect_type' in port and 'cloud_provider' in port:
                 if port['cloud_interconnect_type'] == 'aws-hosted-connection' \
                         or port['cloud_interconnect_type'] == 'gcp-partner-interconnect' \
                         or port['cloud_interconnect_type'] == 'azure-express-route':
                     # facility by cloud peering port
-                    fac_name = re.sub("\s|:|\(|\)", "_", f"Cloud_Facility:{port['cloud_provider']}")
+                    fac_name = re.sub("\s|:|\(|\)", "-", f"Cloud-Facility:{port['cloud_provider']}")
                     # print(f'Facility: {fac_name}\n')
-                    faci_name = re.sub("\s|:|\(|\)", "_", f"{port['cloud_provider']}:{port['cloud_region']}:{port_name}")
+                    faci_name = re.sub("\s|:|\(|\)", "-",
+                                       f"{port['cloud_provider']}:{port['cloud_region']}:{port_name}")
                     # facility_port attributes
                     facility_port_labs = f.Labels()
                     facility_port_labs = _update_vlan_label(facility_port_labs, vlan_range)
-                    facility_port_labs = f.Labels.update(facility_port_labs, device_name=port['cloud_region'])
-                    facility_port_labs = f.Labels.update(facility_port_labs, local_name=port_name + ':peer')
+                    facility_port_labs = f.Labels.update(facility_port_labs,
+                                                         region=_tralsate_cloud_region_name(port['cloud_region']))
+                    facility_port_labs = f.Labels.update(facility_port_labs, device_name=port['device_name'])
+                    facility_port_labs = f.Labels.update(facility_port_labs, local_name=port['interface_name'])
                     facility_port_caps = f.Capacities()
                     facility_port_caps = f.Labels.update(facility_port_caps, bw=speed_gbps)
                     if fac_name in cloud_facs:
                         facs = cloud_facs[fac_name]
                         # add an interface / facility_port to the facility
                         faci = facs.add_interface(name=faci_name, node_id=f"{port_nid}:{fac_name}:facility_port",
-                                                                     itype=InterfaceType.FacilityPort,
-                                                                     labels=facility_port_labs,
-                                                                     capacities=facility_port_caps)
+                                                  itype=InterfaceType.FacilityPort,
+                                                  labels=facility_port_labs,
+                                                  capacities=facility_port_caps)
                         self.topology.add_link(name=fac_name + '-link:' + port_name,
                                                node_id=f'{port_nid}:facility+{fac_name}+link',
                                                ltype=f.LinkType.L2Path,  # could be Patch too
                                                interfaces=[sp, faci])  # add additional interface to the facility
                     else:
                         facn = self.topology.add_node(name=fac_name, node_id=f'{port_nid}:facility+{fac_name}',
-                                                         site=re.sub("\s|:|\(|\)", "_", port['cloud_provider']), ntype=NodeType.Facility)
-                        facs = facn.add_network_service(name=facn.name + '-ns', node_id=f'{port_nid}:facility+{fac_name}-ns',
+                                                      site=re.sub("\s|:|\(|\)", "-", port['cloud_provider']),
+                                                      ntype=NodeType.Facility)
+                        facs = facn.add_network_service(name=facn.name + '-ns',
+                                                        node_id=f'{port_nid}:facility+{fac_name}-ns',
                                                         nstype=ServiceType.VLAN)
                         faci = facs.add_interface(name=faci_name, node_id=f"{port_nid}:{fac_name}:facility_port",
-                                                                     itype=InterfaceType.FacilityPort,
-                                                                     labels=facility_port_labs,
-                                                                     capacities=facility_port_caps)
+                                                  itype=InterfaceType.FacilityPort,
+                                                  labels=facility_port_labs,
+                                                  capacities=facility_port_caps)
 
                         if 'description' in port:
                             faci.details = port['description']
                         # connect it to the switch port via link
                         self.topology.add_link(name=fac_name + '-link:' + port_name,
                                                node_id=f'{port_nid}:facility+{fac_name}+link',
                                                ltype=f.LinkType.L2Path,  # could be Patch too
```

### Comparing `fim_utils-1.4.9/fimutil/al2s/oess.py` & `fim_utils-1.5.0rc3/fimutil/al2s/oess.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,18 +166,20 @@
             endpoint_list = []
             for entity in entities:
                 for interface in entity['interfaces']:
                     endpoint = {}
                     vlan_range = ""
                     for acl in interface['acls']:
                         if acl['workgroup_id'] == workgid:
+                            new_range = acl["start"] + "-" + acl["end"]
                             if vlan_range:
-                                vlan_range = vlan_range + ',' + acl["start"] + "-" + acl["end"]
+                                if (vlan_range.find(new_range) == -1):
+                                    vlan_range = vlan_range + ',' + new_range
                             else:
-                                vlan_range = acl["start"] + "-" + acl["end"]
+                                vlan_range = new_range
                     
                     if vlan_range: 
                         endpoint['name'] = interface['node'] + ':' + interface['name']
                         endpoint['description'] = interface['description']
                         endpoint['device_name'] = interface['node']
                         endpoint['interface_name'] = interface['name']
                         endpoint['capacity'] =str(int(float(interface['bandwidth'])/1000.0))
@@ -202,18 +204,20 @@
                                 grandparent_name = self.get_parent_entity_name(parent_name, entities)
                                 if grandparent_name == 'Cloud Providers':
                                     endpoint['cloud_provider'] = parent_name
                                 else:
                                     endpoint['cloud_provider'] = grandparent_name
                             vlan_range = ""
                             for acl in interface['acls']:
+                                new_range = acl["start"] + "-" + acl["end"]
                                 if vlan_range:
-                                    vlan_range = vlan_range + ',' + acl["start"] + "-" + acl["end"]
+                                    if (vlan_range.find(new_range) == -1):
+                                        vlan_range = vlan_range + ',' + new_range
                                 else:
-                                    vlan_range = acl["start"] + "-" + acl["end"]
+                                    vlan_range = new_range
                             endpoint['vlan_range'] = vlan_range
                             if endpoint not in endpoint_list:
                                 endpoint_list.append(endpoint)
                         
             return endpoint_list
         except HTTPError as http_err:
             print(f'HTTP error occurred: {http_err}')
```

### Comparing `fim_utils-1.4.9/fimutil/netam/arm.py` & `fim_utils-1.5.0rc3/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/netam/nso.py` & `fim_utils-1.5.0rc3/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/netam/sr_pce.py` & `fim_utils-1.5.0rc3/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/asset.py` & `fim_utils-1.5.0rc3/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.0rc3/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.0rc3/fimutil/ralph/ethernetport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import logging
-import re
 from fimutil.ralph.asset import RalphAsset, RalphAssetType, RalphAssetMimatch
 
 from fimutil.ralph.ralph_uri import RalphURI
 
 
 class EthernetPort(RalphAsset):
     """
@@ -39,15 +37,16 @@
     # "Description: "Intel Corporation I350 Gigabit Network Connection (rev 01) in NIC Port 2 (0000:02:00.1)"
     # "Connection": "Connected to port 7 on uky2-data-sw"
     REGEX_FIELDS = {'BDF': ['Description', ".+?\\(([0-9a-f:.]+)\\).*"],
                     'vBDF': ['Description', ".+/\\(([0-9a-f:.]+)\\).*"],
                     'Peer_port': ['Connection', ".+port ([\\w\\d/]+) .+"],
                     'VLAN': ['Connection', ".+ VLAN ([\\d]+) on.+"],
                     'Model': ['Description', ".+\\[([\\w-]+).*?\\].*"],
-                    'Slot': ['Description', ".+Slot ([\\d]+) .*"]}
+                    'Slot': ['Description', ".+Slot ([\\d]+) .*"],
+                    'NUMA': ['Description', '.+ NUMA Node ([\\+\\-\\d]+).*']}
 
     def __init__(self, *, uri: str, ralph: RalphURI):
         super().__init__(uri=uri, ralph=ralph)
         self.type = RalphAssetType.EthernetCardPF
 
     def parse(self):
         super().parse()
@@ -62,14 +61,15 @@
                      desc: str or None = None,
                      speed: str or None = None,
                      connection: str or None = None,
                      peer_port: str or None = None,
                      vlan: str or None = None,
                      model: str or None = None,
                      slot: str or None = None,
+                     numa: str or None = None,
                      ctype: RalphAssetType = RalphAssetType.EthernetCardPF):
         """
         when you just want to force values without parsing. type defaults to a VF
         """
         self.type = ctype
         if bdf:
             self.fields['BDF'] = bdf
@@ -87,7 +87,9 @@
             self.fields['MAC'] = mac
         if desc:
             self.fields['Description'] = desc
         if speed:
             self.fields['Speed'] = speed
         if connection:
             self.fields['Connection'] = connection
+        if numa:
+            self.fields['NUMA'] = numa
```

### Comparing `fim_utils-1.4.9/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.0rc3/fimutil/ralph/fim_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from fim.user.topology import SubstrateTopology
 from fim.user.node import Node, NodeType
 from fim.user.interface import Interface, InterfaceType
 from fim.user.component import Component, ComponentType
 from fim.user.link import LinkType
 from fim.user.network_service import ServiceType
 from fim.slivers.identifiers import *
-from fim.slivers.capacities_labels import Capacities, Labels, Location
+from fim.slivers.capacities_labels import Capacities, Labels, Location, Flags
 
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.site import Site
 from fimutil.ralph.gpu import GPU
+from fimutil.ralph.fpga import FPGA
 from fimutil.ralph.ethernetport import EthernetCardPort, EthernetPort
 from fimutil.ralph.nvme import NVMeDrive
 from fimutil.ralph.asset import RalphAssetType, RalphAsset
 
 SIZE_REGEX = "([\\d.]+)[ ]?([MGTP])B?"
 SPEED_REGEX = "([\\d.]+)[ ]?([MGT])(bps)?"
 
@@ -180,33 +181,60 @@
     Add a GPU to a topology node
     """
     node.add_component(name=node.name + '-' + gpu_name,
                        model=gpu.Model,
                        node_id=node.node_id + '-' + gpu_name,
                        ctype=ComponentType.GPU,
                        capacities=Capacities(unit=1),
-                       labels=Labels(bdf=gpu.BDF),
+                       labels=Labels(bdf=gpu.BDF, numa=gpu.NUMA),
                        details=gpu.Description)
 
 
+def __add_fpga(node: Node, fpga_name: str, fpga: FPGA, port_map: Dict[str, str]) -> None:
+    """
+    Add FPGA to a node
+    """
+    interface_node_ids = list()
+    interface_labels = list()
+    fpga_node_id = f'fpga-{fpga.SN}'
+    port_id = 1
+    for p in fpga.Ports:
+        interface_node_ids.append(f'{fpga_node_id}-p{port_id}')
+        interface_labels.append(Labels(vlan_range='1-4096'))
+        port_id += 1
+    c = node.add_component(name=node.name + '-' + fpga_name,
+                           model=fpga.Model,
+                           node_id=fpga_node_id,
+                           ctype=ComponentType.FPGA,
+                           capacities=Capacities(unit=1),
+                           labels=Labels(bdf=fpga.BDF, usb_id=fpga.USB_ID, numa=fpga.NUMA),
+                           interface_node_ids=interface_node_ids,
+                           interface_labels=interface_labels,
+                           details=fpga.Description)
+    for intf in c.interface_list:
+        # use local name index (p1, p2 etc) to index into the Ports array
+        port_index = int(intf.labels.local_name[1:])
+        port_map[fpga.Ports[port_index - 1]] = intf
+
+
 def __add_nvme(node: Node, nvme_name: str, nvme: NVMeDrive) -> None:
     """
     Add an NVME drive to a topology node
     """
     # {"SN": "PHLJ015301K31P0FGN", "Description": "Dell ....",
     # "BDF": "0000:22:00.0", "Model": "P4510"}
     disk_size, disk_units = __parse_size_spec(nvme.fields['Disk'])
     disk_size = __normalize_units(disk_size, disk_units, 'G')
     disk_size_int = int(disk_size)
     node.add_component(name=node.name + '-' + nvme_name,
                        model=nvme.fields['Model'],
                        node_id=nvme.fields['SN'],
                        ctype=ComponentType.NVME,
                        capacities=Capacities(unit=1, disk=disk_size_int),
-                       labels=Labels(bdf=nvme.fields['BDF']),
+                       labels=Labels(bdf=nvme.fields['BDF'], numa=nvme.fields.get('NUMA', '-1')),
                        details=nvme.fields['Description'])
 
 
 def __process_card_port(port: EthernetCardPort, org: CardOrganizer) -> None:
     """
     Aggregate and organize the ports:
     - VFs need to be kept together (matched by parent PCI id) - 100s of ports
@@ -224,51 +252,55 @@
     elif port.type == RalphAssetType.EthernetCardVF:
         org.add_vf(port)
     else:
         logging.error(f'Unsupported port type {port.type=}')
         raise RuntimeError('Unable to continue')
 
 
-def __convert_vf_list_to_interface_labels(vfs: List[EthernetCardPort]) -> Tuple[List[str], List[str], List[str]]:
+def __convert_vf_list_to_interface_labels(vfs: List[EthernetCardPort]) -> Tuple[List[str], List[str], List[str], List[str]]:
     """
     Take a list of VFs of a single parent PF and convert into a tuple of lists one for MAC, child BDF and VLAN
     (in that order)
     """
     macs = list()
     bdfs = list()
     vlans = list()
+    numas = list()
     for vf in vfs:
         macs.append(vf.fields['MAC'])
         bdfs.append(vf.fields['vBDF'])
         vlans.append(vf.fields['VLAN'])
+        numas.append(vf.fields.get('NUMA', '-1'))
 
-    return macs, bdfs, vlans
+    return macs, bdfs, vlans, numas
 
 
-def __convert_pf_list_to_interface_data(pfs: List[EthernetCardPort]) -> Tuple[List[str], List[str], List[str]]:
+def __convert_pf_list_to_interface_data(pfs: List[EthernetCardPort]) -> Tuple[List[str], List[str], List[str], List[str]]:
     """
-    Take a list of PF ports of the same card and convert into tuple of two lists -
-    macs, bdfs and peer ports
+    Take a list of PF ports of the same card and convert into tuple of  lists -
+    macs, bdfs and peer ports and numa nodes
     """
     macs = list()
     bdfs = list()
     peers = list()
+    numas = list()
     slot = None
     for pf in pfs:
         macs.append(pf.fields['MAC'])
         bdfs.append(pf.fields['BDF'])
         peers.append(pf.fields['Peer_port'])
+        numas.append(pf.fields.get('NUMA', '-1'))
         if slot is None:
             slot = pf.fields['Slot']
         else:
             if slot != pf.fields['Slot']:
                 logging.error(f'Slot of {pf} does not match the slot of other PFs in this card')
                 raise RuntimeError()
 
-    return macs, bdfs, peers
+    return macs, bdfs, peers, numas
 
 
 def site_to_fim(site: Site, address: str, config: Dict = None) -> SubstrateTopology:
     """
     Produce a site substrate topology advertisements from Ralph site information.
     Optionally supply externally obtained postal address.
     """
@@ -293,58 +325,62 @@
         cap = Capacities(unit=1,
                          cpu=int(worker.model.fields['CPU']),
                          core=int(worker.model.fields['Core']),
                          ram=ram_size_int,
                          disk=disk_size_int)
         w = topo.add_node(name=worker.fields['Name'], model=worker.model.fields['Model'],
                           node_id=worker.fields['SN'], ntype=NodeType.Server,
-                          capacities=cap, site=site.name, location=loc)
+                          capacities=cap, site=site.name, location=loc, flags=Flags(ptp=worker.ptp))
         #
         # handle various component types
         #
         org = CardOrganizer()
 
         # NVMEs and GPUs; Network Cards (need to merge ports to cards), FPGAs (later)
         for comp_name, comp in worker.components.items():
             if isinstance(comp, NVMeDrive):
                 __add_nvme(w, comp_name, comp)
             elif isinstance(comp, EthernetCardPort):
                 __process_card_port(comp, org)
             elif isinstance(comp, GPU):
                 __add_gpu(w, comp_name, comp)
+            elif isinstance(comp, FPGA):
+                __add_fpga(w, comp_name, comp, port_map)
 
         org.organize()
 
         logging.debug('Adding shared SR-IOV cards')
         # create VF components
         for k, v in org.get_shared_cards().items():
             logging.debug(f'Processing {v}')
-            parent_macs, parent_bdfs, parent_peers = __convert_pf_list_to_interface_data(v)
+            parent_macs, parent_bdfs, parent_peers, parent_numas = __convert_pf_list_to_interface_data(v)
             units = 0
             labs = list()
             child_bdfs = list()
+            child_numas = list()
             for pf_parent in v:
                 child_vfs = org.get_vfs_of_parent(pf_parent.fields['BDF'])
-                macs, bdfs, vlans = __convert_vf_list_to_interface_labels(child_vfs)
-                labs.append(Labels(mac=macs, bdf=bdfs, vlan=vlans))
+                macs, bdfs, vlans, numas = __convert_vf_list_to_interface_labels(child_vfs)
+                labs.append(Labels(mac=macs, vlan=vlans))
                 child_bdfs.extend(bdfs)
+                child_numas.extend(numas)
                 units += len(child_vfs)
             slot = v[0].fields['Slot']
             model = v[0].fields['Model']
             descr = v[0].fields['Description']
             interface_node_ids = list(map(mac_to_node_id, parent_macs))
             shnic = w.add_component(name=w.name + '-slot' + slot,
                                     node_id=w.node_id + '-slot' + slot,
                                     model=model,
                                     network_service_node_id=w.node_id + '-slot' + slot + '-ns',
                                     # these are lists with element for every PF
                                     interface_node_ids=interface_node_ids,
                                     interface_labels=labs,
                                     capacities=Capacities(unit=units),
-                                    labels=Labels(bdf=child_bdfs),
+                                    labels=Labels(bdf=child_bdfs, numa=child_numas),
                                     ctype=ComponentType.SharedNIC,
                                     details=descr
                                     )
             # need to match interfaces of the component
             for intf in shnic.interface_list:
                 # becase ports/interfaces on shared cards don't carry parent MAC
                 # we have to trace it back from (any) child MAC to parent MAC
@@ -354,30 +390,30 @@
                 parent_mac = parent.fields['MAC']
                 port_map[parent_peers[parent_macs.index(parent_mac)]] = intf
 
         # create PF components
         logging.debug('Adding physical cards')
         for k, v in org.get_dedicated_cards().items():
             logging.debug(f'Processing {v}')
-            macs, bdfs, peers = __convert_pf_list_to_interface_data(v)
+            macs, bdfs, peers, numas = __convert_pf_list_to_interface_data(v)
             interface_node_ids = list(map(mac_to_node_id, macs))
             labels = list()
             for m in macs:
                 labels.append(Labels(mac=m, vlan_range='1-4096'))
 
             # k is PCI id, v is list of EthernetCardPorts
             smnic = w.add_component(name=w.name + '-slot' + v[0].fields['Slot'],
                                     node_id=w.node_id + '-slot' + v[0].fields['Slot'],
                                     model=v[0].fields['Model'],
                                     network_service_node_id=w.node_id + '-slot' + v[0].fields['Slot'] + '-ns',
                                     interface_node_ids=interface_node_ids,
                                     interface_labels=labels,
                                     ctype=ComponentType.SmartNIC,
                                     capacities=Capacities(unit=1),
-                                    labels=Labels(bdf=bdfs),
+                                    labels=Labels(bdf=bdfs, numa=numas),
                                     details=v[0].fields['Description']
                                     )
             for intf in smnic.interface_list:
                 intf_lab = intf.get_property('labels')
                 intf_mac = intf_lab.mac
                 port_map[peers[macs.index(intf_mac)]] = intf
```

### Comparing `fim_utils-1.4.9/fimutil/ralph/gpu.py` & `fim_utils-1.5.0rc3/fimutil/ralph/gpu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import List, Any
 from dataclasses import dataclass
 
 import pyjq
 
-GPU_MODELS = ['Quadro RTX 6000/8000', 'Tesla T4']
+GPU_MODELS = ['Quadro RTX 6000/8000', 'Tesla T4', 'A40', 'A30 PCIe']
 
 
 @dataclass(frozen=True)
 class GPU:
     """
     Note that because GPUs aren't properly part of Ralph catalog structure,
     they appear as special fields inside the node and as such are not
     subclassed from RalphAsset (they don't have a URL).
     """
     Model: str
     Description: str
     BDF: str
+    NUMA: str
 
     @staticmethod
     def find_gpus(node_raw_json) -> List[Any]:
         """
         Find if there are GPUs in this node. Returns a list
         of GPU objects (which can be empty).
         """
@@ -27,9 +28,11 @@
         ret = list()
         for field in custom_fields:
             for gpu_model in GPU_MODELS:
                 if gpu_model in custom_fields[field]:
                     model = gpu_model
                     description = custom_fields[field]
                     bdf = custom_fields[field + '_pci_id']
-                    ret.append(GPU(model, description, bdf))
+                    # -1 means unknown
+                    numa = custom_fields.get(field + '_numa_node', '-1')
+                    ret.append(GPU(model, description, bdf, numa))
         return ret
```

### Comparing `fim_utils-1.4.9/fimutil/ralph/model.py` & `fim_utils-1.5.0rc3/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/nvme.py` & `fim_utils-1.5.0rc3/fimutil/ralph/nvme.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 
 
 class NVMeDrive(RalphAsset):
     """
     This class knows how to parse necessary worker fields in Ralph
     """
     FIELD_MAP = '{SN: .serial_number, Description: .model_name}'
-    # "Description": "Dell Express Flash NVMe P4510 1TB SFF in PCIe
-    # SSD Slot 22 in Bay 2 (0000:21:00.0)", "BDF": "0000:21:00.0"
+    # "Description": "Dell Express Flash NVMe P4510 1TB SFF in PCIe SSD Slot 22 in Bay 2 (0000:21:00.0)",
+    # "BDF": "0000:21:00.0"
+    # or
+    # "Description": "Dell DC NVMe PE8010 RI U.2 960GB in PCIe SSD Slot 22 in Bay 2 (0000:21:00.0) on NUMA Node 0"
     REGEX_FIELDS = {'BDF': ["Description", ".+\\(([0-9a-f:.]+)\\).*"],
                     'Model': ["Description", ".+(P4510|CD5|CD6|PE8010) ([\\w]+).*"],
-                    'Disk': ["Description", ".+ ([\\d]+[MGTP]B|[\\d]+[MGTP]) .*"]}
+                    'Disk': ["Description", ".+ ([\\d]+[MGTP]B|[\\d]+[MGTP]) .*"],
+                    'NUMA': ["Description", ".+ NUMA Node ([\\+\\-\\d]+).*"]}
 
     def __init__(self, *, uri: str, ralph: RalphURI):
         super().__init__(uri=uri, ralph=ralph)
         self.type = RalphAssetType.NVMe
 
     def parse(self):
         super().parse()
```

### Comparing `fim_utils-1.4.9/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.0rc3/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/site.py` & `fim_utils-1.5.0rc3/fimutil/ralph/site.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from abc import ABC
 from urllib.parse import urlencode
 import pyjq
 from typing import Dict
+import json
 
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.worker_node import WorkerNode
 from fimutil.ralph.storage import Storage
 from fimutil.ralph.dp_switch import DPSwitch
 
 
@@ -18,26 +19,28 @@
     def __init__(self, *, site_name: str, ralph: RalphURI, config: Dict = None, domain: str = '.fabric-testbed.net'):
         """
         Site name can be upper or lower case
         """
         self.workers = list()
         self.storage = None
         self.dp_switch = None
+        self.ptp = False
         self.name = site_name
         self.domain = domain
         self.ralph = ralph
         self.config = config
 
     def catalog(self):
         """
         Catalog what the site has by querying for regular expressions. Names of nodes
         are expected to conform to the following convention:
         - workers: <site>-w[\\d]+.fabric-testbed.net
         - storage: <site>-storage.fabric-testbed.net
         - dp switch: <site>-data-sw.fabric-testbed.net
+        - PTP server: <site>-time.fabric-testbed.net
         """
         query = {'hostname': f'{self.name.lower()}-data-sw' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
 
         # config file can override dp switch URL
         dp_switch_url = None
@@ -57,25 +60,38 @@
             if not dp_switch_url:
                 raise ValueError
             self.dp_switch = DPSwitch(uri=dp_switch_url, ralph=self.ralph)
             self.dp_switch.parse()
         except ValueError:
             logging.warning('Unable to find a dataplane switch in site, continuing')
 
+        query = {'hostname': f'{self.name.lower()}-time' + self.domain}
+        results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
+                                             urlencode(query))
+        ptp_url = None
+        try:
+            ptp_url = pyjq.one('[ .results[0].url ]', results)[0]
+            logging.info(f'Identified PTP server {ptp_url=}')
+            if not ptp_url:
+                raise ValueError
+            self.ptp = True
+        except ValueError:
+            logging.warning('Unable to find PTP server in site, continuing')
+
         query = {'hostname__regex': f'{self.name.lower()}-w[1234567890]+' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
 
         worker_urls = pyjq.one('[ .results[].url ]', results)
         logging.info(f'Identified {len(worker_urls)} workers')
 
         for worker in worker_urls:
             logging.info(f'Parsing {worker=}')
             ralph_worker = WorkerNode(uri=worker, ralph=self.ralph, site=self.name,
-                                      dp_switch=self.dp_switch, config=self.config)
+                                      dp_switch=self.dp_switch, config=self.config, ptp=self.ptp)
             ralph_worker.parse()
             self.workers.append(ralph_worker)
 
         query = {'hostname': f'{self.name.lower()}-storage' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
         storage_url = None
@@ -101,15 +117,20 @@
         for w in self.workers:
             assets.append(str(w))
         return '\n'.join(assets)
 
     def to_json(self):
         ret = dict()
         if self.storage:
-            ret["Storage"] = self.storage.fields
+            ret["Storage"] = self.storage.fields.copy()
         if self.dp_switch:
-            ret["DataPlane"] = self.dp_switch.fields
+            ret["DataPlane"] = self.dp_switch.fields.copy()
+        # collect port information from all workers
+        dp_ports = list()
+        for w in self.workers:
+            dp_ports.extend(w.get_dp_ports())
+        ret["DataPlane"]["Connected_ports"] = dp_ports
         n = list()
         for w in self.workers:
             n.append(w.to_json())
         ret["Nodes"] = n
         return ret
```

### Comparing `fim_utils-1.4.9/fimutil/ralph/storage.py` & `fim_utils-1.5.0rc3/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/fimutil/ralph/worker_node.py` & `fim_utils-1.5.0rc3/fimutil/ralph/worker_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import binascii
 from typing import Dict
 
 from fimutil.ralph.asset import RalphAsset, RalphAssetType, RalphJSONError, RalphAssetMimatch
 from fimutil.ralph.nvme import NVMeDrive
 from fimutil.ralph.ethernetport import EthernetCardPort
 from fimutil.ralph.gpu import GPU
+from fimutil.ralph.fpga import FPGA
 from fimutil.ralph.model import WorkerModel
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.dp_switch import DPSwitch
 
 
 class WorkerNode(RalphAsset):
     """
@@ -24,20 +25,22 @@
     # don't start at 1 - that's typically 'uplink'
     OPENSTACK_NIC_INDEX = 10
     OPENSTACK_VNIC_COUNT = 2000 # randomly set 2000 vNICs to be created
     WORKER_NAME_REGEX = r'^[\w]+-w([\d]+).fabric-testbed.net$'
     # first octet must be even
     OPENSTACK_NIC_MAC_REG = r'([a-fA-F0-9][aceACE02468])[:-]([a-fA-F0-9]{2})'
 
-    def __init__(self, *, uri: str, ralph: RalphURI, site: str = None, dp_switch: DPSwitch, config: Dict = None):
+    def __init__(self, *, uri: str, ralph: RalphURI, site: str = None, dp_switch: DPSwitch, config: Dict = None,
+                 ptp: bool = False):
         super().__init__(uri=uri, ralph=ralph)
         self.type = RalphAssetType.Node
         self.model = None
         self.site = site
         self.config = config
+        self.ptp = ptp # comes from site
         # so we can get VLAN info
         self.dp_switch = dp_switch
 
     @staticmethod
     def generate_openstack_mac(site_offset: str, worker: str, count: int) -> str:
         """
         generate a unique MAC address for a single OpenStack vNIC on a given
@@ -75,25 +78,39 @@
         super().parse()
 
         # find model
         model_url = pyjq.one('.model.url', self.raw_json_obj)
         self.model = WorkerModel(uri=model_url, ralph=self.ralph)
         try:
             self.model.parse()
-            # override from config if present
-            if self.config and self.config.get(self.site) and self.config.get(self.site).get('workers') and \
-                self.config.get(self.site).get('workers').get(self.fields['Name']):
-                worker_override = self.config.get(self.site).get('workers').get(self.fields['Name'])
-                self.model.fields['RAM'] = worker_override.get('RAM', self.model.fields['RAM'])
-                self.model.fields['CPU'] = worker_override.get('CPU', self.model.fields['CPU'])
-                self.model.fields['Core'] = worker_override.get('Core', self.model.fields['Core'])
-                self.model.fields['Disk'] = worker_override.get('Disk', self.model.fields['Disk'])
         except RalphAssetMimatch:
             pass
 
+        custom_fields_dict = pyjq.one('.custom_fields', self.raw_json_obj)
+
+        # check for usable_ram _disk and _cores custom fields provided from OpenStack -
+        # they override anything on the model. Note they are reported without units
+        self.model.fields['Core'] = custom_fields_dict.get('usable_cores', self.model.fields['Core'])
+        # RAM is in MB reported by OpenStack
+        ram = int(custom_fields_dict.get('usable_memory', '0'))//1024
+        if ram > 0:
+            self.model.fields['RAM'] = f'{ram}G'
+        disk = custom_fields_dict.get('usable_disk')
+        if disk:
+            self.model.fields['Disk'] = f'{disk}G'
+
+        # override from config if present
+        if self.config and self.config.get(self.site) and self.config.get(self.site).get('workers') and \
+            self.config.get(self.site).get('workers').get(self.fields['Name']):
+            worker_override = self.config.get(self.site).get('workers').get(self.fields['Name'])
+            self.model.fields['RAM'] = worker_override.get('RAM', self.model.fields['RAM'])
+            self.model.fields['CPU'] = worker_override.get('CPU', self.model.fields['CPU'])
+            self.model.fields['Core'] = worker_override.get('Core', self.model.fields['Core'])
+            self.model.fields['Disk'] = worker_override.get('Disk', self.model.fields['Disk'])
+
         # find NVMe drives in 'disks' section
         try:
             disk_urls = pyjq.all('.disk[].url', self.raw_json_obj)
         except ValueError:
             logging.warning('Unable to find any disks in node, continuing')
             disk_urls = list()
 
@@ -117,15 +134,15 @@
                 raise RuntimeError('For OpenStack sites you must specify "mac_offset" under site static configuration')
 
             port_index = 1
             # 'parent'
             port = EthernetCardPort(uri='no-url', ralph=self.ralph)
             port.force_values(model='OpenStack-vNIC', desc='OpenStack parent NIC', speed='1Gbps',
                               bdf='0000:00:00.0', mac=self.generate_openstack_mac(mac_offset, self.fields['Name'], 1),
-                              peer_port=str(self.OPENSTACK_NIC_INDEX))
+                              peer_port=str(self.OPENSTACK_NIC_INDEX), numa='-1')
             self.components['port-' + str(port_index)] = port
             port_index += 1
             if not self.dp_switch.vlan_ranges:
                 raise RuntimeError('OpenStack sites should define at least local VLANs '
                                    '(and usually AL2S vlans) as custom fields of dp switch in Ralph, none found')
 
             # Add children with bdf=0000:00:00.0 and vBDF=0000:AB:CD.0 have VLAN 0 set (VLANs are saved on NetworkService)
@@ -134,15 +151,15 @@
                 port = EthernetCardPort(uri='no-url', ralph=self.ralph)
                 # make all vbdfs different and reflection of VLAN tag
                 vbdf_diff = binascii.hexlify(vnic_idx.to_bytes(2, 'big'), ':', 1).decode('utf-8')
                 port.force_values(model='OpenStack-vNIC', desc='OpenStack vNIC', speed='1Gbps', vlan='0',
                                   bdf='0000:00:00.0', vbdf='0000:' + vbdf_diff + '.0',
                                   ctype=RalphAssetType.EthernetCardVF,
                                   mac=self.generate_openstack_mac(mac_offset, self.fields['Name'], vnic_idx),
-                                  peer_port=str(self.OPENSTACK_NIC_INDEX))
+                                  peer_port=str(self.OPENSTACK_NIC_INDEX), numa='-1')
                 self.components['port-' + str(port_index)] = port
                 port_index += 1
             type(self).OPENSTACK_NIC_INDEX += 1
         else:
             # scan for physical NICs and virtual NICs
             try:
                 port_urls = pyjq.all('.ethernet[].url', self.raw_json_obj)
@@ -162,20 +179,27 @@
 
         gpus = GPU.find_gpus(self.raw_json_obj)
         gpu_index = 1
         for gpu in gpus:
             self.components['gpu-' + str(gpu_index)] = gpu
             gpu_index += 1
 
+        fpgas = FPGA.find_fpgas(self.raw_json_obj)
+        fpga_index = 1
+        for fpga in fpgas:
+            self.components['fpga-' + str(fpga_index)] = fpga
+            fpga_index += 1
+
     def __str__(self):
         retl = list()
         if RalphAsset.PRINT_SUMMARY:
-            retl.append(str(self.type) + " " + self.fields['Name'])
+            retl.append(str(self.type) + " " + self.fields['Name'] + f" Flags: {{ PTP: {self.ptp} }}")
         else:
-            retl.append(str(self.type) + "[" + self.uri + "]: " + json.dumps(self.fields))
+            retl.append(str(self.type) + "[" + self.uri + "]: " + json.dumps(self.fields) +
+                        f" Flags: {{ PTP: {self.ptp} }}")
             retl.append('\t' + str(self.model))
         vfcount = 0
         for n, comp in self.components.items():
             if comp.__dict__.get('type', None) is None:
                 # GPU or some other typeless thing
                 retl.append('\t' + n + " " + str(comp))
             elif comp.type != RalphAssetType.EthernetCardVF:
@@ -187,27 +211,38 @@
         retl.append(f'\tDetected {vfcount} SR-IOV functions')
         ret = "\n".join(retl)
         return ret
 
     def to_json(self):
         ret = {
                 'Name': self.fields['Name'],
+                'PTP': self.ptp,
+                'SN': self.fields.get('SN', 'Not available'),
                 'Model': self.model.fields.copy()
         }
         comps = list()
         for n, comp in self.components.items():
             if comp.__dict__.get('type') and comp.type != RalphAssetType.EthernetCardVF:
                 d = comp.fields.copy()
                 d['Type'] = str(comp.type)
                 comps.append(d)
             elif not comp.__dict__.get('type'):
-                # GPU
+                # GPU or FPGA
                 d = comp.__dict__.copy()
                 d['Type'] = str(RalphAssetType.GPU)
                 comps.append(d)
         ret['Components'] = comps
         return ret
 
+    def get_dp_ports(self):
+        """
+        Return a list of names of DP switch ports this node is connected to
+        """
+        dp_ports = list()
+        for n, comp in self.components.items():
+            if comp.__dict__.get('type') and comp.type == RalphAssetType.EthernetCardPF:
+                if comp.fields.get('Peer_port'):
+                    dp_ports.append(comp.fields.get('Peer_port'))
+            if isinstance(comp, FPGA):
+                dp_ports.extend(comp.Ports)
 
-
-
-
+        return dp_ports
```

### Comparing `fim_utils-1.4.9/setup.py` & `fim_utils-1.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/utilities/generate_instance_flavors.py` & `fim_utils-1.5.0rc3/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.4.9/utilities/scan_net.py` & `fim_utils-1.5.0rc3/fimutil/utilities/scan_net.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import argparse
 import logging
 import sys
 
 from fimutil.netam.arm import NetworkARM
 
-if __name__ == "__main__":
 
+def main():
     parser = argparse.ArgumentParser()
     # split into different mutually exclusive operations
 
     parser.add_argument("-c", "--config", action="store",
                         help="config file")
     parser.add_argument("-d", "--debug", action="count",
                         help="Turn on debugging")
@@ -47,7 +47,9 @@
     arm.delegate_topology(delegation1)
 
     logging.info(f'Model completed, saving to {args.model}')
     arm.write_topology(file_name=args.model)
     logging.info('Saving completed')
 
 
+if __name__ == "__main__":
+    main()
```

### Comparing `fim_utils-1.4.9/utilities/scan_site.py` & `fim_utils-1.5.0rc3/fimutil/utilities/scan_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 """
 Scan a site given on command line printing to stdout all pertinent info
 """
 
 import argparse
-import traceback
 import logging
 import sys
 import json
 
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.site import Site
 from fimutil.ralph.asset import RalphAsset
 
 from fimutil.ralph.fim_helper import site_to_fim
 
 from fim.slivers.delegations import DelegationType, Pools
 from fim.slivers.capacities_labels import Location, LocationException
 
-if __name__ == "__main__":
 
+def main():
     parser = argparse.ArgumentParser()
     # split into different mutually exclusive operations
 
     parser.add_argument("-s", "--site", action="store",
                         help="Scan a site for information")
     parser.add_argument("-b", "--base_uri", action="store",
                         help="Base URL of API")
@@ -131,7 +130,10 @@
     if args.print:
         print(site)
 
     if args.json:
         with open(args.json, 'w') as f:
             json.dump(site.to_json(), f, indent=2, sort_keys=True)
 
+
+if __name__ == "__main__":
+    main()
```

### Comparing `fim_utils-1.4.9/utilities/scan_worker.py` & `fim_utils-1.5.0rc3/fimutil/utilities/scan_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 import sys
 
 from fimutil.ralph.ralph_uri import RalphURI
 from fimutil.ralph.worker_node import WorkerNode
 
-if __name__ == "__main__":
+def main():
 
     parser = argparse.ArgumentParser()
     # split into different mutually exclusive operations
 
     parser.add_argument("-w", "--worker", action="store",
                         help="Scan single worker information (use FQDN)")
     parser.add_argument("-b", "--base_uri", action="store",
@@ -50,11 +50,14 @@
     if args.token is None:
         print('You must specify a Ralph API token, you can find it in your profile page in Ralph',
               file=sys.stderr)
         sys.exit(-1)
 
     ralph = RalphURI(token=args.token, base_uri=args.base_uri, disable_ssl=args.no_ssl)
     worker = WorkerNode(uri=args.base_uri + 'data-center-assets/?hostname=' + args.worker,
-                        ralph=ralph)
+                        ralph=ralph, dp_switch=None)
     worker.parse()
     print(worker)
 
+if __name__ == "__main__":
+    main()
+
```

