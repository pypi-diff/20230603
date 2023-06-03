# Comparing `tmp/python-selve-new-2.1.9.tar.gz` & `tmp/python-selve-new-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.1.9.tar", last modified: Thu Jun  1 21:25:48 2023, max compression
+gzip compressed data, was "python-selve-new-2.2.0.tar", last modified: Sat Jun  3 20:57:19 2023, max compression
```

## Comparing `python-selve-new-2.1.9.tar` & `python-selve-new-2.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.198929 python-selve-new-2.1.9/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 21:25:48.000000 python-selve-new-2.1.9/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.198929 python-selve-new-2.1.9/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    50814 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:25:48.202929 python-selve-new-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 21:25:43.000000 python-selve-new-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:19.995442 python-selve-new-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-03 20:57:19.995442 python-selve-new-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:19.991442 python-selve-new-2.2.0/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-03 20:57:19.000000 python-selve-new-2.2.0/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-03 20:57:19.000000 python-selve-new-2.2.0/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:57:19.000000 python-selve-new-2.2.0/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 20:57:19.000000 python-selve-new-2.2.0/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 20:57:19.000000 python-selve-new-2.2.0/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:19.991442 python-selve-new-2.2.0/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    51136 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:19.991442 python-selve-new-2.2.0/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:57:19.995442 python-selve-new-2.2.0/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:57:19.995442 python-selve-new-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-03 20:57:16.000000 python-selve-new-2.2.0/setup.py
```

### Comparing `python-selve-new-2.1.9/LICENSE` & `python-selve-new-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/PKG-INFO` & `python-selve-new-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.9/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.2.0/python_selve_new.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.1.9
+Version: 2.2.0
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.1.9/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.2.0/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/__init__.py` & `python-selve-new-2.2.0/selve/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     """Implementation of the serial communication to the Selve Gateway"""
 
     def __init__(self, port=None, discover=True, develop=False, logger=None):
         # Gateway state
         self._callbacks = set()
         self.lastLogEvent = None
         self.state = None
-        self._stopThread = False
 
         # Data from Duty Cycle Event
         self.utilization = 0
         self.sendingBlocked = DutyMode.NOT_BLOCKED
 
         # Known devices
         self.devices: dict = {
@@ -56,39 +55,44 @@
             SelveTypes.GROUP.value: {},
             SelveTypes.SENSIM.value: {},
             SelveTypes.SENSOR.value: {},
             SelveTypes.SENDER.value: {}
         }
 
         # Flags for enabling reader and writer in the worker thread
-        self._pauseReader = False
-        self._pauseWriter = False
-        self._pauseWorker = False
-        
+        self._pauseReader = asyncio.Event()
+        self._pauseWriter = asyncio.Event()
+        self._pauseWorker = asyncio.Event()
+        self._stopThread = asyncio.Event()
+
         # The worker thread
         self.workerTask = None
 
         # Port where the Selve gateway was found
         self._port = port
+        self._serial = None
 
         # Write lock to safely write to the gateway
         self._writeLock = asyncio.Lock()
         self._readLock = asyncio.Lock()
 
+        self.txQ = None
+        self.rxQ = None
+
         self._LOGGER = logger
 
-    
+
     async def _worker(self):
         # Infinite loop to collect all incoming data
-        self._LOGGER.debug("Worker started")
-        
+        self._LOGGER.debug("(Selve Worker): " + "Worker started")
+
         try:
             while True:
-                if not self._pauseWorker:
-                    if not self._pauseReader:
+                if not self._pauseWorker.is_set():
+                    if not self._pauseReader.is_set():
                         async with self._readLock:
                             if not self._serial.is_open:
                                 self._serial.open()
                             if self._serial.in_waiting > 0:
                                 msg = ""
                                 while True:
                                     response = self._serial.readline().strip()
@@ -96,47 +100,45 @@
                                     if response.decode() == '':
                                         break
 
                                 # do something with the received data
                                 await self.processResponse(msg)
 
                                 # if msg.rstrip() == b' ':
-                                self._LOGGER.debug(f'Received: {msg}')
-                    else:
-                        self._LOGGER.debug("Reader stopped")
-                    if not self._pauseWriter:
+                                self._LOGGER.debug(f'(Selve Worker): Worker received: {msg}')
+
+                    if not self._pauseWriter.is_set():
                         if not self.txQ.empty():
                             data: Command = await self.txQ.get()
                             commandstr = data.serializeToXML()
-                            self._LOGGER.debug('Gateway writing: ' + str(commandstr))
+                            self._LOGGER.debug("(Selve Worker): " + 'Gateway writing: ' + str(commandstr))
                             try:
                                 async with self._writeLock:
                                     if not self._serial.is_open:
                                         self._serial.open()
                                     self._serial.write(commandstr)
                                     self._serial.flush()
                             except Exception as e:
