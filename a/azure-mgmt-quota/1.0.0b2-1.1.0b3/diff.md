# Comparing `tmp/azure-mgmt-quota-1.0.0b2.zip` & `tmp/azure-mgmt-quota-1.1.0b3.zip`

## zipinfo {}

```diff
@@ -1,47 +1,55 @@
-Zip file size: 50030 bytes, number of entries: 45
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/
--rw-rw-r--  2.0 unx       67 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/setup.cfg
--rw-rw-r--  2.0 unx     1153 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/README.md
--rw-rw-r--  2.0 unx      126 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx     2641 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/PKG-INFO
--rw-rw-r--  2.0 unx      570 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/_meta.json
--rw-rw-r--  2.0 unx     3026 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/setup.py
--rw-rw-r--  2.0 unx      293 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/CHANGELOG.md
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/
--rw-rw-r--  2.0 unx       65 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/
--rw-rw-r--  2.0 unx     4398 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_azure_quota_extension_api.py
--rw-rw-r--  2.0 unx      722 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/__init__.py
--rw-rw-r--  2.0 unx     2980 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_configuration.py
--rw-rw-r--  2.0 unx      488 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_version.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/
--rw-rw-r--  2.0 unx     4373 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/_azure_quota_extension_api.py
--rw-rw-r--  2.0 unx      568 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/__init__.py
--rw-rw-r--  2.0 unx     2932 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/_configuration.py
--rw-rw-r--  2.0 unx    23944 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_operations.py
--rw-rw-r--  2.0 unx     4824 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_operation_operations.py
--rw-rw-r--  2.0 unx      835 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     8779 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_usages_operations.py
--rw-rw-r--  2.0 unx     9986 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py
--rw-rw-r--  2.0 unx    37250 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_models_py3.py
--rw-rw-r--  2.0 unx     1886 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_azure_quota_extension_api_enums.py
--rw-rw-r--  2.0 unx     4251 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/__init__.py
--rw-rw-r--  2.0 unx    35373 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_models.py
--rw-rw-r--  2.0 unx    24088 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_operations.py
--rw-rw-r--  2.0 unx     4884 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_operation_operations.py
--rw-rw-r--  2.0 unx      835 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/__init__.py
--rw-rw-r--  2.0 unx     8881 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_usages_operations.py
--rw-rw-r--  2.0 unx    10106 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_request_status_operations.py
--rw-rw-r--  2.0 unx     1320 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      105 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     2641 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 21-Nov-04 02:36 azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/dependency_links.txt
-45 files, 204463 bytes uncompressed, 41420 bytes compressed:  79.7%
+Zip file size: 73566 bytes, number of entries: 53
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/
+-rw-rw-r--  2.0 unx      415 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx      211 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/MANIFEST.in
+-rw-rw-r--  2.0 unx     1352 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/README.md
+-rw-rw-r--  2.0 unx     2816 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/setup.py
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/LICENSE
+-rw-rw-r--  2.0 unx      618 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/_meta.json
+-rw-rw-r--  2.0 unx       38 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/setup.cfg
+-rw-rw-r--  2.0 unx     2652 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/
+-rw-rw-r--  2.0 unx      488 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_version.py
+-rw-rw-r--  2.0 unx    77450 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_serialization.py
+-rw-rw-r--  2.0 unx     1169 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_patch.py
+-rw-rw-r--  2.0 unx     4718 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_azure_quota_extension_api.py
+-rw-rw-r--  2.0 unx     3522 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_configuration.py
+-rw-rw-r--  2.0 unx       26 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/py.typed
+-rw-rw-r--  2.0 unx      922 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_patch.py
+-rw-rw-r--  2.0 unx     4803 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_azure_quota_extension_api.py
+-rw-rw-r--  2.0 unx     3526 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_configuration.py
+-rw-rw-r--  2.0 unx      869 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/__init__.py
+-rw-rw-r--  2.0 unx    38617 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_operations.py
+-rw-rw-r--  2.0 unx     6160 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_operation_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    10965 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     9968 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx    44256 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_models_py3.py
+-rw-rw-r--  2.0 unx     1240 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_azure_quota_extension_api_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_patch.py
+-rw-rw-r--  2.0 unx     2888 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/__init__.py
+-rw-rw-r--  2.0 unx    42784 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_operations.py
+-rw-rw-r--  2.0 unx     6897 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_operation_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_patch.py
+-rw-rw-r--  2.0 unx    13284 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_request_status_operations.py
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/__init__.py
+-rw-rw-r--  2.0 unx    11913 b- defN 22-Nov-11 02:23 azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_usages_operations.py
+-rw-rw-r--  2.0 unx     1544 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx      116 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     2652 b- defN 22-Nov-11 02:24 azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/PKG-INFO
+53 files, 305609 bytes uncompressed, 63496 bytes compressed:  79.2%
```

## zipnote {}

```diff
@@ -1,136 +1,160 @@
-Filename: azure-mgmt-quota-1.0.0b2/
+Filename: azure-mgmt-quota-1.1.0b3/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/
+Filename: azure-mgmt-quota-1.1.0b3/azure/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/setup.cfg
+Filename: azure-mgmt-quota-1.1.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/README.md
+Filename: azure-mgmt-quota-1.1.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/MANIFEST.in
+Filename: azure-mgmt-quota-1.1.0b3/README.md
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/PKG-INFO
+Filename: azure-mgmt-quota-1.1.0b3/setup.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/_meta.json
+Filename: azure-mgmt-quota-1.1.0b3/LICENSE
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/setup.py
+Filename: azure-mgmt-quota-1.1.0b3/_meta.json
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/CHANGELOG.md
+Filename: azure-mgmt-quota-1.1.0b3/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/
+Filename: azure-mgmt-quota-1.1.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/
+Filename: azure-mgmt-quota-1.1.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_azure_quota_extension_api.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_version.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_configuration.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_version.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_patch.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/_azure_quota_extension_api.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_azure_quota_extension_api.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/_configuration.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/py.typed
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_operation_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_usages_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_azure_quota_extension_api.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_models_py3.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_azure_quota_extension_api_enums.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_operation_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_models.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_operation_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/__init__.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_usages_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_usages_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_request_status_operations.py
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_azure_quota_extension_api_enums.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/SOURCES.txt
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/top_level.txt
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/requires.txt
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/not-zip-safe
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_operation_operations.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/PKG-INFO
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/dependency_links.txt
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_quota_request_status_operations.py
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_usages_operations.py
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/requires.txt
+Comment: 
+
+Filename: azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-quota-1.0.0b2/README.md` & `azure-mgmt-quota-1.1.0b3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Quota Management Client Library.
-This package has been tested with Python 2.7, 3.6+.
+This package has been tested with Python 3.7+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
+## _Disclaimer_
+
+_Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 # Usage
 
 
 To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
-
-
  
 For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
 Code samples for this package can be found at [Quota Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
 Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 # Provide Feedback
```

## Comparing `azure-mgmt-quota-1.0.0b2/setup.py` & `azure-mgmt-quota-1.1.0b3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,14 @@
 PACKAGE_PPRINT_NAME = "Quota Management"
 
 # a-b-c => a/b/c
 package_folder_path = PACKAGE_NAME.replace('-', '/')
 # a-b-c => a.b.c
 namespace_name = PACKAGE_NAME.replace('-', '.')
 
-# azure v0.x is not compatible with this package
-# azure v0.x used to have a __version__ attribute (newer versions don't)
-try:
-    import azure
-    try:
-        ver = azure.__version__
-        raise Exception(
-            'This package is incompatible with azure=={}. '.format(ver) +
-            'Uninstall it with "pip uninstall azure".'
-        )
-    except AttributeError:
-        pass
-except ImportError:
-    pass
-
 # Version extraction inspired from 'requests'
 with open(os.path.join(package_folder_path, 'version.py')
           if os.path.exists(os.path.join(package_folder_path, 'version.py'))
           else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
     version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
@@ -56,35 +41,39 @@
     description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
+    keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.mgmt',
     ]),
+    include_package_data=True,
+    package_data={
+        'pytyped': ['py.typed'],
+    },
     install_requires=[
-        'msrest>=0.6.21',
-        'azure-common~=1.1',
-        'azure-mgmt-core>=1.2.0,<2.0.0',
+        "msrest>=0.7.1",
+        "azure-common~=1.1",
+        "azure-mgmt-core>=1.3.2,<2.0.0",
+        "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    extras_require={
-        ":python_version<'3.0'": ['azure-mgmt-nspkg'],
-    }
+    python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_azure_quota_extension_api.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/_azure_quota_extension_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,91 +2,90 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from copy import deepcopy
+from typing import Any, TYPE_CHECKING
 
+from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
-from msrest import Deserializer, Serializer
+
+from . import models
+from ._configuration import AzureQuotaExtensionAPIConfiguration
+from ._serialization import Deserializer, Serializer
+from .operations import QuotaOperationOperations, QuotaOperations, QuotaRequestStatusOperations, UsagesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Optional
-
     from azure.core.credentials import TokenCredential
-    from azure.core.pipeline.transport import HttpRequest, HttpResponse
 
-from ._configuration import AzureQuotaExtensionAPIConfiguration
-from .operations import UsagesOperations
-from .operations import QuotaOperations
-from .operations import QuotaRequestStatusOperations
-from .operations import QuotaOperationOperations
-from . import models
 
