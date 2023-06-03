# Comparing `tmp/LumosWeb-1.0.1.tar.gz` & `tmp/LumosWeb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-1.0.1.tar", last modified: Wed May 31 20:54:58 2023, max compression
+gzip compressed data, was "LumosWeb-1.0.2.tar", last modified: Sat Jun  3 14:08:11 2023, max compression
```

## Comparing `LumosWeb-1.0.1.tar` & `LumosWeb-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:58.257871 LumosWeb-1.0.1/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:57.908526 LumosWeb-1.0.1/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.1/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4872 2023-05-31 19:49:07.000000 LumosWeb-1.0.1/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.1/LumosWeb/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.1/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.1/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-31 20:54:58.198842 LumosWeb-1.0.1/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-31 20:54:57.000000 LumosWeb-1.0.1/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4269 2023-05-31 20:54:58.250866 LumosWeb-1.0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4098 2023-05-31 19:57:30.000000 LumosWeb-1.0.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-31 20:54:58.260935 LumosWeb-1.0.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-05-31 20:54:53.000000 LumosWeb-1.0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.747745 LumosWeb-1.0.2/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.377385 LumosWeb-1.0.2/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-1.0.2/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5438 2023-06-03 13:53:15.000000 LumosWeb-1.0.2/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-05-31 20:54:27.000000 LumosWeb-1.0.2/LumosWeb/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-1.0.2/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      976 2023-05-31 12:39:35.000000 LumosWeb-1.0.2/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-03 14:08:11.688496 LumosWeb-1.0.2/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4332 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      309 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-06-03 14:08:10.000000 LumosWeb-1.0.2/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4332 2023-06-03 14:08:11.740742 LumosWeb-1.0.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4162 2023-06-03 11:15:30.000000 LumosWeb-1.0.2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-03 14:08:11.751058 LumosWeb-1.0.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1845 2023-06-03 14:07:04.000000 LumosWeb-1.0.2/setup.py
```

### Comparing `LumosWeb-1.0.1/LumosWeb/api.py` & `LumosWeb-1.0.2/LumosWeb/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import select
 import socket
 from webob import Request
 from parse import parse
 import inspect
 from requests import Session as RequestsSession
 from wsgiadapter import WSGIAdapter as RequestsWSGIAdapter
 from wsgiref.simple_server import make_server
@@ -21,14 +22,16 @@
 
         self.exception_handler = None
 
         self.whitenoise = WhiteNoise(self.wsgi_app, root=static_dir)
 
         self.middleware = Middleware(self)    
 
+        self._server = None
+
     def __call__(self, environ, start_response):
         path_info = environ["PATH_INFO"]
 
         if path_info.startswith("/static"):
             environ["PATH_INFO"] = path_info[len("/static"):]
             return self.whitenoise(environ, start_response)
         
@@ -103,25 +106,40 @@
     
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
         self.middleware.add(middleware_cls)
         
-    def run(self, host="localhost", port=8080):
+    def is_running(self):
+        return self._server is not None and not self._server._BaseServer__is_shut_down.is_set()
+    
+    def run(self, host="localhost", port=8080, timeout=None):
+        attempts = 0
         while True:
             try:
-                server = make_server(host, port, self)
-                break  # Exit the loop if the server is created successfully
-            except OSError as e:
-                if e.errno == socket.errno.EADDRINUSE:
-                    # Port is already in use, try another port
-                    port += 1
-                    print(f"Port {port-1} is not available, trying port {port}")
-                else:
-                    # Other error occurred, raise the exception
-                    raise
-
+                # Check if the port is available
+                sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                sock.bind((host, port))
+                sock.close()
+                break  # Exit the loop if the port is available
+            except OSError:
+                print(f"Port {port} is not available, trying the next port")
+                attempts += 1
+                port += 1
+                if attempts > 10:
+                    raise Exception("No ports available to run the API")
+                
+        server = make_server(host, port, self)
+        self._server = server
         actual_port = server.server_port
         print(f"Starting Lumos server on {host}:{actual_port}")
-        server.serve_forever()
 
+        if timeout is None:
+            server.serve_forever()
+        else:
+            while True:
+                r, _, _ = select.select([server], [], [], timeout)
+                if r:
+                    server.handle_request()
+                else:
+                    break
```

### Comparing `LumosWeb-1.0.1/LumosWeb/cli.py` & `LumosWeb-1.0.2/LumosWeb/cli.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.1/LumosWeb/middleware.py` & `LumosWeb-1.0.2/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.1/LumosWeb/response.py` & `LumosWeb-1.0.2/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-1.0.1/LumosWeb.egg-info/PKG-INFO` & `LumosWeb-1.0.2/LumosWeb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.1
+Version: 1.0.2
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
+- [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
 e.g. pip install LumosWeb==0.0.2
```

### Comparing `LumosWeb-1.0.1/PKG-INFO` & `LumosWeb-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LumosWeb
-Version: 1.0.1
+Version: 1.0.2
 Summary: LumosWeb is web framework, simple and effective usage
 Author: Sddilora
 Author-email: sumeyyedilaradogan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
+- [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
 e.g. pip install LumosWeb==0.0.2
```

### Comparing `LumosWeb-1.0.1/README.md` & `LumosWeb-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## LumosWeb ![PyPI](https://img.shields.io/pypi/v/LumosWeb.svg)
 
 - To ensure compatibility and access the latest features and improvements, it is highly recommended to use version 1.0.0 or higher of the package. 
 - LumosWeb is web framework written in python
 - It's a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 - [PyPI Release](https://pypi.org/project/LumosWeb/)
+- [Sample App](https://github.com/Sddilora/LumosWeb-SampleApp)
 
 
 
 ## Installation
 ```shell
 pip install LumosWeb==<latest_version>
 e.g. pip install LumosWeb==0.0.2
```

### Comparing `LumosWeb-1.0.1/setup.py` & `LumosWeb-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

