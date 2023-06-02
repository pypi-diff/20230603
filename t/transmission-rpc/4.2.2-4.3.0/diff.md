# Comparing `tmp/transmission_rpc-4.2.2.tar.gz` & `tmp/transmission_rpc-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-4.2.2.tar", max compression
+gzip compressed data, was "transmission_rpc-4.3.0.tar", max compression
```

## Comparing `transmission_rpc-4.2.2.tar` & `transmission_rpc-4.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1127 2023-05-07 20:19:35.684022 transmission_rpc-4.2.2/LICENSE
--rw-r--r--   0        0        0     1630 2023-05-07 20:19:35.684022 transmission_rpc-4.2.2/README.md
--rw-r--r--   0        0        0     3262 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     2087 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    47234 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/client.py
--rw-r--r--   0        0        0    11533 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1639 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/error.py
--rw-r--r--   0        0        0    12990 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/session.py
--rw-r--r--   0        0        0    23734 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1498 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-06-02 23:49:10.732450 transmission_rpc-4.3.0/LICENSE
+-rw-r--r--   0        0        0     2267 2023-06-02 23:49:10.732450 transmission_rpc-4.3.0/README.md
+-rw-r--r--   0        0        0     3103 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2087 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    44456 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/client.py
+-rw-r--r--   0        0        0    11533 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1639 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12990 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/session.py
+-rw-r--r--   0        0        0    24142 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1498 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2023-06-02 23:49:10.736450 transmission_rpc-4.3.0/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 transmission_rpc-4.3.0/PKG-INFO
```

### Comparing `transmission_rpc-4.2.2/LICENSE` & `transmission_rpc-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/pyproject.toml` & `transmission_rpc-4.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "4.2.2"
+version = "4.3.0"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -29,37 +29,31 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 # dependencies
 requests = "^2.23.0"
 typing-extensions = "*"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = { version = "==6.2.1", python = "^3.9" }
