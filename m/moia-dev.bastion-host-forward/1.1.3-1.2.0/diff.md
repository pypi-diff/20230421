# Comparing `tmp/moia-dev.bastion-host-forward-1.1.3.tar.gz` & `tmp/moia-dev.bastion-host-forward-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moia-dev.bastion-host-forward-1.1.3.tar", last modified: Thu Oct 20 14:35:06 2022, max compression
+gzip compressed data, was "moia-dev.bastion-host-forward-1.2.0.tar", last modified: Fri Apr 21 08:44:27 2023, max compression
```

## Comparing `moia-dev.bastion-host-forward-1.1.3.tar` & `moia-dev.bastion-host-forward-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14464 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.046857 moia-dev.bastion-host-forward-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.046857 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/
--rw-r--r--   0 runner    (1001) docker     (121)    41613 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    72191 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@1.1.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 14:34:56.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 14:35:06.050857 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14464 2022-10-20 14:35:05.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-10-20 14:35:06.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 14:35:05.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-20 14:35:05.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-20 14:35:05.000000 moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.246864 moia-dev.bastion-host-forward-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.246864 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)    41613 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72856 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@1.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:44:16.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:44:27.250865 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-04-21 08:44:26.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-21 08:44:27.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:44:26.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 08:44:27.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 08:44:27.000000 moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/top_level.txt
```

### Comparing `moia-dev.bastion-host-forward-1.1.3/LICENSE` & `moia-dev.bastion-host-forward-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moia-dev.bastion-host-forward-1.1.3/PKG-INFO` & `moia-dev.bastion-host-forward-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moia-dev.bastion-host-forward
-Version: 1.1.3
+Version: 1.2.0
 Summary: CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine
 Home-page: https://github.com/moia-oss/bastion-host-forward
 Author: MOIA GmbH
 License: Apache-2.0
 Project-URL: Source, https://github.com/moia-oss/bastion-host-forward
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `moia-dev.bastion-host-forward-1.1.3/README.md` & `moia-dev.bastion-host-forward-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `moia-dev.bastion-host-forward-1.1.3/setup.py` & `moia-dev.bastion-host-forward-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "moia-dev.bastion-host-forward",
-    "version": "1.1.3",
+    "version": "1.2.0",
     "description": "CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine",
     "license": "Apache-2.0",
     "url": "https://github.com/moia-oss/bastion-host-forward",
     "long_description_content_type": "text/markdown",
     "author": "MOIA GmbH",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "moia_dev.bastion_host_forward",
         "moia_dev.bastion_host_forward._jsii"
     ],
     "package_data": {
         "moia_dev.bastion_host_forward._jsii": [
-            "bastion-host-forward@1.1.3.jsii.tgz"
+            "bastion-host-forward@1.2.0.jsii.tgz"
         ],
         "moia_dev.bastion_host_forward": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.18.0, <3.0.0",
-        "constructs>=10.0.102, <11.0.0",
-        "jsii>=1.69.0, <2.0.0",
+        "aws-cdk-lib>=2.76.0, <3.0.0",
+        "constructs>=10.2.1, <11.0.0",
+        "jsii>=5.0.3, <6.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `moia-dev.bastion-host-forward-1.1.3/src/moia_dev/bastion_host_forward/__init__.py` & `moia-dev.bastion-host-forward-1.2.0/src/moia_dev/bastion_host_forward/__init__.py`

 * *Files identical despite different names*

### Comparing `moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO` & `moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moia-dev.bastion-host-forward
-Version: 1.1.3
+Version: 1.2.0
 Summary: CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine
 Home-page: https://github.com/moia-oss/bastion-host-forward
 Author: MOIA GmbH
 License: Apache-2.0
 Project-URL: Source, https://github.com/moia-oss/bastion-host-forward
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `moia-dev.bastion-host-forward-1.1.3/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt` & `moia-dev.bastion-host-forward-1.2.0/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
 src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
 src/moia_dev.bastion_host_forward.egg-info/requires.txt
 src/moia_dev.bastion_host_forward.egg-info/top_level.txt
 src/moia_dev/bastion_host_forward/__init__.py
 src/moia_dev/bastion_host_forward/py.typed
 src/moia_dev/bastion_host_forward/_jsii/__init__.py
-src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@1.1.3.jsii.tgz
+src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@1.2.0.jsii.tgz
```

