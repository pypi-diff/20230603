# Comparing `tmp/rdns_reaper-0.1.1.tar.gz` & `tmp/rdns_reaper-0.1.1rc1.tar.gz`

## Comparing `rdns_reaper-0.1.1.tar` & `rdns_reaper-0.1.1rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/SECURITY.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/rdns_reaper/__init__.py
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/rdns_reaper/rdns_reaper.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/.gitignore
--rw-r--r--   0        0        0    35270 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/LICENSE
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/README.md
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/SECURITY.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/rdns_reaper/__init__.py
+-rw-r--r--   0        0        0    18919 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/rdns_reaper/rdns_reaper.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/.gitignore
+-rw-r--r--   0        0        0    35270 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/LICENSE
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/README.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 rdns_reaper-0.1.1rc1/PKG-INFO
```

### Comparing `rdns_reaper-0.1.1/CHANGELOG.md` & `rdns_reaper-0.1.1rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `rdns_reaper-0.1.1/SECURITY.md` & `rdns_reaper-0.1.1rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `rdns_reaper-0.1.1/rdns_reaper/rdns_reaper.py` & `rdns_reaper-0.1.1rc1/rdns_reaper/rdns_reaper.py`

 * *Files 12% similar despite different names*

```diff
@@ -146,16 +146,15 @@
         if kwargs.get("autosave") is True:
             if (self._options_dict["filename"] is not None) and (
                 self._options_dict["filemode"] == "w"
             ):
                 self._options_dict["autosave"] = True
             else:
                 raise ValueError(
-                    "Autosave enabled but filename/mode not set correctly."
-                    ' Filename must be present and mode must be "w".'
+                    'Autosave enabled but filename/mode not set correctly.  Filename must be present and mode must be "w".'
                 )
 
     def __add__(self, new):
         """Add two instances together and return a deepcopy."""
         self_copy = copy.deepcopy(self)
         if isinstance(new, RdnsReaper):
             self_copy._dns_dict.update(new._dns_dict)
@@ -273,41 +272,14 @@
 
         """
         if not isinstance(option, bool):
             raise TypeError
 
         self._options_dict["allow_reserved_networks"] = option
 
-    def autosave(self, option: bool):
-        """Allow users to enable/disable automatic saving of disk based cache
-
-        The filename and filemode options must already be set or attempting to turn this on will
-        cause an exception to be raised.
-
-        Args:
-            option (bool) Set to True to enable automatic saving of disk based cache
-
-        """
-        if not isinstance(option, bool):
-            raise TypeError()
-
-        if option:
-            if (self._options_dict["filename"] is not None) and (
-                self._options_dict["filemode"] == "w"
-            ):
-                self._options_dict["autosave"] = True
-            else:
-                raise ValueError(
-                    "Autosave enabled but filename/mode not set correctly."
-                    ' Filename must be present and mode must be "w".'
-                )
-
-        if option is False:
-            self._options_dict["autosave"] = False
-
     def clear_all_hostnames(self):
         """Clear all the hostnames from existing entries."""
         new_ip_dict = {ip: None for ip in self._dns_dict}
         self._dns_dict = new_ip_dict
 
     def clearname(self, ip_address: str):
         """Clear a specific IP's hostname.
@@ -450,35 +422,32 @@
         ):
             filename = self._options_dict["filename"]
 
         with open(filename, "w", encoding="UTF-8") as f_handle:
             f_handle.write("---\n")
             f_handle.write(yaml.dump(self._dns_dict))
 
-    def set_file(self, filename, filemode=None):
-        """Set the filename and filemode for the disk based cache
+    def set_name(self, ip_address: str, hostname: str):
+        """Force the hostname of an IP.
 
         Args:
-            filename (str): Filename (path optional) for disk based cache
-            filemode (str): Read/write mode ("r"|"w") option for disk based cache
-
+            ip_address (str): String containing an IP address to be modified
+            hostname (str): Desired FQDN hostname to be set for this entry
+                Can be None to reset record to allow for subsequent lookup
         """
-        if not (isinstance(filename, str) or filename is None):
-            raise TypeError("String type expected")
-
-        if filename is None or filemode is None:
-            self._options_dict["filename"] = None
-            self._options_dict["filemode"] = None
-            return
-
-        if filemode not in ("r", "w"):
-            raise ValueError('Filemode must be "R" or "W"')
+        try:
+            IPAddress(ip_address)
+        except AddrFormatError as error_case:
+            raise TypeError(f"IP Error: {error_case}") from error_case
 
-        self._options_dict["filename"] = filename
-        self._options_dict["filemode"] = filemode
+        if ip_address not in self._dns_dict.keys():
+            raise KeyError("Address does not exist")
+        self._dns_dict[ip_address] = hostname
+        # except KeyError as error_case:
+        # raise KeyError("Address does not exist")
 
     def set_filter(self, filter_data: str, **kwargs):
         """Define a custom filter."""
         if kwargs.get("mode") is None:
             self._options_dict["filter_mode"] = "block"
         elif kwargs.get("mode").lower() in ("allow", "block"):
             self._options_dict["filter_mode"] = kwargs.get("mode").lower()
@@ -491,33 +460,14 @@
             filter_data = IPSet(filter_data)
 
         if not isinstance(filter_data, IPSet):
             raise TypeError
 
         self._options_dict["filter"] = filter_data
 
-    def set_name(self, ip_address: str, hostname: str):
-        """Force the hostname of an IP.
-
-        Args:
-            ip_address (str): String containing an IP address to be modified
-            hostname (str): Desired FQDN hostname to be set for this entry
-                Can be None to reset record to allow for subsequent lookup
-        """
-        try:
-            IPAddress(ip_address)
-        except AddrFormatError as error_case:
-            raise TypeError(f"IP Error: {error_case}") from error_case
-
-        if ip_address not in self._dns_dict.keys():
-            raise KeyError("Address does not exist")
-        self._dns_dict[ip_address] = hostname
-        # except KeyError as error_case:
-        # raise KeyError("Address does not exist")
-
     def values(self) -> list:
         """Return the hostnames as values in list format."""
         return list(self._dns_dict.values())
 
     @staticmethod
     def _isrfc1918(address_txt) -> bool:
         """Determine if an address is RFC1918 private or not."""
```

### Comparing `rdns_reaper-0.1.1/.gitignore` & `rdns_reaper-0.1.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `rdns_reaper-0.1.1/LICENSE` & `rdns_reaper-0.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdns_reaper-0.1.1/README.md` & `rdns_reaper-0.1.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,30 +116,28 @@
 * iter() - will provider an iterator that returns address/name tuples
 * len() - number of unique IP addresses in a resolver instance
 
 ### Supported custom methods
 * add_ip(IP) - adds an IP address (provided as a string)
 * add_ip_list(IP_LIST) - adds IP addresses (provided as a list of strings)
 * allow_reserved_networks() - disable/enable automatic filter of reserved networks
-* autosave() - disable/enable automatic saving of disk based cache
 * clear_all_hostnames() - resets all names to None across entire instance
 * clearname(IP) - resets a name to None
 * get_dict() - returns a dictionary with addresses as keys and names as values
 * get_filter() - returns a tuple with custom filter information or None if not set
 * get_options() - returns a dictionary listing options that have been set
 * keys() - returns a list of all IP addresses in the instance
 * loadfile() - forces a load of the YAML based disk cache
 * limit_to_rfc1918 - disable/enable automatic filtering to only IPv4 RFC1918 networks
 * remove_ip(IP) - removes an IP address (provided as a string)
 * resolve_all() - launches a threaded resolver process
 * resolve_all_serial() - launches a singular serial resolver process
 * savefile() - forces a save of the YAML based disk cache
-* set_file(FILENAME, MODE) - sets the filename and mode ("r"|"w") for disk based cache
-* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
 * set_name(IP, NAME) - forces the name for a value (provided as strings)
+* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
 * values() - returns a list of all DNS names
 
 Issues and contributing
 -----------------------
 
 If you find any issues, feel free to create a new issue at our github repository at: https://github.com/mullaneywt/rdns_reaper/issues
```

### Comparing `rdns_reaper-0.1.1/pyproject.toml` & `rdns_reaper-0.1.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="rdns_reaper"
-version="0.1.1"
+version="0.1.1.rc1"
 authors=[
   {name ="Will Mullaney",email="rdns-reaper@mullaneywt.anonaddy.com"}
 ]
 description="Reverse DNS lookup engine"
 readme = "README.md"
 keywords=["reverse", "dns"]
 license={ text="GNU GPL v3.0" }
```

### Comparing `rdns_reaper-0.1.1/PKG-INFO` & `rdns_reaper-0.1.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdns_reaper
-Version: 0.1.1
+Version: 0.1.1rc1
 Summary: Reverse DNS lookup engine
 Project-URL: Home Page, https://github.com/mullaneywt/rdns_reaper
 Project-URL: Bug Tracker, https://github.com/mullaneywt/rdns_reaper/issues
 Project-URL: Source, https://github.com/mullaneywt/rdns_reaper
 Project-URL: Documentation, https://rdns-reaper.readthedocs.io
 Author-email: Will Mullaney <rdns-reaper@mullaneywt.anonaddy.com>
 License: GNU GPL v3.0
@@ -155,30 +155,28 @@
 * iter() - will provider an iterator that returns address/name tuples
 * len() - number of unique IP addresses in a resolver instance
 
 ### Supported custom methods
 * add_ip(IP) - adds an IP address (provided as a string)
 * add_ip_list(IP_LIST) - adds IP addresses (provided as a list of strings)
 * allow_reserved_networks() - disable/enable automatic filter of reserved networks
-* autosave() - disable/enable automatic saving of disk based cache
 * clear_all_hostnames() - resets all names to None across entire instance
 * clearname(IP) - resets a name to None
 * get_dict() - returns a dictionary with addresses as keys and names as values
 * get_filter() - returns a tuple with custom filter information or None if not set
 * get_options() - returns a dictionary listing options that have been set
 * keys() - returns a list of all IP addresses in the instance
 * loadfile() - forces a load of the YAML based disk cache
 * limit_to_rfc1918 - disable/enable automatic filtering to only IPv4 RFC1918 networks
 * remove_ip(IP) - removes an IP address (provided as a string)
 * resolve_all() - launches a threaded resolver process
 * resolve_all_serial() - launches a singular serial resolver process
 * savefile() - forces a save of the YAML based disk cache
-* set_file(FILENAME, MODE) - sets the filename and mode ("r"|"w") for disk based cache
-* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
 * set_name(IP, NAME) - forces the name for a value (provided as strings)
+* set_filter(IPSet, [mode=]) - sets a custom filter based on an IPSet, IP network in a string, or a list of strings containing IP networks.  Optional mode argument can be `block` or `allow` to set filtering to a block list or allow list
 * values() - returns a list of all DNS names
 
 Issues and contributing
 -----------------------
 
 If you find any issues, feel free to create a new issue at our github repository at: https://github.com/mullaneywt/rdns_reaper/issues
```

