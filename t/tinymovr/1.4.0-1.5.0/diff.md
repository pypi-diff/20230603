# Comparing `tmp/tinymovr-1.4.0.tar.gz` & `tmp/tinymovr-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinymovr-1.4.0.tar", last modified: Sun Apr 30 22:59:46 2023, max compression
+gzip compressed data, was "tinymovr-1.5.0.tar", last modified: Sat Jun  3 08:28:35 2023, max compression
```

## Comparing `tinymovr-1.4.0.tar` & `tinymovr-1.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.446589 tinymovr-1.4.0/
--rw-r--r--   0 yanconst   (501) staff       (20)      426 2023-04-29 08:24:21.000000 tinymovr-1.4.0/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-30 22:59:46.446398 tinymovr-1.4.0/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.4.0/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-30 22:59:46.446637 tinymovr-1.4.0/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-04-17 16:47:58.000000 tinymovr-1.4.0/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.439984 tinymovr-1.4.0/tinymovr/
--rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3489 2023-04-27 23:25:49.000000 tinymovr-1.4.0/tinymovr/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2845 2023-04-20 17:24:50.000000 tinymovr-1.4.0/tinymovr/cli.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.441827 tinymovr-1.4.0/tinymovr/codec/
--rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.4.0/tinymovr/codec/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/codec/codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.442477 tinymovr-1.4.0/tinymovr/config/
--rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/config/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4111 2023-04-30 22:31:52.000000 tinymovr-1.4.0/tinymovr/config/config.py
--rw-r--r--   0 yanconst   (501) staff       (20)    16329 2023-04-30 22:31:52.000000 tinymovr-1.4.0/tinymovr/config/device.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/constants.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.4.0/tinymovr/discovery.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.443733 tinymovr-1.4.0/tinymovr/gui/
--rw-r--r--   0 yanconst   (501) staff       (20)      474 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1701 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/gui.py
--rw-r--r--   0 yanconst   (501) staff       (20)    14256 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/helpers.py
--rw-r--r--   0 yanconst   (501) staff       (20)    12941 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/gui/window.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-04-17 16:47:58.000000 tinymovr-1.4.0/tinymovr/gui/worker.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.437887 tinymovr-1.4.0/tinymovr/resources/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.445968 tinymovr-1.4.0/tinymovr/resources/icons/
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-20 17:24:50.000000 tinymovr-1.4.0/tinymovr/resources/icons/call.png
--rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    22790 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call_dark.png
--rw-r--r--   0 yanconst   (501) staff       (20)    22672 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/call_dark@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    26604 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty.png
--rw-r--r--   0 yanconst   (501) staff       (20)    44831 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)    30381 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty_dark.png
--rw-r--r--   0 yanconst   (501) staff       (20)    51206 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/resources/icons/empty_dark@2x.png
--rw-r--r--   0 yanconst   (501) staff       (20)     3343 2023-04-29 08:24:21.000000 tinymovr-1.4.0/tinymovr/tee.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-30 22:59:46.441476 tinymovr-1.4.0/tinymovr.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      897 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-04-30 22:59:46.000000 tinymovr-1.4.0/tinymovr.egg-info/top_level.txt
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.724094 tinymovr-1.5.0/
+-rw-r--r--   0 yanconst   (501) staff       (20)      426 2023-05-14 20:28:29.000000 tinymovr-1.5.0/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-06-03 08:28:35.723916 tinymovr-1.5.0/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1689 2023-04-08 07:47:15.000000 tinymovr-1.5.0/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-06-03 08:28:35.724143 tinymovr-1.5.0/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)     2334 2023-05-14 20:28:54.000000 tinymovr-1.5.0/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.718204 tinymovr-1.5.0/tinymovr/
+-rw-r--r--   0 yanconst   (501) staff       (20)       55 2023-04-08 07:47:15.000000 tinymovr-1.5.0/tinymovr/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3489 2023-05-14 20:29:00.000000 tinymovr-1.5.0/tinymovr/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2845 2023-05-14 20:28:58.000000 tinymovr-1.5.0/tinymovr/cli.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.719587 tinymovr-1.5.0/tinymovr/codec/
+-rw-r--r--   0 yanconst   (501) staff       (20)       65 2022-02-09 17:27:03.000000 tinymovr-1.5.0/tinymovr/codec/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2944 2023-04-08 07:47:15.000000 tinymovr-1.5.0/tinymovr/codec/codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.720248 tinymovr-1.5.0/tinymovr/config/
+-rw-r--r--   0 yanconst   (501) staff       (20)      160 2023-04-08 07:47:15.000000 tinymovr-1.5.0/tinymovr/config/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4140 2023-06-03 08:01:45.000000 tinymovr-1.5.0/tinymovr/config/config.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    18659 2023-06-03 08:01:45.000000 tinymovr-1.5.0/tinymovr/config/device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     1075 2023-04-08 07:47:15.000000 tinymovr-1.5.0/tinymovr/constants.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3292 2023-04-08 07:47:15.000000 tinymovr-1.5.0/tinymovr/discovery.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.721494 tinymovr-1.5.0/tinymovr/gui/
+-rw-r--r--   0 yanconst   (501) staff       (20)      474 2023-05-14 20:29:05.000000 tinymovr-1.5.0/tinymovr/gui/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1701 2023-05-14 20:29:04.000000 tinymovr-1.5.0/tinymovr/gui/gui.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    14256 2023-05-14 20:29:03.000000 tinymovr-1.5.0/tinymovr/gui/helpers.py
+-rw-r--r--   0 yanconst   (501) staff       (20)    12941 2023-05-14 20:29:02.000000 tinymovr-1.5.0/tinymovr/gui/window.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4472 2023-05-14 20:29:01.000000 tinymovr-1.5.0/tinymovr/gui/worker.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.716317 tinymovr-1.5.0/tinymovr/resources/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.723506 tinymovr-1.5.0/tinymovr/resources/icons/
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/call.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3184 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/call@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22790 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/call_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    22672 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/call_dark@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    26604 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/empty.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    44831 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/empty@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    30381 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/empty_dark.png
+-rw-r--r--   0 yanconst   (501) staff       (20)    51206 2023-05-14 20:28:29.000000 tinymovr-1.5.0/tinymovr/resources/icons/empty_dark@2x.png
+-rw-r--r--   0 yanconst   (501) staff       (20)     3343 2023-05-14 20:28:57.000000 tinymovr-1.5.0/tinymovr/tee.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-03 08:28:35.719282 tinymovr-1.5.0/tinymovr.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2144 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)      897 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       82 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)      166 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        9 2023-06-03 08:28:35.000000 tinymovr-1.5.0/tinymovr.egg-info/top_level.txt
```

### Comparing `tinymovr-1.4.0/PKG-INFO` & `tinymovr-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.4.0/README.md` & `tinymovr-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/setup.py` & `tinymovr-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/channel.py` & `tinymovr-1.5.0/tinymovr/channel.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/cli.py` & `tinymovr-1.5.0/tinymovr/cli.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/codec/codec.py` & `tinymovr-1.5.0/tinymovr/codec/codec.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/config/config.py` & `tinymovr-1.5.0/tinymovr/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,29 +68,29 @@
     # the remote. This is ok as long as we know that the
     # hash endpoint will always be the 0th one. If there
     # is a hash mismatch, we raise an exception, otherwise
     # we return the device node as is.
     node._channel = chan
     # hash_uint32 is local, proto_hash is remote
     if node.hash_uint32 != node.protocol_hash:
-        raise ProtocolVersionError()
+        raise ProtocolVersionError(node_id, "")
     return node
 
 
 def create_device_with_hash_msg(heartbeat_msg):
     """
     Create a device, the heartbeat msg will be used
     to decode the actual hash value and id
     """
     node_id = heartbeat_msg.arbitration_id & 0x3F
     chan = CANChannel(node_id)
     node = deserialize(dev_def)
     hash, *_ = chan.serializer.deserialize(heartbeat_msg.data[:4], DataType.UINT32)
     if node.hash_uint32 != hash:  # hash_uint32 is local, hash is remote
-        version_str = "".join(heartbeat_msg.data[4:])
+        version_str = "".join([chr(n) for n in heartbeat_msg.data[4:]])
         if not version_str.strip():
             version_str = "1.3.1"
         raise ProtocolVersionError(node_id, version_str)
     node._channel = chan
     return node
```

### Comparing `tinymovr-1.4.0/tinymovr/config/device.yaml` & `tinymovr-1.5.0/tinymovr/config/device.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             dtype: float
             unit: ampere
             meta: {dynamic: True}
             getter_name: controller_get_Iq_estimate_user_frame
             summary: The Iq estimate.
           - name: bandwidth
             dtype: float
-            unit: rad/s
+            unit: Hz
             meta: {export: True}
             getter_name: controller_get_I_bw
             setter_name: controller_set_I_bw
             summary: The current controller bandwidth.
           - name: Iq_p_gain
             dtype: float
             getter_name: controller_get_Iq_gain
@@ -360,15 +360,15 @@
         dtype: uint8
         meta: {export: True}
         getter_name: encoder_get_type
         setter_name: encoder_set_type
         summary: The encoder type. Either INTERNAL or HALL.
       - name: bandwidth
         dtype: float
-        unit: rad/s
+        unit: Hz
         meta: {export: True}
         getter_name: observer_get_bw
         setter_name: observer_set_bw
         summary: The encoder observer bandwidth.
       - name: calibrated
         dtype: bool
         meta: {dynamic: True}
