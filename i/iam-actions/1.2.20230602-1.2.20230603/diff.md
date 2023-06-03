# Comparing `tmp/iam_actions-1.2.20230602.tar.gz` & `tmp/iam_actions-1.2.20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230602.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230603.tar", max compression
```

## Comparing `iam_actions-1.2.20230602.tar` & `iam_actions-1.2.20230603.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/README.md
--rw-r--r--   0        0        0      228 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/__init__.py
--rw-r--r--   0        0        0  4282803 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-02 02:43:25.531787 iam_actions-1.2.20230602/iam_actions/generate/services.py
--rw-r--r--   0        0        0   551055 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/policies.json
--rw-r--r--   0        0        0   195514 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   534521 2023-06-02 02:45:18.791907 iam_actions-1.2.20230602/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-02 02:45:19.547908 iam_actions-1.2.20230602/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230602/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230602/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/README.md
+-rw-r--r--   0        0        0      228 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4284913 2023-06-03 02:42:07.387619 iam_actions-1.2.20230603/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-03 02:40:21.397250 iam_actions-1.2.20230603/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   551159 2023-06-03 02:42:07.387619 iam_actions-1.2.20230603/iam_actions/policies.json
+-rw-r--r--   0        0        0   195776 2023-06-03 02:42:07.387619 iam_actions-1.2.20230603/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   534622 2023-06-03 02:42:07.387619 iam_actions-1.2.20230603/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-03 02:42:08.171637 iam_actions-1.2.20230603/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230603/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230603/PKG-INFO
```

### Comparing `iam_actions-1.2.20230602/LICENSE` & `iam_actions-1.2.20230603/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/README.md` & `iam_actions-1.2.20230603/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/actions.json` & `iam_actions-1.2.20230603/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998097541344912%*

 * *Differences: {"'athena'": "{'DeleteCapacityReservation': OrderedDict([('access_level', 'Undocumented'), "*

 * *             "('action', 'DeleteCapacityReservation'), ('condition_keys', []), ('description', "*

 * *             "'Not Documented by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'aws-marketplace-management'": "{'uploadFiles': {'description': 'Allows access to the File "*

 * *                                 "Upload page inside the AWS Marketplace Management Portal'}, "*

 * *                                 "'viewMarketing' […]*

```diff
@@ -8189,14 +8189,22 @@
             ],
             "description": "Grants permission to create a workgroup",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
+        "DeleteCapacityReservation": {
+            "access_level": "Undocumented",
+            "action": "DeleteCapacityReservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDataCatalog": {
             "access_level": "Write",
             "action": "DeleteDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to delete a datacatalog",
             "orphan": false,
             "resources": [
@@ -10603,114 +10611,114 @@
             "description": "Grants permission to users to see their account's subscriptions",
             "orphan": false,
             "resources": []
         }
     },
     "aws-marketplace-management": {
         "GetAdditionalSellerNotificationRecipients": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAdditionalSellerNotificationRecipients",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view additional seller notification recipients",
             "orphan": false,
             "resources": []
         },
         "GetBankAccountVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetBankAccountVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view bank account verification status",
             "orphan": false,
             "resources": []
         },
         "GetSecondaryUserVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSecondaryUserVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view secondary user account verification status",
             "orphan": false,
             "resources": []
         },
         "GetSellerVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSellerVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to view account verification status",
             "orphan": false,
             "resources": []
         },
         "PutAdditionalSellerNotificationRecipients": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutAdditionalSellerNotificationRecipients",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update additional seller notification recipients",
             "orphan": false,
             "resources": []
         },
         "PutBankAccountVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutBankAccountVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update bank account verification status",
             "orphan": false,
             "resources": []
         },
         "PutSecondaryUserVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutSecondaryUserVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update secondary user account verification status",
             "orphan": false,
             "resources": []
         },
         "PutSellerVerificationDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutSellerVerificationDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update account verification status",
             "orphan": false,
             "resources": []
         },
         "uploadFiles": {
             "access_level": "Write",
             "action": "uploadFiles",
             "condition_keys": [],
-            "description": "Allows access to the File Upload page inside the AWS Marketplace Management Portal.",
+            "description": "Allows access to the File Upload page inside the AWS Marketplace Management Portal",
             "orphan": false,
             "resources": []
         },
         "viewMarketing": {
             "access_level": "List",
             "action": "viewMarketing",
             "condition_keys": [],
-            "description": "Allows access to the Marketing page inside the AWS Marketplace Management Portal.",
+            "description": "Allows access to the Marketing page inside the AWS Marketplace Management Portal",
             "orphan": false,
             "resources": []
         },
         "viewReports": {
             "access_level": "List",
             "action": "viewReports",
             "condition_keys": [],
-            "description": "Allows access to the Reports page inside the AWS Marketplace Management Portal.",
+            "description": "Allows access to the Reports page inside the AWS Marketplace Management Portal",
             "orphan": false,
             "resources": []
         },
         "viewSettings": {
             "access_level": "List",
             "action": "viewSettings",
             "condition_keys": [],
-            "description": "Allows access to the Settings page inside the AWS Marketplace Management Portal.",
+            "description": "Allows access to the Settings page inside the AWS Marketplace Management Portal",
             "orphan": false,
             "resources": []
         },
         "viewSupport": {
             "access_level": "List",
             "action": "viewSupport",
             "condition_keys": [],
-            "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal.",
+            "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal",
             "orphan": false,
             "resources": []
         }
     },
     "aws-portal": {
         "GetConsoleActionSetEnforced": {
             "access_level": "Read",
@@ -21490,14 +21498,22 @@
             "condition_keys": [],
             "description": "Grants permission to restore an event data store",
             "orphan": false,
             "resources": [
                 "eventdatastore"
             ]
         },
+        "StartEventDataStoreIngestion": {
+            "access_level": "Undocumented",
+            "action": "StartEventDataStoreIngestion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartImport": {
             "access_level": "Write",
             "action": "StartImport",
             "condition_keys": [],
             "description": "Grants permission to start an import of logged trail events from a source S3 bucket to a destination event data store",
             "orphan": false,
             "resources": []
@@ -21518,14 +21534,22 @@
             "condition_keys": [],
             "description": "Grants permission to start a new query on a specified event data store",
             "orphan": false,
             "resources": [
                 "eventdatastore"
             ]
         },
+        "StopEventDataStoreIngestion": {
+            "access_level": "Undocumented",
+            "action": "StopEventDataStoreIngestion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopImport": {
             "access_level": "Write",
             "action": "StopImport",
             "condition_keys": [],
             "description": "Grants permission to stop a specified import",
             "orphan": false,
             "resources": []
@@ -38683,19 +38707,21 @@
                 "aws:TagKeys",
                 "dms:req-tag/${TagKey}"
             ],
             "description": "Grants permission to add metadata tags to DMS resources, including replication instances, endpoints, security groups, and migration tasks",
             "orphan": false,
             "resources": [
                 "Certificate",
+                "DataMigration",
                 "DataProvider",
                 "Endpoint",
                 "EventSubscription",
                 "InstanceProfile",
                 "MigrationProject",
+                "ReplicationConfig",
                 "ReplicationInstance",
                 "ReplicationSubnetGroup",
                 "ReplicationTask"
             ]
         },
         "ApplyPendingMaintenanceAction": {
             "access_level": "Write",
@@ -38762,20 +38788,26 @@
             "description": "Grants permission to cancel a single premigration assessment run",
             "orphan": false,
             "resources": [
                 "ReplicationTaskAssessmentRun"
             ]
         },
         "CreateDataMigration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateDataMigration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "dms:req-tag/${TagKey}"
+            ],
+            "description": "Grants permission to create a database migration using the provided settings",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "MigrationProject"
+            ]
         },
         "CreateDataProvider": {
             "access_level": "Write",
             "action": "CreateDataProvider",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -38841,20 +38873,26 @@
             "orphan": false,
             "resources": [
                 "DataProvider",
                 "InstanceProfile"
             ]
         },
         "CreateReplicationConfig": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateReplicationConfig",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "dms:req-tag/${TagKey}"
+            ],
+            "description": "Grants permission to create a replication config using the provided settings",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "Endpoint"
+            ]
         },
         "CreateReplicationInstance": {
             "access_level": "Write",
             "action": "CreateReplicationInstance",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -38909,20 +38947,22 @@
             "orphan": false,
             "resources": [
                 "Endpoint",
                 "ReplicationInstance"
             ]
         },
         "DeleteDataMigration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteDataMigration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete the specified database migration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "DataMigration"
+            ]
         },
         "DeleteDataProvider": {
             "access_level": "Write",
             "action": "DeleteDataProvider",
             "condition_keys": [],
             "description": "Grants permission to delete the specified data provider",
             "orphan": false,
@@ -38983,20 +39023,22 @@
             "description": "Grants permission to delete the specified migration project",
             "orphan": false,
             "resources": [
                 "MigrationProject"
             ]
         },
         "DeleteReplicationConfig": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteReplicationConfig",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete the specified replication config",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "DeleteReplicationInstance": {
             "access_level": "Write",
             "action": "DeleteReplicationInstance",
             "condition_keys": [],
             "description": "Grants permission to delete the specified replication instance",
             "orphan": false,
@@ -39066,18 +39108,18 @@
             "action": "DescribeConnections",
             "condition_keys": [],
             "description": "Grants permission to describe the status of the connections that have been made between the replication instance and an endpoint",
             "orphan": false,
             "resources": []
         },
         "DescribeDataMigrations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeDataMigrations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return information about database migrations for your account in the specified region",
             "orphan": false,
             "resources": []
         },
         "DescribeEndpointSettings": {
             "access_level": "Read",
             "action": "DescribeEndpointSettings",
             "condition_keys": [],
@@ -39204,18 +39246,18 @@
             "description": "Grants permission to returns the status of the RefreshSchemas operation",
             "orphan": false,
             "resources": [
                 "Endpoint"
             ]
         },
         "DescribeReplicationConfigs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeReplicationConfigs",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe replication configs",
             "orphan": false,
             "resources": []
         },
         "DescribeReplicationInstanceTaskLogs": {
             "access_level": "Read",
             "action": "DescribeReplicationInstanceTaskLogs",
             "condition_keys": [
@@ -39241,20 +39283,22 @@
             "action": "DescribeReplicationSubnetGroups",
             "condition_keys": [],
             "description": "Grants permission to return information about the replication subnet groups",
             "orphan": false,
             "resources": []
         },
         "DescribeReplicationTableStatistics": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeReplicationTableStatistics",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe replication table statistics",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "DescribeReplicationTaskAssessmentResults": {
             "access_level": "Read",
             "action": "DescribeReplicationTaskAssessmentResults",
             "condition_keys": [],
             "description": "Grants permission to return the latest task assessment results from Amazon S3",
             "orphan": false,
@@ -39290,18 +39334,18 @@
             "action": "DescribeReplicationTasks",
             "condition_keys": [],
             "description": "Grants permission to return information about replication tasks for your account in the current region",
             "orphan": false,
             "resources": []
         },
         "DescribeReplications": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeReplications",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe replications",
             "orphan": false,
             "resources": []
         },
         "DescribeSchemas": {
             "access_level": "Read",
             "action": "DescribeSchemas",
             "condition_keys": [],
@@ -39448,28 +39492,35 @@
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list all tags for an AWS DMS resource",
             "orphan": false,
             "resources": [
                 "Certificate",
+                "DataMigration",
+                "DataProvider",
                 "Endpoint",
                 "EventSubscription",
+                "InstanceProfile",
+                "MigrationProject",
+                "ReplicationConfig",
                 "ReplicationInstance",
                 "ReplicationSubnetGroup",
                 "ReplicationTask"
             ]
         },
         "ModifyDataMigration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyDataMigration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to modify the specified database migration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "DataMigration"
+            ]
         },
         "ModifyEndpoint": {
             "access_level": "Write",
             "action": "ModifyEndpoint",
             "condition_keys": [],
             "description": "Grants permission to modify the specified endpoint",
             "orphan": false,
@@ -39499,20 +39550,22 @@
             "action": "ModifyFleetAdvisorCollectorStatuses",
             "condition_keys": [],
             "description": "Grants permission to modify the status of the specified Fleet Advisor collector",
             "orphan": false,
             "resources": []
         },
         "ModifyReplicationConfig": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyReplicationConfig",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to modify the specified replication config",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "ModifyReplicationInstance": {
             "access_level": "Write",
             "action": "ModifyReplicationInstance",
             "condition_keys": [],
             "description": "Grants permission to modify the replication instance to apply new settings",
             "orphan": false,
@@ -39567,20 +39620,22 @@
             "orphan": false,
             "resources": [
                 "Endpoint",
                 "ReplicationInstance"
             ]
         },
         "ReloadReplicationTables": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ReloadReplicationTables",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to reload the target database table with the source for a replication",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "ReloadTables": {
             "access_level": "Write",
             "action": "ReloadTables",
             "condition_keys": [],
             "description": "Grants permission to reload the target database table with the source data",
             "orphan": false,
@@ -39594,39 +39649,43 @@
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove metadata tags from a DMS resource",
             "orphan": false,
             "resources": [
                 "Certificate",
+                "DataMigration",
                 "DataProvider",
                 "Endpoint",
                 "EventSubscription",
                 "InstanceProfile",
                 "MigrationProject",
+                "ReplicationConfig",
                 "ReplicationInstance",
                 "ReplicationSubnetGroup",
                 "ReplicationTask"
             ]
         },
         "RunFleetAdvisorLsaAnalysis": {
             "access_level": "Write",
             "action": "RunFleetAdvisorLsaAnalysis",
             "condition_keys": [],
             "description": "Grants permission to run a large-scale assessment (LSA) analysis on every Fleet Advisor collector in your account",
             "orphan": false,
             "resources": []
         },
         "StartDataMigration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartDataMigration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start the database migration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "DataMigration"
+            ]
         },
         "StartMetadataModelAssessment": {
             "access_level": "Write",
             "action": "StartMetadataModelAssessment",
             "condition_keys": [],
             "description": "Grants permission to start a new assessment of metadata model",
             "orphan": false,
@@ -39679,20 +39738,22 @@
             "action": "StartRecommendations",
             "condition_keys": [],
             "description": "Grants permission to start the analysis of your source database to provide recommendations of target engines",
             "orphan": false,
             "resources": []
         },
         "StartReplication": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartReplication",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start a replication",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "StartReplicationTask": {
             "access_level": "Write",
             "action": "StartReplicationTask",
             "condition_keys": [],
             "description": "Grants permission to start the replication task",
             "orphan": false,
@@ -39717,28 +39778,32 @@
             "description": "Grants permission to start a new premigration assessment run for one or more individual assessments of a migration task",
             "orphan": false,
             "resources": [
                 "ReplicationTask"
             ]
         },
         "StopDataMigration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopDataMigration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to stop the database migration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "DataMigration"
+            ]
         },
         "StopReplication": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StopReplication",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to stop a replication",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "ReplicationConfig"
+            ]
         },
         "StopReplicationTask": {
             "access_level": "Write",
             "action": "StopReplicationTask",
             "condition_keys": [],
             "description": "Grants permission to stop the replication task",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230603/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230603/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/generate.py` & `iam_actions-1.2.20230603/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230603/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230603/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/generate/services.py` & `iam_actions-1.2.20230603/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230602/iam_actions/policies.json` & `iam_actions-1.2.20230603/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999994064053945%*

 * *Differences: {"'serviceMap'": "{'Amazon Athena': {'Actions': {insert: [(11, 'DeleteCapacityReservation')]}}, "*

 * *                 "'AWS CloudTrail': {'Actions': {insert: [(40, 'StartEventDataStoreIngestion'), "*

 * *                 "(44, 'StopEventDataStoreIngestion')]}}}"}*

```diff
@@ -1650,17 +1650,19 @@
                 "LookupEvents",
                 "PutEventSelectors",
                 "PutInsightSelectors",
                 "PutResourcePolicy",
                 "RegisterOrganizationDelegatedAdmin",
                 "RemoveTags",
                 "RestoreEventDataStore",
+                "StartEventDataStoreIngestion",
                 "StartImport",
                 "StartLogging",
                 "StartQuery",
+                "StopEventDataStoreIngestion",
                 "StopImport",
                 "StopLogging",
                 "UpdateChannel",
                 "UpdateEventDataStore",
                 "UpdateServiceLinkedChannel",
                 "UpdateTrail"
             ],
