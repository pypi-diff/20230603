# Comparing `tmp/synapseclient-2.7.1.tar.gz` & `tmp/synapseclient-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapseclient-2.7.1.tar", last modified: Fri Apr 21 02:24:18 2023, max compression
+gzip compressed data, was "synapseclient-2.7.2.tar", last modified: Sat Jun  3 03:19:55 2023, max compression
```

## Comparing `synapseclient-2.7.1.tar` & `synapseclient-2.7.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11346 2023-04-21 02:24:02.000000 synapseclient-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-21 02:24:02.000000 synapseclient-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-04-21 02:24:18.926428 synapseclient-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6786 2023-04-21 02:24:02.000000 synapseclient-2.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-21 02:24:02.000000 synapseclient-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-21 02:24:18.926428 synapseclient-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4406 2023-04-21 02:24:02.000000 synapseclient-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/.synapseConfig
--rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    62616 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13165 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/activity.py
--rw-r--r--   0 runner    (1001) docker     (122)    14566 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)   192200 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14358 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/constants/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/concrete_types.py
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/config_file_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/credentials/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/cached_sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6160 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/cred_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10606 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/cumulative_transfer_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/dozer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5354 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/logging_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/models/
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/custom_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/dict_object.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseclient/core/multithread_download/
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/multithread_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15019 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/multithread_download/download_threads.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/pool_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/remote_file_storage_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6342 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/retry.py
--rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/sts_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseclient/core/upload/
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22537 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (122)    10111 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/upload_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    32442 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6173 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/version_check.py
--rw-r--r--   0 runner    (1001) docker     (122)    31930 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     9339 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-21 02:24:03.000000 synapseclient-2.7.1/synapseclient/synapsePythonClient
--rw-r--r--   0 runner    (1001) docker     (122)    97630 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/team.py
--rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 02:24:13.000000 synapseclient-2.7.1/synapseclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseutils/
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34034 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/copy_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/describe_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    53112 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/migrate_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    44835 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/walk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11346 2023-06-03 03:19:41.000000 synapseclient-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-03 03:19:41.000000 synapseclient-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-03 03:19:55.519813 synapseclient-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6786 2023-06-03 03:19:41.000000 synapseclient-2.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-03 03:19:41.000000 synapseclient-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-03 03:19:55.523813 synapseclient-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4524 2023-06-03 03:19:41.000000 synapseclient-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.511813 synapseclient-2.7.2/synapseclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/.synapseConfig
+-rw-r--r--   0 runner    (1001) docker     (122)    10843 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62616 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13165 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/activity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14566 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192487 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.515813 synapseclient-2.7.2/synapseclient/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14358 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.515813 synapseclient-2.7.2/synapseclient/core/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/constants/concrete_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/constants/config_file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/constants/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/synapseclient/core/credentials/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/credentials/cached_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6160 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/credentials/cred_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11370 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/credentials/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/cumulative_transfer_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/dozer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5354 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/logging_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/synapseclient/core/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/models/custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/models/dict_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/synapseclient/core/multithread_download/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/multithread_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15019 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/multithread_download/download_threads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/pool_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/remote_file_storage_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6342 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/retry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/sts_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/synapseclient/core/upload/
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22537 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/upload/multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10111 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/upload/upload_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32442 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6173 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/core/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31930 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9339 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/synapsePythonClient
+-rw-r--r--   0 runner    (1001) docker     (122)    97716 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/team.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseclient/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.515813 synapseclient-2.7.2/synapseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 03:19:47.000000 synapseclient-2.7.2/synapseclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-03 03:19:55.000000 synapseclient-2.7.2/synapseclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 03:19:55.519813 synapseclient-2.7.2/synapseutils/
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34034 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/copy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/describe_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53112 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/migrate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44839 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-06-03 03:19:41.000000 synapseclient-2.7.2/synapseutils/walk_functions.py
```

### Comparing `synapseclient-2.7.1/LICENSE` & `synapseclient-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/PKG-INFO` & `synapseclient-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 2.7.1
+Version: 2.7.2
 Summary: A client for Synapse, a collaborative compute space  that allows scientists to share and analyze data together.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache
 Project-URL: Documentation, https://python-docs.synapse.org
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/synapsePythonClient
```

### Comparing `synapseclient-2.7.1/README.md` & `synapseclient-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/setup.py` & `synapseclient-2.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,18 @@
     "pytest>=5.0.0,<7.0",
     "pytest-mock>=3.0,<4.0",
     "flake8>=3.7.0,<4.0",
     "pytest-xdist[psutil]>=2.2,<3.0.0",
 ]
 
 install_requires = [
+    # "requests>=2.22.0,<2.30.0; python_version<'3.10'",
     "requests>=2.22.0,<3.0",
+    "urllib3<2",
+    # "urllib3>=2; python_version>='3.10'",
     "keyring>=15,<23.5",
     "deprecated>=1.2.4,<2.0",
     "importlib-metadata<5.0",
 ]
 
 # on Linux specify a cryptography dependency that will not
 # require a Rust compiler to compile from source (< 3.4).