-sphinx-rtd-theme = { version = "==1.2.0", python = "^3.9" }
-sphinx-autobuild = { version = "2021.3.14", python = "^3.9" }
+sphinx = { version = "^7.0.0", python = "^3.9" }
+furo = { version = "2023.05.20", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
-python-dotenv = [
-    { version = "0.21.1", python = "<3.8" },
-    { version = "^1.0.0", python = "^3.8" }
-]
-
 yarl = "==1.9.2"
 # tests
 pytest = "==7.3.1"
-pytest-github-actions-annotate-failures = "==0.1.8"
-coverage = "==7.2.5"
+pytest-github-actions-annotate-failures = "==0.2.0"
+coverage = "==7.2.7"
 
 # linter and formatter
-pre-commit = { version = "==3.2.2", markers = "implementation_name != 'pypy'", python = "^3.9" }
-mypy = { version = "==1.2.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.0.263"
+pre-commit = { version = "==3.3.2", markers = "implementation_name != 'pypy'", python = "^3.9" }
+mypy = { version = "==1.3.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
+ruff = "0.0.270"
 
 # stubs
-types-requests = "==2.29.0.0"
+types-requests = "==2.31.0.1"
 pytz = "==2023.3"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.isort]
 default_section = 'THIRDPARTY'
@@ -72,14 +66,15 @@
 use_parentheses = true
 include_trailing_comma = true
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
 
 [tool.mypy]
+python_version = "3.7"
 disallow_untyped_defs = true
 ignore_missing_imports = true
 warn_return_any = false
 warn_unused_configs = true
 show_error_codes = true
 
 [tool.black]
```

### Comparing `transmission_rpc-4.2.2/transmission_rpc/__init__.py` & `transmission_rpc-4.3.0/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/transmission_rpc/client.py` & `transmission_rpc-4.3.0/transmission_rpc/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import types
 import string
 import logging
 import pathlib
 import warnings
 import urllib.parse
-from typing import Any, Dict, List, Type, Tuple, Union, BinaryIO, Iterable, Optional
+from typing import Any, Dict, List, Type, Tuple, Union, TypeVar, BinaryIO, Iterable, Optional
 from urllib.parse import quote
 
 import requests
 import requests.auth
 import requests.exceptions
 from typing_extensions import Literal, TypedDict
 
@@ -191,15 +191,15 @@
                     headers=self._http_header,
                     json=query,
                     timeout=timeout,
                 )
             except requests.exceptions.Timeout as e:
                 raise TransmissionTimeoutError("timeout when connection to transmission daemon") from e
             except requests.exceptions.ConnectionError as e:
-                raise TransmissionConnectError(f"can't connect to transmission daemon: {str(e)}") from e
+                raise TransmissionConnectError(f"can't connect to transmission daemon: {e!s}") from e
 
             self.session_id = r.headers.get("X-Transmission-Session-Id", "0")
             self.logger.debug(r.text)
             if r.status_code in {401, 403}:
                 self.logger.debug(r.request.headers)
                 raise TransmissionAuthError("transmission daemon require auth", original=r)
             if r.status_code != 409:
@@ -387,48 +387,32 @@
         labels:
             Array of string labels.
             Add in rpc 17.
         """
         if torrent is None:
             raise ValueError("add_torrent requires data or a URI.")
 
-        kwargs: Dict[str, Any] = {}
-        if download_dir is not None:
-            kwargs["download-dir"] = download_dir
-
-        if files_unwanted is not None:
-            kwargs["files-unwanted"] = files_unwanted
-
-        if files_wanted is not None:
-            kwargs["files-wanted"] = files_wanted
-
-        if paused is not None:
-            kwargs["paused"] = paused
-
-        if peer_limit is not None:
-            kwargs["peer-limit"] = peer_limit
-
-        if priority_high is not None:
-            kwargs["priority-high"] = priority_high
-
-        if priority_low is not None:
-            kwargs["priority-low"] = priority_low
-
-        if priority_normal is not None:
-            kwargs["priority-normal"] = priority_normal
-
-        if bandwidthPriority is not None:
-            kwargs["bandwidthPriority"] = bandwidthPriority
-
-        if cookies is not None:
-            kwargs["cookies"] = cookies
-
         if labels is not None:
             self._rpc_version_warning(17)
-            kwargs["labels"] = list(labels)
+
+        kwargs: Dict[str, Any] = remove_unset_value(
+            {
+                "download-dir": download_dir,
+                "files-unwanted": files_unwanted,
+                "files-wanted": files_wanted,
+                "paused": paused,
+                "peer-limit": peer_limit,
+                "priority-high": priority_high,
+                "priority-low": priority_low,
+                "priority-normal": priority_normal,
+                "bandwidthPriority": bandwidthPriority,
+                "cookies": cookies,
+                "labels": list_or_none(labels),
+            }
+        )
 
         torrent_data = _try_read_torrent(torrent)
         if torrent_data:
             kwargs["metainfo"] = torrent_data
         else:
             kwargs["filename"] = torrent
 
@@ -602,19 +586,19 @@
         priority_normal: Optional[Iterable[int]] = None,
         queue_position: Optional[int] = None,
         seed_idle_limit: Optional[int] = None,
         seed_idle_mode: Optional[int] = None,
         seed_ratio_limit: Optional[float] = None,
         seed_ratio_mode: Optional[int] = None,
         tracker_add: Optional[Iterable[str]] = None,
-        tracker_remove: Optional[Iterable[int]] = None,
-        tracker_replace: Optional[Iterable[Tuple[int, str]]] = None,
         labels: Optional[Iterable[str]] = None,
         group: Optional[str] = None,
         tracker_list: Optional[Iterable[Iterable[str]]] = None,
+        tracker_replace: Optional[Iterable[Tuple[int, str]]] = None,
+        tracker_remove: Optional[Iterable[int]] = None,
         **kwargs: Any,
     ) -> None:
         """Change torrent parameters for the torrent(s) with the supplied id's.
 
         Parameters
         ----------
         ids
@@ -657,14 +641,24 @@
             Valid options are :py:class:`transmission_rpc.constants.RatioLimitMode`
         seed_idle_limit
             torrent-level seeding ratio
         seed_idle_mode
             Seed inactivity mode.
 
             Valid options are :py:class:`transmission_rpc.constants.IdleMode`
+        labels
+            Array of string labels.
+            Add in rpc 16.
+        group
+            The name of this torrent's bandwidth group.
+            Add in rpc 17.
+
+        tracker_list
+            A ``Iterable[Iterable[str]]``, each ``Iterable[str]`` for a tracker tier.
+            Add in rpc 17.
 
         tracker_add:
             Array of string with announce URLs to add.
 
             Warnings
             --------
             since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
@@ -679,90 +673,57 @@
         tracker_replace:
             Array of (id, url) tuples where the announcement URL should be replaced.
 
             Warnings
             --------
             since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
 
-        labels
-            Array of string labels.
-            Add in rpc 16.
-
-        group
-            The name of this torrent's bandwidth group.
-            Add in rpc 17.
-
-        tracker_list
-            A ``Iterable[Iterable[str]]``, each ``Iterable[str]`` for a tracker tier.
-            Add in rpc 17.
-
-
         Warnings
         ----
         ``kwargs`` is for the future features not supported yet, it's not compatibility promising.
 
         It will be bypassed to request arguments **as-is**, the underline in the key will not be replaced, so you should use kwargs like ``{'a-argument': 'value'}``
         """
-
-        args: Dict[str, Any] = {}
-
-        if bandwidth_priority is not None:
-            args["bandwidthPriority"] = bandwidth_priority
-
-        if download_limit is not None:
-            args["downloadLimit"] = download_limit
-        if download_limited is not None:
-            args["downloadLimited"] = download_limited
-        if upload_limit is not None:
-            args["uploadLimit"] = upload_limit
-        if upload_limited is not None:
-            args["uploadLimited"] = upload_limited
-        if files_unwanted is not None:
-            args["files-unwanted"] = list(files_unwanted)
-        if files_wanted is not None:
-            args["files-wanted"] = list(files_wanted)
-        if honors_session_limits is not None:
-            args["honorsSessionLimits"] = honors_session_limits
-        if location is not None:
-            args["location"] = location
-        if peer_limit is not None:
-            args["peer-limit"] = peer_limit
-        if priority_high is not None:
-            args["priority-high"] = list(priority_high)
-        if priority_low is not None:
-            args["priority-low"] = list(priority_low)
-        if priority_normal is not None:
-            args["priority-normal"] = list(priority_normal)
-        if queue_position is not None:
-            args["queuePosition"] = queue_position
-        if seed_idle_limit is not None:
-            args["seedIdleLimit"] = seed_idle_limit
-        if seed_idle_mode is not None:
-            args["seedIdleMode"] = seed_idle_mode
-        if seed_ratio_limit is not None:
-            args["seedRatioLimit"] = seed_ratio_limit
-        if seed_ratio_mode is not None:
-            args["seedRatioMode"] = seed_ratio_mode
-        if tracker_add is not None:
-            args["trackerAdd"] = tracker_add
-        if tracker_remove is not None:
-            args["trackerRemove"] = tracker_remove
-        if tracker_replace is not None:
-            args["trackerReplace"] = tracker_replace
         if labels is not None:
             self._rpc_version_warning(16)
-            args["labels"] = list(labels)
 
         if tracker_list is not None:
             self._rpc_version_warning(17)
-            args["trackerList"] = " ".join("\n".join(x) for x in tracker_list)
 
         if group is not None:
             self._rpc_version_warning(17)
-            args["group"] = str(group)
+
+        args: Dict[str, Any] = remove_unset_value(
+            {
+                "bandwidthPriority": bandwidth_priority,
+                "downloadLimit": download_limit,
+                "downloadLimited": download_limited,
+                "uploadLimit": upload_limit,
+                "uploadLimited": upload_limited,
+                "files-unwanted": list_or_none(files_unwanted),
+                "files-wanted": list_or_none(files_wanted),
+                "honorsSessionLimits": honors_session_limits,
+                "location": location,
+                "peer-limit": peer_limit,
+                "priority-high": list_or_none(priority_high),
+                "priority-low": list_or_none(priority_low),
+                "priority-normal": list_or_none(priority_normal),
+                "queuePosition": queue_position,
+                "seedIdleLimit": seed_idle_limit,
+                "seedIdleMode": seed_idle_mode,
+                "seedRatioLimit": seed_ratio_limit,
+                "seedRatioMode": seed_ratio_mode,
+                "trackerAdd": tracker_add,
+                "trackerRemove": tracker_remove,
+                "trackerReplace": tracker_replace,
+                "labels": list_or_none(labels),
+                "trackerList": None if tracker_list is None else " ".join("\n".join(x) for x in tracker_list),
+                "group": group,
+            }
+        )
 
         args.update(kwargs)
 
         if args:
             self._request(RpcMethod.TorrentSet, args, ids, True, timeout=timeout)
         else:
             ValueError("No arguments to set")
@@ -1041,119 +1002,80 @@
 
         Warnings
         ----
         ``kwargs`` is pass the arguments not supported yet future, it's not compatibility promising.
 
         transmission-rpc will merge ``kwargs`` in rpc arguments *as-is*
         """
-        args: Dict[str, Any] = {}
 
-        if alt_speed_down is not None:
-            args["alt-speed-down"] = alt_speed_down
-        if alt_speed_enabled is not None:
-            args["alt-speed-enabled"] = alt_speed_enabled
-        if alt_speed_time_begin is not None:
-            args["alt-speed-time-begin"] = alt_speed_time_begin
-        if alt_speed_time_day is not None:
-            args["alt-speed-time-day"] = alt_speed_time_day
-        if alt_speed_time_enabled is not None:
-            args["alt-speed-time-enabled"] = alt_speed_time_enabled
-        if alt_speed_time_end is not None:
-            args["alt-speed-time-end"] = alt_speed_time_end
-        if alt_speed_up is not None:
-            args["alt-speed-up"] = alt_speed_up
-        if blocklist_enabled is not None:
-            args["blocklist-enabled"] = blocklist_enabled
-        if blocklist_url is not None:
-            args["blocklist-url"] = blocklist_url
-        if cache_size_mb is not None:
-            args["cache-size-mb"] = cache_size_mb
-        if dht_enabled is not None:
-            args["dht-enabled"] = dht_enabled
-        if download_dir is not None:
-            args["download-dir"] = download_dir
-        if download_queue_enabled is not None:
-            args["download-queue-enabled"] = download_queue_enabled
-        if download_queue_size is not None:
-            args["download-queue-size"] = download_queue_size
-        if encryption is not None:
-            if encryption not in ["required", "preferred", "tolerated"]:
-                raise ValueError("Invalid encryption value")
-            args["encryption"] = encryption
-        if idle_seeding_limit_enabled is not None:
-            args["idle-seeding-limit-enabled"] = idle_seeding_limit_enabled
-        if idle_seeding_limit is not None:
-            args["idle-seeding-limit"] = idle_seeding_limit
-        if incomplete_dir is not None:
-            args["incomplete-dir"] = incomplete_dir
-        if incomplete_dir_enabled is not None:
-            args["incomplete-dir-enabled"] = incomplete_dir_enabled
-        if lpd_enabled is not None:
-            args["lpd-enabled"] = lpd_enabled
-        if peer_limit_global is not None:
-            args["peer-limit-global"] = peer_limit_global
-        if peer_limit_per_torrent is not None:
-            args["peer-limit-per-torrent"] = peer_limit_per_torrent
-        if peer_port_random_on_start is not None:
-            args["peer-port-random-on-start"] = peer_port_random_on_start
-        if peer_port is not None:
-            args["peer-port"] = peer_port
-        if pex_enabled is not None:
-            args["pex-enabled"] = pex_enabled
-        if port_forwarding_enabled is not None:
-            args["port-forwarding-enabled"] = port_forwarding_enabled
-        if queue_stalled_enabled is not None:
-            args["queue-stalled-enabled"] = queue_stalled_enabled
-        if queue_stalled_minutes is not None:
-            args["queue-stalled-minutes"] = queue_stalled_minutes
-        if rename_partial_files is not None:
-            args["rename-partial-files"] = rename_partial_files
-        if script_torrent_done_enabled is not None:
-            args["script-torrent-done-enabled"] = script_torrent_done_enabled
-        if script_torrent_done_filename is not None:
-            args["script-torrent-done-filename"] = script_torrent_done_filename
-        if seed_queue_enabled is not None:
-            args["seed-queue-enabled"] = seed_queue_enabled
-        if seed_queue_size is not None:
-            args["seed-queue-size"] = seed_queue_size
-        if seed_ratio_limit is not None:
-            args["seedRatioLimit"] = seed_ratio_limit
-        if seed_ratio_limited is not None:
-            args["seedRatioLimited"] = seed_ratio_limited
-        if speed_limit_down is not None:
-            args["speed-limit-down"] = speed_limit_down
-        if speed_limit_down_enabled is not None:
-            args["speed-limit-down-enabled"] = speed_limit_down_enabled
-        if speed_limit_up is not None:
-            args["speed-limit-up"] = speed_limit_up
-        if speed_limit_up_enabled is not None:
-            args["speed-limit-up-enabled"] = speed_limit_up_enabled
-        if start_added_torrents is not None:
-            args["start-added-torrents"] = start_added_torrents
-        if trash_original_torrent_files is not None:
-            args["trash-original-torrent-files"] = trash_original_torrent_files
-        if utp_enabled is not None:
-            args["utp-enabled"] = utp_enabled
+        if encryption is not None and encryption not in ["required", "preferred", "tolerated"]:
+            raise ValueError("Invalid encryption value")
 
         if default_trackers is not None:
             self._rpc_version_warning(17)
-            args["default-trackers"] = "\n".join(default_trackers)
-
         if script_torrent_done_seeding_filename is not None:
             self._rpc_version_warning(17)
-            args["script-torrent-done-seeding-filename"] = script_torrent_done_seeding_filename
         if script_torrent_done_seeding_enabled is not None:
             self._rpc_version_warning(17)
-            args["script-torrent-done-seeding-enabled"] = script_torrent_done_seeding_enabled
         if script_torrent_added_enabled is not None:
             self._rpc_version_warning(17)
-            args["script-torrent-added-enabled"] = script_torrent_added_enabled
         if script_torrent_added_filename is not None:
             self._rpc_version_warning(17)
-            args["script-torrent-added-filename"] = script_torrent_added_filename
+
+        args: Dict[str, Any] = remove_unset_value(
+            {
+                "alt-speed-down": alt_speed_down,
+                "alt-speed-enabled": alt_speed_enabled,
+                "alt-speed-time-begin": alt_speed_time_begin,
+                "alt-speed-time-day": alt_speed_time_day,
+                "alt-speed-time-enabled": alt_speed_time_enabled,
+                "alt-speed-time-end": alt_speed_time_end,
+                "alt-speed-up": alt_speed_up,
+                "blocklist-enabled": blocklist_enabled,
+                "blocklist-url": blocklist_url,
+                "cache-size-mb": cache_size_mb,
+                "dht-enabled": dht_enabled,
+                "download-dir": download_dir,
+                "download-queue-enabled": download_queue_enabled,
+                "download-queue-size": download_queue_size,
+                "idle-seeding-limit-enabled": idle_seeding_limit_enabled,
+                "idle-seeding-limit": idle_seeding_limit,
+                "incomplete-dir": incomplete_dir,
+                "incomplete-dir-enabled": incomplete_dir_enabled,
+                "lpd-enabled": lpd_enabled,
+                "peer-limit-global": peer_limit_global,
+                "peer-limit-per-torrent": peer_limit_per_torrent,
+                "peer-port-random-on-start": peer_port_random_on_start,
+                "peer-port": peer_port,
+                "pex-enabled": pex_enabled,
+                "port-forwarding-enabled": port_forwarding_enabled,
+                "queue-stalled-enabled": queue_stalled_enabled,
+                "queue-stalled-minutes": queue_stalled_minutes,
+                "rename-partial-files": rename_partial_files,
+                "script-torrent-done-enabled": script_torrent_done_enabled,
+                "script-torrent-done-filename": script_torrent_done_filename,
+                "seed-queue-enabled": seed_queue_enabled,
+                "seed-queue-size": seed_queue_size,
+                "seedRatioLimit": seed_ratio_limit,
+                "seedRatioLimited": seed_ratio_limited,
+                "speed-limit-down": speed_limit_down,
+                "speed-limit-down-enabled": speed_limit_down_enabled,
+                "speed-limit-up": speed_limit_up,
+                "speed-limit-up-enabled": speed_limit_up_enabled,
+                "start-added-torrents": start_added_torrents,
+                "trash-original-torrent-files": trash_original_torrent_files,
+                "utp-enabled": utp_enabled,
+                "encryption": encryption,
+                "script-torrent-added-filename": script_torrent_added_filename,
+                "script-torrent-done-seeding-filename": script_torrent_done_seeding_filename,
+                "script-torrent-done-seeding-enabled": script_torrent_done_seeding_enabled,
+                "script-torrent-added-enabled": script_torrent_added_enabled,
+                "default-trackers": "\n".join(default_trackers) if default_trackers is not None else None,
+            }
+        )
 
         args.update(kwargs)
 
         if args:
             self._request(RpcMethod.SessionSet, args, timeout=timeout)
 
     def blocklist_update(self, timeout: Optional[_Timeout] = None) -> Optional[int]:
@@ -1193,30 +1115,24 @@
         honors_session_limits: Optional[bool] = None,
         speed_limit_down: Optional[int] = None,
         speed_limit_up_enabled: Optional[bool] = None,
         speed_limit_up: Optional[int] = None,
         speed_limit_down_enabled: Optional[bool] = None,
     ) -> None:
         self._rpc_version_warning(17)
