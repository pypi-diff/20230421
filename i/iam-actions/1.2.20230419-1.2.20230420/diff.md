# Comparing `tmp/iam_actions-1.2.20230419.tar.gz` & `tmp/iam_actions-1.2.20230420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230419.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230420.tar", max compression
```

## Comparing `iam_actions-1.2.20230419.tar` & `iam_actions-1.2.20230420.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/README.md
--rw-r--r--   0        0        0      228 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/__init__.py
--rw-r--r--   0        0        0  4214762 2023-04-19 02:29:01.410602 iam_actions-1.2.20230419/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-19 02:27:38.502802 iam_actions-1.2.20230419/iam_actions/generate/services.py
--rw-r--r--   0        0        0   540792 2023-04-19 02:29:01.410602 iam_actions-1.2.20230419/iam_actions/policies.json
--rw-r--r--   0        0        0   190619 2023-04-19 02:29:01.410602 iam_actions-1.2.20230419/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   524379 2023-04-19 02:29:01.410602 iam_actions-1.2.20230419/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-19 02:29:02.166599 iam_actions-1.2.20230419/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230419/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230419/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/README.md
+-rw-r--r--   0        0        0      228 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4214781 2023-04-20 02:27:05.567826 iam_actions-1.2.20230420/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-20 02:25:27.900090 iam_actions-1.2.20230420/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   540796 2023-04-20 02:27:05.567826 iam_actions-1.2.20230420/iam_actions/policies.json
+-rw-r--r--   0        0        0   190619 2023-04-20 02:27:05.567826 iam_actions-1.2.20230420/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   524383 2023-04-20 02:27:05.567826 iam_actions-1.2.20230420/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-20 02:27:06.351823 iam_actions-1.2.20230420/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230420/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230420/PKG-INFO
```

### Comparing `iam_actions-1.2.20230419/LICENSE` & `iam_actions-1.2.20230420/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/README.md` & `iam_actions-1.2.20230420/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/actions.json` & `iam_actions-1.2.20230420/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999967212254748%*

 * *Differences: {"'connect'": "{'UpdateRule': {'resources': ['rule']}}",*

 * * "'iotroborunner'": "{'ListDestinations': {'resources': ['SiteResource']}}"}*

```diff
@@ -31449,15 +31449,15 @@
             "action": "UpdateRule",
             "condition_keys": [
                 "connect:InstanceId"
             ],
             "description": "Grants permission to update a rule for an existing Amazon Connect instance",
             "orphan": false,
             "resources": [
-                "instance"
+                "rule"
             ]
         },
         "UpdateSecurityProfile": {
             "access_level": "Write",
             "action": "UpdateSecurityProfile",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
@@ -77831,15 +77831,17 @@
         },
         "ListDestinations": {
             "access_level": "Read",
             "action": "ListDestinations",
             "condition_keys": [],
             "description": "Grants permission to list destinations",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "SiteResource"
+            ]
         },
         "ListSites": {
             "access_level": "Read",
             "action": "ListSites",
             "condition_keys": [],
             "description": "Grants permission to list sites",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230420/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230420/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/generate.py` & `iam_actions-1.2.20230420/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230420/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230420/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/generate/services.py` & `iam_actions-1.2.20230420/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/policies.json` & `iam_actions-1.2.20230420/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999887387387387%*

 * *Differences: {"'serviceMap'": "{'Amazon EC2 Instance Connect': {'ARNFormat': "*

 * *                 "'arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}'}}"}*

```diff
@@ -12668,15 +12668,15 @@
                 "imagebuilder:CreatedResourceTag/<key>",
                 "imagebuilder:CreatedResourceTagKeys",
                 "imagebuilder:Ec2MetadataHttpTokens",
                 "imagebuilder:StatusTopicArn"
             ]
         },
         "Amazon EC2 Instance Connect": {
-            "ARNFormat": "arn:aws:ec2:<region>:<account>:<resourceType>/<resourcePath>",
+            "ARNFormat": "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:ec2:.+",
             "Actions": [
                 "SendSSHPublicKey",
                 "SendSerialConsoleSSHPublicKey"
             ],
             "HasResource": true,
             "StringPrefix": "ec2-instance-connect",
```

### Comparing `iam_actions-1.2.20230419/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230420/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230419/iam_actions/services.json` & `iam_actions-1.2.20230420/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998819641170915%*

 * *Differences: {"'ec2-instance-connect'": "{'ARNFormats': "*

 * *                           "['arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}']}"}*

```diff
@@ -6878,15 +6878,15 @@
         "HasResource": true,
         "ServiceNames": [
             "Amazon EC2"
         ]
     },
     "ec2-instance-connect": {
         "ARNFormats": [
-            "arn:aws:ec2:<region>:<account>:<resourceType>/<resourcePath>"
+            "arn:aws:ec2:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:aws:ec2:.+"
         ],
         "Actions": [
             "SendSSHPublicKey",
             "SendSerialConsoleSSHPublicKey"
```

### Comparing `iam_actions-1.2.20230419/pyproject.toml` & `iam_actions-1.2.20230420/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230419"
+version = "1.2.20230420"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230419/setup.py` & `iam_actions-1.2.20230420/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230419',
+    'version': '1.2.20230420',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230419/PKG-INFO` & `iam_actions-1.2.20230420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230419
+Version: 1.2.20230420
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