@@ -75,15 +78,15 @@
     # requirements
     python_requires=">=3.7",
     install_requires=install_requires,
     extras_require={
         "pandas": ["pandas>=0.25.0,<1.5"],
         "pysftp": ["pysftp>=0.2.8,<0.3"],
         "boto3": ["boto3>=1.7.0,<2.0"],
-        "docs": ["sphinx>=3.0,<4.0", "sphinx-argparse>=0.2,<0.3"],
+        "docs": ["sphinx>=4.0,<5.0", "sphinx-argparse>=0.2,<0.3"],
         "tests": test_deps,
         ':sys_platform=="linux"': ["keyrings.alt==3.1"],
     },
     # command line
     entry_points={"console_scripts": ["synapse = synapseclient.__main__:main"]},
     # data
     package_data={"synapseclient": ["synapsePythonClient", ".synapseConfig"]},
```

### Comparing `synapseclient-2.7.1/synapseclient/.synapseConfig` & `synapseclient-2.7.2/synapseclient/.synapseConfig`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/__init__.py` & `synapseclient-2.7.2/synapseclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 `Synapse <https://docs.synapse.org/articles/getting_started.html>`_.
 
 
 Next Major Release (3.0.0)
 ==========================
 - Support only pandas `>=` 1.5
 - Remove support for Python 3.7 due to its end of life.
-- Remove support for login via passwords for best security practices.
 - There will be major cosmetic changes to the cli such as
   removing all camel case or non-standard single dash long command line interface (cli)
   parameters.
   Example: command line arguments like `-parent` will become
   `--parent`.  Commands that support camel case like `--parentId`
   will be changed to `--parent-id`.
 
@@ -70,23 +69,23 @@
     python setup.py <install or develop>
 
 
 Connecting to Synapse
 =====================
 
 To use Synapse, you'll need to `register <https://www.synapse.org/register>`_ for an account. The Synapse
-website can authenticate using a Google account, but you'll need to take the extra step of creating a Synapse password
-to use the programmatic clients.
+website can authenticate using a Google account, but you'll need to take the extra step of creating a Synapse
+personal access token to use the programmatic clients.
 
 Once that's done, you'll be able to load the library, create a :py:class:`Synapse` object and login::
 
     import synapseclient
     syn = synapseclient.Synapse()
 
-    syn.login('my_username', 'my_password')
+    syn.login(authToken=<PAT>)
 
 For more information, see:
 
 - :py:class:`Synapse`
 - :py:func:`Synapse.login`
 - :py:func:`Synapse.logout`