-        arguments: Dict[str, Any] = {"name": name}
-
-        if honors_session_limits is not None:
-            arguments["honorsSessionLimits"] = honors_session_limits
-
-        if speed_limit_down is not None:
-            arguments["speed-limit-down"] = speed_limit_down
-
-        if speed_limit_up_enabled is not None:
-            arguments["speed-limit-up-enabled"] = speed_limit_up_enabled
-
-        if speed_limit_up is not None:
-            arguments["speed-limit-up"] = speed_limit_up
-
-        if speed_limit_down_enabled is not None:
-            arguments["speed-limit-down-enabled"] = speed_limit_down_enabled
+        arguments: Dict[str, Any] = remove_unset_value(
+            {
+                "name": name,
+                "honorsSessionLimits": honors_session_limits,
+                "speed-limit-down": speed_limit_down,
+                "speed-limit-up-enabled": speed_limit_up_enabled,
+                "speed-limit-up": speed_limit_up,
+                "speed-limit-down-enabled": speed_limit_down_enabled,
+            }
+        )
 
         self._request(RpcMethod.GroupSet, arguments, timeout=timeout)
 
     def get_group(self, name: str, *, timeout: Optional[_Timeout] = None) -> Optional[Group]:
         self._rpc_version_warning(17)
         result: Dict[str, Any] = self._request(RpcMethod.GroupGet, {"group": name}, timeout=timeout)
 
