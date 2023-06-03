# Comparing `tmp/flxtrd-0.1.0.tar.gz` & `tmp/flxtrd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.1.0.tar", max compression
+gzip compressed data, was "flxtrd-0.1.1.tar", max compression
```

## Comparing `flxtrd-0.1.0.tar` & `flxtrd-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     9136 2023-06-03 18:45:23.386447 flxtrd-0.1.0/LICENSE
--rw-r--r--   0        0        0     4046 2023-06-03 18:48:16.702096 flxtrd-0.1.0/README.md
--rw-r--r--   0        0        0     2117 2023-06-03 18:45:23.386447 flxtrd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      610 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.0/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     4769 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      581 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4405 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     2451 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/types.py
--rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.0/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0     8590 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 flxtrd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-03 18:45:23.386447 flxtrd-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3999 2023-06-03 18:51:18.453728 flxtrd-0.1.1/README.md
+-rw-r--r--   0        0        0     2117 2023-06-03 18:52:35.405572 flxtrd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.1/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     4769 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      581 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4405 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     2451 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.1/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0     8590 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     4740 1970-01-01 00:00:00.000000 flxtrd-0.1.1/PKG-INFO
```

### Comparing `flxtrd-0.1.0/LICENSE` & `flxtrd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/README.md` & `flxtrd-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     log(INFO, pformat(response.request_response.json()))
     log(INFO, response.request_response.status_code)
 
     # Send the market order to the message broker with AMPQ protocol
     # The connection to the market message broker will be initiated automatically
     response, err = trading_client.send_order(
         method="",
-        endpoint="ask",
         verify_ssl=False,
         order=market_order,
     )
 
     if err:
         log(ERROR, err)
         sys.exit(1)
@@ -99,15 +98,14 @@
     log(INFO, "Received response from message broker")
     log(INFO, response.order_response)
 
     # Send the market order to the message broker with AMPQ protocol
     # The connection to the market message broker will be initiated automatically
     response, err = trading_client.send_order(
         method="",
-        endpoint="bi",
         verify_ssl=False,
         order=market_order,
     )
 
     if err:
         log(ERROR, err)
         sys.exit(1)
```

### Comparing `flxtrd-0.1.0/pyproject.toml` & `flxtrd-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.1.0"
+version = "0.1.1"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
```

### Comparing `flxtrd-0.1.0/src/flxtrd/__init__.py` & `flxtrd-0.1.1/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/core/api_client.py` & `flxtrd-0.1.1/src/flxtrd/core/api_client.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/core/logger.py` & `flxtrd-0.1.1/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.1.1/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.1.1/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/core/types.py` & `flxtrd-0.1.1/src/flxtrd/core/types.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/protocols/ampq.py` & `flxtrd-0.1.1/src/flxtrd/protocols/ampq.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/src/flxtrd/protocols/restapi.py` & `flxtrd-0.1.1/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.0/PKG-INFO` & `flxtrd-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -101,15 +101,14 @@
     log(INFO, pformat(response.request_response.json()))
     log(INFO, response.request_response.status_code)
 
     # Send the market order to the message broker with AMPQ protocol
     # The connection to the market message broker will be initiated automatically
     response, err = trading_client.send_order(
         method="",
-        endpoint="ask",
         verify_ssl=False,
         order=market_order,
     )
 
     if err:
         log(ERROR, err)
         sys.exit(1)
@@ -117,15 +116,14 @@
     log(INFO, "Received response from message broker")
     log(INFO, response.order_response)
 
     # Send the market order to the message broker with AMPQ protocol
     # The connection to the market message broker will be initiated automatically
     response, err = trading_client.send_order(
         method="",
-        endpoint="bi",
         verify_ssl=False,
         order=market_order,
     )
 
     if err:
         log(ERROR, err)
         sys.exit(1)
```