```

### Comparing `synapseclient-2.7.1/synapseclient/__main__.py` & `synapseclient-2.7.2/synapseclient/__main__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/activity.py` & `synapseclient-2.7.2/synapseclient/activity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/annotations.py` & `synapseclient-2.7.2/synapseclient/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/client.py` & `synapseclient-2.7.2/synapseclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,14 +425,19 @@
 
         # Final check on login success
         if not self.credentials:
             raise SynapseNoCredentialsError("No credentials provided.")
 
         # Save the API key in the cache
         if rememberMe:
+            message = (
+                "The rememberMe parameter will be deprecated by early 2024. Please use the ~/.synapseConfig "
+                "or SYNAPSE_AUTH_TOKEN environmental variable to set up your Synapse connection."
+            )
+            self.logger.warning(message)
             delete_stored_credentials(self.credentials.username)
             self.credentials.store_to_keyring()
             cached_sessions.set_most_recent_user(self.credentials.username)
 
         if not silent:
             profile = self.getUserProfile(refresh=True)
             # TODO-PY3: in Python2, do we need to ensure that this is encoded in utf-8
```

### Comparing `synapseclient-2.7.1/synapseclient/core/cache.py` & `synapseclient-2.7.2/synapseclient/core/cache.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/constants/concrete_types.py` & `synapseclient-2.7.2/synapseclient/core/constants/concrete_types.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/credentials/cached_sessions.py` & `synapseclient-2.7.2/synapseclient/core/credentials/cached_sessions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/credentials/cred_data.py` & `synapseclient-2.7.2/synapseclient/core/credentials/cred_data.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/credentials/credential_provider.py` & `synapseclient-2.7.2/synapseclient/core/credentials/credential_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,20 +37,34 @@
         :param ``synapseclient.client.Synapse`` syn:        Synapse client instance
         :param ``cred_data.UserLoginArgs`` user_login_args: subset of arguments passed during syn.login()
         :return: `SynapseCredentials` if valid credentials can be found by this provider, None otherwise
         """
         return self._create_synapse_credential(syn, *self._get_auth_info(syn, user_login_args))
 
     def _create_synapse_credential(self, syn, username, password, api_key, auth_token):
+        login_deprecation_warning = (
+            "This message will disappear if you use a Synapse Personal Access Token to login."
+        )
         if username is not None:
             if password is not None:
+                message = (
+                    "Logging into Synapse via passwords will be deprecated by "
+                    f"early 2024. {login_deprecation_warning}"
+                )
+                syn.logger.warning(message)
                 retrieved_session_token = syn._getSessionToken(email=username, password=password)
                 return SynapseApiKeyCredentials(syn._getAPIKey(retrieved_session_token), username)
 
             elif auth_token is None and api_key is not None:
+                message = (
+                    "Logging into Synapse via apikeys will be deprecated by early 2024.  "
+                    "If you've used `rememberMe=True` in the past, you may also be getting this message, "
+                    f"please delete your ~/.synapseCache/.session file. {login_deprecation_warning}"
+                )
+                syn.logger.warning(message)
                 # auth token takes precedence over api key
                 return SynapseApiKeyCredentials(api_key, username)
 
         if auth_token is not None:
             credentials = SynapseAuthTokenCredentials(auth_token)
             profile = syn.restGET('/userProfile', auth=credentials)
             profile_username = profile.get('userName')
@@ -135,15 +149,14 @@
     """
 
     def _get_auth_info(self, syn, user_login_args):
         username = None
         password = None
         api_key = None
         auth_token = None
-
         if not user_login_args.skip_cache:
             username = user_login_args.username or cached_sessions.get_most_recent_user()
             if username:
                 api_creds = SynapseApiKeyCredentials.get_from_keyring(username)
                 auth_token_creds = SynapseAuthTokenCredentials.get_from_keyring(username)
 
                 api_key = api_creds.secret if api_creds else None
