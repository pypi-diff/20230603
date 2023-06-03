# Comparing `tmp/pykeadhcp-0.1.3.tar.gz` & `tmp/pykeadhcp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.1.3.tar", max compression
+gzip compressed data, was "pykeadhcp-0.2.0.tar", max compression
```

## Comparing `pykeadhcp-0.1.3.tar` & `pykeadhcp-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,64 @@
--rw-r--r--   0        0        0    11356 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/LICENSE
--rw-r--r--   0        0        0     5301 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/README.md
--rw-r--r--   0        0        0       30 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    25295 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    21553 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     7453 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      207 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      448 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      472 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      341 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      542 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      202 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      375 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      491 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0      495 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      247 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0     1589 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      156 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      364 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      406 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      488 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      175 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      244 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      472 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      385 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      447 2023-06-01 16:33:00.681895 pykeadhcp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5906 1970-01-01 00:00:00.000000 pykeadhcp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7331 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/README.md
+-rw-r--r--   0        0        0       30 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    25620 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    21878 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     7934 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      778 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      207 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      448 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      679 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      892 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      341 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      533 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      202 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      375 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      491 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1550 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      472 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      278 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      403 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1494 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2433 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      394 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      624 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      364 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      406 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      136 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      474 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      244 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      472 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      385 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0     2036 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0      522 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0      825 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      447 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.2.0/PKG-INFO
```

### Comparing `pykeadhcp-0.1.3/LICENSE` & `pykeadhcp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.3/README.md` & `pykeadhcp-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -123,17 +123,55 @@
 
 ```
 server.dhcp4.refresh_cached_config()
 ```
 
 For API calls that don't amend the configuration (eg. lease4-add, lease6-add, config-get, etc....), there is no need to refresh the relevant daemon configuration. Maybe I will add a feature in the future to allow the user to specify if they want the cached_config to be automatically refreshed when a function is called that requires a refresh but for now its manual.
 
+## Parsers
+
+Majority of the useful API functionality requires a subscription for the premium hooks to use API commands like `subnet4-add` or `network6-add` as an example. This is typically the recommended way to interact with Kea as there is some additional validation that the API will perform and potentially prevent misconfiguration of your daemons (Dhcp4, Dhcp6, Control Agent, DDNS) that pykeadhcp may not correctly implement.
+
+However with the use of `config-test` and `config-set` API commands which are supported for all daemons in the free version of ISC Kea DHCP, you can utilize the various parsers implemented in pykeadhcp which provides similar functionality to create, read, update and delete various resources like subnets, shared networks, reservations etc... The parsers attempt to parse a local configuration (eg. server.dhcp4.cached_config) and should be used with the 2 API commands `config-test` and `config-set`. The problem with `config-set` is that it will restart the daemon on the server unlike the specific commands to directly interact with the configuration.
+
+Before continuing, these parsers are manually crafted and can break at anytime when ISC release an update that changes the behaviour of the configuration model. Therefore you should use parsers at your own risk.
+
+### Example of Dhcp4Parser to retrieve a specific subnet by a CIDR
+
+```python
+from pykeadhcp import Kea
+from pykeadhcp.parsers.dhcp4 import Dhcp4Parser
+
+cidr_to_find = "192.168.1.0/24"
+
+server = Kea(host="http://localhost", port=8000)
+parser = Dhcp4Parser(config=server.dhcp4.cached_config)
+subnet = parser.get_subnet_by_cidr(cidr=cidr_to_find)
+
+if not subnet:
+    exit(f"Unable to find subnet: {cidr_to_find}")
+
+print(f"Found Subnet {cidr_to_find} (Subnet ID: {subnet.id})")
+
+option_data = subnet.option_data
+for option in option_data:
+    print(f"Code: {option.code}")
+    print(f"Data: {option.data}")
+
+# Output
+# Found Subnet 192.168.1.0/24 (Subnet ID: 1)
+# Code: 3
+# Data: 192.168.1.1
+# Code: 6
+# Data: 1.1.1.1,9.9.9.9
+```
+
 ## API Reference
 
-All supported commands by the daemons are in the format of the API referenced commands with the exception of replacing any hypthen or space with an underscore. Eg. the `build-report` API command for all daemons is implemented as `build_report` so it heavily ties into the Kea predefined commands when looking at their documentation. Currently everything is built towards Kea 2.2.0. Pydantic variables will replace any hyphens with an underscore however when loading/exporting the data models, it will replace all keys with the hyphen to adhere to the Kea expected variables, ensure that the `KeaBaseModel` (located in `from pykeadhcp.models.generic.base import KeaBaseModel` instead of `from pydantic import BaseModel`) is used when creating any Pydantic models to inherit this functionality.
+All supported commands by the daemons are in the format of the API referenced commands with the exception of replacing any hyphen or space with an underscore. Eg. the `build-report` API command for all daemons is implemented as `build_report` so it heavily ties into the Kea predefined commands when looking at their documentation. Currently everything is built towards Kea 2.2.0. Pydantic variables will replace any hyphens with an underscore however when loading/exporting the data models, it will replace all keys with the hyphen to adhere to the Kea expected variables, ensure that the `KeaBaseModel` (located in `from pykeadhcp.models.generic.base import KeaBaseModel` instead of `from pydantic import BaseModel`) is used when creating any Pydantic models to inherit this functionality.
 
 ## Development / Contribution
 
 See [this document which explains the development/setup to contribute to this project](CONTRIBUTING.md)
 
 ## Commands Implemented/Tested
