# Comparing `tmp/pulumi_pulumiservice-0.7.3a1685744332.tar.gz` & `tmp/pulumi_pulumiservice-0.7.3a1685755724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_pulumiservice-0.7.3a1685744332.tar", last modified: Fri Jun  2 22:22:27 2023, max compression
+gzip compressed data, was "dist/pulumi_pulumiservice-0.7.3a1685755724.tar", last modified: Sat Jun  3 01:32:47 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.7.3a1685744332.tar` & `pulumi_pulumiservice-0.7.3a1685755724.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-02 22:22:27.000000 pulumi_pulumiservice-0.7.3a1685744332/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:32:47.000000 pulumi_pulumiservice-0.7.3a1685755724/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-03 01:32:46.000000 pulumi_pulumiservice-0.7.3a1685755724/setup.py
```

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/PKG-INFO` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_pulumiservice
-Version: 0.7.3a1685744332
+Name: pulumi-pulumiservice
+Version: 0.7.3a1685755724
 Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/README.md` & `pulumi_pulumiservice-0.7.3a1685755724/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_enums.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/deployment_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/org_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.7.3a1685755724/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-pulumiservice
-Version: 0.7.3a1685744332
+Name: pulumi_pulumiservice
+Version: 0.7.3a1685755724
 Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.7.3a1685755724/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.3a1685744332/setup.py` & `pulumi_pulumiservice-0.7.3a1685755724/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.3a1685744332"
-PLUGIN_VERSION = "0.7.3-alpha.1685744332+29b26792"
+VERSION = "0.7.3a1685755724"
+PLUGIN_VERSION = "0.7.3-alpha.1685755724+9802e4b8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
```