-
-class AzureQuotaExtensionAPI(object):
+class AzureQuotaExtensionAPI:  # pylint: disable=client-accepts-api-version-keyword
     """Microsoft Azure Quota Resource Provider.
 
     :ivar usages: UsagesOperations operations
     :vartype usages: azure.mgmt.quota.operations.UsagesOperations
     :ivar quota: QuotaOperations operations
     :vartype quota: azure.mgmt.quota.operations.QuotaOperations
     :ivar quota_request_status: QuotaRequestStatusOperations operations
     :vartype quota_request_status: azure.mgmt.quota.operations.QuotaRequestStatusOperations
     :ivar quota_operation: QuotaOperationOperations operations
     :vartype quota_operation: azure.mgmt.quota.operations.QuotaOperationOperations
-    :param credential: Credential needed for the client to connect to Azure.
+    :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param str base_url: Service URL
-    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+    :param base_url: Service URL. Default value is "https://management.azure.com".
+    :type base_url: str
+    :keyword api_version: Api Version. Default value is "2021-03-15-preview". Note that overriding
+     this default value may result in unsupported behavior.
+    :paramtype api_version: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(
-        self,
-        credential,  # type: "TokenCredential"
-        base_url=None,  # type: Optional[str]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        if not base_url:
-            base_url = 'https://management.azure.com'
-        self._config = AzureQuotaExtensionAPIConfiguration(credential, **kwargs)
+        self, credential: "TokenCredential", base_url: str = "https://management.azure.com", **kwargs: Any
+    ) -> None:
+        self._config = AzureQuotaExtensionAPIConfiguration(credential=credential, **kwargs)
         self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
-        self._serialize.client_side_validation = False
         self._deserialize = Deserializer(client_models)
-
-        self.usages = UsagesOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.quota = QuotaOperations(
-            self._client, self._config, self._serialize, self._deserialize)
+        self._serialize.client_side_validation = False
+        self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.quota = QuotaOperations(self._client, self._config, self._serialize, self._deserialize)
         self.quota_request_status = QuotaRequestStatusOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.quota_operation = QuotaOperationOperations(
-            self._client, self._config, self._serialize, self._deserialize)
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.quota_operation = QuotaOperationOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, http_request, **kwargs):
-        # type: (HttpRequest, Any) -> HttpResponse
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
-        :param http_request: The network request you want to make. Required.
-        :type http_request: ~azure.core.pipeline.transport.HttpRequest
-        :keyword bool stream: Whether the response payload will be streamed. Defaults to True.
+        >>> from azure.core.rest import HttpRequest
+        >>> request = HttpRequest("GET", "https://www.example.org/")
+        <HttpRequest [GET], url: 'https://www.example.org/'>
+        >>> response = client._send_request(request)
+        <HttpResponse: 200 OK>
+
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.HttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
-        http_request.url = self._client.format_url(http_request.url)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
+
+        request_copy = deepcopy(request)
+        request_copy.url = self._client.format_url(request_copy.url)
+        return self._client.send_request(request_copy, **kwargs)
 
     def close(self):
         # type: () -> None
         self._client.close()
 
     def __enter__(self):
         # type: () -> AzureQuotaExtensionAPI
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/__init__.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._azure_quota_extension_api import AzureQuotaExtensionAPI
 from ._version import VERSION
 
 __version__ = VERSION
-__all__ = ['AzureQuotaExtensionAPI']
 
 try:
-    from ._patch import patch_sdk  # type: ignore
-    patch_sdk()
+    from ._patch import __all__ as _patch_all
+    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
 except ImportError:
-    pass
+    _patch_all = []
+from ._patch import patch_sdk as _patch_sdk
+
+__all__ = [
+    "AzureQuotaExtensionAPI",
+]
+__all__.extend([p for p in _patch_all if p not in __all__])
+
+_patch_sdk()
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/_configuration.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,64 +2,66 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+import sys
+from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
-
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
-class AzureQuotaExtensionAPIConfiguration(Configuration):
+class AzureQuotaExtensionAPIConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for AzureQuotaExtensionAPI.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
-    :param credential: Credential needed for the client to connect to Azure.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :param credential: Credential needed for the client to connect to Azure. Required.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :keyword api_version: Api Version. Default value is "2021-03-15-preview". Note that overriding
+     this default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
 
-    def __init__(
-        self,
-        credential,  # type: "TokenCredential"
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def __init__(self, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
+        super(AzureQuotaExtensionAPIConfiguration, self).__init__(**kwargs)
+        api_version = kwargs.pop("api_version", "2021-03-15-preview")  # type: Literal["2021-03-15-preview"]
+
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
-        super(AzureQuotaExtensionAPIConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
-        self.api_version = "2021-03-15-preview"
-        self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
-        kwargs.setdefault('sdk_moniker', 'mgmt-quota/{}'.format(VERSION))
+        self.api_version = api_version
+        self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
+        kwargs.setdefault("sdk_moniker", "mgmt-quota/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
-        self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
-        self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
-        self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
-        self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
-        self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
-        self.authentication_policy = kwargs.get('authentication_policy')
+    def _configure(self, **kwargs: Any) -> None:
+        self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
+        self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
+        self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
+        self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
+        self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = policies.BearerTokenCredentialPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+                self.credential, *self.credential_scopes, **kwargs
+            )
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/_azure_quota_extension_api.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/_azure_quota_extension_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,87 +2,90 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import Any, Optional, TYPE_CHECKING
+from copy import deepcopy
+from typing import Any, Awaitable, TYPE_CHECKING
 
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
-from msrest import Deserializer, Serializer
+
+from .. import models
+from .._serialization import Deserializer, Serializer
+from ._configuration import AzureQuotaExtensionAPIConfiguration
+from .operations import QuotaOperationOperations, QuotaOperations, QuotaRequestStatusOperations, UsagesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-from ._configuration import AzureQuotaExtensionAPIConfiguration
-from .operations import UsagesOperations
-from .operations import QuotaOperations
-from .operations import QuotaRequestStatusOperations
-from .operations import QuotaOperationOperations
-from .. import models
-
 
-class AzureQuotaExtensionAPI(object):
+class AzureQuotaExtensionAPI:  # pylint: disable=client-accepts-api-version-keyword
     """Microsoft Azure Quota Resource Provider.
 
     :ivar usages: UsagesOperations operations
     :vartype usages: azure.mgmt.quota.aio.operations.UsagesOperations
     :ivar quota: QuotaOperations operations
     :vartype quota: azure.mgmt.quota.aio.operations.QuotaOperations
     :ivar quota_request_status: QuotaRequestStatusOperations operations
     :vartype quota_request_status: azure.mgmt.quota.aio.operations.QuotaRequestStatusOperations
     :ivar quota_operation: QuotaOperationOperations operations
     :vartype quota_operation: azure.mgmt.quota.aio.operations.QuotaOperationOperations
-    :param credential: Credential needed for the client to connect to Azure.
+    :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param str base_url: Service URL
-    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+    :param base_url: Service URL. Default value is "https://management.azure.com".
+    :type base_url: str
+    :keyword api_version: Api Version. Default value is "2021-03-15-preview". Note that overriding
+     this default value may result in unsupported behavior.
+    :paramtype api_version: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(
-        self,
-        credential: "AsyncTokenCredential",
-        base_url: Optional[str] = None,
-        **kwargs: Any
+        self, credential: "AsyncTokenCredential", base_url: str = "https://management.azure.com", **kwargs: Any
     ) -> None:
-        if not base_url:
-            base_url = 'https://management.azure.com'
-        self._config = AzureQuotaExtensionAPIConfiguration(credential, **kwargs)
+        self._config = AzureQuotaExtensionAPIConfiguration(credential=credential, **kwargs)
         self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
-        self._serialize.client_side_validation = False
         self._deserialize = Deserializer(client_models)
-
-        self.usages = UsagesOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.quota = QuotaOperations(
-            self._client, self._config, self._serialize, self._deserialize)
+        self._serialize.client_side_validation = False
+        self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.quota = QuotaOperations(self._client, self._config, self._serialize, self._deserialize)
         self.quota_request_status = QuotaRequestStatusOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.quota_operation = QuotaOperationOperations(
-            self._client, self._config, self._serialize, self._deserialize)
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.quota_operation = QuotaOperationOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    async def _send_request(self, http_request: HttpRequest, **kwargs: Any) -> AsyncHttpResponse:
+    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
-        :param http_request: The network request you want to make. Required.
-        :type http_request: ~azure.core.pipeline.transport.HttpRequest
-        :keyword bool stream: Whether the response payload will be streamed. Defaults to True.
+        >>> from azure.core.rest import HttpRequest
+        >>> request = HttpRequest("GET", "https://www.example.org/")
+        <HttpRequest [GET], url: 'https://www.example.org/'>
+        >>> response = await client._send_request(request)
+        <AsyncHttpResponse: 200 OK>
+
+        For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.AsyncHttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
-        http_request.url = self._client.format_url(http_request.url)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = await self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
+
+        request_copy = deepcopy(request)
+        request_copy.url = self._client.format_url(request_copy.url)
+        return self._client.send_request(request_copy, **kwargs)
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "AzureQuotaExtensionAPI":
         await self._client.__aenter__()
         return self
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/__init__.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,13 +7,19 @@
 # --------------------------------------------------------------------------
 
 from ._usages_operations import UsagesOperations
 from ._quota_operations import QuotaOperations
 from ._quota_request_status_operations import QuotaRequestStatusOperations
 from ._quota_operation_operations import QuotaOperationOperations
 
+from ._patch import __all__ as _patch_all
+from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import patch_sdk as _patch_sdk
+
 __all__ = [
-    'UsagesOperations',
-    'QuotaOperations',
-    'QuotaRequestStatusOperations',
-    'QuotaOperationOperations',
+    "UsagesOperations",
+    "QuotaOperations",
+    "QuotaRequestStatusOperations",
+    "QuotaOperationOperations",
 ]
+__all__.extend([p for p in _patch_all if p not in __all__])
+_patch_sdk()
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_usages_operations.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_usages_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,185 +1,219 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
-import warnings
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._usages_operations import build_get_request, build_list_request
 
-T = TypeVar('T')
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-class UsagesOperations:
-    """UsagesOperations async operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class UsagesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.quota.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.quota.aio.AzureQuotaExtensionAPI`'s
+        :attr:`usages` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
-
-    async def get(
-        self,
-        resource_name: str,
-        scope: str,
-        **kwargs: Any
-    ) -> "_models.CurrentUsagesBase":
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def get(self, resource_name: str, scope: str, **kwargs: Any) -> _models.CurrentUsagesBase:
         """Get the current usage of a resource.
 
         :param resource_name: Resource name for a given resource provider. For example:
 
 
          * SKU name for Microsoft.Compute
          * SKU or TotalLowPriorityCores for Microsoft.MachineLearningServices