```

### Comparing `pykeadhcp-0.1.3/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.2.0/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.3/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.2.0/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp4.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 
         This function should be called after any interaction with the API that potentially changes the configuration
         eg. subnet4-add, commands like lease4-add won't need a config refresh to keep the cached config up to date
         """
         config = self.config_get()
         self.cached_config = config.arguments
 
+    def get_next_available_subnet_id(self) -> int:
+        """Returns the next available subnet-id for use with Dhcp4 subnets"""
+        subnets = self.subnet4_list()
+        subnet_ids = [subnet.id for subnet in subnets]
+        next_id = self.api.get_next_available_subnet_id(subnet_ids=subnet_ids)
+        return next_id
+
     def build_report(self) -> KeaResponse:
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
```

### Comparing `pykeadhcp-0.1.3/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp6.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 
         This function should be called after any interaction with the API that potentially changes the configuration
         eg. subnet6-add, commands like lease6-add won't need a config refresh to keep the cached config up to date
         """
         config = self.config_get()
         self.cached_config = config.arguments
 
+    def get_next_available_subnet_id(self) -> int:
+        """Returns the next available subnet-id for use with Dhcp4 subnets"""
+        subnets = self.subnet6_list()
+        subnet_ids = [subnet.id for subnet in subnets]
+        next_id = self.api.get_next_available_subnet_id(subnet_ids=subnet_ids)
+        return next_id
+
     def build_report(self) -> KeaResponse:
         """Returns list of compilation options that this particular binary was built with
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-build-report
         """
         return self.api.send_command(command="build-report", service=self.service)
```

### Comparing `pykeadhcp-0.1.3/pykeadhcp/exceptions.py` & `pykeadhcp-0.2.0/pykeadhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.1.3/pykeadhcp/kea.py` & `pykeadhcp-0.2.0/pykeadhcp/kea.py`

 * *Files 11% similar despite different names*

```diff
@@ -196,7 +196,20 @@
             body={
                 "command": command,
                 "service": [service] if service else [],
                 "arguments": arguments,
             },
         )
         return command_results
+
+    def get_next_available_subnet_id(self, subnet_ids: List[int]) -> int:
+        """Returns the next available subnet-id based on a given list of
+        existing subnet-ids
+
+        Args:
+            subnet_ids:     Existing list of subnet-ids gathered via
+                subnet4_list/subnet6_list or manually gathered via parser
+        """
+        next_id = next(
+            i for i, e in enumerate(sorted(subnet_ids) + [None], 1) if i != e
+        )
+        return next_id
```

### Comparing `pykeadhcp-0.1.3/pykeadhcp/models/dhcp6/pd_pool.py` & `pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/pd_pool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, List
 from pykeadhcp.models.generic.base import KeaBaseModel
 from pykeadhcp.models.generic.option_data import OptionData
 
 
 class PDPool(KeaBaseModel):
-    pd_prefix: str
-    pd_prefix_len: int
-    pd_delegated_len: int
+    prefix: str
+    prefix_len: int
+    delegated_len: int
     option_data: Optional[List[OptionData]]
     client_class: Optional[str]
     require_client_classes: Optional[List[str]]
     excluded_prefix: Optional[str]
     excluded_prefix_len: Optional[int]
     user_context: Optional[dict]
     comment: Optional[str]
```

### Comparing `pykeadhcp-0.1.3/pykeadhcp/models/generic/dhcp_common.py` & `pykeadhcp-0.2.0/pykeadhcp/models/generic/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 from typing import Optional, List, Union
 from pykeadhcp.models.generic.base import KeaBaseModel
+from pykeadhcp.models.generic.hook import Hook
+from pykeadhcp.models.generic.logger import Logger
 from pykeadhcp.models.generic.option_data import OptionData
 from pykeadhcp.models.enums import ReservationMode, DDNSReplaceClientNameEnum
 
 
-class CommonDHCPParams(KeaBaseModel):
-    """Any param shared between v4/v6 Shared Networks and Subnets"""
+class CommonConfig(KeaBaseModel):
+    store_extended_info: Optional[bool]
+    user_context: Optional[dict]
+    comment: Optional[str]
+    unknown_map_entry: Optional[str]
+
 
+class CommonDhcpConfig(CommonConfig):
     valid_lifetime: Optional[int]
     min_valid_lifetime: Optional[int]
     max_valid_lifetime: Optional[int]
-    interface: Optional[str]
     renew_timer: Optional[int]
     rebind_timer: Optional[int]
     option_data: Optional[List[OptionData]]
-    client_class: Optional[str]
-    require_client_classes: Optional[List[str]]
     reservation_mode: Optional[ReservationMode]
     reservations_global: Optional[bool]
     reservations_in_subnet: Optional[bool]
     reservations_out_of_pool: Optional[bool]