@@ -1234,7 +1150,20 @@
         return {x["name"]: Group(fields=x) for x in result["arguments"]["group"]}
 
     def __enter__(self) -> "Client":
         return self
 
     def __exit__(self, exc_type: Type[Exception], exc_val: Exception, exc_tb: types.TracebackType) -> None:
         self._http_session.close()
+
+
+T = TypeVar("T")
+
+
+def list_or_none(v: Optional[Iterable[T]]) -> Optional[List[T]]:
+    if v is None:
+        return None
+    return list(v)
+
+
+def remove_unset_value(data: Dict[str, Any]) -> Dict[str, Any]:
+    return {key: value for key, value in data.items() if value is not None}
```

### Comparing `transmission_rpc-4.2.2/transmission_rpc/constants.py` & `transmission_rpc-4.3.0/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/transmission_rpc/error.py` & `transmission_rpc-4.3.0/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/transmission_rpc/session.py` & `transmission_rpc-4.3.0/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/transmission_rpc/torrent.py` & `transmission_rpc-4.3.0/transmission_rpc/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 import warnings
 from typing import Any, Dict, List, Optional
 from datetime import datetime, timezone, timedelta
 
 from transmission_rpc.types import File, Container
 from transmission_rpc.utils import format_timedelta
 from transmission_rpc.constants import PRIORITY, IDLE_LIMIT, RATIO_LIMIT, Priority
