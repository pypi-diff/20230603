# Comparing `tmp/bkapi-bk-apigateway-1.0.8.tar.gz` & `tmp/bkapi-bk-apigateway-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bkapi-bk-apigateway-1.0.8.tar", last modified: Sat Jun  3 08:16:07 2023, max compression
+gzip compressed data, was "dist/bkapi-bk-apigateway-1.0.9.tar", last modified: Tue Dec 13 05:26:27 2022, max compression
```

## Comparing `bkapi-bk-apigateway-1.0.8.tar` & `bkapi-bk-apigateway-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi/
--rw-r--r--   0 root         (0) root         (0)      170 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/
--rw-r--r--   0 root         (0) root         (0)       46 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4787 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/client.py
--rw-r--r--   0 root         (0) root         (0)     3122 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/client.pyi
--rw-r--r--   0 root         (0) root         (0)      467 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapigw/
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2323 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/base.py
--rw-r--r--   0 root         (0) root         (0)     3285 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/client.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/conf.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2873 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/resources.py
--rw-r--r--   0 root         (0) root         (0)     2218 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/shortcuts.py
--rw-r--r--   0 root         (0) root         (0)       68 2022-11-22 08:39:18.000000 bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 08:16:07.000000 bkapi-bk-apigateway-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      692 2022-12-05 07:30:51.000000 bkapi-bk-apigateway-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/
+-rw-r--r--   0 root         (0) root         (0)     3297 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/client.pyi
+-rw-r--r--   0 root         (0) root         (0)       46 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      467 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)     5058 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/
+-rw-r--r--   0 root         (0) root         (0)       80 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/
+-rw-r--r--   0 root         (0) root         (0)     2323 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/base.py
+-rw-r--r--   0 root         (0) root         (0)      451 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)       80 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/resources.py
+-rw-r--r--   0 root         (0) root         (0)       68 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2022-12-08 10:14:27.000000 bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      289 2022-12-13 05:26:27.000000 bkapi-bk-apigateway-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      692 2022-12-13 03:11:00.000000 bkapi-bk-apigateway-1.0.9/setup.py
```

### Comparing `bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/client.py` & `bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,23 @@
     release = bind_property(
         Operation,
         name="release",
         method="POST",
         path="/api/v1/apis/{api_name}/resource_versions/release/",
     )
 
+    # bkapi resource revoke_permissions
+    # 回收应用访问网关 API 的权限
+    revoke_permissions = bind_property(
+        Operation,
+        name="revoke_permissions",
+        method="DELETE",
+        path="/api/v1/apis/{api_name}/permissions/revoke/",
+    )
+
     # bkapi resource sync_api
     # 同步网关
     sync_api = bind_property(
         Operation,
         name="sync_api",
         method="POST",
         path="/api/v1/apis/{api_name}/sync/",
```

### Comparing `bkapi-bk-apigateway-1.0.8/bkapi/bk_apigateway/client.pyi` & `bkapi-bk-apigateway-1.0.9/bkapi/bk_apigateway/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,21 @@
     def release(self) -> Operation:
         """
         bkapi resource release
         发布版本
         """
 
     @property
+    def revoke_permissions(self) -> Operation:
+        """
+        bkapi resource revoke_permissions
+        回收应用访问网关 API 的权限
+        """
+
+    @property
     def sync_api(self) -> Operation:
         """
         bkapi resource sync_api
         同步网关
         """
 
     @property
```

### Comparing `bkapi-bk-apigateway-1.0.8/bkapi_bk_apigateway.egg-info/SOURCES.txt` & `bkapi-bk-apigateway-1.0.9/bkapi_bk_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/base.py` & `bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/base.py`

 * *Files identical despite different names*

### Comparing `bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/client.py` & `bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/client.py`

 * *Files identical despite different names*

### Comparing `bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/conf.py` & `bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/conf.py`

 * *Files identical despite different names*

### Comparing `bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/resources.py` & `bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
         self.import_resource_docs_by_archive = RequestAPI(client=self.client, method="POST", host=self.host, path="/api/v1/apis/{api_name}/resource-docs/import/by-archive/")
 
         self.import_resource_docs_by_swagger = RequestAPI(client=self.client, method="POST", host=self.host, path="/api/v1/apis/{api_name}/resource-docs/import/by-swagger/")
 
         self.add_related_apps = RequestAPI(client=self.client, method="POST", host=self.host, path="/api/v1/apis/{api_name}/related-apps/")
 
+        self.revoke_permissions = RequestAPI(client=self.client, method="DELETE", host=self.host, path="/api/v1/apis/{api_name}/permissions/revoke/")
+
         self.generate_sdk = RequestAPI(client=self.client, method="POST", host=self.host, path="/api/v1/apis/{api_name}/sdk/")
 
         self.get_apis = RequestAPI(client=self.client, method="GET", host=self.host, path="/api/v1/apis/")
 
         self.get_stages = RequestAPI(client=self.client, method="GET", host=self.host, path="/api/v1/apis/{api_name}/stages/")
 
         self.get_released_resources = RequestAPI(client=self.client, method="GET", host=self.host, path="/api/v1/apis/{api_name}/released/stages/{stage_name}/resources/")
```

### Comparing `bkapi-bk-apigateway-1.0.8/bkapigw/bk_apigateway/shortcuts.py` & `bkapi-bk-apigateway-1.0.9/bkapigw/bk_apigateway/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bkapi-bk-apigateway-1.0.8/setup.py` & `bkapi-bk-apigateway-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description=r'''蓝鲸API网关''',
     long_description=readme,
     name='bkapi-bk-apigateway',
-    version='1.0.8',
+    version='1.0.9',
     python_requires='!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<4.0,>=2.7',
     author='blueking',
     license='Apach License 2.0',
     packages=find_packages(),
     namespace_packages=find_packages(exclude=["*.*"]),
     package_dir={"": "."},
     package_data={"bkapi.bk_apigateway": ["py.typed", "*.pyi"]},
```