-    user_context: Optional[dict]
-    comment: Optional[str]
     calculate_tee_times: Optional[bool]
     t1_percent: Optional[float]
     t2_percent: Optional[float]
     cache_threshold: Optional[float]
     cache_max_age: Optional[int]
     ddns_send_updates: Optional[bool]
     ddns_override_no_update: Optional[bool]
     ddns_override_client_update: Optional[bool]
     ddns_replace_client_name: Optional[Union[DDNSReplaceClientNameEnum, bool]]
     ddns_generated_prefix: Optional[str]
     ddns_qualifying_suffix: Optional[str]
     ddns_update_on_renew: Optional[bool]
     ddns_use_conflict_resolution: Optional[bool]
-    store_extended_info: Optional[bool]
-    unknown_map_entry: Optional[str]
-
-    class Config:
-        use_enum_values = True
```

### Comparing `pykeadhcp-0.1.3/PKG-INFO` & `pykeadhcp-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.1.3
+Version: 0.2.0
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -139,17 +139,55 @@
 
 ```
 server.dhcp4.refresh_cached_config()
 ```
 
 For API calls that don't amend the configuration (eg. lease4-add, lease6-add, config-get, etc....), there is no need to refresh the relevant daemon configuration. Maybe I will add a feature in the future to allow the user to specify if they want the cached_config to be automatically refreshed when a function is called that requires a refresh but for now its manual.
 
+## Parsers
+
+Majority of the useful API functionality requires a subscription for the premium hooks to use API commands like `subnet4-add` or `network6-add` as an example. This is typically the recommended way to interact with Kea as there is some additional validation that the API will perform and potentially prevent misconfiguration of your daemons (Dhcp4, Dhcp6, Control Agent, DDNS) that pykeadhcp may not correctly implement.
+
+However with the use of `config-test` and `config-set` API commands which are supported for all daemons in the free version of ISC Kea DHCP, you can utilize the various parsers implemented in pykeadhcp which provides similar functionality to create, read, update and delete various resources like subnets, shared networks, reservations etc... The parsers attempt to parse a local configuration (eg. server.dhcp4.cached_config) and should be used with the 2 API commands `config-test` and `config-set`. The problem with `config-set` is that it will restart the daemon on the server unlike the specific commands to directly interact with the configuration.
+
+Before continuing, these parsers are manually crafted and can break at anytime when ISC release an update that changes the behaviour of the configuration model. Therefore you should use parsers at your own risk.
+
+### Example of Dhcp4Parser to retrieve a specific subnet by a CIDR
+
+```python
+from pykeadhcp import Kea
+from pykeadhcp.parsers.dhcp4 import Dhcp4Parser
+
+cidr_to_find = "192.168.1.0/24"
+
+server = Kea(host="http://localhost", port=8000)
+parser = Dhcp4Parser(config=server.dhcp4.cached_config)
+subnet = parser.get_subnet_by_cidr(cidr=cidr_to_find)
+
+if not subnet:
+    exit(f"Unable to find subnet: {cidr_to_find}")
+
+print(f"Found Subnet {cidr_to_find} (Subnet ID: {subnet.id})")
+
+option_data = subnet.option_data
+for option in option_data:
+    print(f"Code: {option.code}")
+    print(f"Data: {option.data}")
+
+# Output
+# Found Subnet 192.168.1.0/24 (Subnet ID: 1)
+# Code: 3
+# Data: 192.168.1.1
+# Code: 6
+# Data: 1.1.1.1,9.9.9.9
+```
+
 ## API Reference
 
-All supported commands by the daemons are in the format of the API referenced commands with the exception of replacing any hypthen or space with an underscore. Eg. the `build-report` API command for all daemons is implemented as `build_report` so it heavily ties into the Kea predefined commands when looking at their documentation. Currently everything is built towards Kea 2.2.0. Pydantic variables will replace any hyphens with an underscore however when loading/exporting the data models, it will replace all keys with the hyphen to adhere to the Kea expected variables, ensure that the `KeaBaseModel` (located in `from pykeadhcp.models.generic.base import KeaBaseModel` instead of `from pydantic import BaseModel`) is used when creating any Pydantic models to inherit this functionality.
+All supported commands by the daemons are in the format of the API referenced commands with the exception of replacing any hyphen or space with an underscore. Eg. the `build-report` API command for all daemons is implemented as `build_report` so it heavily ties into the Kea predefined commands when looking at their documentation. Currently everything is built towards Kea 2.2.0. Pydantic variables will replace any hyphens with an underscore however when loading/exporting the data models, it will replace all keys with the hyphen to adhere to the Kea expected variables, ensure that the `KeaBaseModel` (located in `from pykeadhcp.models.generic.base import KeaBaseModel` instead of `from pydantic import BaseModel`) is used when creating any Pydantic models to inherit this functionality.
 
 ## Development / Contribution
 
 See [this document which explains the development/setup to contribute to this project](CONTRIBUTING.md)
 
 ## Commands Implemented/Tested
```

