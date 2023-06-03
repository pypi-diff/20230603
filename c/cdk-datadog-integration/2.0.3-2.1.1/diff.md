# Comparing `tmp/cdk-datadog-integration-2.0.3.tar.gz` & `tmp/cdk-datadog-integration-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-datadog-integration-2.0.3.tar", last modified: Sat Sep 10 20:16:06 2022, max compression
+gzip compressed data, was "cdk-datadog-integration-2.1.1.tar", last modified: Sat Jun  3 21:01:48 2023, max compression
```

## Comparing `cdk-datadog-integration-2.0.3.tar` & `cdk-datadog-integration-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/
--rw-r--r--   0 runner    (1001) docker     (121)    47492 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31900 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 20:15:51.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-10 20:16:06.579498 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-09-10 20:16:06.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-09-10 20:16:06.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-10 20:16:06.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-10 20:16:06.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-10 20:16:06.000000 cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:01:48.765022 cdk-datadog-integration-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    61591 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35284 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/_jsii/cdk-datadog-integration@2.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:01:36.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:01:48.769022 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-03 21:01:48.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-03 21:01:48.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:01:48.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-03 21:01:48.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 21:01:48.000000 cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/top_level.txt
```

### Comparing `cdk-datadog-integration-2.0.3/LICENSE` & `cdk-datadog-integration-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-datadog-integration-2.0.3/PKG-INFO` & `cdk-datadog-integration-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.0.3
+Version: 2.1.1
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,21 +49,21 @@
    const app = new cdk.App();
    new MonitoringInfrastructureStack(app, "MonitoringInfrastructure");
    ```
 
    ```python
    import * as cdk from "aws-cdk-lib";
    import * as secrets from "aws-cdk-lib/aws-secretsmanager";
