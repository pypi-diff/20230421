# Comparing `tmp/cdktf-cdktf-provider-dnsimple-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-dnsimple-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dnsimple-5.0.0.tar", last modified: Tue Apr 18 20:37:37 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dnsimple-5.0.1.tar", last modified: Fri Apr 21 13:39:11 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dnsimple-5.0.0.tar` & `cdktf-cdktf-provider-dnsimple-5.0.1.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.430281 cdktf-cdktf-provider-dnsimple-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130208 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
--rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60021 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/contact/
+-rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/domain_delegation/
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/ds_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    26171 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/email_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26531 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/registered_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    51885 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.309000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/zone_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-04-21 13:39:00.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:11.305000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-21 13:39:11.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-21 13:39:11.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:39:11.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 13:39:11.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 13:39:11.000000 cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/LICENSE` & `cdktf-cdktf-provider-dnsimple-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 5.0.0
+Version: 5.0.1
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/README.md` & `cdktf-cdktf-provider-dnsimple-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/setup.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dnsimple",
-    "version": "5.0.0",
+    "version": "5.0.1",
     "description": "Prebuilt dnsimple Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dnsimple.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -19,25 +19,29 @@
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdktf_cdktf_provider_dnsimple",
         "cdktf_cdktf_provider_dnsimple._jsii",
+        "cdktf_cdktf_provider_dnsimple.contact",
         "cdktf_cdktf_provider_dnsimple.data_dnsimple_certificate",
         "cdktf_cdktf_provider_dnsimple.data_dnsimple_zone",
         "cdktf_cdktf_provider_dnsimple.domain",
+        "cdktf_cdktf_provider_dnsimple.domain_delegation",
+        "cdktf_cdktf_provider_dnsimple.ds_record",
         "cdktf_cdktf_provider_dnsimple.email_forward",
         "cdktf_cdktf_provider_dnsimple.lets_encrypt_certificate",
         "cdktf_cdktf_provider_dnsimple.provider",
+        "cdktf_cdktf_provider_dnsimple.registered_domain",
         "cdktf_cdktf_provider_dnsimple.zone_record"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dnsimple._jsii": [