@@ -18,33 +19,52 @@
 
 
 def get_status(code: int) -> str:
     """Get the torrent status using new status codes"""
     return _STATUS_NEW_MAPPING.get(code) or f"unknown status {code}"
 
 
-class Status(str):
-    """A wrapped ``str`` for torrent status.
+class Status(str, enum.Enum):
+    """enum for torrent status"""
 
-    returned by :py:attr:`.Torrent.status`
-    """
+    STOPPED = "stopped"
+    CHECK_PENDING = "check pending"
+    CHECKING = "checking"
+    DOWNLOAD_PENDING = "download pending"
+    DOWNLOADING = "downloading"
+    SEED_PENDING = "seed pending"
+    SEEDING = "seeding"
 
-    stopped: bool
-    check_pending: bool
-    checking: bool
-    download_pending: bool
-    downloading: bool
-    seed_pending: bool
-    seeding: bool
-
-    def __new__(cls, raw: str) -> "Status":
-        obj = super().__new__(cls, raw)
-        for status in _STATUS_NEW_MAPPING.values():
-            setattr(obj, status.replace(" ", "_"), raw == status)
-        return obj
+    @property
+    def stopped(self) -> bool:
+        return self == "stopped"
+
+    @property
+    def check_pending(self) -> bool:
+        return self == "check pending"
+
+    @property
+    def checking(self) -> bool:
+        return self == "checking"
+
+    @property
+    def download_pending(self) -> bool:
+        return self == "download pending"
+
+    @property
+    def downloading(self) -> bool:
+        return self == "downloading"
+
+    @property
+    def seed_pending(self) -> bool:
+        return self == "seed pending"
+
+    @property
+    def seeding(self) -> bool:
+        return self == "seeding"
 
 
 class FileStat(Container):
     @property
     def bytesCompleted(self) -> int:
         return self.fields["bytesCompleted"]