@@ -9918,14 +9920,15 @@
                 "CreateCapacityReservation",
                 "CreateDataCatalog",
                 "CreateNamedQuery",
                 "CreateNotebook",
                 "CreatePreparedStatement",
                 "CreatePresignedNotebookUrl",
                 "CreateWorkGroup",
+                "DeleteCapacityReservation",
                 "DeleteDataCatalog",
                 "DeleteNamedQuery",
                 "DeleteNotebook",
                 "DeletePreparedStatement",
                 "DeleteWorkGroup",
                 "ExportNotebook",
                 "GetCalculationExecution",
```

### Comparing `iam_actions-1.2.20230602/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230603/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997863247863248%*

 * *Differences: {"'dms'": "{'DataMigration': OrderedDict([('arn_pattern', 'arn:*:dms:*:*:data-migration:*'), "*

 * *          "('condition_keys', 'aws:ResourceTag/${TagKey}')]), 'ReplicationConfig': "*

 * *          "OrderedDict([('arn_pattern', 'arn:*:dms:*:*:replication-config:*'), ('condition_keys', "*

 * *          "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -1768,14 +1768,18 @@
         }
     },
     "dms": {
         "Certificate": {
             "arn_pattern": "arn:*:dms:*:*:cert:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "DataMigration": {
+            "arn_pattern": "arn:*:dms:*:*:data-migration:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "DataProvider": {
             "arn_pattern": "arn:*:dms:*:*:data-provider:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Endpoint": {
             "arn_pattern": "arn:*:dms:*:*:endpoint:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -1788,14 +1792,18 @@
             "arn_pattern": "arn:*:dms:*:*:instance-profile:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "MigrationProject": {
             "arn_pattern": "arn:*:dms:*:*:migration-project:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "ReplicationConfig": {
+            "arn_pattern": "arn:*:dms:*:*:replication-config:*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "ReplicationInstance": {
             "arn_pattern": "arn:*:dms:*:*:rep:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "ReplicationSubnetGroup": {
             "arn_pattern": "arn:*:dms:*:*:subgrp:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230602/iam_actions/services.json` & `iam_actions-1.2.20230603/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999937837453822%*

 * *Differences: {"'athena'": "{'Actions': {insert: [(11, 'DeleteCapacityReservation')]}}",*

 * * "'cloudtrail'": "{'Actions': {insert: [(40, 'StartEventDataStoreIngestion'), (44, "*

 * *                 "'StopEventDataStoreIngestion')]}}"}*

```diff
@@ -1323,14 +1323,15 @@
             "CreateCapacityReservation",
             "CreateDataCatalog",
             "CreateNamedQuery",
             "CreateNotebook",
             "CreatePreparedStatement",
             "CreatePresignedNotebookUrl",
             "CreateWorkGroup",
+            "DeleteCapacityReservation",
             "DeleteDataCatalog",
             "DeleteNamedQuery",
             "DeleteNotebook",
             "DeletePreparedStatement",
             "DeleteWorkGroup",
             "ExportNotebook",
             "GetCalculationExecution",
@@ -3252,17 +3253,19 @@
             "LookupEvents",
             "PutEventSelectors",
             "PutInsightSelectors",
             "PutResourcePolicy",
             "RegisterOrganizationDelegatedAdmin",
             "RemoveTags",
             "RestoreEventDataStore",
+            "StartEventDataStoreIngestion",
             "StartImport",
             "StartLogging",
             "StartQuery",
+            "StopEventDataStoreIngestion",
             "StopImport",
             "StopLogging",
             "UpdateChannel",
             "UpdateEventDataStore",
             "UpdateServiceLinkedChannel",
             "UpdateTrail"
         ],
```

### Comparing `iam_actions-1.2.20230602/pyproject.toml` & `iam_actions-1.2.20230603/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230602"
+version = "1.2.20230603"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230602/setup.py` & `iam_actions-1.2.20230603/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230602',
+    'version': '1.2.20230603',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230602/PKG-INFO` & `iam_actions-1.2.20230603/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230602
+Version: 1.2.20230603
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

