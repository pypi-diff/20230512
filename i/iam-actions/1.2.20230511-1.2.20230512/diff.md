# Comparing `tmp/iam_actions-1.2.20230511.tar.gz` & `tmp/iam_actions-1.2.20230512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230511.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230512.tar", max compression
```

## Comparing `iam_actions-1.2.20230511.tar` & `iam_actions-1.2.20230512.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-11 02:25:10.114679 iam_actions-1.2.20230511/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/README.md
--rw-r--r--   0        0        0      228 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/__init__.py
--rw-r--r--   0        0        0  4251216 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-11 02:25:10.118679 iam_actions-1.2.20230511/iam_actions/generate/services.py
--rw-r--r--   0        0        0   546752 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/policies.json
--rw-r--r--   0        0        0   193758 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   530388 2023-05-11 02:26:45.768498 iam_actions-1.2.20230511/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-11 02:26:46.508512 iam_actions-1.2.20230511/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230511/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230511/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/README.md
+-rw-r--r--   0        0        0      228 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4252634 2023-05-12 02:26:03.608984 iam_actions-1.2.20230512/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-12 02:24:01.492382 iam_actions-1.2.20230512/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   546779 2023-05-12 02:26:03.608984 iam_actions-1.2.20230512/iam_actions/policies.json
+-rw-r--r--   0        0        0   193791 2023-05-12 02:26:03.608984 iam_actions-1.2.20230512/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   530414 2023-05-12 02:26:03.608984 iam_actions-1.2.20230512/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-12 02:26:04.456988 iam_actions-1.2.20230512/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230512/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230512/PKG-INFO
```

### Comparing `iam_actions-1.2.20230511/LICENSE` & `iam_actions-1.2.20230512/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/README.md` & `iam_actions-1.2.20230512/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/actions.json` & `iam_actions-1.2.20230512/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999176280411491%*

 * *Differences: {"'memorydb'": "{'Connect': {'access_level': 'Write', 'condition_keys': "*

 * *               "['aws:ResourceTag/${TagKey}'], 'description': 'Allows an IAM user or role to "*

 * *               "connect as a specified MemoryDB user to a node in a cluster', 'resources': "*

 * *               "['cluster', 'user']}}",*

 * * "'mq'": "{'CreateReplicaBroker': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *         "'CreateReplicaBroker'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *         "AWS'), ('or […]*

```diff
@@ -95300,20 +95300,25 @@
             "description": "Grants permissions to apply service updates",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
         "Connect": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "Connect",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}"
+            ],
+            "description": "Allows an IAM user or role to connect as a specified MemoryDB user to a node in a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster",
+                "user"
+            ]
         },
         "CopySnapshot": {
             "access_level": "Write",
             "action": "CopySnapshot",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
@@ -99115,14 +99120,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a new configuration for the specified configuration name. Amazon MQ uses the default configuration (the engine type and engine version)",
             "orphan": false,
             "resources": []
         },
+        "CreateReplicaBroker": {
+            "access_level": "Undocumented",
+            "action": "CreateReplicaBroker",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateTags": {
             "access_level": "Tagging",
             "action": "CreateTags",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -108483,28 +108496,35 @@
             "description": "Grants permission to create an alias for a theme version",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
         "CreateTopic": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTopic",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "CreateTopicRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateTopicRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a refresh schedule for a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [],
             "description": "Grants permission to provision Amazon QuickSight authors and readers",
             "orphan": false,
@@ -108729,28 +108749,35 @@
             "description": "Grants permission to delete the alias of a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
         "DeleteTopic": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTopic",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to delete a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DeleteTopicRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteTopicRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a refresh schedule for a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DeleteUser": {
             "access_level": "Write",
             "action": "DeleteUser",
             "condition_keys": [],
             "description": "Grants permission to delete a QuickSight user, given the user name",
             "orphan": false,
@@ -109089,44 +109116,61 @@
             "description": "Grants permission to describe permissions for a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
         "DescribeTopic": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeTopic",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to describe a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DescribeTopicPermissions": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "DescribeTopicPermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to describe the resource policy of a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DescribeTopicRefresh": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeTopicRefresh",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to describe the refresh status of a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DescribeTopicRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeTopicRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a refresh schedule for a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "DescribeUser": {
             "access_level": "Read",
             "action": "DescribeUser",
             "condition_keys": [],
             "description": "Grants permission to describe a QuickSight user given the user name",
             "orphan": false,
@@ -109373,15 +109417,16 @@
             "description": "Grants permission to list tags of a QuickSight resource",
             "orphan": false,
             "resources": [
                 "customization",
                 "dashboard",
                 "folder",
                 "template",
-                "theme"
+                "theme",
+                "topic"
             ]
         },
         "ListTemplateAliases": {
             "access_level": "List",
             "action": "ListTemplateAliases",
             "condition_keys": [],
             "description": "Grants permission to list all aliases for a template",
@@ -109437,26 +109482,29 @@
             "description": "Grants permission to list all themes in an account",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
         "ListTopicRefreshSchedules": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListTopicRefreshSchedules",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all refresh schedules on a topic",
             "orphan": false,
             "resources": []
         },
         "ListTopics": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListTopics",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to list all topics",
             "orphan": false,
             "resources": []
         },
         "ListUserGroups": {
             "access_level": "List",
             "action": "ListUserGroups",
             "condition_keys": [],
@@ -109656,14 +109704,15 @@
                 "dashboard",
                 "dataset",
                 "datasource",
                 "folder",
                 "ingestion",
                 "template",
                 "theme",
+                "topic",
                 "vpcconnection"
             ]
         },
         "Unsubscribe": {
             "access_level": "Write",
             "action": "Unsubscribe",
             "condition_keys": [],
@@ -109685,14 +109734,15 @@
                 "dashboard",
                 "dataset",
                 "datasource",
                 "folder",
                 "ingestion",
                 "template",
                 "theme",
+                "topic",
                 "vpcconnection"
             ]
         },
         "UpdateAccountCustomization": {
             "access_level": "Write",
             "action": "UpdateAccountCustomization",
             "condition_keys": [],
@@ -109962,36 +110012,49 @@
             "description": "Grants permission to update permissions for a theme",
             "orphan": false,
             "resources": [
                 "theme"
             ]
         },
         "UpdateTopic": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateTopic",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to update a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset",
+                "topic"
+            ]
         },
         "UpdateTopicPermissions": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "UpdateTopicPermissions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to update the resource policy of a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "UpdateTopicRefreshSchedule": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateTopicRefreshSchedule",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a refresh schedule for a topic",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "topic"
+            ]
         },
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update an Amazon QuickSight user",
             "orphan": false,
@@ -136912,25 +136975,30 @@
             "resources": [
                 "association"
             ]
         },
         "StartAutomationExecution": {
             "access_level": "Write",
             "action": "StartAutomationExecution",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to initiate the execution of an Automation document",
             "orphan": false,
             "resources": [
                 "automation-definition"
             ]
         },
         "StartChangeRequestExecution": {
             "access_level": "Write",
             "action": "StartChangeRequestExecution",
             "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
                 "ssm:AutoApprove"
             ],
             "description": "Grants permission to initiate the execution of an Automation Change Template document",
             "orphan": false,
             "resources": [
                 "automation-definition"
             ]
```

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230512/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230512/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/generate.py` & `iam_actions-1.2.20230512/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230512/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230512/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/generate/services.py` & `iam_actions-1.2.20230512/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230511/iam_actions/policies.json` & `iam_actions-1.2.20230512/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999995181930311%*

 * *Differences: {"'serviceMap'": "{'Amazon MQ': {'Actions': {insert: [(2, 'CreateReplicaBroker')]}}}"}*

```diff
@@ -15256,14 +15256,15 @@
         },
         "Amazon MQ": {
             "ARNFormat": "arn:aws:mq:${Region}:${Account}:.+",
             "ARNRegex": "^arn:aws:mq:.+",
             "Actions": [
                 "CreateBroker",
                 "CreateConfiguration",
+                "CreateReplicaBroker",
                 "CreateTags",
                 "CreateUser",
                 "DeleteBroker",
                 "DeleteTags",
                 "DeleteUser",
                 "DescribeBroker",
                 "DescribeBrokerEngineTypes",
```

### Comparing `iam_actions-1.2.20230511/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230512/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999322965026306%*

 * *Differences: {"'aws-marketplace'": "{'SellerDashboard': {'arn_pattern': "*

 * *                      "'arn:*:aws-marketplace::*:*/ReportingData/*/Dashboard/*'}}",*

 * * "'quicksight'": "{'topic': {'condition_keys': 'aws:ResourceTag/${TagKey}'}}"}*

```diff
@@ -715,15 +715,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Entity": {
             "arn_pattern": "arn:*:aws-marketplace:*:*:*/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "SellerDashboard": {
-            "arn_pattern": "arn:*:aws-marketplace::*:*/SellerDashboard/*",
+            "arn_pattern": "arn:*:aws-marketplace::*:*/ReportingData/*/Dashboard/*",
             "condition_keys": null
         }
     },
     "aws-marketplace-management": {},
     "aws-portal": {},
     "awsconnector": {},
     "backup": {
@@ -4922,15 +4922,15 @@
         },
         "theme": {
             "arn_pattern": "arn:*:quicksight:*:*:theme/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "topic": {
             "arn_pattern": "arn:*:quicksight:*:*:topic/*",
-            "condition_keys": null
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "user": {
             "arn_pattern": "arn:*:quicksight:*:*:user/*",
             "condition_keys": null
         },
         "vpcconnection": {
             "arn_pattern": "arn:*:quicksight:*:*:vpcConnection/*",
```

### Comparing `iam_actions-1.2.20230511/iam_actions/services.json` & `iam_actions-1.2.20230512/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999949537765936%*

 * *Differences: {"'mq'": "{'Actions': {insert: [(2, 'CreateReplicaBroker')]}}"}*

```diff
@@ -13897,14 +13897,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:mq:.+"
         ],
         "Actions": [
             "CreateBroker",
             "CreateConfiguration",
+            "CreateReplicaBroker",
             "CreateTags",
             "CreateUser",
             "DeleteBroker",
             "DeleteTags",
             "DeleteUser",
             "DescribeBroker",
             "DescribeBrokerEngineTypes",
```

### Comparing `iam_actions-1.2.20230511/pyproject.toml` & `iam_actions-1.2.20230512/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230511"
+version = "1.2.20230512"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230511/setup.py` & `iam_actions-1.2.20230512/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230511',
+    'version': '1.2.20230512',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230511/PKG-INFO` & `iam_actions-1.2.20230512/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230511
+Version: 1.2.20230512
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

