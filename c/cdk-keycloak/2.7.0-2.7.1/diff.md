# Comparing `tmp/cdk-keycloak-2.7.0.tar.gz` & `tmp/cdk-keycloak-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-keycloak-2.7.0.tar", last modified: Tue Mar 28 13:42:02 2023, max compression
+gzip compressed data, was "cdk-keycloak-2.7.1.tar", last modified: Fri Apr 21 01:42:29 2023, max compression
```

## Comparing `cdk-keycloak-2.7.0.tar` & `cdk-keycloak-2.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:42:02.711313 cdk-keycloak-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-03-28 13:42:02.711313 cdk-keycloak-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:42:02.711313 cdk-keycloak-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:42:02.707313 cdk-keycloak-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:42:02.707313 cdk-keycloak-2.7.0/src/cdk_keycloak/
--rw-r--r--   0 runner    (1001) docker     (123)    91011 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/src/cdk_keycloak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:42:02.711313 cdk-keycloak-2.7.0/src/cdk_keycloak/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/src/cdk_keycloak/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51153 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/src/cdk_keycloak/_jsii/cdk-keycloak@2.7.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:41:47.000000 cdk-keycloak-2.7.0/src/cdk_keycloak/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:42:02.711313 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-03-28 13:42:02.000000 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-28 13:42:02.000000 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:42:02.000000 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-28 13:42:02.000000 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 13:42:02.000000 cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:42:29.645466 cdk-keycloak-2.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/src/cdk_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (123)    91011 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/src/cdk_keycloak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/src/cdk_keycloak/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/src/cdk_keycloak/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51151 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/src/cdk_keycloak/_jsii/cdk-keycloak@2.7.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:42:15.000000 cdk-keycloak-2.7.1/src/cdk_keycloak/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:42:29.649466 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-21 01:42:29.000000 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 01:42:29.000000 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:42:29.000000 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 01:42:29.000000 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 01:42:29.000000 cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/top_level.txt
```

### Comparing `cdk-keycloak-2.7.0/LICENSE` & `cdk-keycloak-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-keycloak-2.7.0/PKG-INFO` & `cdk-keycloak-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-keycloak
-Version: 2.7.0
+Version: 2.7.1
 Summary: CDK construct library that allows you to create KeyCloak service on AWS in TypeScript or Python
 Home-page: https://github.com/aws-samples/cdk-keycloak.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-keycloak.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-keycloak-2.7.0/README.md` & `cdk-keycloak-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-keycloak-2.7.0/setup.py` & `cdk-keycloak-2.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-keycloak",
-    "version": "2.7.0",
+    "version": "2.7.1",
     "description": "CDK construct library that allows you to create KeyCloak service on AWS in TypeScript or Python",
     "license": "Apache-2.0",
     "url": "https://github.com/aws-samples/cdk-keycloak.git",
     "long_description_content_type": "text/markdown",
     "author": "Pahud Hsieh<pahudnet@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_keycloak",
         "cdk_keycloak._jsii"
     ],
     "package_data": {
         "cdk_keycloak._jsii": [
-            "cdk-keycloak@2.7.0.jsii.tgz"
+            "cdk-keycloak@2.7.1.jsii.tgz"
         ],
         "cdk_keycloak": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-keycloak-2.7.0/src/cdk_keycloak/__init__.py` & `cdk-keycloak-2.7.1/src/cdk_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-keycloak-2.7.0/src/cdk_keycloak.egg-info/PKG-INFO` & `cdk-keycloak-2.7.1/src/cdk_keycloak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-keycloak
-Version: 2.7.0
+Version: 2.7.1
 Summary: CDK construct library that allows you to create KeyCloak service on AWS in TypeScript or Python
 Home-page: https://github.com/aws-samples/cdk-keycloak.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws-samples/cdk-keycloak.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

