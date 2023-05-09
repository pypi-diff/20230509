# Comparing `tmp/iam_actions-1.2.20230508.tar.gz` & `tmp/iam_actions-1.2.20230509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230508.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230509.tar", max compression
```

## Comparing `iam_actions-1.2.20230508.tar` & `iam_actions-1.2.20230509.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/README.md
--rw-r--r--   0        0        0      228 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/__init__.py
--rw-r--r--   0        0        0  4245819 2023-05-08 02:28:59.335684 iam_actions-1.2.20230508/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-08 02:27:33.922578 iam_actions-1.2.20230508/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545884 2023-05-08 02:28:59.335684 iam_actions-1.2.20230508/iam_actions/policies.json
--rw-r--r--   0        0        0   193571 2023-05-08 02:28:59.335684 iam_actions-1.2.20230508/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529410 2023-05-08 02:28:59.335684 iam_actions-1.2.20230508/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-08 02:29:00.259739 iam_actions-1.2.20230508/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230508/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230508/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/README.md
+-rw-r--r--   0        0        0      228 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4248083 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-09 02:27:11.256299 iam_actions-1.2.20230509/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-09 02:27:11.260299 iam_actions-1.2.20230509/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   546214 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/policies.json
+-rw-r--r--   0        0        0   193734 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529800 2023-05-09 02:28:42.381904 iam_actions-1.2.20230509/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-09 02:28:43.121917 iam_actions-1.2.20230509/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230509/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230509/PKG-INFO
```

### Comparing `iam_actions-1.2.20230508/LICENSE` & `iam_actions-1.2.20230509/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/README.md` & `iam_actions-1.2.20230509/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/actions.json` & `iam_actions-1.2.20230509/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996655805713723%*

 * *Differences: {"'codeguru-security'": "{'GetFindings': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                        "'GetFindings'), ('condition_keys', []), ('description', 'Not Documented "*

 * *                        "by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'customer-verification'": "OrderedDict([('GetCustomerVerificationEligibility', "*

 * *                            "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                            "'GetCustomerVerificationEligibilit […]*

```diff
@@ -24743,14 +24743,22 @@
             "access_level": "Undocumented",
             "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetFindings": {
+            "access_level": "Undocumented",
+            "action": "GetFindings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetScan": {
             "access_level": "Undocumented",
             "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -32696,14 +32704,48 @@
             "action": "ValidateReportDestination",
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
+    "customer-verification": {
+        "CreateCustomerVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "CreateCustomerVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetCustomerVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "GetCustomerVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetCustomerVerificationEligibility": {
+            "access_level": "Undocumented",
+            "action": "GetCustomerVerificationEligibility",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateCustomerVerificationDetails": {
+            "access_level": "Undocumented",
+            "action": "UpdateCustomerVerificationDetails",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "databrew": {
         "BatchDeleteRecipeVersion": {
             "access_level": "Write",
             "action": "BatchDeleteRecipeVersion",
             "condition_keys": [],
             "description": "Grants permission to delete one or more recipe versions",
             "orphan": false,
@@ -73563,14 +73605,22 @@
             "access_level": "List",
             "action": "ListUsageTotals",
             "condition_keys": [],
             "description": "Grants permission to retrieve aggregated usage data for an account",
             "orphan": false,
             "resources": []
         },
+        "SearchVulnerabilities": {
+            "access_level": "Undocumented",
+            "action": "SearchVulnerabilities",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -108450,16 +108500,19 @@
             "resources": [
                 "user"
             ]
         },
         "CreateVPCConnection": {
             "access_level": "Write",
             "action": "CreateVPCConnection",
-            "condition_keys": [],
-            "description": "Grants permission to create a VPC connection",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a vpc connection",
             "orphan": false,
             "resources": []
         },
         "DeleteAccountCustomization": {
             "access_level": "Write",
             "action": "DeleteAccountCustomization",
             "condition_keys": [],
@@ -108687,18 +108740,23 @@
             "resources": [
                 "user"
             ]
         },
         "DeleteVPCConnection": {
             "access_level": "Write",
             "action": "DeleteVPCConnection",
-            "condition_keys": [],
-            "description": "Grants permission to delete a VPC connection",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to delete a vpc connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpcconnection"
+            ]
         },
         "DescribeAccountCustomization": {
             "access_level": "Read",
             "action": "DescribeAccountCustomization",
             "condition_keys": [],
             "description": "Grants permission to describe an account customization for QuickSight account or namespace",
             "orphan": false,
@@ -109014,20 +109072,25 @@
             "description": "Grants permission to describe a QuickSight user given the user name",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "DescribeVPCConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeVPCConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to describe a vpc connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpcconnection"
+            ]
         },
         "GenerateEmbedUrlForAnonymousUser": {
             "access_level": "Write",
             "action": "GenerateEmbedUrlForAnonymousUser",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -109335,18 +109398,21 @@
             "description": "Grants permission to list all of the QuickSight users belonging to this account",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "ListVPCConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListVPCConnections",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to list all vpc connections",
             "orphan": false,
             "resources": []
         },
         "PassDataSet": {
             "access_level": "Read",
             "action": "PassDataSet",
             "condition_keys": [
@@ -109514,15 +109580,16 @@
                 "customization",
                 "dashboard",
                 "dataset",
                 "datasource",
                 "folder",
                 "ingestion",
                 "template",
-                "theme"
+                "theme",
+                "vpcconnection"
             ]
         },
         "Unsubscribe": {
             "access_level": "Write",
             "action": "Unsubscribe",
             "condition_keys": [],
             "description": "Grants permission to unsubscribe from Amazon QuickSight, which permanently deletes all users and their resources from Amazon QuickSight",
@@ -109542,15 +109609,16 @@
                 "customization",
                 "dashboard",
                 "dataset",
                 "datasource",
                 "folder",
                 "ingestion",
                 "template",
-                "theme"
+                "theme",
+                "vpcconnection"
             ]
         },
         "UpdateAccountCustomization": {
             "access_level": "Write",
             "action": "UpdateAccountCustomization",
             "condition_keys": [],
             "description": "Grants permission to update an account customization for QuickSight account or namespace",
@@ -109829,20 +109897,25 @@
             "description": "Grants permission to update an Amazon QuickSight user",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "UpdateVPCConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateVPCConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to update a vpc connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpcconnection"
+            ]
         }
     },
     "ram": {
         "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
             "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
@@ -128167,20 +128240,22 @@
             "description": "Grants permission to enable standards in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
         "BatchGetControlEvaluations": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "BatchGetControlEvaluations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the enablement and compliance status of controls, the findings count for controls, and the overall security score for controls on the Security Hub console",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "hub"
+            ]
         },
         "BatchGetSecurityControls": {
             "access_level": "Read",
             "action": "BatchGetSecurityControls",
             "condition_keys": [],
             "description": "Grants permission to get details about specific security controls identified by ID or ARN",
             "orphan": false,
@@ -128524,20 +128599,22 @@
             "description": "Grants permission to retrieve details for a finding aggregator, which configures finding aggregation across Regions",
             "orphan": false,
             "resources": [
                 "finding-aggregator"
             ]
         },
         "GetFindingHistory": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetFindingHistory",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a list of finding history from Security Hub",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "hub"
+            ]
         },
         "GetFindings": {
             "access_level": "Read",
             "action": "GetFindings",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of findings from Security Hub",
             "orphan": false,
@@ -140886,14 +140963,22 @@
             "condition_keys": [],
             "description": "Grants permission to update a Slack channel configuration for your account",
             "orphan": false,
             "resources": []
         }
     },
     "supportplans": {
+        "CreateSupportPlanSchedule": {
+            "access_level": "Undocumented",
+            "action": "CreateSupportPlanSchedule",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetSupportPlan": {
             "access_level": "Read",
             "action": "GetSupportPlan",
             "condition_keys": [],
             "description": "Grants permission to view details about the current support plan for this AWS account",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230509/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230509/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/generate.py` & `iam_actions-1.2.20230509/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230509/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230509/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/generate/services.py` & `iam_actions-1.2.20230509/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230508/iam_actions/policies.json` & `iam_actions-1.2.20230509/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996881766381766%*

 * *Differences: {"'serviceMap'": "{'Amazon CodeGuru Security': {'Actions': {insert: [(4, 'GetFindings')]}, "*

 * *                 "'ARNFormat': 'arn:aws:codeguru-security:${Region}:${Account}:*', 'ARNRegex': "*

 * *                 "'^arn:aws:codeguru-security:.+:.+:.+', 'HasResource': True}, 'Amazon Connect': "*

 * *                 "{'Actions': {delete: [194]}}, 'Amazon Inspector2': {'Actions': {insert: [(31, "*

 * *                 "'SearchVulnerabilities')]}}, 'AWS Support Plans': {'Actions': {insert: [(0, "*

 * *                 "'CreateSupp […]*

```diff
@@ -2449,14 +2449,24 @@
                 "PutClassicReportPreferences",
                 "PutReportDefinition",
                 "ValidateReportDestination"
             ],
             "HasResource": true,
             "StringPrefix": "cur"
         },