-                                self._LOGGER.error("error communicating: " + str(e))
+                                self._LOGGER.error("(Selve Worker): " + "error communicating: " + str(e))
 
                             self.txQ.task_done()
 
                             # always sleep after writing
-                            await asyncio.sleep(0.2)
-                    else:
-                        self._LOGGER.debug("Writer stopped")
+                            #await asyncio.sleep(0.2)
+
                 await asyncio.sleep(0.01)
-                if self._stopThread:
-                    self._LOGGER.debug('Exiting worker loop...')
+                if self._stopThread.is_set():
+                    self._LOGGER.debug("(Selve Worker): " + 'Exiting worker loop...')
                     break
             return True
         # serial port exceptions, all of these notify that we are in some
         # serious trouble
         except serial.SerialException:
             # log message
-            self._LOGGER.error('Serial Port RX error')
+            self._LOGGER.error("(Selve Worker): " + 'Serial Port RX error')
 
 
     async def setup(self, discover=False, fromConfigFlow=False):
         self._LOGGER.info("Setup")
 
         self.rxQ = asyncio.Queue()
         self.txQ = asyncio.Queue()
@@ -149,29 +151,30 @@
                     baudrate=115200,
                     bytesize=serial.EIGHTBITS,
                     parity=serial.PARITY_NONE,
                     stopbits=serial.STOPBITS_ONE,
                     xonxoff=False,
                     rtscts=False,
                     dsrdtr=False)
-                
+
                 if await self.pingGateway():
                     if not fromConfigFlow:
                         if discover:
                             self._LOGGER.info("Discovering devices")
-                            await self.discover() 
-                        await self.startWorker()   
+                            await self.discover()
+                        await self.startWorker()
                     return
             except serial.SerialException as e:
                 self._LOGGER.debug("Configured port not valid! " + str(e))
             except Exception as e:
                 self._LOGGER.error("Unknown exception: " + str(e))
-                
+
 
         available_ports = list_ports.comports()
+        self._LOGGER.debug("available comports: " + str(available_ports))
 
         if len(available_ports) == 0:
             self._LOGGER.error("No available comports!")
             raise PortError
 
         for p in available_ports:
             try:
@@ -191,54 +194,62 @@
                 except:
                     self._LOGGER.debug("Cannot close com port")
                 pass
             if await self.pingGateway():
                 if not fromConfigFlow:
                     if discover:
                         self._LOGGER.info("Discovering devices")
-                        await self.discover() 
-                    await self.startWorker() 
+                        await self.discover()
+                    await self.startWorker()
                 self._port = p.device
                 return
             else:
                 self._serial.close()
                 self._serial = None
         else:
             self._LOGGER.error("No gateway on comports found!")
             raise PortError
-        
-        
+
+
 
     async def startWorker(self):
         self._LOGGER.debug("Starting worker")
-        self._pauseReader = False
-        self._pauseWriter = False
-        self._pauseWorker = False
-        self._stopThread = False
+        if self.workerTask is not None:
+            self._LOGGER.debug("Running worker detected")
+            await self.stopWorker()
+        self._pauseReader.clear()
+        self._pauseWriter.clear()
+        self._pauseWorker.clear()
+        self._stopThread.clear()
+        self._LOGGER.debug("Set variables")
         self.workerTask = asyncio.create_task(self._worker())
+        self._LOGGER.debug("created task")
 
     async def stopWorker(self):
         self._LOGGER.debug("Stopping worker")
-        self._pauseReader = True
-        self._pauseWriter = True
-        self._pauseWorker = True
-        self._stopThread = True
+        self._pauseReader.set()
+        self._pauseWriter.set()
+        self._pauseWorker.set()
+        self._stopThread.set()
         try:
             if self.workerTask is not None and not self.workerTask.cancelled() and not self.workerTask.done():
+                self._LOGGER.debug("Task is still running, waiting with timeout...")
                 await asyncio.wait_for(self.workerTask, timeout=5)
+        except TimeoutError:
+            self._LOGGER.debug("Task timed out")
         except Exception as e:
             self._LOGGER.debug("Task stopping exception: " + str(e))
         self.workerTask = None
 
 
     async def stopGateway(self):
         # wait for the rx/tx thread to end, these need to be gathered to
         # collect all the exceptions
         self._LOGGER.debug("Preparing for termination")
-        self._stopThread = True
+        self._stopThread.set()
         if self.workerTask is not None:
             self.workerTask.cancel()
             await self.workerTask
         # close the serial port, do the cleanup
         if self._serial.is_open:
             self._serial.close()
         self._serial = None