-            "provider-dnsimple@5.0.0.jsii.tgz"
+            "provider-dnsimple@5.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dnsimple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,26 +101,34 @@
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
 __all__ = [
+    "contact",
     "data_dnsimple_certificate",
     "data_dnsimple_zone",
     "domain",
+    "domain_delegation",
+    "ds_record",
     "email_forward",
     "lets_encrypt_certificate",
     "provider",
+    "registered_domain",
     "zone_record",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
+from . import contact
 from . import data_dnsimple_certificate
 from . import data_dnsimple_zone
 from . import domain
+from . import domain_delegation
+from . import ds_record
 from . import email_forward
 from . import lets_encrypt_certificate
 from . import provider
+from . import registered_domain
 from . import zone_record
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dnsimple_certificate`
 
-Refer to the Terraform Registory for docs: [`data_dnsimple_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate).
+Refer to the Terraform Registory for docs: [`data_dnsimple_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataDnsimpleCertificate(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate dnsimple_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate dnsimple_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         certificate_id: jsii.Number,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate dnsimple_certificate} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate dnsimple_certificate} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -177,16 +177,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -280,25 +280,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def certificate_id(self) -> jsii.Number:
         '''Certificate ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
         '''
         result = self._values.get("certificate_id")
         assert result is not None, "Required property 'certificate_id' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
         '''Domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         '''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dnsimple_zone`
 
-Refer to the Terraform Registory for docs: [`data_dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone).
+Refer to the Terraform Registory for docs: [`data_dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataDnsimpleZone(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleZone.DataDnsimpleZone",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone dnsimple_zone}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone dnsimple_zone}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -38,19 +38,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone dnsimple_zone} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone dnsimple_zone} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -145,15 +145,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9051fabefb514091998aee3b06ffda795da4195d413ca0bc91120a12dc8cf592)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -245,15 +245,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Zone Name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_domain`
 
-Refer to the Terraform Registory for docs: [`dnsimple_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain).
+Refer to the Terraform Registory for docs: [`dnsimple_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Domain(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.domain.Domain",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain dnsimple_domain}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain dnsimple_domain}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -38,19 +38,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain dnsimple_domain} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain dnsimple_domain} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain#name Domain#name}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -165,15 +165,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain#name Domain#name}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -263,15 +263,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/domain#name Domain#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_email_forward`
 
-Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward).
+Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class EmailForward(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForward",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward dnsimple_email_forward}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward dnsimple_email_forward}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias_name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward dnsimple_email_forward} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward dnsimple_email_forward} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#domain EmailForward#domain}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -184,17 +184,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#domain EmailForward#domain}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -288,29 +288,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def alias_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.'''
         result = self._values.get("alias_name")
         assert result is not None, "Required property 'alias_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def destination_email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.'''
         result = self._values.get("destination_email")
         assert result is not None, "Required property 'destination_email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/email_forward#domain EmailForward#domain}.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_lets_encrypt_certificate`
 
-Refer to the Terraform Registory for docs: [`dnsimple_lets_encrypt_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate).
+Refer to the Terraform Registory for docs: [`dnsimple_lets_encrypt_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,43 @@
 
 
 class LetsEncryptCertificate(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.letsEncryptCertificate.LetsEncryptCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         domain_id: builtins.str,
         name: builtins.str,
+        alternate_names: typing.Optional[typing.Sequence[builtins.str]] = None,
         signature_algorithm: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -65,26 +67,31 @@
             type_hints = typing.get_type_hints(_typecheckingstub__baf9170565dd5a0e411aa9fc260d074a96b9161acd4607bcb9162bf772464ea0)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = LetsEncryptCertificateConfig(
             auto_renew=auto_renew,
             domain_id=domain_id,
             name=name,
+            alternate_names=alternate_names,
             signature_algorithm=signature_algorithm,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
         jsii.create(self.__class__, self, [scope, id, config])
 
+    @jsii.member(jsii_name="resetAlternateNames")
+    def reset_alternate_names(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAlternateNames", []))
+
     @jsii.member(jsii_name="resetSignatureAlgorithm")
     def reset_signature_algorithm(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSignatureAlgorithm", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
@@ -131,14 +138,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="years")
     def years(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "years"))
 
     @builtins.property
+    @jsii.member(jsii_name="alternateNamesInput")
+    def alternate_names_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "alternateNamesInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="autoRenewInput")
     def auto_renew_input(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "autoRenewInput"))
 
     @builtins.property
@@ -153,14 +165,26 @@
 
     @builtins.property
     @jsii.member(jsii_name="signatureAlgorithmInput")
     def signature_algorithm_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "signatureAlgorithmInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="alternateNames")
+    def alternate_names(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "alternateNames"))
+
+    @alternate_names.setter
+    def alternate_names(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__525a0dd1c3e8fb79c6c5af8046da13c044eaf9789d7ebc3b25139d2a3dba196b)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "alternateNames", value)
+
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
@@ -218,14 +242,15 @@
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "auto_renew": "autoRenew",
         "domain_id": "domainId",
         "name": "name",
+        "alternate_names": "alternateNames",
         "signature_algorithm": "signatureAlgorithm",
     },
 )
 class LetsEncryptCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
@@ -235,28 +260,30 @@
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         domain_id: builtins.str,
         name: builtins.str,
+        alternate_names: typing.Optional[typing.Sequence[builtins.str]] = None,
         signature_algorithm: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -264,14 +291,15 @@
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
             check_type(argname="argument domain_id", value=domain_id, expected_type=type_hints["domain_id"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument alternate_names", value=alternate_names, expected_type=type_hints["alternate_names"])
             check_type(argname="argument signature_algorithm", value=signature_algorithm, expected_type=type_hints["signature_algorithm"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "auto_renew": auto_renew,
             "domain_id": domain_id,
             "name": name,
         }
         if connection is not None:
@@ -284,14 +312,16 @@
             self._values["for_each"] = for_each
         if lifecycle is not None:
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
+        if alternate_names is not None:
+            self._values["alternate_names"] = alternate_names
         if signature_algorithm is not None:
             self._values["signature_algorithm"] = signature_algorithm
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
@@ -353,36 +383,42 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
         result = self._values.get("auto_renew")
         assert result is not None, "Required property 'auto_renew' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def domain_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
         result = self._values.get("domain_id")
         assert result is not None, "Required property 'domain_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def alternate_names(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.'''
+        result = self._values.get("alternate_names")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def signature_algorithm(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
         result = self._values.get("signature_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -404,26 +440,33 @@
 def _typecheckingstub__baf9170565dd5a0e411aa9fc260d074a96b9161acd4607bcb9162bf772464ea0(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     domain_id: builtins.str,
     name: builtins.str,
+    alternate_names: typing.Optional[typing.Sequence[builtins.str]] = None,
     signature_algorithm: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__525a0dd1c3e8fb79c6c5af8046da13c044eaf9789d7ebc3b25139d2a3dba196b(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__a1c625380326aede0264f73d07321e723c6fdd40a105f44e3019b524a24c1ec6(
     value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f1f0420bef8d392657f46cb05288fdcec9f81b26774869507832adb9f190c50b(
@@ -452,11 +495,12 @@
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     domain_id: builtins.str,
     name: builtins.str,
+    alternate_names: typing.Optional[typing.Sequence[builtins.str]] = None,
     signature_algorithm: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`dnsimple`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs).
+Refer to the Terraform Registory for docs: [`dnsimple`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,38 +22,38 @@
 
 
 class DnsimpleProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.provider.DnsimpleProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs dnsimple}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs dnsimple}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         account: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs dnsimple} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs dnsimple} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7ef56b7728822c45a23750e2602fff787208bfb71fa54a96467397e10a6e47c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DnsimpleProviderConfig(
             account=account,
@@ -236,20 +236,20 @@
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38b8bc1cdf1e0a8d7a730ac02381391ddfa090074fe8470d004c65b043c59d30)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument prefetch", value=prefetch, expected_type=type_hints["prefetch"])
             check_type(argname="argument sandbox", value=sandbox, expected_type=type_hints["sandbox"])
@@ -269,64 +269,64 @@
         if user_agent is not None:
             self._values["user_agent"] = user_agent
 
     @builtins.property
     def account(self) -> typing.Optional[builtins.str]:
         '''The account for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#account DnsimpleProvider#account}
         '''
         result = self._values.get("account")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#alias DnsimpleProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefetch(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the prefetch of zone records.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#prefetch DnsimpleProvider#prefetch}
         '''
         result = self._values.get("prefetch")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def sandbox(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the sandbox API.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#sandbox DnsimpleProvider#sandbox}
         '''
         result = self._values.get("sandbox")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The API v2 token for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#token DnsimpleProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_agent(self) -> typing.Optional[builtins.str]:
         '''Custom string to append to the user agent used for sending HTTP requests to the API.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         result = self._values.get("user_agent")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_zone_record`
 
-Refer to the Terraform Registory for docs: [`dnsimple_zone_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record).
+Refer to the Terraform Registory for docs: [`dnsimple_zone_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ZoneRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.zoneRecord.ZoneRecord",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record dnsimple_zone_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record dnsimple_zone_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record dnsimple_zone_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record dnsimple_zone_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.
-        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -263,20 +263,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.
-        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -378,49 +378,49 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#name ZoneRecord#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#type ZoneRecord#type}.'''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#value ZoneRecord#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.'''
         result = self._values.get("zone_name")
         assert result is not None, "Required property 'zone_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def priority(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#priority ZoneRecord#priority}.'''
         result = self._values.get("priority")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.1.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.'''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 5.0.0
+Version: 5.0.1
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dnsimple-5.0.1/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 src/cdktf_cdktf_provider_dnsimple/py.typed
 src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
-src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.1.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
+src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
 src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
 src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
 src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
```