-   import { DatadogIntegrationStack } from "cdk-datadog-integration";
+   import { DatadogIntegration } from "cdk-datadog-integration";
 
    export class MonitoringInfrastructureStack extends cdk.Stack {
      constructor(scope: cdk.App, id: string, props?: cdk.StackProps) {
        super(scope, id, props);
 
-       const datadog = new DatadogIntegrationStack(this, "Datadog", {
+       const datadog = new DatadogIntegration(this, "Datadog", {
          // Generate an ID here: https://app.datadoghq.com/account/settings#integrations/amazon-web-services
          externalId: "",
 
          // Create or lookup a `Secret` that contains your Datadog API Key
          // See https://docs.aws.amazon.com/cdk/api/latest/docs/aws-secretsmanager-readme.html for details on Secrets in CDK
          // Get your API key here: https://app.datadoghq.com/account/settings#api
          apiKey: secrets.Secret.fromSecretNameV2(
@@ -115,9 +115,7 @@
 ## Contributing
 
 PRs are welcome!
 
 ### Releasing
 
 To release, merge your PR to `main`.
-
-
```

### Comparing `cdk-datadog-integration-2.0.3/README.md` & `cdk-datadog-integration-2.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,21 @@
    const app = new cdk.App();
    new MonitoringInfrastructureStack(app, "MonitoringInfrastructure");
    ```
 
    ```python
    import * as cdk from "aws-cdk-lib";
    import * as secrets from "aws-cdk-lib/aws-secretsmanager";
-   import { DatadogIntegrationStack } from "cdk-datadog-integration";
+   import { DatadogIntegration } from "cdk-datadog-integration";
 
    export class MonitoringInfrastructureStack extends cdk.Stack {
      constructor(scope: cdk.App, id: string, props?: cdk.StackProps) {
        super(scope, id, props);
 
-       const datadog = new DatadogIntegrationStack(this, "Datadog", {
+       const datadog = new DatadogIntegration(this, "Datadog", {
          // Generate an ID here: https://app.datadoghq.com/account/settings#integrations/amazon-web-services
          externalId: "",
 
          // Create or lookup a `Secret` that contains your Datadog API Key
          // See https://docs.aws.amazon.com/cdk/api/latest/docs/aws-secretsmanager-readme.html for details on Secrets in CDK
          // Get your API key here: https://app.datadoghq.com/account/settings#api
          apiKey: secrets.Secret.fromSecretNameV2(
```

### Comparing `cdk-datadog-integration-2.0.3/setup.py` & `cdk-datadog-integration-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-datadog-integration",
-    "version": "2.0.3",
+    "version": "2.1.1",
     "description": "cdk-datadog-integration",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-datadog-integration.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer",
     "bdist_wheel": {
         "universal": true
@@ -22,36 +22,38 @@
     },
     "packages": [
         "cdk_datadog_integration",
         "cdk_datadog_integration._jsii"
     ],
     "package_data": {
         "cdk_datadog_integration._jsii": [
-            "cdk-datadog-integration@2.0.3.jsii.tgz"
+            "cdk-datadog-integration@2.1.1.jsii.tgz"
         ],
         "cdk_datadog_integration": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.1.0, <3.0.0",
+        "aws-cdk-lib>=2.56.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.60.0, <2.0.0",
-        "publication>=0.0.3"
+        "jsii>=1.82.0, <2.0.0",
+        "publication>=0.0.3",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-datadog-integration-2.0.3/src/cdk_datadog_integration/__init__.py` & `cdk-datadog-integration-2.1.1/src/cdk_datadog_integration/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,21 +26,21 @@
    const app = new cdk.App();
    new MonitoringInfrastructureStack(app, "MonitoringInfrastructure");
    ```
 
    ```python
    import * as cdk from "aws-cdk-lib";
    import * as secrets from "aws-cdk-lib/aws-secretsmanager";
-   import { DatadogIntegrationStack } from "cdk-datadog-integration";
+   import { DatadogIntegration } from "cdk-datadog-integration";
 
    export class MonitoringInfrastructureStack extends cdk.Stack {
      constructor(scope: cdk.App, id: string, props?: cdk.StackProps) {
        super(scope, id, props);
 
-       const datadog = new DatadogIntegrationStack(this, "Datadog", {
+       const datadog = new DatadogIntegration(this, "Datadog", {
          // Generate an ID here: https://app.datadoghq.com/account/settings#integrations/amazon-web-services
          externalId: "",
 
          // Create or lookup a `Secret` that contains your Datadog API Key
          // See https://docs.aws.amazon.com/cdk/api/latest/docs/aws-secretsmanager-readme.html for details on Secrets in CDK
          // Get your API key here: https://app.datadoghq.com/account/settings#api
          apiKey: secrets.Secret.fromSecretNameV2(
@@ -103,42 +103,44 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
+from typeguard import check_type
+
 from ._jsii import *
 
-import aws_cdk
-import aws_cdk.aws_s3
-import aws_cdk.aws_secretsmanager
-import constructs
+import aws_cdk as _aws_cdk_ceddda9d
+import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
+import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class DatadogIntegration(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-datadog-integration.DatadogIntegration",
 ):
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        api_key: aws_cdk.aws_secretsmanager.ISecret,
+        api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
         external_id: builtins.str,
         additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        cloud_trails: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         forwarder_name: typing.Optional[builtins.str] = None,
         forwarder_version: typing.Optional[builtins.str] = None,
         iam_role_name: typing.Optional[builtins.str] = None,
         install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
-        log_archives: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         permissions: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param api_key: API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).
@@ -150,14 +152,18 @@
         :param forwarder_version: Specify a version of the forwarder to use. See https://github.com/DataDog/datadog-serverless-functions/releases. Pass this parameter as a version string, e.g., '3.9.0' Default: latest
         :param iam_role_name: Customize the name of IAM role for Datadog AWS integration. Default: DatadogIntegrationRole
         :param install_datadog_policy_macro: If you already deployed a stack using this template, set this parameter to false to skip the installation of the DatadogPolicy Macro again. Default: true
         :param log_archives: S3 paths to store log archives for log rehydration. Permissions will be automatically added to the Datadog integration IAM role. https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         :param permissions: Customize the permission level for the Datadog IAM role. Select "Core" to only grant Datadog read-only permissions (not recommended). Default: Full
         :param site: Define your Datadog Site to send data to. For the Datadog EU site, set to datadoghq.eu Default: datadoghq.com
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__6eef2e92fcef25509de72f7d20eedd3cd3b3fb23cfe569b9b88802bf6c3e597c)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DatadogIntegrationConfig(
             api_key=api_key,
             external_id=external_id,
             additional_forwarder_params=additional_forwarder_params,
             additional_integration_role_params=additional_integration_role_params,
             cloud_trails=cloud_trails,
             forwarder_name=forwarder_name,
@@ -190,24 +196,24 @@
         "site": "site",
     },
 )
 class DatadogIntegrationConfig:
     def __init__(
         self,
         *,
-        api_key: aws_cdk.aws_secretsmanager.ISecret,
+        api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
         external_id: builtins.str,
         additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        cloud_trails: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         forwarder_name: typing.Optional[builtins.str] = None,
         forwarder_version: typing.Optional[builtins.str] = None,
         iam_role_name: typing.Optional[builtins.str] = None,
         install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
-        log_archives: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         permissions: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param api_key: API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).
         :param external_id: External ID for the Datadog role (generate at https://app.datadoghq.com/account/settings#integrations/amazon-web-services).
         :param additional_forwarder_params: Additional parameters to pass through to the underlying Forwarder CloudFormation template. Use this construct if you need to specify a template variable not yet exposed through this library. See https://datadog-cloudformation-template.s3.amazonaws.com/aws/forwarder/latest.yaml for the latest parameters.
@@ -217,15 +223,29 @@
         :param forwarder_version: Specify a version of the forwarder to use. See https://github.com/DataDog/datadog-serverless-functions/releases. Pass this parameter as a version string, e.g., '3.9.0' Default: latest
         :param iam_role_name: Customize the name of IAM role for Datadog AWS integration. Default: DatadogIntegrationRole
         :param install_datadog_policy_macro: If you already deployed a stack using this template, set this parameter to false to skip the installation of the DatadogPolicy Macro again. Default: true
         :param log_archives: S3 paths to store log archives for log rehydration. Permissions will be automatically added to the Datadog integration IAM role. https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         :param permissions: Customize the permission level for the Datadog IAM role. Select "Core" to only grant Datadog read-only permissions (not recommended). Default: Full
         :param site: Define your Datadog Site to send data to. For the Datadog EU site, set to datadoghq.eu Default: datadoghq.com
         '''
-        self._values: typing.Dict[str, typing.Any] = {
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__44fa621160bdd64de013f756d1f25c947b0015b7f2c0120beaea14eed5c3b640)
+            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
+            check_type(argname="argument external_id", value=external_id, expected_type=type_hints["external_id"])
+            check_type(argname="argument additional_forwarder_params", value=additional_forwarder_params, expected_type=type_hints["additional_forwarder_params"])
+            check_type(argname="argument additional_integration_role_params", value=additional_integration_role_params, expected_type=type_hints["additional_integration_role_params"])
+            check_type(argname="argument cloud_trails", value=cloud_trails, expected_type=type_hints["cloud_trails"])
+            check_type(argname="argument forwarder_name", value=forwarder_name, expected_type=type_hints["forwarder_name"])
+            check_type(argname="argument forwarder_version", value=forwarder_version, expected_type=type_hints["forwarder_version"])
+            check_type(argname="argument iam_role_name", value=iam_role_name, expected_type=type_hints["iam_role_name"])
+            check_type(argname="argument install_datadog_policy_macro", value=install_datadog_policy_macro, expected_type=type_hints["install_datadog_policy_macro"])
+            check_type(argname="argument log_archives", value=log_archives, expected_type=type_hints["log_archives"])
+            check_type(argname="argument permissions", value=permissions, expected_type=type_hints["permissions"])
+            check_type(argname="argument site", value=site, expected_type=type_hints["site"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "api_key": api_key,
             "external_id": external_id,
         }
         if additional_forwarder_params is not None:
             self._values["additional_forwarder_params"] = additional_forwarder_params
         if additional_integration_role_params is not None:
             self._values["additional_integration_role_params"] = additional_integration_role_params
@@ -243,19 +263,19 @@
             self._values["log_archives"] = log_archives
         if permissions is not None:
             self._values["permissions"] = permissions
         if site is not None:
             self._values["site"] = site
 
     @builtins.property
-    def api_key(self) -> aws_cdk.aws_secretsmanager.ISecret:
+    def api_key(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
         '''API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).'''
         result = self._values.get("api_key")
         assert result is not None, "Required property 'api_key' is missing"
-        return typing.cast(aws_cdk.aws_secretsmanager.ISecret, result)
+        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, result)
 
     @builtins.property
     def external_id(self) -> builtins.str:
         '''External ID for the Datadog role (generate at https://app.datadoghq.com/account/settings#integrations/amazon-web-services).'''
         result = self._values.get("external_id")
         assert result is not None, "Required property 'external_id' is missing"
         return typing.cast(builtins.str, result)
@@ -287,23 +307,25 @@
         See https://datadog-cloudformation-template.s3.amazonaws.com/aws/datadog_integration_role.yaml
         for the latest parameters.
         '''
         result = self._values.get("additional_integration_role_params")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
-    def cloud_trails(self) -> typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]]:
+    def cloud_trails(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]]:
         '''S3 buckets for Datadog CloudTrail integration.
 
         Permissions will be automatically
         added to the Datadog integration IAM role.
         https://docs.datadoghq.com/integrations/amazon_cloudtrail
         '''
         result = self._values.get("cloud_trails")
-        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]], result)
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]], result)
 
     @builtins.property
     def forwarder_name(self) -> typing.Optional[builtins.str]:
         '''The Datadog Forwarder Lambda function name.
 
         DO NOT change when updating an existing
         CloudFormation stack, otherwise the current forwarder function will be replaced and
@@ -342,22 +364,24 @@
 
         :default: true
         '''
         result = self._values.get("install_datadog_policy_macro")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def log_archives(self) -> typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]]:
+    def log_archives(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]]:
         '''S3 paths to store log archives for log rehydration.
 
         Permissions will be automatically added to the Datadog integration IAM role.
         https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         '''
         result = self._values.get("log_archives")
-        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]], result)
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]], result)
 
     @builtins.property
     def permissions(self) -> typing.Optional[builtins.str]:
         '''Customize the permission level for the Datadog IAM role.
 
         Select "Core" to only grant Datadog read-only permissions (not recommended).
 
@@ -386,40 +410,42 @@
     def __repr__(self) -> str:
         return "DatadogIntegrationConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 class DatadogIntegrationStack(
-    aws_cdk.Stack,
+    _aws_cdk_ceddda9d.Stack,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-datadog-integration.DatadogIntegrationStack",
 ):
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        api_key: aws_cdk.aws_secretsmanager.ISecret,
+        api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
         external_id: builtins.str,
         additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        cloud_trails: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         forwarder_name: typing.Optional[builtins.str] = None,
         forwarder_version: typing.Optional[builtins.str] = None,
         iam_role_name: typing.Optional[builtins.str] = None,
         install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
-        log_archives: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         permissions: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
+        cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        env: typing.Optional[aws_cdk.Environment] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
-        synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
+        synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param api_key: API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).
@@ -431,92 +457,107 @@
         :param forwarder_version: Specify a version of the forwarder to use. See https://github.com/DataDog/datadog-serverless-functions/releases. Pass this parameter as a version string, e.g., '3.9.0' Default: latest
         :param iam_role_name: Customize the name of IAM role for Datadog AWS integration. Default: DatadogIntegrationRole
         :param install_datadog_policy_macro: If you already deployed a stack using this template, set this parameter to false to skip the installation of the DatadogPolicy Macro again. Default: true
         :param log_archives: S3 paths to store log archives for log rehydration. Permissions will be automatically added to the Datadog integration IAM role. https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         :param permissions: Customize the permission level for the Datadog IAM role. Select "Core" to only grant Datadog read-only permissions (not recommended). Default: Full
         :param site: Define your Datadog Site to send data to. For the Datadog EU site, set to datadoghq.eu Default: datadoghq.com
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
+        :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. Default: - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag is set, ``LegacyStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__82a6b6f80a71ddfdf5adc118127ee2b20923041977d797bc2d0c3ee639fc3a5e)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DatadogIntegrationStackConfig(
             api_key=api_key,
             external_id=external_id,
             additional_forwarder_params=additional_forwarder_params,
             additional_integration_role_params=additional_integration_role_params,
             cloud_trails=cloud_trails,
             forwarder_name=forwarder_name,
             forwarder_version=forwarder_version,
             iam_role_name=iam_role_name,
             install_datadog_policy_macro=install_datadog_policy_macro,
             log_archives=log_archives,
             permissions=permissions,
             site=site,
             analytics_reporting=analytics_reporting,
+            cross_region_references=cross_region_references,
             description=description,
             env=env,
+            permissions_boundary=permissions_boundary,
             stack_name=stack_name,
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
 @jsii.data_type(
     jsii_type="cdk-datadog-integration.DatadogIntegrationStackConfig",
-    jsii_struct_bases=[DatadogIntegrationConfig, aws_cdk.StackProps],
+    jsii_struct_bases=[DatadogIntegrationConfig, _aws_cdk_ceddda9d.StackProps],
     name_mapping={
         "api_key": "apiKey",
         "external_id": "externalId",
         "additional_forwarder_params": "additionalForwarderParams",
         "additional_integration_role_params": "additionalIntegrationRoleParams",
         "cloud_trails": "cloudTrails",
         "forwarder_name": "forwarderName",
         "forwarder_version": "forwarderVersion",
         "iam_role_name": "iamRoleName",
         "install_datadog_policy_macro": "installDatadogPolicyMacro",
         "log_archives": "logArchives",
         "permissions": "permissions",
         "site": "site",
         "analytics_reporting": "analyticsReporting",
+        "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
+        "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
         "synthesizer": "synthesizer",
         "tags": "tags",
         "termination_protection": "terminationProtection",
     },
 )
-class DatadogIntegrationStackConfig(DatadogIntegrationConfig, aws_cdk.StackProps):
+class DatadogIntegrationStackConfig(
+    DatadogIntegrationConfig,
+    _aws_cdk_ceddda9d.StackProps,
+):
     def __init__(
         self,
         *,
-        api_key: aws_cdk.aws_secretsmanager.ISecret,
+        api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
         external_id: builtins.str,
         additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
-        cloud_trails: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         forwarder_name: typing.Optional[builtins.str] = None,
         forwarder_version: typing.Optional[builtins.str] = None,
         iam_role_name: typing.Optional[builtins.str] = None,
         install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
-        log_archives: typing.Optional[typing.Sequence[aws_cdk.aws_s3.Bucket]] = None,
+        log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
         permissions: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
+        cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
-        env: typing.Optional[aws_cdk.Environment] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
-        synthesizer: typing.Optional[aws_cdk.IStackSynthesizer] = None,
+        synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param api_key: API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).
         :param external_id: External ID for the Datadog role (generate at https://app.datadoghq.com/account/settings#integrations/amazon-web-services).
         :param additional_forwarder_params: Additional parameters to pass through to the underlying Forwarder CloudFormation template. Use this construct if you need to specify a template variable not yet exposed through this library. See https://datadog-cloudformation-template.s3.amazonaws.com/aws/forwarder/latest.yaml for the latest parameters.
@@ -526,24 +567,49 @@
         :param forwarder_version: Specify a version of the forwarder to use. See https://github.com/DataDog/datadog-serverless-functions/releases. Pass this parameter as a version string, e.g., '3.9.0' Default: latest
         :param iam_role_name: Customize the name of IAM role for Datadog AWS integration. Default: DatadogIntegrationRole
         :param install_datadog_policy_macro: If you already deployed a stack using this template, set this parameter to false to skip the installation of the DatadogPolicy Macro again. Default: true
         :param log_archives: S3 paths to store log archives for log rehydration. Permissions will be automatically added to the Datadog integration IAM role. https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         :param permissions: Customize the permission level for the Datadog IAM role. Select "Core" to only grant Datadog read-only permissions (not recommended). Default: Full
         :param site: Define your Datadog Site to send data to. For the Datadog EU site, set to datadoghq.eu Default: datadoghq.com
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
+        :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. Default: - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag is set, ``LegacyStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
         '''
         if isinstance(env, dict):
-            env = aws_cdk.Environment(**env)
-        self._values: typing.Dict[str, typing.Any] = {
+            env = _aws_cdk_ceddda9d.Environment(**env)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ead28fadd359def1dfa88cffb1526afb62d1ead36f18794acea0b5f0a9b282e8)
+            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
+            check_type(argname="argument external_id", value=external_id, expected_type=type_hints["external_id"])
+            check_type(argname="argument additional_forwarder_params", value=additional_forwarder_params, expected_type=type_hints["additional_forwarder_params"])
+            check_type(argname="argument additional_integration_role_params", value=additional_integration_role_params, expected_type=type_hints["additional_integration_role_params"])
+            check_type(argname="argument cloud_trails", value=cloud_trails, expected_type=type_hints["cloud_trails"])
+            check_type(argname="argument forwarder_name", value=forwarder_name, expected_type=type_hints["forwarder_name"])
+            check_type(argname="argument forwarder_version", value=forwarder_version, expected_type=type_hints["forwarder_version"])
+            check_type(argname="argument iam_role_name", value=iam_role_name, expected_type=type_hints["iam_role_name"])
+            check_type(argname="argument install_datadog_policy_macro", value=install_datadog_policy_macro, expected_type=type_hints["install_datadog_policy_macro"])
+            check_type(argname="argument log_archives", value=log_archives, expected_type=type_hints["log_archives"])
+            check_type(argname="argument permissions", value=permissions, expected_type=type_hints["permissions"])
+            check_type(argname="argument site", value=site, expected_type=type_hints["site"])
+            check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
+            check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
+            check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
+            check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
+            check_type(argname="argument synthesizer", value=synthesizer, expected_type=type_hints["synthesizer"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument termination_protection", value=termination_protection, expected_type=type_hints["termination_protection"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "api_key": api_key,
             "external_id": external_id,
         }
         if additional_forwarder_params is not None:
             self._values["additional_forwarder_params"] = additional_forwarder_params
         if additional_integration_role_params is not None:
             self._values["additional_integration_role_params"] = additional_integration_role_params
@@ -561,33 +627,37 @@
             self._values["log_archives"] = log_archives
         if permissions is not None:
             self._values["permissions"] = permissions
         if site is not None:
             self._values["site"] = site
         if analytics_reporting is not None:
             self._values["analytics_reporting"] = analytics_reporting
+        if cross_region_references is not None:
+            self._values["cross_region_references"] = cross_region_references
         if description is not None:
             self._values["description"] = description
         if env is not None:
             self._values["env"] = env
+        if permissions_boundary is not None:
+            self._values["permissions_boundary"] = permissions_boundary
         if stack_name is not None:
             self._values["stack_name"] = stack_name
         if synthesizer is not None:
             self._values["synthesizer"] = synthesizer
         if tags is not None:
             self._values["tags"] = tags
         if termination_protection is not None:
             self._values["termination_protection"] = termination_protection
 
     @builtins.property
-    def api_key(self) -> aws_cdk.aws_secretsmanager.ISecret:
+    def api_key(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
         '''API key for the Datadog account (find at https://app.datadoghq.com/account/settings#api).'''
         result = self._values.get("api_key")
         assert result is not None, "Required property 'api_key' is missing"
-        return typing.cast(aws_cdk.aws_secretsmanager.ISecret, result)
+        return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, result)
 
     @builtins.property
     def external_id(self) -> builtins.str:
         '''External ID for the Datadog role (generate at https://app.datadoghq.com/account/settings#integrations/amazon-web-services).'''
         result = self._values.get("external_id")
         assert result is not None, "Required property 'external_id' is missing"
         return typing.cast(builtins.str, result)
@@ -619,23 +689,25 @@
         See https://datadog-cloudformation-template.s3.amazonaws.com/aws/datadog_integration_role.yaml
         for the latest parameters.
         '''
         result = self._values.get("additional_integration_role_params")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
-    def cloud_trails(self) -> typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]]:
+    def cloud_trails(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]]:
         '''S3 buckets for Datadog CloudTrail integration.
 
         Permissions will be automatically
         added to the Datadog integration IAM role.
         https://docs.datadoghq.com/integrations/amazon_cloudtrail
         '''
         result = self._values.get("cloud_trails")
-        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]], result)
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]], result)
 
     @builtins.property
     def forwarder_name(self) -> typing.Optional[builtins.str]:
         '''The Datadog Forwarder Lambda function name.
 
         DO NOT change when updating an existing
         CloudFormation stack, otherwise the current forwarder function will be replaced and
@@ -674,22 +746,24 @@
 
         :default: true
         '''
         result = self._values.get("install_datadog_policy_macro")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def log_archives(self) -> typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]]:
+    def log_archives(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]]:
         '''S3 paths to store log archives for log rehydration.
 
         Permissions will be automatically added to the Datadog integration IAM role.
         https://docs.datadoghq.com/logs/archives/rehydrating/?tab=awss
         '''
         result = self._values.get("log_archives")
-        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_s3.Bucket]], result)
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.Bucket]], result)
 
     @builtins.property
     def permissions(self) -> typing.Optional[builtins.str]:
         '''Customize the permission level for the Datadog IAM role.
 
         Select "Core" to only grant Datadog read-only permissions (not recommended).
 
@@ -718,24 +792,38 @@
         ``analyticsReporting`` setting of containing ``App``, or value of
         'aws:cdk:version-reporting' context key
         '''
         result = self._values.get("analytics_reporting")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def cross_region_references(self) -> typing.Optional[builtins.bool]:
+        '''Enable this flag to allow native cross region stack references.
+
+        Enabling this will create a CloudFormation custom resource
+        in both the producing stack and consuming stack in order to perform the export/import
+
+        This feature is currently experimental
+
+        :default: false
+        '''
+        result = self._values.get("cross_region_references")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A description of the stack.
 
         :default: - No description.
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def env(self) -> typing.Optional[aws_cdk.Environment]:
+    def env(self) -> typing.Optional[_aws_cdk_ceddda9d.Environment]:
         '''The AWS environment (account/region) where this stack will be deployed.
 
         Set the ``region``/``account`` fields of ``env`` to either a concrete value to
         select the indicated environment (recommended for production stacks), or to
         the values of environment variables
         ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment
         depend on the AWS credentials/configuration that the CDK CLI is executed
@@ -794,36 +882,47 @@
             
             // Define an environment-agnostic stack:
             // `.account` and `.region` will resolve to `{ "Ref": "AWS::AccountId" }` and `{ "Ref": "AWS::Region" }` respectively.
             // which will only resolve to actual values by CloudFormation during deployment.
             new MyStack(app, 'Stack1');
         '''
         result = self._values.get("env")
-        return typing.cast(typing.Optional[aws_cdk.Environment], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Environment], result)
+
+    @builtins.property
+    def permissions_boundary(
+        self,
+    ) -> typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary]:
+        '''Options for applying a permissions boundary to all IAM Roles and Users created within this Stage.
+
+        :default: - no permissions boundary is applied
+        '''
+        result = self._values.get("permissions_boundary")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary], result)
 
     @builtins.property
     def stack_name(self) -> typing.Optional[builtins.str]:
         '''Name to deploy the stack with.
 
         :default: - Derived from construct path.
         '''
         result = self._values.get("stack_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def synthesizer(self) -> typing.Optional[aws_cdk.IStackSynthesizer]:
+    def synthesizer(self) -> typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer]:
         '''Synthesis method to use while deploying this stack.
 
         :default:
 
         - ``DefaultStackSynthesizer`` if the ``@aws-cdk/core:newStyleStackSynthesis`` feature flag
         is set, ``LegacyStackSynthesizer`` otherwise.
         '''
         result = self._values.get("synthesizer")
-        return typing.cast(typing.Optional[aws_cdk.IStackSynthesizer], result)
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Stack tags that will be applied to all the taggable resources and the stack itself.
 
         :default: {}
         '''
@@ -855,7 +954,101 @@
     "DatadogIntegration",
     "DatadogIntegrationConfig",
     "DatadogIntegrationStack",
     "DatadogIntegrationStackConfig",
 ]
 
 publication.publish()
+
+def _typecheckingstub__6eef2e92fcef25509de72f7d20eedd3cd3b3fb23cfe569b9b88802bf6c3e597c(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    external_id: builtins.str,
+    additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    forwarder_name: typing.Optional[builtins.str] = None,
+    forwarder_version: typing.Optional[builtins.str] = None,
+    iam_role_name: typing.Optional[builtins.str] = None,
+    install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
+    log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    permissions: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__44fa621160bdd64de013f756d1f25c947b0015b7f2c0120beaea14eed5c3b640(
+    *,
+    api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    external_id: builtins.str,
+    additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    forwarder_name: typing.Optional[builtins.str] = None,
+    forwarder_version: typing.Optional[builtins.str] = None,
+    iam_role_name: typing.Optional[builtins.str] = None,
+    install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
+    log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    permissions: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__82a6b6f80a71ddfdf5adc118127ee2b20923041977d797bc2d0c3ee639fc3a5e(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    external_id: builtins.str,
+    additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    forwarder_name: typing.Optional[builtins.str] = None,
+    forwarder_version: typing.Optional[builtins.str] = None,
+    iam_role_name: typing.Optional[builtins.str] = None,
+    install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
+    log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    permissions: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+    analytics_reporting: typing.Optional[builtins.bool] = None,
+    cross_region_references: typing.Optional[builtins.bool] = None,
+    description: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    stack_name: typing.Optional[builtins.str] = None,
+    synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ead28fadd359def1dfa88cffb1526afb62d1ead36f18794acea0b5f0a9b282e8(
+    *,
+    api_key: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
+    external_id: builtins.str,
+    additional_forwarder_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    additional_integration_role_params: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    cloud_trails: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    forwarder_name: typing.Optional[builtins.str] = None,
+    forwarder_version: typing.Optional[builtins.str] = None,
+    iam_role_name: typing.Optional[builtins.str] = None,
+    install_datadog_policy_macro: typing.Optional[builtins.bool] = None,
+    log_archives: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.Bucket]] = None,
+    permissions: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+    analytics_reporting: typing.Optional[builtins.bool] = None,
+    cross_region_references: typing.Optional[builtins.bool] = None,
+    description: typing.Optional[builtins.str] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    stack_name: typing.Optional[builtins.str] = None,
+    synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    termination_protection: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cdk-datadog-integration-2.0.3/src/cdk_datadog_integration.egg-info/PKG-INFO` & `cdk-datadog-integration-2.1.1/src/cdk_datadog_integration.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-datadog-integration
-Version: 2.0.3
+Version: 2.1.1
 Summary: cdk-datadog-integration
 Home-page: https://github.com/blimmer/cdk-datadog-integration.git
 Author: Ben Limmer
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-datadog-integration.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,21 +49,21 @@
    const app = new cdk.App();
    new MonitoringInfrastructureStack(app, "MonitoringInfrastructure");
    ```
 
    ```python
    import * as cdk from "aws-cdk-lib";
    import * as secrets from "aws-cdk-lib/aws-secretsmanager";
-   import { DatadogIntegrationStack } from "cdk-datadog-integration";
+   import { DatadogIntegration } from "cdk-datadog-integration";
 
    export class MonitoringInfrastructureStack extends cdk.Stack {
      constructor(scope: cdk.App, id: string, props?: cdk.StackProps) {
        super(scope, id, props);
 
-       const datadog = new DatadogIntegrationStack(this, "Datadog", {
+       const datadog = new DatadogIntegration(this, "Datadog", {
          // Generate an ID here: https://app.datadoghq.com/account/settings#integrations/amazon-web-services
          externalId: "",
 
          // Create or lookup a `Secret` that contains your Datadog API Key
          // See https://docs.aws.amazon.com/cdk/api/latest/docs/aws-secretsmanager-readme.html for details on Secrets in CDK
          // Get your API key here: https://app.datadoghq.com/account/settings#api
          apiKey: secrets.Secret.fromSecretNameV2(
@@ -115,9 +115,7 @@
 ## Contributing
 
 PRs are welcome!
 
 ### Releasing
 
 To release, merge your PR to `main`.
-
-
```

