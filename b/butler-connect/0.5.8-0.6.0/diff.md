# Comparing `tmp/butler-connect-0.5.8.tar.gz` & `tmp/butler-connect-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.5.8.tar", last modified: Fri May 19 11:02:39 2023, max compression
+gzip compressed data, was "butler-connect-0.6.0.tar", last modified: Sat Jun  3 09:30:42 2023, max compression
```

## Comparing `butler-connect-0.5.8.tar` & `butler-connect-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 11:02:39.330198 butler-connect-0.5.8/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.5.8/LICENSE
--rw-rw-rw-   0        0        0     2321 2023-05-19 11:02:39.329201 butler-connect-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-05-19 09:41:31.000000 butler-connect-0.5.8/README.md
--rw-rw-rw-   0        0        0      738 2023-05-19 11:00:55.000000 butler-connect-0.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 11:02:39.330198 butler-connect-0.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 11:02:39.300198 butler-connect-0.5.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 11:02:39.311201 butler-connect-0.5.8/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.5.8/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18606 2023-05-19 11:02:25.000000 butler-connect-0.5.8/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-05-19 11:02:39.315197 butler-connect-0.5.8/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.5.8/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.5.8/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.5.8/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.5.8/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     1656 2023-05-12 19:37:09.000000 butler-connect-0.5.8/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-05-19 11:02:39.328208 butler-connect-0.5.8/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2321 2023-05-19 11:02:39.000000 butler-connect-0.5.8/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-19 11:02:39.000000 butler-connect-0.5.8/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 11:02:39.000000 butler-connect-0.5.8/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-05-19 11:02:39.000000 butler-connect-0.5.8/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-19 11:02:39.000000 butler-connect-0.5.8/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 09:30:42.796655 butler-connect-0.6.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2404 2023-06-03 09:30:42.795656 butler-connect-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-06-03 09:30:00.000000 butler-connect-0.6.0/README.md
+-rw-rw-rw-   0        0        0      738 2023-06-03 09:30:23.000000 butler-connect-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:30:42.796655 butler-connect-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 09:30:42.762423 butler-connect-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 09:30:42.765684 butler-connect-0.6.0/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.6.0/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.6.0/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:30:42.775600 butler-connect-0.6.0/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.6.0/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.6.0/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.6.0/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.6.0/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     1911 2023-06-03 09:28:15.000000 butler-connect-0.6.0/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:30:42.795656 butler-connect-0.6.0/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2404 2023-06-03 09:30:42.000000 butler-connect-0.6.0/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-06-03 09:30:42.000000 butler-connect-0.6.0/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:30:42.000000 butler-connect-0.6.0/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-03 09:30:42.000000 butler-connect-0.6.0/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-03 09:30:42.000000 butler-connect-0.6.0/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.5.8/LICENSE` & `butler-connect-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.8/PKG-INFO` & `butler-connect-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.8
+Version: 0.6.0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,7 +48,10 @@
 - adding group-types
 ### 0.5.2
 - adding signalOptionType and groupOptionType with forwardingMQTT
 ### 0.5.5
 - Solving problems on publishing data without connecting dest
 ### 0.5.5
 - Solving Problems with createConsumer with same topic an different routing_keys
+
+### 0.6.0
+- add new signal  types f.ex. system_state or set_temperature.heater
```

### Comparing `butler-connect-0.5.8/README.md` & `butler-connect-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 ### 0.5.0
 - adding group-types
 ### 0.5.2
 - adding signalOptionType and groupOptionType with forwardingMQTT
 ### 0.5.5
 - Solving problems on publishing data without connecting dest
 ### 0.5.5
-- Solving Problems with createConsumer with same topic an different routing_keys
+- Solving Problems with createConsumer with same topic an different routing_keys
+
+### 0.6.0
+- add new signal  types f.ex. system_state or set_temperature.heater
```

### Comparing `butler-connect-0.5.8/pyproject.toml` & `butler-connect-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.5.8"
+version = "0.6.0"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.5.8/src/butlerConnect/pikaButler.py` & `butler-connect-0.6.0/src/butlerConnect/pikaButler.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,18 @@
         
         
         queue_name =  f'{self.connectionName}' #_consume_{self.topic}'
         if self.routing_key is not None:
             queue_name = f'{queue_name}_{self.routing_key}'
         result = self.channel.queue_declare(queue=queue_name, exclusive=self.exclusive)
         if self.createExchangeIfNotExists:
-            self.channel.exchange_declare(exchange=self.topic, exchange_type=self.createExchangeType)
+            try:
+                self.channel.exchange_declare(exchange=self.topic, exchange_type=self.createExchangeType)
+            except:
+                LOG.warning(f'Error on creating exchange {self.topic}')
         self.channel.queue_bind(exchange=self.topic, queue=queue_name,routing_key=self.routing_key )
         self.channel.basic_consume(queue=queue_name,
                             auto_ack=True,
                             on_message_callback=self.callback)
 
         try:
             if self.reconnectingCallback != None: self.reconnectingCallback()
```

### Comparing `butler-connect-0.5.8/src/butlerDescription/control.py` & `butler-connect-0.6.0/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.5.8/src/butlerDescription/signal.py` & `butler-connect-0.6.0/src/butlerDescription/signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 from marshmallow import Schema, fields,post_load
 from datetime import datetime
 
 class SignalType():
     unDef = 'undef'
     temperature = 'temperature'
     setTemperature = 'set_temperature'
+    class setTemperature_():
+        heater = 'set_temperature.heater'
+        cooler = 'set_temperature.cooler'
     humidity = 'humidity'
     windowIsOpen = 'window_is_open'
     presence = 'presence'
     motion = 'motion'
     presence_merged = 'presence_merged'
     illumination = 'illumination'
     actuatorValue = 'actuator_value'
+    systemState = 'system_state'
+    class systemState_():
+        heater = 'system_state.heater'
+        cooler = 'system_state.cooler'
+    
 
 class SignalOptionType():
     unDef = 'undef'
     forwardingMQTT = 'forwarding_mqtt'
```

### Comparing `butler-connect-0.5.8/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.6.0/src/butler_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.5.8
+Version: 0.6.0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,7 +48,10 @@
 - adding group-types
 ### 0.5.2
 - adding signalOptionType and groupOptionType with forwardingMQTT
 ### 0.5.5
 - Solving problems on publishing data without connecting dest
 ### 0.5.5
 - Solving Problems with createConsumer with same topic an different routing_keys
+
+### 0.6.0
+- add new signal  types f.ex. system_state or set_temperature.heater
```