```

### Comparing `transmission_rpc-4.2.2/transmission_rpc/types.py` & `transmission_rpc-4.3.0/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/transmission_rpc/utils.py` & `transmission_rpc-4.3.0/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.2/PKG-INFO` & `transmission_rpc-4.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 4.2.2
+Version: 4.3.0
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.7,<4.0
@@ -14,19 +14,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/Trim21/transmission-rpc
 Description-Content-Type: text/markdown
 
@@ -34,15 +29,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/transmission-rpc)](https://pypi.org/project/transmission-rpc/)
 [![Documentation Status](https://readthedocs.org/projects/transmission-rpc/badge/)](https://transmission-rpc.readthedocs.io/)
 [![ci](https://github.com/Trim21/transmission-rpc/workflows/ci/badge.svg)](https://github.com/Trim21/transmission-rpc/actions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/transmission-rpc)](https://pypi.org/project/transmission-rpc/)
 [![Codecov branch](https://img.shields.io/codecov/c/github/Trim21/transmission-rpc/master)](https://codecov.io/gh/Trim21/transmission-rpc/branch/master)
 
-`transmission-rpc` is a python wrapper of on top of [transmission](https://github.com/transmission/transmission) JSON RPC protocol,
+`transmission-rpc` is a python wrapper on top of [transmission](https://github.com/transmission/transmission) JSON RPC protocol,
 hosted on GitHub at [github.com/trim21/transmission-rpc](https://github.com/trim21/transmission-rpc)
 
 ## Introduction
 
 `transmission-rpc` is a python module implementing the json-rpc client protocol for the BitTorrent client Transmission.
 
 Support 14 <= rpc version <= 17 (2.40 <= transmission version <= 4.0.2),
@@ -63,11 +58,45 @@
 
 <https://transmission-rpc.readthedocs.io/>
 
 ## Contributing
 
 All kinds of PRs (docs, feature, bug fixes and eta...) are most welcome.
 
+### Setup Local Development Environment
+
+At first, you need to install [python](https://python.org/), [poetry](https://python-poetry.org/) and [task](https://taskfile.dev/) (or you can also run command in `taskfile.yaml` directly).
+
+It's recommended to python3.10 as local development python version.
+
+```shell
+poetry install --sync
+poetry run pre-commit install # install git pre-commit hooks
+```
+
+### Lint
+
+```shell
+task lint
+```
+
+### Testing
+
+You need to have a transmission daemon running
+
+then add a `.env` file
+
+```shell
+export TR_HOST="..."
+export TR_PORT="..."
+export TR_USER="..."
+export TR_PASS="..."
+```
+
+```shell
+task test
+```
+
 ## License
 
 `transmission-rpc` is licensed under the MIT license.
```

