# Comparing `tmp/myjdapi-1.1.6.tar.gz` & `tmp/myjdapi-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myjdapi-1.1.6.tar", last modified: Sun Sep 18 09:20:19 2022, max compression
+gzip compressed data, was "myjdapi-1.1.7.tar", last modified: Sat Jun  3 15:17:13 2023, max compression
```

## Comparing `myjdapi-1.1.6.tar` & `myjdapi-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 09:20:19.241803 myjdapi-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-18 09:20:12.000000 myjdapi-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-09-18 09:20:19.241803 myjdapi-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-09-18 09:20:12.000000 myjdapi-1.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 09:20:19.241803 myjdapi-1.1.6/myjdapi/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-18 09:20:12.000000 myjdapi-1.1.6/myjdapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-09-18 09:20:12.000000 myjdapi-1.1.6/myjdapi/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-09-18 09:20:12.000000 myjdapi-1.1.6/myjdapi/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    42904 2022-09-18 09:20:12.000000 myjdapi-1.1.6/myjdapi/myjdapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 09:20:19.241803 myjdapi-1.1.6/myjdapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-09-18 09:20:19.000000 myjdapi-1.1.6/myjdapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-18 09:20:19.000000 myjdapi-1.1.6/myjdapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 09:20:19.000000 myjdapi-1.1.6/myjdapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-18 09:20:19.000000 myjdapi-1.1.6/myjdapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-18 09:20:19.000000 myjdapi-1.1.6/myjdapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 09:20:19.241803 myjdapi-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-18 09:20:12.000000 myjdapi-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:17:13.508155 myjdapi-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-03 15:17:02.000000 myjdapi-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-03 15:17:13.508155 myjdapi-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-03 15:17:02.000000 myjdapi-1.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:17:13.508155 myjdapi-1.1.7/myjdapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-03 15:17:02.000000 myjdapi-1.1.7/myjdapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-03 15:17:02.000000 myjdapi-1.1.7/myjdapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-06-03 15:17:02.000000 myjdapi-1.1.7/myjdapi/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47860 2023-06-03 15:17:02.000000 myjdapi-1.1.7/myjdapi/myjdapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:17:13.508155 myjdapi-1.1.7/myjdapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-03 15:17:13.000000 myjdapi-1.1.7/myjdapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 15:17:13.000000 myjdapi-1.1.7/myjdapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:17:13.000000 myjdapi-1.1.7/myjdapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 15:17:13.000000 myjdapi-1.1.7/myjdapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 15:17:13.000000 myjdapi-1.1.7/myjdapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:17:13.508155 myjdapi-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-03 15:17:02.000000 myjdapi-1.1.7/setup.py
```

### Comparing `myjdapi-1.1.6/LICENSE` & `myjdapi-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myjdapi-1.1.6/PKG-INFO` & `myjdapi-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myjdapi
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library to use My.Jdownloader API in an easy way.
 Home-page: https://github.com/mmarquezs/My.Jdownloader-API-Python-Library/
 Author: Marc Marquez Santamaria
 Author-email: mmsa1994@gmail.com
 License: MIT
 Keywords: myjdapi jdownloader my.jdownloader api development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `myjdapi-1.1.6/README.rst` & `myjdapi-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `myjdapi-1.1.6/myjdapi/__init__.py` & `myjdapi-1.1.7/myjdapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     MYJDStorageLimitReachedException,
     MYJDStorageNotFoundException,
     MYJDTokenInvalidException,
     MYJDTooManyRequestsException,
     MYJDUnknownException,
 )
 
-__version__ = "1.1.6"
+__version__ = "1.1.7"
```

### Comparing `myjdapi-1.1.6/myjdapi/const.py` & `myjdapi-1.1.7/myjdapi/const.py`

 * *Files identical despite different names*

### Comparing `myjdapi-1.1.6/myjdapi/exception.py` & `myjdapi-1.1.7/myjdapi/exception.py`

 * *Files identical despite different names*

### Comparing `myjdapi-1.1.6/myjdapi/myjdapi.py` & `myjdapi-1.1.7/myjdapi/myjdapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,29 +151,38 @@
         return resp
 
     def update_available(self):
         self.run_update_check()
         resp = self.is_update_available()
         return resp
 