+        "AWS Customer Verification Service": {
+            "Actions": [
+                "CreateCustomerVerificationDetails",
+                "GetCustomerVerificationDetails",
+                "GetCustomerVerificationEligibility",
+                "UpdateCustomerVerificationDetails"
+            ],
+            "HasResource": false,
+            "StringPrefix": "customer-verification"
+        },
         "AWS Data Exchange": {
             "ARNFormat": "arn:aws:dataexchange:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:dataexchange:.+",
             "Actions": [
                 "CancelJob",
                 "CreateAsset",
                 "CreateDataSet",
@@ -8416,14 +8426,15 @@
             "HasResource": false,
             "StringPrefix": "supportapp"
         },
         "AWS Support Plans": {
             "ARNFormat": "^arn:${Partition}:supportplans::${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:${Partition}:supportplans::.+:.+",
             "Actions": [
+                "CreateSupportPlanSchedule",
                 "GetSupportPlan",
                 "GetSupportPlanUpdateStatus",
                 "StartSupportPlanUpdate"
             ],
             "HasResource": false,
             "StringPrefix": "supportplans"
         },
@@ -10844,27 +10855,28 @@
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "Amazon CodeGuru Security": {
-            "ARNFormat": "arn:${Partition}:codeguru-security:${Region}:${Account}:*",
-            "ARNRegex": "^arn:${Partition}:codeguru-security:.+:.+:.+",
+            "ARNFormat": "arn:aws:codeguru-security:${Region}:${Account}:*",
+            "ARNRegex": "^arn:aws:codeguru-security:.+:.+:.+",
             "Actions": [
                 "BatchGetFindings",
                 "CreateScan",
                 "CreateUploadUrl",
                 "DeleteScansByCategory",
+                "GetFindings",
                 "GetScan",
                 "ListFindings",
                 "ListScans",
                 "UpdateAccountConfiguration"
             ],
-            "HasResource": false,
+            "HasResource": true,
             "StringPrefix": "codeguru-security"
         },
         "Amazon CodeWhisperer": {
             "ARNFormat": "arn:aws:codewhisperer:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:codewhisperer:.+:[0-9]+:.+",
             "Actions": [
                 "CreateProfile",
@@ -11398,16 +11410,15 @@
                 "UpdateTrafficDistribution",
                 "UpdateUserHierarchy",
                 "UpdateUserHierarchyGroupName",
                 "UpdateUserHierarchyStructure",
                 "UpdateUserIdentityInfo",
                 "UpdateUserPhoneConfig",
                 "UpdateUserRoutingProfile",
-                "UpdateUserSecurityProfiles",
-                "UpdatedescribeContent"
+                "UpdateUserSecurityProfiles"
             ],
             "HasResource": true,
             "StringPrefix": "connect",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
@@ -14286,14 +14297,15 @@
                 "ListDelegatedAdminAccounts",
                 "ListFilters",
                 "ListFindingAggregations",
                 "ListFindings",
                 "ListMembers",
                 "ListTagsForResource",
                 "ListUsageTotals",
+                "SearchVulnerabilities",
                 "TagResource",
                 "UntagResource",
                 "UpdateConfiguration",
                 "UpdateEc2DeepInspectionConfiguration",
                 "UpdateFilter",
                 "UpdateOrgEc2DeepInspectionConfiguration",
                 "UpdateOrganizationConfiguration"
```

### Comparing `iam_actions-1.2.20230508/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230509/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971291123525761%*

 * *Differences: {"'customer-verification'": 'OrderedDict()',*

 * * "'quicksight'": "{'vpcconnection': OrderedDict([('arn_pattern', "*

 * *                 "'arn:*:quicksight:*:*:vpcConnection/*'), ('condition_keys', "*

 * *                 "'aws:ResourceTag/${TagKey}')])}"}*

```diff
@@ -1484,14 +1484,15 @@
     "controltower": {},
     "cur": {
         "cur": {
             "arn_pattern": "arn:*:cur:*:*:definition/*",
             "condition_keys": null
         }
     },
+    "customer-verification": {},
     "databrew": {
         "Dataset": {
             "arn_pattern": "arn:*:databrew:*:*:dataset/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Job": {
             "arn_pattern": "arn:*:databrew:*:*:job/*",
@@ -4926,14 +4927,18 @@
         "topic": {
             "arn_pattern": "arn:*:quicksight:*:*:topic/*",
             "condition_keys": null
         },
         "user": {
             "arn_pattern": "arn:*:quicksight:*:*:user/*",
             "condition_keys": null
+        },
+        "vpcconnection": {
+            "arn_pattern": "arn:*:quicksight:*:*:vpcConnection/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ram": {},
     "rbin": {
         "rule": {
             "arn_pattern": "arn:*:rbin:*:*:rule/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230508/iam_actions/services.json` & `iam_actions-1.2.20230509/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968119319900046%*

 * *Differences: {"'codeguru-security'": "{'Actions': {insert: [(4, 'GetFindings')]}, 'ARNFormats': "*

 * *                        "['arn:aws:codeguru-security:${Region}:${Account}:*'], 'ARNRegexes': "*

 * *                        "['^arn:aws:codeguru-security:.+:.+:.+'], 'HasResource': True}",*

 * * "'connect'": "{'Actions': {delete: [194]}}",*

 * * "'customer-verification'": "OrderedDict([('Actions', ['CreateCustomerVerificationDetails', "*

 * *                            "'GetCustomerVerificationDetails', "*

 * *                            "'GetCusto […]*

```diff
@@ -3778,31 +3778,32 @@
         "HasResource": true,
         "ServiceNames": [
             "Amazon CodeGuru Reviewer"
         ]
     },
     "codeguru-security": {
         "ARNFormats": [
-            "arn:${Partition}:codeguru-security:${Region}:${Account}:*"
+            "arn:aws:codeguru-security:${Region}:${Account}:*"
         ],
         "ARNRegexes": [
-            "^arn:${Partition}:codeguru-security:.+:.+:.+"
+            "^arn:aws:codeguru-security:.+:.+:.+"
         ],
         "Actions": [
             "BatchGetFindings",
             "CreateScan",
             "CreateUploadUrl",
             "DeleteScansByCategory",
+            "GetFindings",
             "GetScan",
             "ListFindings",
             "ListScans",
             "UpdateAccountConfiguration"
         ],
         "ConditionKeys": [],
-        "HasResource": false,
+        "HasResource": true,
         "ServiceNames": [
             "Amazon CodeGuru Security"
         ]
     },
     "codepipeline": {
         "ARNFormats": [
             "arn:aws:codepipeline:${Region}:${Account}:${PathToPipelineResource}"
@@ -4708,16 +4709,15 @@
             "UpdateTrafficDistribution",
             "UpdateUserHierarchy",
             "UpdateUserHierarchyGroupName",
             "UpdateUserHierarchyStructure",
             "UpdateUserIdentityInfo",
             "UpdateUserPhoneConfig",
             "UpdateUserRoutingProfile",
-            "UpdateUserSecurityProfiles",
-            "UpdatedescribeContent"
+            "UpdateUserSecurityProfiles"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "connect:AttributeType",
             "connect:InstanceId",
@@ -4884,14 +4884,29 @@
         ],
         "ConditionKeys": [],
         "HasResource": true,
         "ServiceNames": [
             "AWS Cost and Usage Report"
         ]
     },
+    "customer-verification": {
+        "ARNFormats": [],
+        "ARNRegexes": [],
+        "Actions": [
+            "CreateCustomerVerificationDetails",
+            "GetCustomerVerificationDetails",
+            "GetCustomerVerificationEligibility",
+            "UpdateCustomerVerificationDetails"
+        ],
+        "ConditionKeys": [],
+        "HasResource": false,
+        "ServiceNames": [
+            "AWS Customer Verification Service"
+        ]
+    },
     "databrew": {
         "ARNFormats": [
             "arn:aws:databrew:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:databrew:.+:.+:.+"
         ],
@@ -10145,14 +10160,15 @@
             "ListDelegatedAdminAccounts",
             "ListFilters",
             "ListFindingAggregations",
             "ListFindings",
             "ListMembers",
             "ListTagsForResource",
             "ListUsageTotals",
+            "SearchVulnerabilities",
             "TagResource",
             "UntagResource",
             "UpdateConfiguration",
             "UpdateEc2DeepInspectionConfiguration",
             "UpdateFilter",
             "UpdateOrgEc2DeepInspectionConfiguration",
             "UpdateOrganizationConfiguration"
@@ -19696,14 +19712,15 @@
         "ARNFormats": [
             "^arn:${Partition}:supportplans::${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:${Partition}:supportplans::.+:.+"
         ],
         "Actions": [
+            "CreateSupportPlanSchedule",
             "GetSupportPlan",
             "GetSupportPlanUpdateStatus",
             "StartSupportPlanUpdate"
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
```

### Comparing `iam_actions-1.2.20230508/pyproject.toml` & `iam_actions-1.2.20230509/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230508"
+version = "1.2.20230509"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230508/setup.py` & `iam_actions-1.2.20230509/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230508',
+    'version': '1.2.20230509',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230508/PKG-INFO` & `iam_actions-1.2.20230509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230508
+Version: 1.2.20230509
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

