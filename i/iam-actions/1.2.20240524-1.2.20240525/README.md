# Comparing `tmp/iam_actions-1.2.20240524.tar.gz` & `tmp/iam_actions-1.2.20240525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240524.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240525.tar", max compression
```

## Comparing `iam_actions-1.2.20240524.tar` & `iam_actions-1.2.20240525.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/README.md
--rw-r--r--   0        0        0      228 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/__init__.py
--rw-r--r--   0        0        0  4849776 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-24 02:22:57.332427 iam_actions-1.2.20240524/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-24 02:22:57.336427 iam_actions-1.2.20240524/iam_actions/generate/services.py
--rw-r--r--   0        0        0   631731 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/policies.json
--rw-r--r--   0        0        0   209748 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   612689 2024-05-24 02:24:49.976906 iam_actions-1.2.20240524/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-24 02:24:50.664909 iam_actions-1.2.20240524/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240524/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240524/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/README.md
+-rw-r--r--   0        0        0      228 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4851189 2024-05-25 02:23:02.833378 iam_actions-1.2.20240525/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-25 02:20:52.022525 iam_actions-1.2.20240525/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   631731 2024-05-25 02:23:02.833378 iam_actions-1.2.20240525/iam_actions/policies.json
+-rw-r--r--   0        0        0   209748 2024-05-25 02:23:02.833378 iam_actions-1.2.20240525/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   612689 2024-05-25 02:23:02.833378 iam_actions-1.2.20240525/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-25 02:23:03.521393 iam_actions-1.2.20240525/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240525/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240525/PKG-INFO
```

### Comparing `iam_actions-1.2.20240524/LICENSE` & `iam_actions-1.2.20240525/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/README.md` & `iam_actions-1.2.20240525/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/actions.json` & `iam_actions-1.2.20240525/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999788358381186%*

 * *Differences: {"'chatbot'": "{'ListTagsForResource': {'access_level': 'Read', 'description': 'Grants permission "*

 * *              "to List all tags associated with the AWS Chatbot Channel Configuration'}, "*

 * *              "'UntagResource': {'access_level': 'Tagging', 'description': 'Grants permission to "*

 * *              "remove tags on AWS Chatbot Channel Configuration'}, 'TagResource': {'access_level': "*

 * *              "'Tagging', 'description': 'Grants permission to create tags on AWS Chatbot Channel "*

 * *              "Config […]*

```diff
@@ -16903,18 +16903,18 @@
             "action": "ListMicrosoftTeamsUserIdentities",
             "condition_keys": [],
             "description": "Grants permission to describe AWS Chatbot Microsoft Teams User Identities",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to List all tags associated with the AWS Chatbot Channel Configuration",
             "orphan": false,
             "resources": []
         },
         "RedeemMicrosoftTeamsOauthCode": {
             "access_level": "Write",
             "action": "RedeemMicrosoftTeamsOauthCode",
             "condition_keys": [],
@@ -16927,26 +16927,26 @@
             "action": "RedeemSlackOauthCode",
             "condition_keys": [],
             "description": "Grants permission to redeem previously generated parameters with Slack API, to acquire OAuth tokens to be used by the AWS Chatbot service",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create tags on AWS Chatbot Channel Configuration",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove tags on AWS Chatbot Channel Configuration",
             "orphan": false,
             "resources": []
         },
         "UpdateAccountPreferences": {
             "access_level": "Write",
             "action": "UpdateAccountPreferences",
             "condition_keys": [],
@@ -54295,26 +54295,19 @@
             "orphan": false,
             "resources": []
         },
         "DescribeAddressesAttribute": {
             "access_level": "List",
             "action": "DescribeAddressesAttribute",
             "condition_keys": [
-                "aws:ResourceTag/${TagKey}",
-                "ec2:AllocationId",
-                "ec2:Domain",
-                "ec2:PublicIpAddress",
-                "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:Region"
             ],
             "description": "Grants permission to describe the attributes of the specified Elastic IP addresses",
             "orphan": false,
-            "resources": [
-                "elastic-ip"
-            ]
+            "resources": []
         },
         "DescribeAggregateIdFormat": {
             "access_level": "List",
             "action": "DescribeAggregateIdFormat",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -55347,19 +55340,25 @@
             "orphan": false,
             "resources": []
         },
         "DescribeSecurityGroupReferences": {
             "access_level": "List",
             "action": "DescribeSecurityGroupReferences",
             "condition_keys": [
-                "ec2:Region"
+                "aws:ResourceTag/${TagKey}",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:SecurityGroupID",
+                "ec2:Vpc"
             ],
             "description": "Grants permission to describe the VPCs on the other side of a VPC peering connection that are referencing specified VPC security groups",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "security-group"
+            ]
         },
         "DescribeSecurityGroupRules": {
             "access_level": "List",
             "action": "DescribeSecurityGroupRules",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -56189,20 +56188,31 @@
             "description": "Grants permission to cancel the deprecation of the specified AMI",
             "orphan": false,
             "resources": [
                 "image"
             ]
         },
         "DisableImageDeregistrationProtection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableImageDeregistrationProtection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to disable deregistration protection for an AMI. When deregistration protection is disabled, the AMI can be deregistered",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "DisableIpamOrganizationAdminAccount": {
             "access_level": "Write",
             "action": "DisableIpamOrganizationAdminAccount",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -56704,20 +56714,31 @@
             "description": "Grants permission to enable deprecation of the specified AMI at the specified date and time",
             "orphan": false,
             "resources": [
                 "image"
             ]
         },
         "EnableImageDeregistrationProtection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableImageDeregistrationProtection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:ImageID",
+                "ec2:ImageType",
+                "ec2:Owner",
+                "ec2:Public",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType"
+            ],
+            "description": "Grants permission to enable deregistration protection for an AMI. When deregistration protection is enabled, the AMI can't be deregistered",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "image"
+            ]
         },
         "EnableIpamOrganizationAdminAccount": {
             "access_level": "Write",
             "action": "EnableIpamOrganizationAdminAccount",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -57123,20 +57144,39 @@
                 "ec2:Region"
             ],
             "description": "Grants permission to view the default instance metadata service (IMDS) settings set for your account in the specified Region",
             "orphan": false,
             "resources": []
         },
         "GetInstanceTpmEkPub": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetInstanceTpmEkPub",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "ec2:AvailabilityZone",
+                "ec2:EbsOptimized",
+                "ec2:InstanceAutoRecovery",
+                "ec2:InstanceID",
+                "ec2:InstanceMarketType",
+                "ec2:InstanceMetadataTags",
+                "ec2:InstanceProfile",
+                "ec2:InstanceType",
+                "ec2:MetadataHttpEndpoint",
+                "ec2:MetadataHttpPutResponseHopLimit",
+                "ec2:MetadataHttpTokens",
+                "ec2:Region",
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:RootDeviceType",
+                "ec2:Tenancy"
+            ],
+            "description": "Grants permission to get the public endorsement key associated with the Nitro Trusted Platform Module (NitroTPM) for the specified instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "GetInstanceTypesFromInstanceRequirements": {
             "access_level": "List",
             "action": "GetInstanceTypesFromInstanceRequirements",
             "condition_keys": [
                 "ec2:Region"
             ],
@@ -67025,20 +67065,22 @@
             "description": "Grants permission to execute interactive workloads on an application",
             "orphan": false,
             "resources": [
                 "application"
             ]
         },
         "AccessLivyEndpoints": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AccessLivyEndpoints",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to execute interactive workloads on Livy Endpoint enabled on an EMR Serverless Application",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "application"
+            ]
         },
         "CancelJobRun": {
             "access_level": "Write",
             "action": "CancelJobRun",
             "condition_keys": [],
             "description": "Grants permission to cancel a job run",
             "orphan": false,
@@ -156092,17 +156134,15 @@
         },
         "GetPatchBaselineForPatchGroup": {
             "access_level": "Read",
             "action": "GetPatchBaselineForPatchGroup",
             "condition_keys": [],
             "description": "Grants permission to view the ID of the current patch baseline for a specified patch group",
             "orphan": false,
-            "resources": [
-                "patchbaseline"
-            ]
+            "resources": []
         },
         "GetResourcePolicies": {
             "access_level": "List",
             "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Grants permission to retrieve lists of Systems Manager resource policies",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240525/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240525/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/generate.py` & `iam_actions-1.2.20240525/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240525/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240525/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/generate/services.py` & `iam_actions-1.2.20240525/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/policies.json` & `iam_actions-1.2.20240525/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240525/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/iam_actions/services.json` & `iam_actions-1.2.20240525/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240524/pyproject.toml` & `iam_actions-1.2.20240525/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240524"
+version = "1.2.20240525"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240524/setup.py` & `iam_actions-1.2.20240525/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240524',
+    'version': '1.2.20240525',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240524/PKG-INFO` & `iam_actions-1.2.20240525/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240524
+Version: 1.2.20240525
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