@@ -252,21 +263,20 @@
         """Remove previously registered callback."""
         self._callbacks.discard(callback)
 
     async def _sendCommandToGateway(self, command: Command):
         commandstr = command.serializeToXML()
         self._LOGGER.debug('Gateway writing: ' + str(commandstr))
         try:
-            async with self._writeLock:
-                if not self._serial.is_open:
-                    self._serial.open()
-                self._serial.write(commandstr)
-                self._serial.flush()
-                # always sleep after writing
-                await asyncio.sleep(0.2)
+            if not self._serial.is_open:
+                self._serial.open()
+            self._serial.write(commandstr)
+            self._serial.flush()
+            # always sleep after writing
+            await asyncio.sleep(0.2)
         except Exception as e:
             self._LOGGER.error("error communicating: " + str(e))
 
     async def processResponse(self, xmlstr):
         """Processes an XML String into a response object. Returns False if something went wrong or the gateway returned an error."""
         # check which command was received
         # do something with the data
@@ -531,77 +541,71 @@
         if methodName == "selve.GW." + str(CommeoEventCommand.DUTYCYCLE.value):
             return DutyCycleResponse(methodName, flat_params_list)
 
         # Any other response (unknown)
         return MethodResponse(methodName, flat_params_list)
 
     async def executeCommand(self, command: Command):
-        self._pauseWorker = False
+        await self.startWorker()
         self.txQ.put_nowait(command)
 
 
     async def executeCommandSyncWithResponse(self, command: Command):
         resp = await self._executeCommandSyncWithResponse(command)
         if (resp == False):
             #something went wrong, try again
             resp = await self._executeCommandSyncWithResponse(command)
-            
+
         return resp
 
     async def _executeCommandSyncWithResponse(self, command: Command):
 
         await self.stopWorker()
 
         if not self._serial.is_open:
             self._serial.open()
-
-        #guarantee exclusivity
-        #self._serial.reset_input_buffer()
-        #self._serial.reset_output_buffer()
-
-        await self._sendCommandToGateway(command)
-
-        start_time = time.time()
-        while True:
+        async with self._writeLock:
             async with self._readLock:
-                if self._serial.in_waiting > 0:
-                    msg = ""
-                    while True:
-                        response = self._serial.readline().strip()
-                        msg += response.decode()
-                        if response.decode() == '':
-                            break
-                    # if msg.rstrip() == b' ':
-                    self._LOGGER.debug(f'Received: {msg}')
-                    await self.startWorker()
-    
-                    resp = await self.processResponse(msg)
-                    
-                    if (resp == False):
-                        #something went wrong, try again
-                        return False
-                    
-                    if isinstance(resp, ErrorResponse):
-                        self._LOGGER.error(resp.message)
-                        # retry
+                await self._sendCommandToGateway(command)
+                start_time = time.time()
+                while True:
+                    if self._serial.in_waiting > 0:
+                        msg = ""
+                        while True:
+                            response = self._serial.readline().strip()
+                            msg += response.decode()
+                            if response.decode() == '':
+                                break
+                        # if msg.rstrip() == b' ':
+                        self._LOGGER.debug(f'Received: {msg}')
+                        await self.startWorker()
+
+                        resp = await self.processResponse(msg)
+
+                        if (resp == False):
+                            #something went wrong, try again
+                            return False
+
+                        if isinstance(resp, ErrorResponse):
+                            self._LOGGER.error(resp.message)
+                            # retry
+                            return False
+
+                        return resp
+                    # When no data is waiting in the input buffer after 10s we can assume, the message was not correctly sent or no input is necessary
+                    if time.time() - start_time > 10:
+                        await self.startWorker()
                         return False
 
-                    return resp
-                # When no data is waiting in the input buffer after 10s we can assume, the message was not correctly sent or no input is necessary
-                if time.time() - start_time < 10:
-                    time.sleep(0.05)
-                else:
-                    await self.startWorker()
-                    return False
-        
+
 
 
     async def discover(self):
 
-        self._pauseWorker = True
+        await self.stopWorker()
 
         if await self.gatewayReady():
             iveoIds: IveoGetIdsResponse = await self.executeCommandSyncWithResponse(IveoGetIds())
             deviceIds: DeviceGetIdsResponse = await self.executeCommandSyncWithResponse(DeviceGetIds())
             groupIds: GroupGetIdsResponse = await self.executeCommandSyncWithResponse(GroupGetIds())
             sensorIds: SensorGetIdsResponse = await self.executeCommandSyncWithResponse(SensorGetIds())
             senderIds: SenderGetIdsResponse = await self.executeCommandSyncWithResponse(SenderGetIds())