```

### Comparing `synapseclient-2.7.1/synapseclient/core/cumulative_transfer_progress.py` & `synapseclient-2.7.2/synapseclient/core/cumulative_transfer_progress.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/dozer.py` & `synapseclient-2.7.2/synapseclient/core/dozer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/exceptions.py` & `synapseclient-2.7.2/synapseclient/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/lock.py` & `synapseclient-2.7.2/synapseclient/core/lock.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/logging_setup.py` & `synapseclient-2.7.2/synapseclient/core/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/models/custom_json.py` & `synapseclient-2.7.2/synapseclient/core/models/custom_json.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/models/dict_object.py` & `synapseclient-2.7.2/synapseclient/core/models/dict_object.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/multithread_download/download_threads.py` & `synapseclient-2.7.2/synapseclient/core/multithread_download/download_threads.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/pool_provider.py` & `synapseclient-2.7.2/synapseclient/core/pool_provider.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/remote_file_storage_wrappers.py` & `synapseclient-2.7.2/synapseclient/core/remote_file_storage_wrappers.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/retry.py` & `synapseclient-2.7.2/synapseclient/core/retry.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/sts_transfer.py` & `synapseclient-2.7.2/synapseclient/core/sts_transfer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/upload/multipart_upload.py` & `synapseclient-2.7.2/synapseclient/core/upload/multipart_upload.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/upload/upload_functions.py` & `synapseclient-2.7.2/synapseclient/core/upload/upload_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/utils.py` & `synapseclient-2.7.2/synapseclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/core/version_check.py` & `synapseclient-2.7.2/synapseclient/core/version_check.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/entity.py` & `synapseclient-2.7.2/synapseclient/entity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/evaluation.py` & `synapseclient-2.7.2/synapseclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/table.py` & `synapseclient-2.7.2/synapseclient/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,23 +182,22 @@
     data = [["John Coltrane",  "Blue Train",   1957, "BLP 1577", "coltraneBlueTrain.jpg"],
             ["Sonny Rollins",  "Vol. 2",       1957, "BLP 1558", "rollinsBN1558.jpg"],
             ["Sonny Rollins",  "Newk's Time",  1958, "BLP 4001", "rollinsBN4001.jpg"],
             ["Kenny Burrel",   "Kenny Burrel", 1956, "BLP 1543", "burrellWarholBN1543.jpg"]]
 
     # upload album covers
     for row in data:
-        file_handle = syn.uploadSynapseManagedFileHandle(os.path.join(covers_dir, row[4]))
+        file_handle = syn.uploadFileHandle(os.path.join(covers_dir, row[4]), parent=project)
         row[4] = file_handle['id']
 
     # store the table data
-    row_reference_set = syn.store(RowSet(columns=cols, schema=schema, rows=[Row(r) for r in data]))
+    row_reference_set = syn.store(RowSet(schema=schema, rows=[Row(r) for r in data]))
 
     # Later, we'll want to query the table and download our album covers
-    results = syn.tableQuery("select artist, album, 'year', catalog, cover from %s where artist = 'Sonny Rollins'" \
-                             % schema.id)
+    results = syn.tableQuery(f"select artist, album, cover from {schema.id} where artist = 'Sonny Rollins'")
     cover_files = syn.downloadTableColumns(results, ['cover'])
 
 -------------
 Deleting rows
 -------------
 
 Query for the rows you want to delete and call syn.delete on the results::
@@ -1875,27 +1874,31 @@
             self.nextPageToken = result.get('nextPageToken', None)
             self.i = 0
 
             rownames = construct_rownames(self.rowset, offset)
             offset += len(self.rowset['rows'])
 
             if not rowIdAndVersionInIndex:
+                # TODO: Look into why this isn't being assigned
                 series['ROW_ID'].append(pd.Series(name='ROW_ID', data=[row['id'] for row in self.rowset['rows']]))
                 series['ROW_VERSION'].append(pd.Series(name='ROW_VERSION',
                                                        data=[row['version'] for row in self.rowset['rows']]))
                 if append_etag:
                     series['ROW_ETAG'] = pd.Series(name='ROW_ETAG',
                                                    data=[row.get('etag') for row in self.rowset['rows']])
 
             for i, header in enumerate(self.rowset["headers"]):
                 column_name = header.name