-           For Microsoft.Network PublicIPAddresses.
+           For Microsoft.Network PublicIPAddresses. Required.
         :type resource_name: str
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CurrentUsagesBase, or the result of cls(response)
+        :return: CurrentUsagesBase or the result of cls(response)
         :rtype: ~azure.mgmt.quota.models.CurrentUsagesBase
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.CurrentUsagesBase"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
-        }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'resourceName': self._serialize.url("resource_name", resource_name, 'str'),
-            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        url = self._client.format_url(url, **path_format_arguments)
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CurrentUsagesBase]
+
+        request = build_get_request(
+            resource_name=resource_name,
+            scope=scope,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        request = self._client.get(url, query_parameters, header_parameters)
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
+            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
-        response_headers['ETag']=self._deserialize('str', response.headers.get('ETag'))
-        deserialized = self._deserialize('CurrentUsagesBase', pipeline_response)
+        response_headers["ETag"] = self._deserialize("str", response.headers.get("ETag"))
+
+        deserialized = self._deserialize("CurrentUsagesBase", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
-    get.metadata = {'url': '/{scope}/providers/Microsoft.Quota/usages/{resourceName}'}  # type: ignore
 
-    def list(
-        self,
-        scope: str,
-        **kwargs: Any
-    ) -> AsyncIterable["_models.UsagesLimits"]:
+    get.metadata = {"url": "/{scope}/providers/Microsoft.Quota/usages/{resourceName}"}  # type: ignore
+
+    @distributed_trace
+    def list(self, scope: str, **kwargs: Any) -> AsyncIterable["_models.CurrentUsagesBase"]:
         """Get a list of current usage for all resources for the scope specified.
 
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either UsagesLimits or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.quota.models.UsagesLimits]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :return: An iterator like instance of either CurrentUsagesBase or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.quota.models.CurrentUsagesBase]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.UsagesLimits"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.UsagesLimits]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
 
-                request = self._client.get(url, query_parameters, header_parameters)
+                request = build_list_request(
+                    scope=scope,
+                    api_version=api_version,
+                    template_url=self.list.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('UsagesLimits', pipeline_response)
+            deserialized = self._deserialize("UsagesLimits", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list.metadata = {'url': '/{scope}/providers/Microsoft.Quota/usages'}  # type: ignore
+        return AsyncItemPaged(get_next, extract_data)
+
+    list.metadata = {"url": "/{scope}/providers/Microsoft.Quota/usages"}  # type: ignore
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/aio/operations/_quota_request_status_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,243 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
-import warnings
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._quota_request_status_operations import build_get_request, build_list_request
 
-T = TypeVar('T')
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-class QuotaRequestStatusOperations:
-    """QuotaRequestStatusOperations async operations.
 
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
+class QuotaRequestStatusOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.quota.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.quota.aio.AzureQuotaExtensionAPI`'s
+        :attr:`quota_request_status` attribute.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def get(
-        self,
-        id: str,
-        scope: str,
-        **kwargs: Any
-    ) -> "_models.QuotaRequestDetails":
+    @distributed_trace_async
+    async def get(self, id: str, scope: str, **kwargs: Any) -> _models.QuotaRequestDetails:
         """Get the quota request details and status by quota request ID for the resources of the resource
         provider at a specific location. The quota request ID **id** is returned in the response of the
         PUT operation.
 
-        :param id: Quota request ID.
+        :param id: Quota request ID. Required.
         :type id: str
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: QuotaRequestDetails, or the result of cls(response)
+        :return: QuotaRequestDetails or the result of cls(response)
         :rtype: ~azure.mgmt.quota.models.QuotaRequestDetails
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.QuotaRequestDetails"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
-        }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'id': self._serialize.url("id", id, 'str'),
-            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        url = self._client.format_url(url, **path_format_arguments)
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.QuotaRequestDetails]
+
+        request = build_get_request(
+            id=id,
+            scope=scope,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)  # type: ignore
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        request = self._client.get(url, query_parameters, header_parameters)
-        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
+            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('QuotaRequestDetails', pipeline_response)
+        deserialized = self._deserialize("QuotaRequestDetails", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
-    get.metadata = {'url': '/{scope}/providers/Microsoft.Quota/quotaRequests/{id}'}  # type: ignore
 
+    get.metadata = {"url": "/{scope}/providers/Microsoft.Quota/quotaRequests/{id}"}  # type: ignore
+
+    @distributed_trace
     def list(
         self,
         scope: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
         skiptoken: Optional[str] = None,
         **kwargs: Any
-    ) -> AsyncIterable["_models.QuotaRequestDetailsList"]:
+    ) -> AsyncIterable["_models.QuotaRequestDetails"]:
         """For the specified scope, get the current quota requests for a one year period ending at the
         time is made. Use the **oData** filter to select quota requests.
 
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
         :param filter: .. list-table::
             :header-rows: 1
 
             * - Field
               - Supported operators
             * -
 
 
          |requestSubmitTime | ge, le, eq, gt, lt
           |provisioningState eq {QuotaRequestState}
-          |resourceName eq {resourceName}.
+          |resourceName eq {resourceName}. Default value is None.
         :type filter: str
-        :param top: Number of records to return.
+        :param top: Number of records to return. Default value is None.
         :type top: int
         :param skiptoken: The **Skiptoken** parameter is used only if a previous operation returned a
          partial result. If a previous response contains a **nextLink** element, its value includes a
-         **skiptoken** parameter that specifies a starting point to use for subsequent calls.
+         **skiptoken** parameter that specifies a starting point to use for subsequent calls. Default
+         value is None.
         :type skiptoken: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either QuotaRequestDetailsList or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.quota.models.QuotaRequestDetailsList]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :return: An iterator like instance of either QuotaRequestDetails or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.quota.models.QuotaRequestDetails]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.QuotaRequestDetailsList"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.QuotaRequestDetailsList]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-                if filter is not None:
-                    query_parameters['$filter'] = self._serialize.query("filter", filter, 'str')
-                if top is not None:
-                    query_parameters['$top'] = self._serialize.query("top", top, 'int', minimum=1)
-                if skiptoken is not None:
-                    query_parameters['$skiptoken'] = self._serialize.query("skiptoken", skiptoken, 'str')
 
-                request = self._client.get(url, query_parameters, header_parameters)
+                request = build_list_request(
+                    scope=scope,
+                    filter=filter,
+                    top=top,
+                    skiptoken=skiptoken,
+                    api_version=api_version,
+                    template_url=self.list.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('QuotaRequestDetailsList', pipeline_response)
+            deserialized = self._deserialize("QuotaRequestDetailsList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(
-            get_next, extract_data
-        )
-    list.metadata = {'url': '/{scope}/providers/Microsoft.Quota/quotaRequests'}  # type: ignore
+        return AsyncItemPaged(get_next, extract_data)
+
+    list.metadata = {"url": "/{scope}/providers/Microsoft.Quota/quotaRequests"}  # type: ignore
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/models/_models_py3.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/models/_models_py3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,641 +1,710 @@
 # coding=utf-8
+# pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import Any, List, Optional, Union
+import sys
+from typing import Any, List, Optional, TYPE_CHECKING, Union
 
-from azure.core.exceptions import HttpResponseError
-import msrest.serialization
+from .. import _serialization
 
-from ._azure_quota_extension_api_enums import *
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from .. import models as _models
+JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
-class CommonResourceProperties(msrest.serialization.Model):
+
+class CommonResourceProperties(_serialization.Model):
     """Resource properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Resource ID.
     :vartype id: str
     :ivar name: Resource name.
     :vartype name: str
     :ivar type: Resource type. Example: "Microsoft.Quota/quotas".
     :vartype type: str
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'type': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        super(CommonResourceProperties, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
 
 
-class CreateGenericQuotaRequestParameters(msrest.serialization.Model):
+class CreateGenericQuotaRequestParameters(_serialization.Model):
     """Quota change requests information.
 
-    :param value: Quota change requests.
-    :type value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+    :ivar value: Quota change requests.
+    :vartype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[CurrentQuotaLimitBase]'},
+        "value": {"key": "value", "type": "[CurrentQuotaLimitBase]"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[List["CurrentQuotaLimitBase"]] = None,
-        **kwargs
-    ):
-        super(CreateGenericQuotaRequestParameters, self).__init__(**kwargs)
+    def __init__(self, *, value: Optional[List["_models.CurrentQuotaLimitBase"]] = None, **kwargs):
+        """
+        :keyword value: Quota change requests.
+        :paramtype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+        """
+        super().__init__(**kwargs)
         self.value = value
 
 
-class CurrentQuotaLimitBase(msrest.serialization.Model):
+class CurrentQuotaLimitBase(_serialization.Model):
     """Quota limit.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: The resource ID.
     :vartype id: str
     :ivar type: The resource type.
     :vartype type: str
     :ivar name: The resource name.
     :vartype name: str
-    :param properties: Quota properties for the specified resource, based on the API called, Quotas
+    :ivar properties: Quota properties for the specified resource, based on the API called, Quotas
      or Usages.
-    :type properties: ~azure.mgmt.quota.models.QuotaProperties
+    :vartype properties: ~azure.mgmt.quota.models.QuotaProperties
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'type': {'readonly': True},
-        'name': {'readonly': True},
+        "id": {"readonly": True},
+        "type": {"readonly": True},
+        "name": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'QuotaProperties'},
+        "id": {"key": "id", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "properties": {"key": "properties", "type": "QuotaProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: Optional["QuotaProperties"] = None,
-        **kwargs
-    ):
-        super(CurrentQuotaLimitBase, self).__init__(**kwargs)
+    def __init__(self, *, properties: Optional["_models.QuotaProperties"] = None, **kwargs):
+        """
+        :keyword properties: Quota properties for the specified resource, based on the API called,
+         Quotas or Usages.
+        :paramtype properties: ~azure.mgmt.quota.models.QuotaProperties
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.type = None
         self.name = None
         self.properties = properties
 
 
-class CurrentUsagesBase(msrest.serialization.Model):
+class CurrentUsagesBase(_serialization.Model):
     """Resource usage.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: The resource ID.
     :vartype id: str
     :ivar type: The resource type.
     :vartype type: str
     :ivar name: The resource name.
     :vartype name: str
-    :param properties: Usage properties for the specified resource.
-    :type properties: ~azure.mgmt.quota.models.UsagesProperties
+    :ivar properties: Usage properties for the specified resource.
+    :vartype properties: ~azure.mgmt.quota.models.UsagesProperties
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'type': {'readonly': True},
-        'name': {'readonly': True},
+        "id": {"readonly": True},
+        "type": {"readonly": True},
+        "name": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'UsagesProperties'},
+        "id": {"key": "id", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "properties": {"key": "properties", "type": "UsagesProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: Optional["UsagesProperties"] = None,
-        **kwargs
-    ):
-        super(CurrentUsagesBase, self).__init__(**kwargs)
+    def __init__(self, *, properties: Optional["_models.UsagesProperties"] = None, **kwargs):
+        """
+        :keyword properties: Usage properties for the specified resource.
+        :paramtype properties: ~azure.mgmt.quota.models.UsagesProperties
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.type = None
         self.name = None
         self.properties = properties
 
 
-class ExceptionResponse(msrest.serialization.Model):
+class ExceptionResponse(_serialization.Model):
     """Error.
 
-    :param error: API error details.
-    :type error: ~azure.mgmt.quota.models.ServiceError
+    :ivar error: API error details.
+    :vartype error: ~azure.mgmt.quota.models.ServiceError
     """
 
     _attribute_map = {
-        'error': {'key': 'error', 'type': 'ServiceError'},
+        "error": {"key": "error", "type": "ServiceError"},
     }
 
-    def __init__(
-        self,
-        *,
-        error: Optional["ServiceError"] = None,
-        **kwargs
-    ):
-        super(ExceptionResponse, self).__init__(**kwargs)
+    def __init__(self, *, error: Optional["_models.ServiceError"] = None, **kwargs):
+        """
+        :keyword error: API error details.
+        :paramtype error: ~azure.mgmt.quota.models.ServiceError
+        """
+        super().__init__(**kwargs)
         self.error = error
 
 
-class LimitJsonObject(msrest.serialization.Model):
+class LimitJsonObject(_serialization.Model):
     """LimitJson abstract class.
 
-    You probably want to use the sub-classes and not this class directly. Known
-    sub-classes are: LimitObject.
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    LimitObject
 
     All required parameters must be populated in order to send to Azure.
 
-    :param limit_object_type: Required. The limit object type.Constant filled by server.  Possible
-     values include: "LimitValue".
-    :type limit_object_type: str or ~azure.mgmt.quota.models.LimitType
+    :ivar limit_object_type: The limit object type. Required. "LimitValue"
+    :vartype limit_object_type: str or ~azure.mgmt.quota.models.LimitType
     """
 
     _validation = {
-        'limit_object_type': {'required': True},
+        "limit_object_type": {"required": True},
     }
 
     _attribute_map = {
-        'limit_object_type': {'key': 'limitObjectType', 'type': 'str'},
+        "limit_object_type": {"key": "limitObjectType", "type": "str"},
     }
 
-    _subtype_map = {
-        'limit_object_type': {'LimitValue': 'LimitObject'}
-    }
+    _subtype_map = {"limit_object_type": {"LimitValue": "LimitObject"}}
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        super(LimitJsonObject, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.limit_object_type = None  # type: Optional[str]
 
 
 class LimitObject(LimitJsonObject):
     """The resource quota limit value.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param limit_object_type: Required. The limit object type.Constant filled by server.  Possible
-     values include: "LimitValue".
-    :type limit_object_type: str or ~azure.mgmt.quota.models.LimitType
-    :param value: Required. The quota/limit value.
-    :type value: int
-    :param limit_type: The quota or usages limit types. Possible values include: "Independent",
+    :ivar limit_object_type: The limit object type. Required. "LimitValue"
+    :vartype limit_object_type: str or ~azure.mgmt.quota.models.LimitType
+    :ivar value: The quota/limit value. Required.
+    :vartype value: int
+    :ivar limit_type: The quota or usages limit types. Known values are: "Independent" and
      "Shared".
-    :type limit_type: str or ~azure.mgmt.quota.models.QuotaLimitTypes
+    :vartype limit_type: str or ~azure.mgmt.quota.models.QuotaLimitTypes
     """
 
     _validation = {
-        'limit_object_type': {'required': True},
-        'value': {'required': True},
+        "limit_object_type": {"required": True},
+        "value": {"required": True},
     }
 
     _attribute_map = {
-        'limit_object_type': {'key': 'limitObjectType', 'type': 'str'},
-        'value': {'key': 'value', 'type': 'int'},
-        'limit_type': {'key': 'limitType', 'type': 'str'},
-    }
-
-    def __init__(
-        self,
-        *,
-        value: int,
-        limit_type: Optional[Union[str, "QuotaLimitTypes"]] = None,
-        **kwargs
-    ):
-        super(LimitObject, self).__init__(**kwargs)
-        self.limit_object_type = 'LimitValue'  # type: str
+        "limit_object_type": {"key": "limitObjectType", "type": "str"},
+        "value": {"key": "value", "type": "int"},
+        "limit_type": {"key": "limitType", "type": "str"},
+    }
+
+    def __init__(self, *, value: int, limit_type: Optional[Union[str, "_models.QuotaLimitTypes"]] = None, **kwargs):
+        """
+        :keyword value: The quota/limit value. Required.
+        :paramtype value: int
+        :keyword limit_type: The quota or usages limit types. Known values are: "Independent" and
+         "Shared".
+        :paramtype limit_type: str or ~azure.mgmt.quota.models.QuotaLimitTypes
+        """
+        super().__init__(**kwargs)
+        self.limit_object_type = "LimitValue"  # type: str
         self.value = value
         self.limit_type = limit_type
 
 
-class OperationDisplay(msrest.serialization.Model):
+class OperationDisplay(_serialization.Model):
     """OperationDisplay.
 
-    :param provider: Provider name.
-    :type provider: str
-    :param resource: Resource name.
-    :type resource: str
-    :param operation: Operation name.
-    :type operation: str
-    :param description: Operation description.
-    :type description: str
+    :ivar provider: Provider name.
+    :vartype provider: str
+    :ivar resource: Resource name.
+    :vartype resource: str
+    :ivar operation: Operation name.
+    :vartype operation: str
+    :ivar description: Operation description.
+    :vartype description: str
     """
 
     _attribute_map = {
-        'provider': {'key': 'provider', 'type': 'str'},
-        'resource': {'key': 'resource', 'type': 'str'},
-        'operation': {'key': 'operation', 'type': 'str'},
-        'description': {'key': 'description', 'type': 'str'},
+        "provider": {"key": "provider", "type": "str"},
+        "resource": {"key": "resource", "type": "str"},
+        "operation": {"key": "operation", "type": "str"},
+        "description": {"key": "description", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
         **kwargs
     ):
-        super(OperationDisplay, self).__init__(**kwargs)
+        """
+        :keyword provider: Provider name.
+        :paramtype provider: str
+        :keyword resource: Resource name.
+        :paramtype resource: str
+        :keyword operation: Operation name.
+        :paramtype operation: str
+        :keyword description: Operation description.
+        :paramtype description: str
+        """
+        super().__init__(**kwargs)
         self.provider = provider
         self.resource = resource
         self.operation = operation
         self.description = description
 
 
-class OperationList(msrest.serialization.Model):
+class OperationList(_serialization.Model):
     """OperationList.
 
-    :param value:
-    :type value: list[~azure.mgmt.quota.models.OperationResponse]
-    :param next_link: URL to get the next page of items.
-    :type next_link: str
+    :ivar value:
+    :vartype value: list[~azure.mgmt.quota.models.OperationResponse]
+    :ivar next_link: URL to get the next page of items.
+    :vartype next_link: str
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[OperationResponse]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[OperationResponse]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self,
-        *,
-        value: Optional[List["OperationResponse"]] = None,
-        next_link: Optional[str] = None,
-        **kwargs
+        self, *, value: Optional[List["_models.OperationResponse"]] = None, next_link: Optional[str] = None, **kwargs
     ):
-        super(OperationList, self).__init__(**kwargs)
+        """
+        :keyword value:
+        :paramtype value: list[~azure.mgmt.quota.models.OperationResponse]
+        :keyword next_link: URL to get the next page of items.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class OperationResponse(msrest.serialization.Model):
+class OperationResponse(_serialization.Model):
     """OperationResponse.
 
-    :param name:
-    :type name: str
-    :param display:
-    :type display: ~azure.mgmt.quota.models.OperationDisplay
-    :param origin:
-    :type origin: str
+    :ivar name:
+    :vartype name: str
+    :ivar display:
+    :vartype display: ~azure.mgmt.quota.models.OperationDisplay
+    :ivar origin:
+    :vartype origin: str
     """
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'str'},
-        'display': {'key': 'display', 'type': 'OperationDisplay'},
-        'origin': {'key': 'origin', 'type': 'str'},
+        "name": {"key": "name", "type": "str"},
+        "display": {"key": "display", "type": "OperationDisplay"},
+        "origin": {"key": "origin", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
-        display: Optional["OperationDisplay"] = None,
+        display: Optional["_models.OperationDisplay"] = None,
         origin: Optional[str] = None,
         **kwargs
     ):
-        super(OperationResponse, self).__init__(**kwargs)
+        """
+        :keyword name:
+        :paramtype name: str
+        :keyword display:
+        :paramtype display: ~azure.mgmt.quota.models.OperationDisplay
+        :keyword origin:
+        :paramtype origin: str
+        """
+        super().__init__(**kwargs)
         self.name = name
         self.display = display
         self.origin = origin
 
 
-class QuotaLimits(msrest.serialization.Model):
+class QuotaLimits(_serialization.Model):
     """Quota limits.
 
-    :param value: List of quota limits.
-    :type value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
-    :param next_link: The URI used to fetch the next page of quota limits. When there are no more
+    :ivar value: List of quota limits.
+    :vartype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+    :ivar next_link: The URI used to fetch the next page of quota limits. When there are no more
      pages, this string is null.
-    :type next_link: str
+    :vartype next_link: str
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[CurrentQuotaLimitBase]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[CurrentQuotaLimitBase]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        value: Optional[List["CurrentQuotaLimitBase"]] = None,
+        value: Optional[List["_models.CurrentQuotaLimitBase"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
-        super(QuotaLimits, self).__init__(**kwargs)
+        """
+        :keyword value: List of quota limits.
+        :paramtype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+        :keyword next_link: The URI used to fetch the next page of quota limits. When there are no more
+         pages, this string is null.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class QuotaLimitsResponse(msrest.serialization.Model):
+class QuotaLimitsResponse(_serialization.Model):
     """Quota limits request response.
 
-    :param value: List of quota limits with the quota request status.
-    :type value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
-    :param next_link: The URI used to fetch the next page of quota limits. When there are no more
+    :ivar value: List of quota limits with the quota request status.
+    :vartype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+    :ivar next_link: The URI used to fetch the next page of quota limits. When there are no more
      pages, this is null.
-    :type next_link: str
+    :vartype next_link: str
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[CurrentQuotaLimitBase]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[CurrentQuotaLimitBase]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        value: Optional[List["CurrentQuotaLimitBase"]] = None,
+        value: Optional[List["_models.CurrentQuotaLimitBase"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
-        super(QuotaLimitsResponse, self).__init__(**kwargs)
+        """
+        :keyword value: List of quota limits with the quota request status.
+        :paramtype value: list[~azure.mgmt.quota.models.CurrentQuotaLimitBase]
+        :keyword next_link: The URI used to fetch the next page of quota limits. When there are no more
+         pages, this is null.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class QuotaProperties(msrest.serialization.Model):
+class QuotaProperties(_serialization.Model):
     """Quota properties for the specified resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param limit: Resource quota limit properties.
-    :type limit: ~azure.mgmt.quota.models.LimitJsonObject
+    :ivar limit: Resource quota limit properties.
+    :vartype limit: ~azure.mgmt.quota.models.LimitJsonObject
     :ivar unit: The quota units, such as Count and Bytes. When requesting quota, use the **unit**
      value returned in the GET response in the request body of your PUT operation.
     :vartype unit: str
-    :param name: Resource name provided by the resource provider. Use this property name when
+    :ivar name: Resource name provided by the resource provider. Use this property name when
      requesting quota.
-    :type name: ~azure.mgmt.quota.models.ResourceName
-    :param resource_type: Resource type name.
-    :type resource_type: str
+    :vartype name: ~azure.mgmt.quota.models.ResourceName
+    :ivar resource_type: Resource type name.
+    :vartype resource_type: str
     :ivar quota_period: The time period over which the quota usage values are summarized. For
      example:
      *P1D (per one day)*\ PT1M (per one minute)
      *PT1S (per one second).
      This parameter is optional because, for some resources like compute, the period is irrelevant.
     :vartype quota_period: str
     :ivar is_quota_applicable: States if quota can be requested for this resource.
     :vartype is_quota_applicable: bool
-    :param properties: Additional properties for the specific resource provider.
-    :type properties: any
+    :ivar properties: Additional properties for the specific resource provider.
+    :vartype properties: JSON
     """
 
     _validation = {
-        'unit': {'readonly': True},
-        'quota_period': {'readonly': True},
-        'is_quota_applicable': {'readonly': True},
+        "unit": {"readonly": True},
+        "quota_period": {"readonly": True},
+        "is_quota_applicable": {"readonly": True},
     }
 
     _attribute_map = {
-        'limit': {'key': 'limit', 'type': 'LimitJsonObject'},
-        'unit': {'key': 'unit', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'ResourceName'},
-        'resource_type': {'key': 'resourceType', 'type': 'str'},
-        'quota_period': {'key': 'quotaPeriod', 'type': 'str'},
-        'is_quota_applicable': {'key': 'isQuotaApplicable', 'type': 'bool'},
-        'properties': {'key': 'properties', 'type': 'object'},
+        "limit": {"key": "limit", "type": "LimitJsonObject"},
+        "unit": {"key": "unit", "type": "str"},
+        "name": {"key": "name", "type": "ResourceName"},
+        "resource_type": {"key": "resourceType", "type": "str"},
+        "quota_period": {"key": "quotaPeriod", "type": "str"},
+        "is_quota_applicable": {"key": "isQuotaApplicable", "type": "bool"},
+        "properties": {"key": "properties", "type": "object"},
     }
 
     def __init__(
         self,
         *,
-        limit: Optional["LimitJsonObject"] = None,
-        name: Optional["ResourceName"] = None,
+        limit: Optional["_models.LimitJsonObject"] = None,
+        name: Optional["_models.ResourceName"] = None,
         resource_type: Optional[str] = None,
-        properties: Optional[Any] = None,
+        properties: Optional[JSON] = None,
         **kwargs
     ):
-        super(QuotaProperties, self).__init__(**kwargs)
+        """
+        :keyword limit: Resource quota limit properties.
+        :paramtype limit: ~azure.mgmt.quota.models.LimitJsonObject
+        :keyword name: Resource name provided by the resource provider. Use this property name when
+         requesting quota.
+        :paramtype name: ~azure.mgmt.quota.models.ResourceName
+        :keyword resource_type: Resource type name.
+        :paramtype resource_type: str
+        :keyword properties: Additional properties for the specific resource provider.
+        :paramtype properties: JSON
+        """
+        super().__init__(**kwargs)
         self.limit = limit
         self.unit = None
         self.name = name
         self.resource_type = resource_type
         self.quota_period = None
         self.is_quota_applicable = None
         self.properties = properties
 
 
-class QuotaRequestDetails(msrest.serialization.Model):
+class QuotaRequestDetails(_serialization.Model):
     """List of quota requests with details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Quota request ID.
     :vartype id: str
     :ivar name: Quota request name.
     :vartype name: str
     :ivar type: Resource type. "Microsoft.Quota/quotas".
     :vartype type: str
-    :ivar provisioning_state: The quota request status. Possible values include: "Accepted",
-     "Invalid", "Succeeded", "Failed", "InProgress".
+    :ivar provisioning_state: The quota request status. Known values are: "Accepted", "Invalid",
+     "Succeeded", "Failed", and "InProgress".
     :vartype provisioning_state: str or ~azure.mgmt.quota.models.QuotaRequestState
     :ivar message: User-friendly status message.
     :vartype message: str
-    :param error: Error details of the quota request.
-    :type error: ~azure.mgmt.quota.models.ServiceErrorDetail
+    :ivar error: Error details of the quota request.
+    :vartype error: ~azure.mgmt.quota.models.ServiceErrorDetail
     :ivar request_submit_time: The quota request submission time. The date conforms to the
      following format specified by the ISO 8601 standard: yyyy-MM-ddTHH:mm:ssZ.
     :vartype request_submit_time: ~datetime.datetime
-    :param value: Quota request details.
-    :type value: list[~azure.mgmt.quota.models.SubRequest]
+    :ivar value: Quota request details.
+    :vartype value: list[~azure.mgmt.quota.models.SubRequest]
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'type': {'readonly': True},
-        'provisioning_state': {'readonly': True},
-        'message': {'readonly': True},
-        'request_submit_time': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "message": {"readonly": True},
+        "request_submit_time": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
-        'message': {'key': 'properties.message', 'type': 'str'},
-        'error': {'key': 'properties.error', 'type': 'ServiceErrorDetail'},
-        'request_submit_time': {'key': 'properties.requestSubmitTime', 'type': 'iso-8601'},
-        'value': {'key': 'properties.value', 'type': '[SubRequest]'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "message": {"key": "properties.message", "type": "str"},
+        "error": {"key": "properties.error", "type": "ServiceErrorDetail"},
+        "request_submit_time": {"key": "properties.requestSubmitTime", "type": "iso-8601"},
+        "value": {"key": "properties.value", "type": "[SubRequest]"},
     }
 
     def __init__(
         self,
         *,
-        error: Optional["ServiceErrorDetail"] = None,
-        value: Optional[List["SubRequest"]] = None,
+        error: Optional["_models.ServiceErrorDetail"] = None,
+        value: Optional[List["_models.SubRequest"]] = None,
         **kwargs
     ):
-        super(QuotaRequestDetails, self).__init__(**kwargs)
+        """
+        :keyword error: Error details of the quota request.
+        :paramtype error: ~azure.mgmt.quota.models.ServiceErrorDetail
+        :keyword value: Quota request details.
+        :paramtype value: list[~azure.mgmt.quota.models.SubRequest]
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.provisioning_state = None
         self.message = None
         self.error = error
         self.request_submit_time = None
         self.value = value
 
 
-class QuotaRequestDetailsList(msrest.serialization.Model):
+class QuotaRequestDetailsList(_serialization.Model):
     """Quota request information.
 
-    :param value: Quota request details.
-    :type value: list[~azure.mgmt.quota.models.QuotaRequestDetails]
-    :param next_link: The URI for fetching the next page of quota limits. When there are no more
+    :ivar value: Quota request details.
+    :vartype value: list[~azure.mgmt.quota.models.QuotaRequestDetails]
+    :ivar next_link: The URI for fetching the next page of quota limits. When there are no more
      pages, this string is null.
-    :type next_link: str
+    :vartype next_link: str
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[QuotaRequestDetails]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[QuotaRequestDetails]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self,
-        *,
-        value: Optional[List["QuotaRequestDetails"]] = None,
-        next_link: Optional[str] = None,
-        **kwargs
+        self, *, value: Optional[List["_models.QuotaRequestDetails"]] = None, next_link: Optional[str] = None, **kwargs
     ):
-        super(QuotaRequestDetailsList, self).__init__(**kwargs)
+        """
+        :keyword value: Quota request details.
+        :paramtype value: list[~azure.mgmt.quota.models.QuotaRequestDetails]
+        :keyword next_link: The URI for fetching the next page of quota limits. When there are no more
+         pages, this string is null.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class QuotaRequestOneResourceSubmitResponse(msrest.serialization.Model):
+class QuotaRequestOneResourceSubmitResponse(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Quota request response.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Quota request ID.
     :vartype id: str
     :ivar name: The name of the quota request.
     :vartype name: str
     :ivar type: Resource type. "Microsoft.Quota/ServiceLimitRequests".
     :vartype type: str
-    :ivar provisioning_state: Quota request status. Possible values include: "Accepted", "Invalid",
-     "Succeeded", "Failed", "InProgress".
+    :ivar provisioning_state: Quota request status. Known values are: "Accepted", "Invalid",
+     "Succeeded", "Failed", and "InProgress".
     :vartype provisioning_state: str or ~azure.mgmt.quota.models.QuotaRequestState
     :ivar message: User-friendly status message.
     :vartype message: str
     :ivar request_submit_time: Quota request submission time. The date conforms to the following
      ISO 8601 standard format: yyyy-MM-ddTHH:mm:ssZ.
     :vartype request_submit_time: ~datetime.datetime
-    :param limit: Resource quota limit properties.
-    :type limit: ~azure.mgmt.quota.models.LimitObject
+    :ivar limit: Resource quota limit properties.
+    :vartype limit: ~azure.mgmt.quota.models.LimitObject
     :ivar current_value: Usage information for the current resource.
     :vartype current_value: int
-    :param unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
+    :ivar unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
      **unit** value returned in the GET response in the request body of your PUT operation.
-    :type unit: str
-    :param name_properties_name: Resource name provided by the resource provider. Use this property
+    :vartype unit: str
+    :ivar name_properties_name: Resource name provided by the resource provider. Use this property
      name when requesting quota.
-    :type name_properties_name: ~azure.mgmt.quota.models.ResourceName
-    :param resource_type: Resource type name.
-    :type resource_type: str
+    :vartype name_properties_name: ~azure.mgmt.quota.models.ResourceName
+    :ivar resource_type: Resource type name.
+    :vartype resource_type: str
     :ivar quota_period: The time period over which the quota usage values are summarized. For
      example:
      *P1D (per one day)*\ PT1M (per one minute)
      *PT1S (per one second).
      This parameter is optional because, for some resources like compute, the period is irrelevant.
     :vartype quota_period: str
     :ivar is_quota_applicable: States if quota can be requested for this resource.
     :vartype is_quota_applicable: bool
-    :param error: Error details of the quota request.
-    :type error: ~azure.mgmt.quota.models.ServiceErrorDetail
-    :param properties: Additional properties for the specific resource provider.
-    :type properties: any
+    :ivar error: Error details of the quota request.
+    :vartype error: ~azure.mgmt.quota.models.ServiceErrorDetail
+    :ivar properties: Additional properties for the specific resource provider.
+    :vartype properties: JSON
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'type': {'readonly': True},
-        'provisioning_state': {'readonly': True},
-        'message': {'readonly': True},
-        'request_submit_time': {'readonly': True},
-        'current_value': {'readonly': True},
-        'quota_period': {'readonly': True},
-        'is_quota_applicable': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "message": {"readonly": True},
+        "request_submit_time": {"readonly": True},
+        "current_value": {"readonly": True},
+        "quota_period": {"readonly": True},
+        "is_quota_applicable": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
-        'message': {'key': 'properties.message', 'type': 'str'},
-        'request_submit_time': {'key': 'properties.requestSubmitTime', 'type': 'iso-8601'},
-        'limit': {'key': 'properties.limit', 'type': 'LimitObject'},
-        'current_value': {'key': 'properties.currentValue', 'type': 'int'},
-        'unit': {'key': 'properties.unit', 'type': 'str'},
-        'name_properties_name': {'key': 'properties.name', 'type': 'ResourceName'},
-        'resource_type': {'key': 'properties.resourceType', 'type': 'str'},
-        'quota_period': {'key': 'properties.quotaPeriod', 'type': 'str'},
-        'is_quota_applicable': {'key': 'properties.isQuotaApplicable', 'type': 'bool'},
-        'error': {'key': 'properties.error', 'type': 'ServiceErrorDetail'},
-        'properties': {'key': 'properties.properties', 'type': 'object'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "message": {"key": "properties.message", "type": "str"},
+        "request_submit_time": {"key": "properties.requestSubmitTime", "type": "iso-8601"},
+        "limit": {"key": "properties.limit", "type": "LimitObject"},
+        "current_value": {"key": "properties.currentValue", "type": "int"},
+        "unit": {"key": "properties.unit", "type": "str"},
+        "name_properties_name": {"key": "properties.name", "type": "ResourceName"},
+        "resource_type": {"key": "properties.resourceType", "type": "str"},
+        "quota_period": {"key": "properties.quotaPeriod", "type": "str"},
+        "is_quota_applicable": {"key": "properties.isQuotaApplicable", "type": "bool"},
+        "error": {"key": "properties.error", "type": "ServiceErrorDetail"},
+        "properties": {"key": "properties.properties", "type": "object"},
     }
 
     def __init__(
         self,
         *,
-        limit: Optional["LimitObject"] = None,
+        limit: Optional["_models.LimitObject"] = None,
         unit: Optional[str] = None,
-        name_properties_name: Optional["ResourceName"] = None,
+        name_properties_name: Optional["_models.ResourceName"] = None,
         resource_type: Optional[str] = None,
-        error: Optional["ServiceErrorDetail"] = None,
-        properties: Optional[Any] = None,
+        error: Optional["_models.ServiceErrorDetail"] = None,
+        properties: Optional[JSON] = None,
         **kwargs
     ):
-        super(QuotaRequestOneResourceSubmitResponse, self).__init__(**kwargs)
+        """
+        :keyword limit: Resource quota limit properties.
+        :paramtype limit: ~azure.mgmt.quota.models.LimitObject
+        :keyword unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
+         **unit** value returned in the GET response in the request body of your PUT operation.
+        :paramtype unit: str
+        :keyword name_properties_name: Resource name provided by the resource provider. Use this
+         property name when requesting quota.
+        :paramtype name_properties_name: ~azure.mgmt.quota.models.ResourceName
+        :keyword resource_type: Resource type name.
+        :paramtype resource_type: str
+        :keyword error: Error details of the quota request.
+        :paramtype error: ~azure.mgmt.quota.models.ServiceErrorDetail
+        :keyword properties: Additional properties for the specific resource provider.
+        :paramtype properties: JSON
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.provisioning_state = None
         self.message = None
         self.request_submit_time = None
         self.limit = limit
@@ -645,456 +714,496 @@
         self.resource_type = resource_type
         self.quota_period = None
         self.is_quota_applicable = None
         self.error = error
         self.properties = properties
 
 
-class QuotaRequestProperties(msrest.serialization.Model):
+class QuotaRequestProperties(_serialization.Model):
     """Quota request properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar provisioning_state: The quota request status. Possible values include: "Accepted",
-     "Invalid", "Succeeded", "Failed", "InProgress".
+    :ivar provisioning_state: The quota request status. Known values are: "Accepted", "Invalid",
+     "Succeeded", "Failed", and "InProgress".
     :vartype provisioning_state: str or ~azure.mgmt.quota.models.QuotaRequestState
     :ivar message: User-friendly status message.
     :vartype message: str
-    :param error: Error details of the quota request.
-    :type error: ~azure.mgmt.quota.models.ServiceErrorDetail
+    :ivar error: Error details of the quota request.
+    :vartype error: ~azure.mgmt.quota.models.ServiceErrorDetail
     :ivar request_submit_time: The quota request submission time. The date conforms to the
      following format specified by the ISO 8601 standard: yyyy-MM-ddTHH:mm:ssZ.
     :vartype request_submit_time: ~datetime.datetime
-    :param value: Quota request details.
-    :type value: list[~azure.mgmt.quota.models.SubRequest]
+    :ivar value: Quota request details.
+    :vartype value: list[~azure.mgmt.quota.models.SubRequest]
     """
 
     _validation = {
-        'provisioning_state': {'readonly': True},
-        'message': {'readonly': True},
-        'request_submit_time': {'readonly': True},
+        "provisioning_state": {"readonly": True},
+        "message": {"readonly": True},
+        "request_submit_time": {"readonly": True},
     }
 
     _attribute_map = {
-        'provisioning_state': {'key': 'provisioningState', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
-        'error': {'key': 'error', 'type': 'ServiceErrorDetail'},
-        'request_submit_time': {'key': 'requestSubmitTime', 'type': 'iso-8601'},
-        'value': {'key': 'value', 'type': '[SubRequest]'},
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "error": {"key": "error", "type": "ServiceErrorDetail"},
+        "request_submit_time": {"key": "requestSubmitTime", "type": "iso-8601"},
+        "value": {"key": "value", "type": "[SubRequest]"},
     }
 
     def __init__(
         self,
         *,
-        error: Optional["ServiceErrorDetail"] = None,
-        value: Optional[List["SubRequest"]] = None,
+        error: Optional["_models.ServiceErrorDetail"] = None,
+        value: Optional[List["_models.SubRequest"]] = None,
         **kwargs
     ):
-        super(QuotaRequestProperties, self).__init__(**kwargs)
+        """
+        :keyword error: Error details of the quota request.
+        :paramtype error: ~azure.mgmt.quota.models.ServiceErrorDetail
+        :keyword value: Quota request details.
+        :paramtype value: list[~azure.mgmt.quota.models.SubRequest]
+        """
+        super().__init__(**kwargs)
         self.provisioning_state = None
         self.message = None
         self.error = error
         self.request_submit_time = None
         self.value = value
 
 
-class QuotaRequestSubmitResponse(msrest.serialization.Model):
+class QuotaRequestSubmitResponse(_serialization.Model):
     """Quota request response.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Quota request ID.
     :vartype id: str
     :ivar name: Quota request name.
     :vartype name: str
-    :param properties: Quota request details.
-    :type properties: ~azure.mgmt.quota.models.QuotaRequestProperties
+    :ivar properties: Quota request details.
+    :vartype properties: ~azure.mgmt.quota.models.QuotaRequestProperties
     :ivar type: Resource type. "Microsoft.Quota/quotas".
     :vartype type: str
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'type': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'properties': {'key': 'properties', 'type': 'QuotaRequestProperties'},
-        'type': {'key': 'type', 'type': 'str'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "properties": {"key": "properties", "type": "QuotaRequestProperties"},
+        "type": {"key": "type", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        properties: Optional["QuotaRequestProperties"] = None,
-        **kwargs
-    ):
-        super(QuotaRequestSubmitResponse, self).__init__(**kwargs)
+    def __init__(self, *, properties: Optional["_models.QuotaRequestProperties"] = None, **kwargs):
+        """
+        :keyword properties: Quota request details.
+        :paramtype properties: ~azure.mgmt.quota.models.QuotaRequestProperties
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.properties = properties
         self.type = None
 
 
-class QuotaRequestSubmitResponse202(msrest.serialization.Model):
+class QuotaRequestSubmitResponse202(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """The quota request response with the quota request ID.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: The quota request ID. To check the request status, use the **id** value in a `Quota
      Request Status
      <https://docs.microsoft.com/en-us/rest/api/reserved-vm-instances/quotarequeststatus/get>`_ GET
      operation.
     :vartype id: str
     :ivar name: Operation ID.
     :vartype name: str
     :ivar type: Resource type.
     :vartype type: str
-    :ivar provisioning_state: Quota request status. Possible values include: "Accepted", "Invalid",
-     "Succeeded", "Failed", "InProgress".
+    :ivar provisioning_state: Quota request status. Known values are: "Accepted", "Invalid",
+     "Succeeded", "Failed", and "InProgress".
     :vartype provisioning_state: str or ~azure.mgmt.quota.models.QuotaRequestState
     :ivar message: User-friendly message.
     :vartype message: str
-    :param limit: Resource quota limit properties.
-    :type limit: ~azure.mgmt.quota.models.LimitObject
-    :param unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
+    :ivar limit: Resource quota limit properties.
+    :vartype limit: ~azure.mgmt.quota.models.LimitObject
+    :ivar unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
      **unit** value returned in the GET response in the request body of your PUT operation.
-    :type unit: str
-    :param name_properties_name: Resource name provided by the resource provider. Use this property
+    :vartype unit: str
+    :ivar name_properties_name: Resource name provided by the resource provider. Use this property
      name when requesting quota.
-    :type name_properties_name: ~azure.mgmt.quota.models.ResourceName
-    :param resource_type: Resource type name.
-    :type resource_type: str
+    :vartype name_properties_name: ~azure.mgmt.quota.models.ResourceName
+    :ivar resource_type: Resource type name.
+    :vartype resource_type: str
     :ivar quota_period: The time period over which the quota usage values are summarized. For
      example:
      *P1D (per one day)*\ PT1M (per one minute)
      *PT1S (per one second).
      This parameter is optional because, for some resources like compute, the period is irrelevant.
     :vartype quota_period: str
-    :param properties: Additional properties for the specific resource provider.
-    :type properties: any
+    :ivar properties: Additional properties for the specific resource provider.
+    :vartype properties: JSON
     """
 
     _validation = {
-        'id': {'readonly': True},
-        'name': {'readonly': True},
-        'type': {'readonly': True},
-        'provisioning_state': {'readonly': True},
-        'message': {'readonly': True},
-        'quota_period': {'readonly': True},
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "message": {"readonly": True},
+        "quota_period": {"readonly": True},
     }
 
     _attribute_map = {
-        'id': {'key': 'id', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'str'},
-        'type': {'key': 'type', 'type': 'str'},
-        'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
-        'message': {'key': 'properties.message', 'type': 'str'},
-        'limit': {'key': 'properties.limit', 'type': 'LimitObject'},
-        'unit': {'key': 'properties.unit', 'type': 'str'},
-        'name_properties_name': {'key': 'properties.name', 'type': 'ResourceName'},
-        'resource_type': {'key': 'properties.resourceType', 'type': 'str'},
-        'quota_period': {'key': 'properties.quotaPeriod', 'type': 'str'},
-        'properties': {'key': 'properties.properties', 'type': 'object'},
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "message": {"key": "properties.message", "type": "str"},
+        "limit": {"key": "properties.limit", "type": "LimitObject"},
+        "unit": {"key": "properties.unit", "type": "str"},
+        "name_properties_name": {"key": "properties.name", "type": "ResourceName"},
+        "resource_type": {"key": "properties.resourceType", "type": "str"},
+        "quota_period": {"key": "properties.quotaPeriod", "type": "str"},
+        "properties": {"key": "properties.properties", "type": "object"},
     }
 
     def __init__(
         self,
         *,
-        limit: Optional["LimitObject"] = None,
+        limit: Optional["_models.LimitObject"] = None,
         unit: Optional[str] = None,
-        name_properties_name: Optional["ResourceName"] = None,
+        name_properties_name: Optional["_models.ResourceName"] = None,
         resource_type: Optional[str] = None,
-        properties: Optional[Any] = None,
+        properties: Optional[JSON] = None,
         **kwargs
     ):
-        super(QuotaRequestSubmitResponse202, self).__init__(**kwargs)
+        """
+        :keyword limit: Resource quota limit properties.
+        :paramtype limit: ~azure.mgmt.quota.models.LimitObject
+        :keyword unit: The quota limit units, such as Count and Bytes. When requesting quota, use the
+         **unit** value returned in the GET response in the request body of your PUT operation.
+        :paramtype unit: str
+        :keyword name_properties_name: Resource name provided by the resource provider. Use this
+         property name when requesting quota.
+        :paramtype name_properties_name: ~azure.mgmt.quota.models.ResourceName
+        :keyword resource_type: Resource type name.
+        :paramtype resource_type: str
+        :keyword properties: Additional properties for the specific resource provider.
+        :paramtype properties: JSON
+        """
+        super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.provisioning_state = None
         self.message = None
         self.limit = limit
         self.unit = unit
         self.name_properties_name = name_properties_name
         self.resource_type = resource_type
         self.quota_period = None
         self.properties = properties
 
 
-class ResourceName(msrest.serialization.Model):
+class ResourceName(_serialization.Model):
     """Name of the resource provided by the resource Provider. When requesting quota, use this property name.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param value: Resource name.
-    :type value: str
+    :ivar value: Resource name.
+    :vartype value: str
     :ivar localized_value: Resource display name.
     :vartype localized_value: str
     """
 
     _validation = {
-        'localized_value': {'readonly': True},
+        "localized_value": {"readonly": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': 'str'},
-        'localized_value': {'key': 'localizedValue', 'type': 'str'},
+        "value": {"key": "value", "type": "str"},
+        "localized_value": {"key": "localizedValue", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: Optional[str] = None,
-        **kwargs
-    ):
-        super(ResourceName, self).__init__(**kwargs)
+    def __init__(self, *, value: Optional[str] = None, **kwargs):
+        """
+        :keyword value: Resource name.
+        :paramtype value: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.localized_value = None
 
 
-class ServiceError(msrest.serialization.Model):
+class ServiceError(_serialization.Model):
     """API error details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param code: Error code.
-    :type code: str
-    :param message: Error message.
-    :type message: str
+    :ivar code: Error code.
+    :vartype code: str
+    :ivar message: Error message.
+    :vartype message: str
     :ivar details: List of error details.
     :vartype details: list[~azure.mgmt.quota.models.ServiceErrorDetail]
     """
 
     _validation = {
-        'details': {'readonly': True},
+        "details": {"readonly": True},
     }
 
     _attribute_map = {
-        'code': {'key': 'code', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
-        'details': {'key': 'details', 'type': '[ServiceErrorDetail]'},
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "details": {"key": "details", "type": "[ServiceErrorDetail]"},
     }
 
-    def __init__(
-        self,
-        *,
-        code: Optional[str] = None,
-        message: Optional[str] = None,
-        **kwargs
-    ):
-        super(ServiceError, self).__init__(**kwargs)
+    def __init__(self, *, code: Optional[str] = None, message: Optional[str] = None, **kwargs):
+        """
+        :keyword code: Error code.
+        :paramtype code: str
+        :keyword message: Error message.
+        :paramtype message: str
+        """
+        super().__init__(**kwargs)
         self.code = code
         self.message = message
         self.details = None
 
 
-class ServiceErrorDetail(msrest.serialization.Model):
+class ServiceErrorDetail(_serialization.Model):
     """Error details.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar code: Error code.
     :vartype code: str
     :ivar message: Error message.
     :vartype message: str
     """
 
     _validation = {
-        'code': {'readonly': True},
-        'message': {'readonly': True},
+        "code": {"readonly": True},
+        "message": {"readonly": True},
     }
 
     _attribute_map = {
-        'code': {'key': 'code', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
     }
 
-    def __init__(
-        self,
-        **kwargs
-    ):
-        super(ServiceErrorDetail, self).__init__(**kwargs)
+    def __init__(self, **kwargs):
+        """ """
+        super().__init__(**kwargs)
         self.code = None
         self.message = None
 
 
-class SubRequest(msrest.serialization.Model):
+class SubRequest(_serialization.Model):
     """Request property.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param name: Resource name.
-    :type name: ~azure.mgmt.quota.models.ResourceName
+    :ivar name: Resource name.
+    :vartype name: ~azure.mgmt.quota.models.ResourceName
     :ivar resource_type: Resource type for which the quota properties were requested.
     :vartype resource_type: str
-    :param unit: Quota limit units, such as Count and Bytes. When requesting quota, use the
-     **unit** value returned in the GET response in the request body of your PUT operation.
-    :type unit: str
-    :ivar provisioning_state: The quota request status. Possible values include: "Accepted",
-     "Invalid", "Succeeded", "Failed", "InProgress".
+    :ivar unit: Quota limit units, such as Count and Bytes. When requesting quota, use the **unit**
+     value returned in the GET response in the request body of your PUT operation.
+    :vartype unit: str
+    :ivar provisioning_state: The quota request status. Known values are: "Accepted", "Invalid",
+     "Succeeded", "Failed", and "InProgress".
     :vartype provisioning_state: str or ~azure.mgmt.quota.models.QuotaRequestState
     :ivar message: User-friendly status message.
     :vartype message: str
     :ivar sub_request_id: Quota request ID.
     :vartype sub_request_id: str
-    :param limit: Resource quota limit properties.
-    :type limit: ~azure.mgmt.quota.models.LimitJsonObject
+    :ivar limit: Resource quota limit properties.
+    :vartype limit: ~azure.mgmt.quota.models.LimitJsonObject
     """
 
     _validation = {
-        'resource_type': {'readonly': True},
-        'provisioning_state': {'readonly': True},
-        'message': {'readonly': True},
-        'sub_request_id': {'readonly': True},
+        "resource_type": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "message": {"readonly": True},
+        "sub_request_id": {"readonly": True},
     }
 
     _attribute_map = {
-        'name': {'key': 'name', 'type': 'ResourceName'},
-        'resource_type': {'key': 'resourceType', 'type': 'str'},
-        'unit': {'key': 'unit', 'type': 'str'},
-        'provisioning_state': {'key': 'provisioningState', 'type': 'str'},
-        'message': {'key': 'message', 'type': 'str'},
-        'sub_request_id': {'key': 'subRequestId', 'type': 'str'},
-        'limit': {'key': 'limit', 'type': 'LimitJsonObject'},
+        "name": {"key": "name", "type": "ResourceName"},
+        "resource_type": {"key": "resourceType", "type": "str"},
+        "unit": {"key": "unit", "type": "str"},
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "sub_request_id": {"key": "subRequestId", "type": "str"},
+        "limit": {"key": "limit", "type": "LimitJsonObject"},
     }
 
     def __init__(
         self,
         *,
-        name: Optional["ResourceName"] = None,
+        name: Optional["_models.ResourceName"] = None,
         unit: Optional[str] = None,
-        limit: Optional["LimitJsonObject"] = None,
+        limit: Optional["_models.LimitJsonObject"] = None,
         **kwargs
     ):
-        super(SubRequest, self).__init__(**kwargs)
+        """
+        :keyword name: Resource name.
+        :paramtype name: ~azure.mgmt.quota.models.ResourceName
+        :keyword unit: Quota limit units, such as Count and Bytes. When requesting quota, use the
+         **unit** value returned in the GET response in the request body of your PUT operation.
+        :paramtype unit: str
+        :keyword limit: Resource quota limit properties.
+        :paramtype limit: ~azure.mgmt.quota.models.LimitJsonObject
+        """
+        super().__init__(**kwargs)
         self.name = name
         self.resource_type = None
         self.unit = unit
         self.provisioning_state = None
         self.message = None
         self.sub_request_id = None
         self.limit = limit
 
 
-class UsagesLimits(msrest.serialization.Model):
+class UsagesLimits(_serialization.Model):
     """Quota limits.
 
-    :param value: List of quota limits.
-    :type value: list[~azure.mgmt.quota.models.CurrentUsagesBase]
-    :param next_link: The URI used to fetch the next page of quota limits. When there are no more
+    :ivar value: List of quota limits.
+    :vartype value: list[~azure.mgmt.quota.models.CurrentUsagesBase]
+    :ivar next_link: The URI used to fetch the next page of quota limits. When there are no more
      pages, this is null.
-    :type next_link: str
+    :vartype next_link: str
     """
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': '[CurrentUsagesBase]'},
-        'next_link': {'key': 'nextLink', 'type': 'str'},
+        "value": {"key": "value", "type": "[CurrentUsagesBase]"},
+        "next_link": {"key": "nextLink", "type": "str"},
     }
 
     def __init__(
-        self,
-        *,
-        value: Optional[List["CurrentUsagesBase"]] = None,
-        next_link: Optional[str] = None,
-        **kwargs
+        self, *, value: Optional[List["_models.CurrentUsagesBase"]] = None, next_link: Optional[str] = None, **kwargs
     ):
-        super(UsagesLimits, self).__init__(**kwargs)
+        """
+        :keyword value: List of quota limits.
+        :paramtype value: list[~azure.mgmt.quota.models.CurrentUsagesBase]
+        :keyword next_link: The URI used to fetch the next page of quota limits. When there are no more
+         pages, this is null.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class UsagesObject(msrest.serialization.Model):
+class UsagesObject(_serialization.Model):
     """The resource usages value.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param value: Required. The usages value.
-    :type value: int
-    :param usages_type: The quota or usages limit types. Possible values include: "Individual",
+    :ivar value: The usages value. Required.
+    :vartype value: int
+    :ivar usages_type: The quota or usages limit types. Known values are: "Individual" and
      "Combined".
-    :type usages_type: str or ~azure.mgmt.quota.models.UsagesTypes
+    :vartype usages_type: str or ~azure.mgmt.quota.models.UsagesTypes
     """
 
     _validation = {
-        'value': {'required': True},
+        "value": {"required": True},
     }
 
     _attribute_map = {
-        'value': {'key': 'value', 'type': 'int'},
-        'usages_type': {'key': 'usagesType', 'type': 'str'},
+        "value": {"key": "value", "type": "int"},
+        "usages_type": {"key": "usagesType", "type": "str"},
     }
 
-    def __init__(
-        self,
-        *,
-        value: int,
-        usages_type: Optional[Union[str, "UsagesTypes"]] = None,
-        **kwargs
-    ):
-        super(UsagesObject, self).__init__(**kwargs)
+    def __init__(self, *, value: int, usages_type: Optional[Union[str, "_models.UsagesTypes"]] = None, **kwargs):
+        """
+        :keyword value: The usages value. Required.
+        :paramtype value: int
+        :keyword usages_type: The quota or usages limit types. Known values are: "Individual" and
+         "Combined".
+        :paramtype usages_type: str or ~azure.mgmt.quota.models.UsagesTypes
+        """
+        super().__init__(**kwargs)
         self.value = value
         self.usages_type = usages_type
 
 
-class UsagesProperties(msrest.serialization.Model):
+class UsagesProperties(_serialization.Model):
     """Usage properties for the specified resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param usages: The quota limit properties for this resource.
-    :type usages: ~azure.mgmt.quota.models.UsagesObject
+    :ivar usages: The quota limit properties for this resource.
+    :vartype usages: ~azure.mgmt.quota.models.UsagesObject
     :ivar unit: The units for the quota usage, such as Count and Bytes. When requesting quota, use
      the **unit** value returned in the GET response in the request body of your PUT operation.
     :vartype unit: str
-    :param name: Resource name provided by the resource provider. Use this property name when
+    :ivar name: Resource name provided by the resource provider. Use this property name when
      requesting quota.
-    :type name: ~azure.mgmt.quota.models.ResourceName
-    :param resource_type: The name of the resource type.
-    :type resource_type: str
+    :vartype name: ~azure.mgmt.quota.models.ResourceName
+    :ivar resource_type: The name of the resource type.
+    :vartype resource_type: str
     :ivar quota_period: The time period for the summary of the quota usage values. For example:
      *P1D (per one day)*\ PT1M (per one minute)
      *PT1S (per one second).
      This parameter is optional because it is not relevant for all resources such as compute.
     :vartype quota_period: str
     :ivar is_quota_applicable: States if quota can be requested for this resource.
     :vartype is_quota_applicable: bool
-    :param properties: Additional properties for the specific resource provider.
-    :type properties: any
+    :ivar properties: Additional properties for the specific resource provider.
+    :vartype properties: JSON
     """
 
     _validation = {
-        'unit': {'readonly': True},
-        'quota_period': {'readonly': True},
-        'is_quota_applicable': {'readonly': True},
+        "unit": {"readonly": True},
+        "quota_period": {"readonly": True},
+        "is_quota_applicable": {"readonly": True},
     }
 
     _attribute_map = {
-        'usages': {'key': 'usages', 'type': 'UsagesObject'},
-        'unit': {'key': 'unit', 'type': 'str'},
-        'name': {'key': 'name', 'type': 'ResourceName'},
-        'resource_type': {'key': 'resourceType', 'type': 'str'},
-        'quota_period': {'key': 'quotaPeriod', 'type': 'str'},
-        'is_quota_applicable': {'key': 'isQuotaApplicable', 'type': 'bool'},
-        'properties': {'key': 'properties', 'type': 'object'},
+        "usages": {"key": "usages", "type": "UsagesObject"},
+        "unit": {"key": "unit", "type": "str"},
+        "name": {"key": "name", "type": "ResourceName"},
+        "resource_type": {"key": "resourceType", "type": "str"},
+        "quota_period": {"key": "quotaPeriod", "type": "str"},
+        "is_quota_applicable": {"key": "isQuotaApplicable", "type": "bool"},
+        "properties": {"key": "properties", "type": "object"},
     }
 
     def __init__(
         self,
         *,
-        usages: Optional["UsagesObject"] = None,
-        name: Optional["ResourceName"] = None,
+        usages: Optional["_models.UsagesObject"] = None,
+        name: Optional["_models.ResourceName"] = None,
         resource_type: Optional[str] = None,
-        properties: Optional[Any] = None,
+        properties: Optional[JSON] = None,
         **kwargs
     ):
-        super(UsagesProperties, self).__init__(**kwargs)
+        """
+        :keyword usages: The quota limit properties for this resource.
+        :paramtype usages: ~azure.mgmt.quota.models.UsagesObject
+        :keyword name: Resource name provided by the resource provider. Use this property name when
+         requesting quota.
+        :paramtype name: ~azure.mgmt.quota.models.ResourceName
+        :keyword resource_type: The name of the resource type.
+        :paramtype resource_type: str
+        :keyword properties: Additional properties for the specific resource provider.
+        :paramtype properties: JSON
+        """
+        super().__init__(**kwargs)
         self.usages = usages
         self.unit = None
         self.name = name
         self.resource_type = resource_type
         self.quota_period = None
         self.is_quota_applicable = None
         self.properties = properties
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/__init__.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,13 +7,19 @@
 # --------------------------------------------------------------------------
 
 from ._usages_operations import UsagesOperations
 from ._quota_operations import QuotaOperations
 from ._quota_request_status_operations import QuotaRequestStatusOperations
 from ._quota_operation_operations import QuotaOperationOperations
 
+from ._patch import __all__ as _patch_all
+from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import patch_sdk as _patch_sdk
+
 __all__ = [
-    'UsagesOperations',
-    'QuotaOperations',
-    'QuotaRequestStatusOperations',
-    'QuotaOperationOperations',
+    "UsagesOperations",
+    "QuotaOperations",
+    "QuotaRequestStatusOperations",
+    "QuotaOperationOperations",
 ]
+__all__.extend([p for p in _patch_all if p not in __all__])
+_patch_sdk()
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure/mgmt/quota/operations/_quota_request_status_operations.py` & `azure-mgmt-quota-1.1.0b3/azure/mgmt/quota/operations/_usages_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,214 +1,274 @@
+# pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
-import warnings
-
-from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import urllib.parse
+
+from azure.core.exceptions import (
+    ClientAuthenticationError,
+    HttpResponseError,
+    ResourceExistsError,
+    ResourceNotFoundError,
+    ResourceNotModifiedError,
+    map_error,
+)
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request, _format_url_section
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_get_request(resource_name: str, scope: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop(
+        "api_version", _params.pop("api-version", "2021-03-15-preview")
+    )  # type: Literal["2021-03-15-preview"]
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Quota/usages/{resourceName}")
+    path_format_arguments = {
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str"),
+        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
+    }
+
+    _url = _format_url_section(_url, **path_format_arguments)
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_request(scope: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version = kwargs.pop(
+        "api_version", _params.pop("api-version", "2021-03-15-preview")
+    )  # type: Literal["2021-03-15-preview"]
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Quota/usages")
+    path_format_arguments = {
+        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
+    }
+
+    _url = _format_url_section(_url, **path_format_arguments)
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
-
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-class QuotaRequestStatusOperations(object):
-    """QuotaRequestStatusOperations operations.
-
-    You should not instantiate this class directly. Instead, you should create a Client instance that
-    instantiates it for you and attaches it as an attribute.
-
-    :ivar models: Alias to model classes used in this operation group.
-    :type models: ~azure.mgmt.quota.models
-    :param client: Client for service requests.
-    :param config: Configuration of service client.
-    :param serializer: An object model serializer.
-    :param deserializer: An object model deserializer.
+
+class UsagesOperations:
     """
+    .. warning::
+        **DO NOT** instantiate this class directly.
 
-    models = _models
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.quota.AzureQuotaExtensionAPI`'s
+        :attr:`usages` attribute.
+    """
 
-    def __init__(self, client, config, serializer, deserializer):
-        self._client = client
-        self._serialize = serializer
-        self._deserialize = deserializer
-        self._config = config
-
-    def get(
-        self,
-        id,  # type: str
-        scope,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.QuotaRequestDetails"
-        """Get the quota request details and status by quota request ID for the resources of the resource
-        provider at a specific location. The quota request ID **id** is returned in the response of the
-        PUT operation.
+    models = _models
 
-        :param id: Quota request ID.
-        :type id: str
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def get(self, resource_name: str, scope: str, **kwargs: Any) -> _models.CurrentUsagesBase:
+        """Get the current usage of a resource.
+
+        :param resource_name: Resource name for a given resource provider. For example:
+
+
+         * SKU name for Microsoft.Compute
+         * SKU or TotalLowPriorityCores for Microsoft.MachineLearningServices
+           For Microsoft.Network PublicIPAddresses. Required.
+        :type resource_name: str
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: QuotaRequestDetails, or the result of cls(response)
-        :rtype: ~azure.mgmt.quota.models.QuotaRequestDetails
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :return: CurrentUsagesBase or the result of cls(response)
+        :rtype: ~azure.mgmt.quota.models.CurrentUsagesBase
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.QuotaRequestDetails"]
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
-        }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'id': self._serialize.url("id", id, 'str'),
-            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        url = self._client.format_url(url, **path_format_arguments)
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.CurrentUsagesBase]
+
+        request = build_get_request(
+            resource_name=resource_name,
+            scope=scope,
+            api_version=api_version,
+            template_url=self.get.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)  # type: ignore
+
+        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
 
-        request = self._client.get(url, query_parameters, header_parameters)
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
+            error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('QuotaRequestDetails', pipeline_response)
+        response_headers = {}
+        response_headers["ETag"] = self._deserialize("str", response.headers.get("ETag"))
+
+        deserialized = self._deserialize("CurrentUsagesBase", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, response_headers)
 
         return deserialized
-    get.metadata = {'url': '/{scope}/providers/Microsoft.Quota/quotaRequests/{id}'}  # type: ignore
 
-    def list(
-        self,
-        scope,  # type: str
-        filter=None,  # type: Optional[str]
-        top=None,  # type: Optional[int]
-        skiptoken=None,  # type: Optional[str]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.QuotaRequestDetailsList"]
-        """For the specified scope, get the current quota requests for a one year period ending at the
-        time is made. Use the **oData** filter to select quota requests.
+    get.metadata = {"url": "/{scope}/providers/Microsoft.Quota/usages/{resourceName}"}  # type: ignore
+
+    @distributed_trace
+    def list(self, scope: str, **kwargs: Any) -> Iterable["_models.CurrentUsagesBase"]:
+        """Get a list of current usage for all resources for the scope specified.
 
         :param scope: The target Azure resource URI. For example,
          ``/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/qms-test/providers/Microsoft.Batch/batchAccounts/testAccount/``.
          This is the target Azure resource URI for the List GET operation. If a ``{resourceName}`` is
          added after ``/quotas``\ , then it's the target Azure resource URI in the GET operation for the
-         specific resource.
+         specific resource. Required.
         :type scope: str
-        :param filter: .. list-table::
-            :header-rows: 1
-
-            * - Field
-              - Supported operators
-            * -
-
-
-         |requestSubmitTime | ge, le, eq, gt, lt
-          |provisioningState eq {QuotaRequestState}
-          |resourceName eq {resourceName}.
-        :type filter: str
-        :param top: Number of records to return.
-        :type top: int
-        :param skiptoken: The **Skiptoken** parameter is used only if a previous operation returned a
-         partial result. If a previous response contains a **nextLink** element, its value includes a
-         **skiptoken** parameter that specifies a starting point to use for subsequent calls.
-        :type skiptoken: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either QuotaRequestDetailsList or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.quota.models.QuotaRequestDetailsList]
-        :raises: ~azure.core.exceptions.HttpResponseError
+        :return: An iterator like instance of either CurrentUsagesBase or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.quota.models.CurrentUsagesBase]
+        :raises ~azure.core.exceptions.HttpResponseError:
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["_models.QuotaRequestDetailsList"]
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version = kwargs.pop(
+            "api_version", _params.pop("api-version", self._config.api_version)
+        )  # type: Literal["2021-03-15-preview"]
+        cls = kwargs.pop("cls", None)  # type: ClsType[_models.UsagesLimits]
+
         error_map = {
-            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-03-15-preview"
-        accept = "application/json"
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-                if filter is not None:
-                    query_parameters['$filter'] = self._serialize.query("filter", filter, 'str')
-                if top is not None:
-                    query_parameters['$top'] = self._serialize.query("top", top, 'int', minimum=1)
-                if skiptoken is not None:
-                    query_parameters['$skiptoken'] = self._serialize.query("skiptoken", skiptoken, 'str')
 
-                request = self._client.get(url, query_parameters, header_parameters)
+                request = build_list_request(
+                    scope=scope,
+                    api_version=api_version,
+                    template_url=self.list.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)  # type: ignore
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('QuotaRequestDetailsList', pipeline_response)
+            deserialized = self._deserialize("UsagesLimits", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, response)
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ExceptionResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(
-            get_next, extract_data
-        )
-    list.metadata = {'url': '/{scope}/providers/Microsoft.Quota/quotaRequests'}  # type: ignore
+        return ItemPaged(get_next, extract_data)
+
+    list.metadata = {"url": "/{scope}/providers/Microsoft.Quota/usages"}  # type: ignore
```

## Comparing `azure-mgmt-quota-1.0.0b2/azure_mgmt_quota.egg-info/SOURCES.txt` & `azure-mgmt-quota-1.1.0b3/azure_mgmt_quota.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 _meta.json
-setup.cfg
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/quota/__init__.py
 azure/mgmt/quota/_azure_quota_extension_api.py
 azure/mgmt/quota/_configuration.py
+azure/mgmt/quota/_patch.py
+azure/mgmt/quota/_serialization.py
+azure/mgmt/quota/_vendor.py
 azure/mgmt/quota/_version.py
+azure/mgmt/quota/py.typed
 azure/mgmt/quota/aio/__init__.py
 azure/mgmt/quota/aio/_azure_quota_extension_api.py
 azure/mgmt/quota/aio/_configuration.py
+azure/mgmt/quota/aio/_patch.py
 azure/mgmt/quota/aio/operations/__init__.py
+azure/mgmt/quota/aio/operations/_patch.py
 azure/mgmt/quota/aio/operations/_quota_operation_operations.py
 azure/mgmt/quota/aio/operations/_quota_operations.py
 azure/mgmt/quota/aio/operations/_quota_request_status_operations.py
 azure/mgmt/quota/aio/operations/_usages_operations.py
 azure/mgmt/quota/models/__init__.py
 azure/mgmt/quota/models/_azure_quota_extension_api_enums.py
-azure/mgmt/quota/models/_models.py
 azure/mgmt/quota/models/_models_py3.py
+azure/mgmt/quota/models/_patch.py
 azure/mgmt/quota/operations/__init__.py
+azure/mgmt/quota/operations/_patch.py
 azure/mgmt/quota/operations/_quota_operation_operations.py
 azure/mgmt/quota/operations/_quota_operations.py
 azure/mgmt/quota/operations/_quota_request_status_operations.py
 azure/mgmt/quota/operations/_usages_operations.py
 azure_mgmt_quota.egg-info/PKG-INFO
 azure_mgmt_quota.egg-info/SOURCES.txt
 azure_mgmt_quota.egg-info/dependency_links.txt
```