@@ -692,16 +696,16 @@
                 device.tempAnalog = config.tempAnalog
                 device.windAnalog = config.windAnalog
                 device.sun1Analog = config.sun1Analog
                 device.dayLightAnalog = config.dayLightAnalog
                 device.sun2Analog = config.sun2Analog
                 device.sun3Analog = config.sun3Analog
                 self.addOrUpdateDevice(device, SelveTypes.SENSIM)
-        
-        self._pauseWorker = False
+
+        await self.startWorker()
         self.list_devices()
 
 
     async def updateAllDevices(self):
         for device in self.devices[SelveTypes.DEVICE.value]:
             await self.updateCommeoDeviceValues(device.id)
         for sensor in self.devices[SelveTypes.SENSOR.value]:
@@ -837,15 +841,15 @@
             if time.time() - start_time >= 10:
                 self._LOGGER.info("Error: Gateway could not be reset or loads too long")
             pass
         self._LOGGER.info("Gateway reset")
 
     async def setEvents(self, eventDevice = False, eventSensor = False, eventSender = False, eventLogging = False, eventDuty = False):
         command = param.ParamSetEvent(eventDevice, eventSensor, eventSender, eventLogging, eventDuty)
-        await self.executeCommand(command)
+        return await self.executeCommandSyncWithResponse(command)
 
     async def processEventResponse(self, response):
         if isinstance(response, CommeoDeviceEventResponse):
             # This is a commeo device response, Iveo does not generate events because it is a one way communication protocol
             if self.is_id_registered(response.id, SelveTypes.DEVICE):
                 device: SelveDevice = self.devices[SelveTypes.DEVICE.value][response.id]
             else:
@@ -928,15 +932,15 @@
 
     async def updateCommeoDeviceValues(self, id: int):
         response: DeviceGetValuesResponse = await self.executeCommandSyncWithResponse(DeviceGetValues(id))
         self.updateCommeoDeviceValuesFromResponse(id, response)
 
     async def updateCommeoDeviceValuesAsync(self, id: int):
         await self.executeCommand(DeviceGetValues(id))
-        
+
     def updateCommeoDeviceValuesFromResponse(self, id: int, response: DeviceGetValuesResponse):
         dev = self.getDevice(id, SelveTypes.DEVICE)
         dev.name = response.name if response.name else "None"
         dev.state = response.movementState if response.movementState else MovementState.UNKOWN.value
         dev.value = response.value if response.value else 0
         dev.targetValue = response.targetValue if response.targetValue else 0
         dev.unreachable = response.unreachable if response.unreachable else True
@@ -947,20 +951,20 @@
         dev.automaticMode = response.automaticMode if response.automaticMode else False
         dev.gatewayNotLearned = response.gatewayNotLearned if response.gatewayNotLearned else False
         dev.windAlarm = response.windAlarm if response.windAlarm else False
         dev.rainAlarm = response.rainAlarm if response.rainAlarm else False
         dev.freezingAlarm = response.freezingAlarm if response.freezingAlarm else False
         dev.dayMode = response.dayMode if response.dayMode else False
         self.addOrUpdateDevice(dev, SelveTypes.DEVICE)
-        
+
     def setDeviceValue(self, id: int, value: int, type: SelveTypes):
         dev = self.getDevice(id, type)
         dev.value = value
         self.addOrUpdateDevice(dev, type)
-        
+
     def setDeviceTargetValue(self, id: int, value: int, type: SelveTypes):
         dev = self.getDevice(id, type)
         dev.targetValue = value
         self.addOrUpdateDevice(dev, type)
 
     def setDeviceState(self, id: int, state: MovementState, type: SelveTypes):
         dev = self.getDevice(id, type)
```

### Comparing `python-selve-new-2.1.9/selve/commands/command.py` & `python-selve-new-2.2.0/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/device.py` & `python-selve-new-2.2.0/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/event.py` & `python-selve-new-2.2.0/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/group.py` & `python-selve-new-2.2.0/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/iveo.py` & `python-selve-new-2.2.0/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/param.py` & `python-selve-new-2.2.0/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/senSim.py` & `python-selve-new-2.2.0/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/sender.py` & `python-selve-new-2.2.0/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/sensor.py` & `python-selve-new-2.2.0/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/commands/service.py` & `python-selve-new-2.2.0/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/device.py` & `python-selve-new-2.2.0/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/group.py` & `python-selve-new-2.2.0/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/iveo.py` & `python-selve-new-2.2.0/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/senSim.py` & `python-selve-new-2.2.0/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/sender.py` & `python-selve-new-2.2.0/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/sensor.py` & `python-selve-new-2.2.0/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/util/__init__.py` & `python-selve-new-2.2.0/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/util/errors.py` & `python-selve-new-2.2.0/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/selve/util/protocol.py` & `python-selve-new-2.2.0/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.1.9/setup.py` & `python-selve-new-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.1.9',  # Required
+    version='2.2.0',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