-                series[column_name] = series[column_name].append(
-                    pd.Series(name=column_name,
-                              data=[row['values'][i] for row in self.rowset['rows']],
-                              index=rownames),
+                series[column_name] = pd.concat(
+                    [
+                        series[column_name],
+                        pd.Series(name=column_name,
+                                  data=[row['values'][i] for row in self.rowset['rows']],
+                                  index=rownames)
+                    ],
                     # can't verify integrity when indices are just numbers instead of 'rowid_rowversion'
                     verify_integrity=rowIdAndVersionInIndex)
 
         return pd.DataFrame(data=series)
 
     def asRowSet(self):
         # Note that as of stack 60, an empty query will omit the headers field
```

### Comparing `synapseclient-2.7.1/synapseclient/team.py` & `synapseclient-2.7.2/synapseclient/team.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient/wiki.py` & `synapseclient-2.7.2/synapseclient/wiki.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseclient.egg-info/PKG-INFO` & `synapseclient-2.7.2/synapseclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 2.7.1
+Version: 2.7.2
 Summary: A client for Synapse, a collaborative compute space  that allows scientists to share and analyze data together.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache
 Project-URL: Documentation, https://python-docs.synapse.org
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/synapsePythonClient
```

### Comparing `synapseclient-2.7.1/synapseclient.egg-info/SOURCES.txt` & `synapseclient-2.7.2/synapseclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/__init__.py` & `synapseclient-2.7.2/synapseutils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/copy_functions.py` & `synapseclient-2.7.2/synapseutils/copy_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/describe_functions.py` & `synapseclient-2.7.2/synapseutils/describe_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/migrate_functions.py` & `synapseclient-2.7.2/synapseutils/migrate_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/monitor.py` & `synapseclient-2.7.2/synapseutils/monitor.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.1/synapseutils/sync.py` & `synapseclient-2.7.2/synapseutils/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                     self._parent.update(
                         finished_id=self._entity_id,
                         files=self._files,
                         provenance=self._provenance
                     )
 
                 # in practice only the root folder sync will be waited on/need notifying
-                self._finished.notifyAll()
+                self._finished.notify_all()
 
     def _manifest_filename(self):
         return os.path.expanduser(
             os.path.normcase(
                 os.path.join(self._path, MANIFEST_FILENAME)
             )
         )
@@ -191,15 +191,15 @@
 
             # an exception that occurred in this container is considered to have also
             # happened in the parent container and up to the root
             if self._parent:
                 self._parent.set_exception(exception)
 
             # an error also results in the folder being finished
-            self._finished.notifyAll()
+            self._finished.notify_all()
 
     def wait_until_finished(self):
         with self._finished:
             self._finished.wait_for(self._is_finished)
             return self._files
 
     def _is_finished(self):
@@ -592,24 +592,24 @@
                     finished_items[item.entity.path] = entity
                     try:
                         pending_provenance.finished(item.entity.path)
 
                         # this item was defined as provenance for another item, now that
                         # it's finished we may be able to upload that depending item, so
                         # wake up he central thread
-                        dependency_condition.notifyAll()
+                        dependency_condition.notify_all()
 
                     except KeyError:
                         # this item is not used in provenance of another item, that's fine
                         pass
 
         except Exception:
             with dependency_condition:
                 abort_event.set()
-                dependency_condition.notifyAll()
+                dependency_condition.notify_all()
             raise
 
         finally:
             self._file_semaphore.release()
 
 
 def generateManifest(syn, allFiles, filename, provenance_cache=None):
```

### Comparing `synapseclient-2.7.1/synapseutils/walk_functions.py` & `synapseclient-2.7.2/synapseutils/walk_functions.py`

 * *Files identical despite different names*