@@ -437,14 +437,70 @@
         arguments:
           - name: pos_setpoint
             dtype: float
       - name: errors
         flags: [INVALID_INPUT, VCRUISE_OVER_LIMIT]
         getter_name: planner_get_errors
         summary: Any errors in the trajectory planner, as a bitmask
+  - name: homing
+    remote_attributes:
+      - name: velocity
+        dtype: float
+        unit: ticks/s
+        meta: {export: True}
+        getter_name: homing_planner_get_homing_velocity
+        setter_name: homing_planner_set_homing_velocity
+        summary: The velocity at which the motor performs homing.
+      - name: max_homing_t
+        dtype: float
+        unit: s
+        meta: {export: True}
+        getter_name: homing_planner_get_max_homing_t
+        setter_name: homing_planner_set_max_homing_t
+        summary: The maximum time the motor is allowed to travel before homing times out and aborts.
+      - name: retract_dist
+        dtype: float
+        unit: ticks
+        meta: {export: True}
+        getter_name: homing_planner_get_retract_distance
+        setter_name: homing_planner_set_retract_distance
+        summary: The retraction distance the motor travels after the endstop has been found.
+      - name: warnings
+        meta: {dynamic: True}
+        flags: [HOMING_TIMEOUT]
+        getter_name: homing_planner_get_warnings
+        summary: Any homing warnings, as a bitmask
+      - name: stall_detect
+        remote_attributes:
+          - name: velocity
+            dtype: float
+            unit: ticks/s
+            meta: {export: True}
+            getter_name: homing_planner_get_max_stall_vel
+            setter_name: homing_planner_set_max_stall_vel
+            summary: The velocity below which (and together with `stall_detect.delta_pos`) stall detection mode is triggered.
+          - name: delta_pos
+            dtype: float
+            unit: ticks
+            meta: {export: True}
+            getter_name: homing_planner_get_max_stall_delta_pos
+            setter_name: homing_planner_set_max_stall_delta_pos
+            summary: The velocity below which (and together with `stall_detect.delta_pos`) stall detection mode is triggered.
+          - name: t
+            dtype: float
+            unit: s
+            meta: {export: True}
+            getter_name: homing_planner_get_max_stall_t
+            setter_name: homing_planner_set_max_stall_t
+            summary: The time to remain in stall detection mode before the motor is considered stalled.
+      - name: home
+        summary: Perform the homing operation.
+        caller_name: homing_planner_home
+        dtype: void
+        arguments: []
   - name: watchdog
     remote_attributes:
       - name: enabled
         dtype: bool
         getter_name: Watchdog_get_enabled
         setter_name: Watchdog_set_enabled
         summary: Whether the watchdog is enabled or not.
```

### Comparing `tinymovr-1.4.0/tinymovr/constants.py` & `tinymovr-1.5.0/tinymovr/constants.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/discovery.py` & `tinymovr-1.5.0/tinymovr/discovery.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/gui/gui.py` & `tinymovr-1.5.0/tinymovr/gui/gui.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/gui/helpers.py` & `tinymovr-1.5.0/tinymovr/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/gui/window.py` & `tinymovr-1.5.0/tinymovr/gui/window.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/gui/worker.py` & `tinymovr-1.5.0/tinymovr/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/call.png` & `tinymovr-1.5.0/tinymovr/resources/icons/call.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/call@2x.png` & `tinymovr-1.5.0/tinymovr/resources/icons/call@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/call_dark.png` & `tinymovr-1.5.0/tinymovr/resources/icons/call_dark.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/call_dark@2x.png` & `tinymovr-1.5.0/tinymovr/resources/icons/call_dark@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/empty.png` & `tinymovr-1.5.0/tinymovr/resources/icons/empty.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/empty@2x.png` & `tinymovr-1.5.0/tinymovr/resources/icons/empty@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/empty_dark.png` & `tinymovr-1.5.0/tinymovr/resources/icons/empty_dark.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/resources/icons/empty_dark@2x.png` & `tinymovr-1.5.0/tinymovr/resources/icons/empty_dark@2x.png`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr/tee.py` & `tinymovr-1.5.0/tinymovr/tee.py`

 * *Files identical despite different names*

### Comparing `tinymovr-1.4.0/tinymovr.egg-info/PKG-INFO` & `tinymovr-1.5.0/tinymovr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinymovr
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tinymovr Studio
 Home-page: https://github.com/yconst/Tinymovr
 Author: Yannis Chatzikonstantinou
 Author-email: info@tinymovr.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `tinymovr-1.4.0/tinymovr.egg-info/SOURCES.txt` & `tinymovr-1.5.0/tinymovr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

