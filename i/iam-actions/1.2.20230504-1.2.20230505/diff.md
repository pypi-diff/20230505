# Comparing `tmp/iam_actions-1.2.20230504.tar.gz` & `tmp/iam_actions-1.2.20230505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230504.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230505.tar", max compression
```

## Comparing `iam_actions-1.2.20230504.tar` & `iam_actions-1.2.20230505.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/README.md
--rw-r--r--   0        0        0      228 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/__init__.py
--rw-r--r--   0        0        0  4244539 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-04 02:24:47.538830 iam_actions-1.2.20230504/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545679 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/policies.json
--rw-r--r--   0        0        0   193569 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529212 2023-05-04 02:26:18.987745 iam_actions-1.2.20230504/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-04 02:26:19.727753 iam_actions-1.2.20230504/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230504/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230504/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/README.md
+-rw-r--r--   0        0        0      228 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4244693 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545743 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/policies.json
+-rw-r--r--   0        0        0   193571 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529274 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-05 02:25:20.072179 iam_actions-1.2.20230505/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230505/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230505/PKG-INFO
```

### Comparing `iam_actions-1.2.20230504/LICENSE` & `iam_actions-1.2.20230505/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/README.md` & `iam_actions-1.2.20230505/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/actions.json` & `iam_actions-1.2.20230505/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999929468904292%*

 * *Differences: {"'ivschat'": "{'TagResource': {'resources': {insert: [(0, 'Logging-Configuration')]}}, "*

 * *              "'UntagResource': {'resources': {insert: [(0, 'Logging-Configuration')]}}}",*

 * * "'mediaconnect'": "{'UpdateGatewayInstance': {'access_level': 'Write', 'description': 'Grants "*

 * *                   "permission to update the configuration of an existing Gateway Instance', "*

 * *                   "'resources': ['GatewayInstance']}}",*

 * * "'sso'": "{'CreatePermissionSet': {'resources': {insert: [(1, 'PermissionSet')]}} […]*

```diff
@@ -81580,26 +81580,28 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to add or update tags for a resource with a specified ARN",
             "orphan": false,
             "resources": [
+                "Logging-Configuration",
                 "Room"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags for a resource with a specified ARN",
             "orphan": false,
             "resources": [
+                "Logging-Configuration",
                 "Room"
             ]
         },
         "UpdateLoggingConfiguration": {
             "access_level": "Write",
             "action": "UpdateLoggingConfiguration",
             "condition_keys": [],
@@ -93228,20 +93230,22 @@
             "action": "UpdateFlowSource",
             "condition_keys": [],
             "description": "Grants permission to update the source of any flow",
             "orphan": false,
             "resources": []
         },
         "UpdateGatewayInstance": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateGatewayInstance",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the configuration of an existing Gateway Instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "GatewayInstance"
+            ]
         }
     },
     "mediaconvert": {
         "AssociateCertificate": {
             "access_level": "Write",
             "action": "AssociateCertificate",
             "condition_keys": [],
@@ -137972,15 +137976,16 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a permission set",
             "orphan": false,
             "resources": [
-                "Instance"
+                "Instance",
+                "PermissionSet"
             ]
         },
         "CreateProfile": {
             "access_level": "Write",
             "action": "CreateProfile",
             "condition_keys": [],
             "description": "Grants permission to create a profile for an application instance",
```

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230505/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230505/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/generate.py` & `iam_actions-1.2.20230505/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230505/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230505/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/generate/services.py` & `iam_actions-1.2.20230505/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230504/iam_actions/policies.json` & `iam_actions-1.2.20230505/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999956232492998%*

 * *Differences: {"'serviceMap'": "{'Amazon Elastic File System': {'conditionKeys': {insert: [(5, "*

 * *                 "'elasticfilesystem:CreateAction')]}}, 'AWS AppSync': {'conditionKeys': {insert: "*

 * *                 "[(0, 'appsync:Visibility')]}}}"}*

```diff
@@ -598,14 +598,15 @@
                 "UpdateGraphqlApi",
                 "UpdateResolver",
                 "UpdateType"
             ],
             "HasResource": true,
             "StringPrefix": "appsync",
             "conditionKeys": [
+                "appsync:Visibility",
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "AWS Application Auto Scaling": {
             "ARNFormat": "arn:aws:application-autoscaling:${Region}:${Account}:${RelativeId}",
@@ -13209,14 +13210,15 @@
             "StringPrefix": "elasticfilesystem",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "elasticfilesystem:AccessPointArn",
                 "elasticfilesystem:AccessedViaMountTarget",
+                "elasticfilesystem:CreateAction",
                 "elasticfilesystem:Encrypted"
             ]
         },
         "Amazon Elastic Inference": {
             "ARNFormat": "arn:aws:elastic-inference:<region>:<account-id>:elastic-inference-accelerator/<identifier>",
             "ARNRegex": "^arn:aws:elastic-inference:.+",
             "Actions": [
```

### Comparing `iam_actions-1.2.20230504/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230505/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997811624649859%*

 * *Differences: {"'auditmanager'": "{'assessmentControlSet': {'arn_pattern': "*

 * *                   "'arn:*:auditmanager:*:*:assessment/*/controlSet/*'}}",*

 * * "'ivschat'": "{'Room': {'arn_pattern': 'arn:*:ivschat:*:*:room/*'}, 'Logging-Configuration': "*

 * *              "{'arn_pattern': 'arn:*:ivschat:*:*:logging-configuration/*'}}"}*

```diff
@@ -682,15 +682,15 @@
     },
     "auditmanager": {
         "assessment": {
             "arn_pattern": "arn:*:auditmanager:*:*:assessment/*",
             "condition_keys": null
         },
         "assessmentControlSet": {
-            "arn_pattern": "arn:*:auditmanager:*:*:assessment/*/ControlSet/*",
+            "arn_pattern": "arn:*:auditmanager:*:*:assessment/*/controlSet/*",
             "condition_keys": null
         },
         "assessmentFramework": {
             "arn_pattern": "arn:*:auditmanager:*:*:assessmentFramework/*",
             "condition_keys": null
         },
         "control": {
@@ -3619,19 +3619,19 @@
         "Stream-Key": {
             "arn_pattern": "arn:*:ivs:*:*:stream-key/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "ivschat": {
         "Logging-Configuration": {
-            "arn_pattern": "arn:*:ivschat::*:logging-configuration/*",
+            "arn_pattern": "arn:*:ivschat:*:*:logging-configuration/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "Room": {
-            "arn_pattern": "arn:*:ivschat::*:room/*",
+            "arn_pattern": "arn:*:ivschat:*:*:room/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "kafka": {
         "cluster": {
             "arn_pattern": "arn:*:kafka:*:*:cluster/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230504/iam_actions/services.json` & `iam_actions-1.2.20230505/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999954148325997%*

 * *Differences: {"'appsync'": "{'ConditionKeys': {insert: [(0, 'appsync:Visibility')]}}",*

 * * "'elasticfilesystem'": "{'ConditionKeys': {insert: [(5, 'elasticfilesystem:CreateAction')]}}"}*

```diff
@@ -1165,14 +1165,15 @@
             "UpdateDomainName",
             "UpdateFunction",
             "UpdateGraphqlApi",
             "UpdateResolver",
             "UpdateType"
         ],
         "ConditionKeys": [
+            "appsync:Visibility",
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS AppSync"
@@ -7470,14 +7471,15 @@
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "elasticfilesystem:AccessPointArn",
             "elasticfilesystem:AccessedViaMountTarget",
+            "elasticfilesystem:CreateAction",
             "elasticfilesystem:Encrypted"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Elastic File System"
         ]
     },
```

### Comparing `iam_actions-1.2.20230504/pyproject.toml` & `iam_actions-1.2.20230505/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230504"
+version = "1.2.20230505"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230504/setup.py` & `iam_actions-1.2.20230505/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230504',
+    'version': '1.2.20230505',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230504/PKG-INFO` & `iam_actions-1.2.20230505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230504
+Version: 1.2.20230505
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