-    
 class Config:
     """
     Class that represents the Config of a Device
     """
 
     def __init__(self, device):
         self.device = device
         self.url = '/config'
 
-    def list(self):
+    def list(self, params=None):
         """
         :return:  List<AdvancedConfigAPIEntry>
         """
-        resp = self.device.action(self.url + "/list")
+        if params != None:
+            resp = self.device.action(self.url + "/list")
+            return resp
+        resp = self.device.action(self.url + "/list", params)
+        return resp
+
+    def listEnum(self, type):
+        """
+        :return:  List<EnumOption>
+        """
+        resp = self.device.action(self.url + "/listEnum", params=[type])
         return resp
 
     def get(self, interface_name, storage, key):
         """
         :param interfaceName: a valid interface name from List<AdvancedConfigAPIEntry>
         :type: str:
         :param storage: 'null' to use default or 'cfg/' + interfaceName
@@ -181,14 +190,70 @@
         :param key: a valid key from from List<AdvancedConfigAPIEntry>
         :type: str:
         """
         params = [interface_name, storage, key]
         resp = self.device.action(self.url + "/get", params)
         return resp
 
+    def getDefault(self, interfaceName, storage, key):
+        """
+        :param interfaceName:  a valid interface name from List<AdvancedConfigAPIEntry>
+        :type: str:
+        :param storage: 'null' to use default or 'cfg/' + interfaceName
+        :type: str:
+        :param key: a valid key from from List<AdvancedConfigAPIEntry>
+        :type: str:
+        """
+        params = [interfaceName, storage, key]
+        resp = self.device.action(self.url + "/getDefault", params)
+        return resp
+
+    def query(self,
+              params=[{
+                "configInterface": "",
+                "defaultValues": True,
+                "description": True,
+                "enumInfo": True,
+                "includeExtensions": True,
+                "pattern": "",
+                "values": True
+              }]):
+        """
+        :param params: A dictionary with options. The default dictionary is
+        configured so it returns you all config API entries with all details, but you
+        can put your own with your options. All the options available are this
+        ones:
+        {
+        "configInterface"  : "",
+        "defaultValues"    : True,
+        "description"      : True,
+        "enumInfo"         : True,
+        "includeExtensions": True,
+        "pattern"          : "",
+        "values"           : ""
+        }
+        :type: Dictionary
+        :rtype: List of dictionaries of this style, with more or less detail based on your options.
+        """
+        resp = self.device.action(self.url + "/query", params)
+        return resp
+
+    def reset(self, interfaceName, storage, key):
+        """
+        :param interfaceName:  a valid interface name from List<AdvancedConfigAPIEntry>
+        :type: str:
+        :param storage: 'null' to use default or 'cfg/' + interfaceName
+        :type: str:
+        :param key: a valid key from from List<AdvancedConfigAPIEntry>
+        :type: str:
+        """
+        params = [interfaceName, storage, key]
+        resp = self.device.action(self.url + "/reset", params)
+        return resp
+
     def set(self, interface_name, storage, key, value):
         """
         :param interfaceName:  a valid interface name from List<AdvancedConfigAPIEntry>
         :type: str:
         :param storage: 'null' to use default or 'cfg/' + interfaceName
         :type: str:
         :param key: a valid key from from List<AdvancedConfigAPIEntry>
@@ -258,14 +323,88 @@
         """
 
         :return:
         """
         resp = self.device.action(self.url + "/getCurrentState")
         return resp
 
+class Extension:
+    def __init__(self, device):
+        self.device = device
+        self.url = "/extensions"
+
+    def list(self,
+             params=[{
+                "configInterface": True,
+                "description": True,
+                "enabled": True,
+                "iconKey": True,
+                "name": True,
+                "pattern" : "",
+                "installed": True
+             }]):
+        """
+        :param params: A dictionary with options. The default dictionary is
+        configured so it returns you all available extensions, but you
+        can put your own with your options. All the options available are this
+        ones:
+        {
+        "configInterface"  : True,
+        "description"      : True,
+        "enabled"          : True,
+        "iconKey"          : True,
+        "name"             : True,
+        "pattern"          : "",
+        "installed"        : True
+        }
+        :type: Dictionary
+        :rtype: List of dictionaries of this style, with more or less detail based on your options.
+        """
+        resp = self.device.action(self.url + "/list", params=params)
+        return resp
+
+    def install(self, id):
+        resp = self.device.action(self.url + "/install", params=[id])
+        return resp
+
+    def isInstalled(self, id):
+        resp = self.device.action(self.url + "/isInstalled", params=[id])
+        return resp
+
+    def isEnabled(self, id):
+        resp = self.device.action(self.url + "/isEnabled", params=[id])
+        return resp
+
+    def setEnabled(self, id, enabled):
+        resp = self.device.action(self.url + "/setEnabled", params=[id, enabled])
+        return resp
+
+class Dialog:
+    """
+    Class that represents the dialogs on myJD
+    """
+    def __init__(self, device):
+        self.device = device
+        self.url = "/dialogs"
+
+    def answer(self, id, data):
+        resp = self.device.action(self.url + "/answer", params=[id, data])
+        return resp
+
+    def get(self, id, icon=True, properties=True):
+        resp = self.device.action(self.url + "/get", params=[id, icon, properties])
+        return resp
+
+    def getTypeInfo(self, dialogType):
+        resp = self.device.action(self.url + "/getTypeInfo", params=[dialogType])
+        return resp
+
+    def list(self):
+        resp = self.device.action(self.url + "/list")
+        return resp
 
 class Linkgrabber:
     """
     Class that represents the linkgrabber of a Device
     """
 
     def __init__(self, device):
@@ -820,14 +959,16 @@
         self.myjd = jd
         self.config = Config(self)
         self.linkgrabber = Linkgrabber(self)
         self.captcha = Captcha(self)
         self.downloads = Downloads(self)
         self.toolbar = Toolbar(self)
         self.downloadcontroller = DownloadController(self)
+        self.extensions = Extension(self)
+        self.dialogs = Dialog(self)
         self.update = Update(self)
         self.jd = Jd(self)
         self.system = System(self)
         self.__direct_connection_info = None
         self.__refresh_direct_connections()
         self.__direct_connection_enabled = True
         self.__direct_connection_cooldown = 0
@@ -1205,18 +1346,20 @@
                 ]
             query = query[0] + "&".join(query[1:])
             encrypted_response = requests.get(api + query, timeout=3)
         else:
             params_request = []
             if params is not None:
                 for param in params:
-                    if not isinstance(param, list):
+                    if isinstance(param, str) or isinstance(param, list):
+                        params_request += [param]
+                    elif isinstance(param, dict) or isinstance(param, bool):
                         params_request += [json.dumps(param)]
                     else:
-                        params_request += [param]
+                        params_request += [str(param)]
             params_request = {
                 "apiVer": self.__api_version,
                 "url": path,
                 "params": params_request,
                 "rid": self.__request_id
             }
             data = json.dumps(params_request)
```

### Comparing `myjdapi-1.1.6/myjdapi.egg-info/PKG-INFO` & `myjdapi-1.1.7/myjdapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myjdapi
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library to use My.Jdownloader API in an easy way.
 Home-page: https://github.com/mmarquezs/My.Jdownloader-API-Python-Library/
 Author: Marc Marquez Santamaria
 Author-email: mmsa1994@gmail.com
 License: MIT
 Keywords: myjdapi jdownloader my.jdownloader api development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `myjdapi-1.1.6/setup.py` & `myjdapi-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name="myjdapi",
-    version="1.1.6",
+    version="1.1.7",
     description="Library to use My.Jdownloader API in an easy way.",
     long_description=long_description,
     url="https://github.com/mmarquezs/My.Jdownloader-API-Python-Library/",
     author="Marc Marquez Santamaria",
     author_email="mmsa1994@gmail.com",
     license="MIT",
     classifiers=[
```

