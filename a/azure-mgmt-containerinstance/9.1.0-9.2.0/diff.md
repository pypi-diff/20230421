# Comparing `tmp/azure-mgmt-containerinstance-9.1.0.zip` & `tmp/azure-mgmt-containerinstance-9.2.0.zip`

## zipinfo {}

```diff
@@ -1,52 +1,55 @@
-Zip file size: 78483 bytes, number of entries: 50
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/tests/
--rw-rw-r--  2.0 unx     1480 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/README.md
--rw-rw-r--  2.0 unx      126 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/MANIFEST.in
--rw-rw-r--  2.0 unx     2913 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/setup.py
--rw-rw-r--  2.0 unx       67 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/setup.cfg
--rw-rw-r--  2.0 unx      594 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/_meta.json
--rw-rw-r--  2.0 unx     7891 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/CHANGELOG.md
--rw-rw-r--  2.0 unx    12327 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     1811 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      105 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/requires.txt
--rw-rw-r--  2.0 unx    12327 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/not-zip-safe
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/
--rw-rw-r--  2.0 unx       64 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/
--rw-rw-r--  2.0 unx       64 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/
--rw-rw-r--  2.0 unx      486 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_version.py
--rw-rw-r--  2.0 unx      755 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/__init__.py
--rw-rw-r--  2.0 unx     3420 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_configuration.py
--rw-rw-r--  2.0 unx     4886 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_container_instance_management_client.py
--rw-rw-r--  2.0 unx    12109 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_location_operations.py
--rw-rw-r--  2.0 unx     4752 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_operations.py
--rw-rw-r--  2.0 unx      802 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/__init__.py
--rw-rw-r--  2.0 unx    45740 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py
--rw-rw-r--  2.0 unx    12956 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_containers_operations.py
--rw-rw-r--  2.0 unx     3674 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py
--rw-rw-r--  2.0 unx     8065 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/__init__.py
--rw-rw-r--  2.0 unx    68226 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_models_py3.py
--rw-rw-r--  2.0 unx    63849 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_models.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/
--rw-rw-r--  2.0 unx      601 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/__init__.py
--rw-rw-r--  2.0 unx     3364 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_configuration.py
--rw-rw-r--  2.0 unx     4853 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py
--rw-rw-r--  2.0 unx    12053 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py
--rw-rw-r--  2.0 unx     4692 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      802 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    45480 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py
--rw-rw-r--  2.0 unx    12709 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_containers_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Oct-14 03:30 azure-mgmt-containerinstance-9.1.0/tests/recordings/
--rw-rw-r--  2.0 unx    11921 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/tests/test_cli_mgmt_containerinstance.py
--rw-rw-r--  2.0 unx     6921 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/tests/disable_test_mgmt_containerinstance.py
--rw-rw-r--  2.0 unx    20010 b- defN 21-Oct-14 03:29 azure-mgmt-containerinstance-9.1.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml
-50 files, 392903 bytes uncompressed, 67077 bytes compressed:  82.9%
+Zip file size: 75173 bytes, number of entries: 53
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/
+-rw-rw-r--  2.0 unx      141 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     2693 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/setup.py
+-rw-rw-r--  2.0 unx     1074 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/LICENSE
+-rw-rw-r--  2.0 unx     7997 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1387 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/setup.cfg
+-rw-rw-r--  2.0 unx    12406 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/PKG-INFO
+-rw-rw-r--  2.0 unx      609 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/_meta.json
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/
+-rw-rw-r--  2.0 unx      486 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_version.py
+-rw-rw-r--  2.0 unx     4813 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_container_instance_management_client.py
+-rw-rw-r--  2.0 unx      884 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/__init__.py
+-rw-rw-r--  2.0 unx     3381 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_configuration.py
+-rw-rw-r--  2.0 unx     1197 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_vendor.py
+-rw-rw-r--  2.0 unx     1529 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_patch.py
+-rw-rw-r--  2.0 unx     5348 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_operations.py
+-rw-rw-r--  2.0 unx      802 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/__init__.py
+-rw-rw-r--  2.0 unx    14413 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_location_operations.py
+-rw-rw-r--  2.0 unx    51363 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py
+-rw-rw-r--  2.0 unx    15581 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_containers_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/
+-rw-rw-r--  2.0 unx     4894 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py
+-rw-rw-r--  2.0 unx      831 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/__init__.py
+-rw-rw-r--  2.0 unx     3399 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1529 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_patch.py
+-rw-rw-r--  2.0 unx     4716 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      802 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    11343 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py
+-rw-rw-r--  2.0 unx    38711 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py
+-rw-rw-r--  2.0 unx    10649 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_containers_operations.py
+-rw-rw-r--  2.0 unx     3421 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py
+-rw-rw-r--  2.0 unx     4830 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/__init__.py
+-rw-rw-r--  2.0 unx    89421 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/tests/recordings/
+-rw-rw-r--  2.0 unx    11921 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/tests/disable_test_cli_mgmt_containerinstance.py
+-rw-rw-r--  2.0 unx     6921 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/tests/disable_test_mgmt_containerinstance.py
+-rw-rw-r--  2.0 unx    20010 b- defN 22-Apr-15 01:57 azure-mgmt-containerinstance-9.2.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml
+-rw-rw-r--  2.0 unx       63 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     1892 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    12406 b- defN 22-Apr-15 01:58 azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/PKG-INFO
+53 files, 354039 bytes uncompressed, 63153 bytes compressed:  82.2%
```

## zipnote {}

```diff
@@ -1,151 +1,160 @@
-Filename: azure-mgmt-containerinstance-9.1.0/
+Filename: azure-mgmt-containerinstance-9.2.0/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/
+Filename: azure-mgmt-containerinstance-9.2.0/tests/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/tests/
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/README.md
+Filename: azure-mgmt-containerinstance-9.2.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/MANIFEST.in
+Filename: azure-mgmt-containerinstance-9.2.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/setup.py
+Filename: azure-mgmt-containerinstance-9.2.0/LICENSE
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/setup.cfg
+Filename: azure-mgmt-containerinstance-9.2.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/_meta.json
+Filename: azure-mgmt-containerinstance-9.2.0/README.md
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/CHANGELOG.md
+Filename: azure-mgmt-containerinstance-9.2.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/PKG-INFO
+Filename: azure-mgmt-containerinstance-9.2.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/dependency_links.txt
+Filename: azure-mgmt-containerinstance-9.2.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/top_level.txt
+Filename: azure-mgmt-containerinstance-9.2.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/requires.txt
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/PKG-INFO
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/not-zip-safe
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_version.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_container_instance_management_client.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_version.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_patch.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_configuration.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_container_instance_management_client.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_location_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_location_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_containers_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_containers_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_models_py3.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_models.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_configuration.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_containers_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/__init__.py
+Filename: azure-mgmt-containerinstance-9.2.0/tests/recordings/
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/tests/disable_test_cli_mgmt_containerinstance.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_containers_operations.py
+Filename: azure-mgmt-containerinstance-9.2.0/tests/disable_test_mgmt_containerinstance.py
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/tests/recordings/
+Filename: azure-mgmt-containerinstance-9.2.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/tests/test_cli_mgmt_containerinstance.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/tests/disable_test_mgmt_containerinstance.py
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-containerinstance-9.1.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/dependency_links.txt
+Comment: 
+
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/top_level.txt
+Comment: 
+
+Filename: azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-containerinstance-9.1.0/README.md` & `azure-mgmt-containerinstance-9.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-## Microsoft Azure SDK for Python
+# Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Container Instance Client Library.
+This package has been tested with Python 3.6+.
+For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
-Azure Resource Manager (ARM) is the next generation of management APIs
-that replace the old Azure Service Management (ASM).
+## _Disclaimer_
 
-This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
+_Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
-For the older Azure Service Management (ASM) libraries, see
-[azure-servicemanagement-legacy](https://pypi.python.org/pypi/azure-servicemanagement-legacy)
-library.
-
-For a more complete set of Azure libraries, see the
-[azure sdk python release](https://aka.ms/azsdk/python/all).
-
-## Usage
+# Usage
 
 
 To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
 
 
-
-For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-Code samples for this package can be found at [Container Instance Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
+ 
+For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/containerinstance)
+Code samples for this package can be found at [Container Instance](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
 Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
-## Provide Feedback
+# Provide Feedback
+
+If you encounter any bugs or have suggestions, please file an issue in the
+[Issues](https://github.com/Azure/azure-sdk-for-python/issues)
+section of the project. 
 
-If you encounter any bugs or have suggestions, please file an issue in
-the [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
-section of the project.
 
-![image](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
+![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
```

## Comparing `azure-mgmt-containerinstance-9.1.0/setup.py` & `azure-mgmt-containerinstance-9.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,31 +16,18 @@
 PACKAGE_PPRINT_NAME = "Container Instance"
 
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
-with open(os.path.join(package_folder_path, '_version.py'), 'r') as fd:
+with open(os.path.join(package_folder_path, 'version.py')
+          if os.path.exists(os.path.join(package_folder_path, 'version.py'))
+          else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
     version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError('Cannot find version information')
 
 with open('README.md', encoding='utf-8') as f:
@@ -54,35 +41,34 @@
     description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
+    keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.mgmt',
     ]),
     install_requires=[
         'msrest>=0.6.21',
         'azure-common~=1.1',
-        'azure-mgmt-core>=1.2.0,<2.0.0',
+        'azure-mgmt-core>=1.3.0,<2.0.0',
     ],
-    extras_require={
-        ":python_version<'3.0'": ['azure-mgmt-nspkg'],
-    }
+    python_requires=">=3.6"
 )
```

## Comparing `azure-mgmt-containerinstance-9.1.0/_meta.json` & `azure-mgmt-containerinstance-9.2.0/_meta.json`

 * *Files 9% similar despite different names*

### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'autorest'": "'3.7.2'",*

 * * "'autorest_command'": "'autorest specification/containerinstance/resource-manager/readme.md "*

 * *                       '--multiapi --python --python-mode=update '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--python3-only --track2 --use=@autorest/python@5.12.0 '*

 * *                       "--use=@autorest/modelerfour@4.19.3 --version=3.7.2'",*

 * * "'commit'": "'5dad3b83d0926768ede15ed41895d5f38defd512'",*

 * * "'use'": "['@aut […]*

```diff
@@ -1,11 +1,11 @@
 {
-    "autorest": "3.4.5",
-    "autorest_command": "autorest specification/containerinstance/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 --use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 --version=3.4.5",
-    "commit": "314f28163917b9cfc527f7776b5e4a1dea69d295",
+    "autorest": "3.7.2",
+    "autorest_command": "autorest specification/containerinstance/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --python3-only --track2 --use=@autorest/python@5.12.0 --use=@autorest/modelerfour@4.19.3 --version=3.7.2",
+    "commit": "5dad3b83d0926768ede15ed41895d5f38defd512",
     "readme": "specification/containerinstance/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@5.8.4",
-        "@autorest/modelerfour@4.19.2"
+        "@autorest/python@5.12.0",
+        "@autorest/modelerfour@4.19.3"
     ]
 }
```

## Comparing `azure-mgmt-containerinstance-9.1.0/CHANGELOG.md` & `azure-mgmt-containerinstance-9.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 9.2.0 (2022-04-15)
+
+**Features**
+
+  - Model IpAddress has a new parameter dns_name_label_reuse_policy
+
 ## 9.1.0 (2021-10-13)
 
 **Features**
 
   - Model ContainerGroup has a new parameter zones
   - Model Resource has a new parameter zones
```

## Comparing `azure-mgmt-containerinstance-9.1.0/PKG-INFO` & `azure-mgmt-containerinstance-9.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerinstance
-Version: 9.1.0
+Version: 9.2.0
 Summary: Microsoft Azure Container Instance Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: ## Microsoft Azure SDK for Python
+Description: # Microsoft Azure SDK for Python
         
         This is the Microsoft Azure Container Instance Client Library.
+        This package has been tested with Python 3.6+.
+        For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
         
-        Azure Resource Manager (ARM) is the next generation of management APIs
-        that replace the old Azure Service Management (ASM).
+        ## _Disclaimer_
         
-        This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
+        _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
         
-        For the older Azure Service Management (ASM) libraries, see
-        [azure-servicemanagement-legacy](https://pypi.python.org/pypi/azure-servicemanagement-legacy)
-        library.
-        
-        For a more complete set of Azure libraries, see the
-        [azure sdk python release](https://aka.ms/azsdk/python/all).
-        
-        ## Usage
+        # Usage
         
         
         To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
         
         
-        
-        For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-        Code samples for this package can be found at [Container Instance Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
+         
+        For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/containerinstance)
+        Code samples for this package can be found at [Container Instance](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
         Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
         
         
-        ## Provide Feedback
+        # Provide Feedback
+        
+        If you encounter any bugs or have suggestions, please file an issue in the
+        [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
+        section of the project. 
         
-        If you encounter any bugs or have suggestions, please file an issue in
-        the [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
-        section of the project.
         
-        ![image](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
+        ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
         
         
         # Release History
         
+        ## 9.2.0 (2022-04-15)
+        
+        **Features**
+        
+          - Model IpAddress has a new parameter dns_name_label_reuse_policy
+        
         ## 9.1.0 (2021-10-13)
         
         **Features**
         
           - Model ContainerGroup has a new parameter zones
           - Model Resource has a new parameter zones
         
@@ -265,19 +266,21 @@
           - Added container group instance view
           - Renamed event class
         
         ## 0.1.0 (2017-07-27)
         
           - Initial preview release
         
+Keywords: azure,azure sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt` & `azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 _meta.json
-setup.cfg
 setup.py
 azure/__init__.py
 azure/mgmt/__init__.py
 azure/mgmt/containerinstance/__init__.py
 azure/mgmt/containerinstance/_configuration.py
 azure/mgmt/containerinstance/_container_instance_management_client.py
+azure/mgmt/containerinstance/_patch.py
+azure/mgmt/containerinstance/_vendor.py
 azure/mgmt/containerinstance/_version.py
 azure/mgmt/containerinstance/aio/__init__.py
 azure/mgmt/containerinstance/aio/_configuration.py
 azure/mgmt/containerinstance/aio/_container_instance_management_client.py
+azure/mgmt/containerinstance/aio/_patch.py
 azure/mgmt/containerinstance/aio/operations/__init__.py
 azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py
 azure/mgmt/containerinstance/aio/operations/_containers_operations.py
 azure/mgmt/containerinstance/aio/operations/_location_operations.py
 azure/mgmt/containerinstance/aio/operations/_operations.py
 azure/mgmt/containerinstance/models/__init__.py
 azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py
-azure/mgmt/containerinstance/models/_models.py
 azure/mgmt/containerinstance/models/_models_py3.py
 azure/mgmt/containerinstance/operations/__init__.py
 azure/mgmt/containerinstance/operations/_container_groups_operations.py
 azure/mgmt/containerinstance/operations/_containers_operations.py
 azure/mgmt/containerinstance/operations/_location_operations.py
 azure/mgmt/containerinstance/operations/_operations.py
 azure_mgmt_containerinstance.egg-info/PKG-INFO
 azure_mgmt_containerinstance.egg-info/SOURCES.txt
 azure_mgmt_containerinstance.egg-info/dependency_links.txt
 azure_mgmt_containerinstance.egg-info/not-zip-safe
 azure_mgmt_containerinstance.egg-info/requires.txt
 azure_mgmt_containerinstance.egg-info/top_level.txt
+tests/disable_test_cli_mgmt_containerinstance.py
 tests/disable_test_mgmt_containerinstance.py
-tests/test_cli_mgmt_containerinstance.py
 tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure_mgmt_containerinstance.egg-info/PKG-INFO` & `azure-mgmt-containerinstance-9.2.0/azure_mgmt_containerinstance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerinstance
-Version: 9.1.0
+Version: 9.2.0
 Summary: Microsoft Azure Container Instance Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: ## Microsoft Azure SDK for Python
+Description: # Microsoft Azure SDK for Python
         
         This is the Microsoft Azure Container Instance Client Library.
+        This package has been tested with Python 3.6+.
+        For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
         
-        Azure Resource Manager (ARM) is the next generation of management APIs
-        that replace the old Azure Service Management (ASM).
+        ## _Disclaimer_
         
-        This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
+        _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
         
-        For the older Azure Service Management (ASM) libraries, see
-        [azure-servicemanagement-legacy](https://pypi.python.org/pypi/azure-servicemanagement-legacy)
-        library.
-        
-        For a more complete set of Azure libraries, see the
-        [azure sdk python release](https://aka.ms/azsdk/python/all).
-        
-        ## Usage
+        # Usage
         
         
         To learn how to use this package, see the [quickstart guide](https://aka.ms/azsdk/python/mgmt)
         
         
-        
-        For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/)
-        Code samples for this package can be found at [Container Instance Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
+         
+        For docs and references, see [Python SDK References](https://docs.microsoft.com/python/api/overview/azure/containerinstance)
+        Code samples for this package can be found at [Container Instance](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com.
         Additional code samples for different Azure services are available at [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
         
         
-        ## Provide Feedback
+        # Provide Feedback
+        
+        If you encounter any bugs or have suggestions, please file an issue in the
+        [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
+        section of the project. 
         
-        If you encounter any bugs or have suggestions, please file an issue in
-        the [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
-        section of the project.
         
-        ![image](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
+        ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerinstance%2FREADME.png)
         
         
         # Release History
         
+        ## 9.2.0 (2022-04-15)
+        
+        **Features**
+        
+          - Model IpAddress has a new parameter dns_name_label_reuse_policy
+        
         ## 9.1.0 (2021-10-13)
         
         **Features**
         
           - Model ContainerGroup has a new parameter zones
           - Model Resource has a new parameter zones
         
@@ -265,19 +266,21 @@
           - Added container group instance view
           - Renamed event class
         
         ## 0.1.0 (2017-07-27)
         
           - Initial preview release
         
+Keywords: azure,azure sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_configuration.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,70 +2,66 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any
-
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class ContainerInstanceManagementClientConfiguration(Configuration):
     """Configuration for ContainerInstanceManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
     :type subscription_id: str
     """
 
     def __init__(
         self,
-        credential,  # type: "TokenCredential"
-        subscription_id,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        credential: "AsyncTokenCredential",
+        subscription_id: str,
+        **kwargs: Any
+    ) -> None:
+        super(ContainerInstanceManagementClientConfiguration, self).__init__(**kwargs)
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
-        super(ContainerInstanceManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-09-01"
+        self.api_version = "2021-10-01"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-containerinstance/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        **kwargs: Any
+    ) -> None:
         self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get('authentication_policy')
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = policies.BearerTokenCredentialPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/_container_instance_management_client.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,103 +2,100 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from typing import TYPE_CHECKING
+from copy import deepcopy
+from typing import Any, Awaitable, Optional, TYPE_CHECKING
 
-from azure.mgmt.core import ARMPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.mgmt.core import AsyncARMPipelineClient
 from msrest import Deserializer, Serializer
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Optional
-
-    from azure.core.credentials import TokenCredential
-    from azure.core.pipeline.transport import HttpRequest, HttpResponse
-
+from .. import models
 from ._configuration import ContainerInstanceManagementClientConfiguration
-from .operations import ContainerGroupsOperations
-from .operations import Operations
-from .operations import LocationOperations
-from .operations import ContainersOperations
-from . import models
+from .operations import ContainerGroupsOperations, ContainersOperations, LocationOperations, Operations
 
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from azure.core.credentials_async import AsyncTokenCredential
 
-class ContainerInstanceManagementClient(object):
+class ContainerInstanceManagementClient:
     """ContainerInstanceManagementClient.
 
     :ivar container_groups: ContainerGroupsOperations operations
-    :vartype container_groups: azure.mgmt.containerinstance.operations.ContainerGroupsOperations
+    :vartype container_groups:
+     azure.mgmt.containerinstance.aio.operations.ContainerGroupsOperations
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.containerinstance.operations.Operations
+    :vartype operations: azure.mgmt.containerinstance.aio.operations.Operations
     :ivar location: LocationOperations operations
-    :vartype location: azure.mgmt.containerinstance.operations.LocationOperations
+    :vartype location: azure.mgmt.containerinstance.aio.operations.LocationOperations
     :ivar containers: ContainersOperations operations
-    :vartype containers: azure.mgmt.containerinstance.operations.ContainersOperations
+    :vartype containers: azure.mgmt.containerinstance.aio.operations.ContainersOperations
     :param credential: Credential needed for the client to connect to Azure.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
+     subscription. The subscription ID forms part of the URI for every service call.
     :type subscription_id: str
-    :param str base_url: Service URL
-    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+    :param base_url: Service URL. Default value is 'https://management.azure.com'.
+    :type base_url: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential,  # type: "TokenCredential"
-        subscription_id,  # type: str
-        base_url=None,  # type: Optional[str]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        if not base_url:
-            base_url = 'https://management.azure.com'
-        self._config = ContainerInstanceManagementClientConfiguration(credential, subscription_id, **kwargs)
-        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        credential: "AsyncTokenCredential",
+        subscription_id: str,
+        base_url: str = "https://management.azure.com",
+        **kwargs: Any
+    ) -> None:
+        self._config = ContainerInstanceManagementClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
-        self._serialize.client_side_validation = False
         self._deserialize = Deserializer(client_models)
+        self._serialize.client_side_validation = False
+        self.container_groups = ContainerGroupsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.location = LocationOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.containers = ContainersOperations(self._client, self._config, self._serialize, self._deserialize)
 
-        self.container_groups = ContainerGroupsOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.operations = Operations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.location = LocationOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.containers = ContainersOperations(
-            self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, http_request, **kwargs):
-        # type: (HttpRequest, Any) -> HttpResponse
+    def _send_request(
+        self,
+        request: HttpRequest,
+        **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
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
+        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-        }
-        http_request.url = self._client.format_url(http_request.url, **path_format_arguments)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
-
-    def close(self):
-        # type: () -> None
-        self._client.close()
-
-    def __enter__(self):
-        # type: () -> ContainerInstanceManagementClient
-        self._client.__enter__()
+
+        request_copy = deepcopy(request)
+        request_copy.url = self._client.format_url(request_copy.url)
+        return self._client.send_request(request_copy, **kwargs)
+
+    async def close(self) -> None:
+        await self._client.close()
+
+    async def __aenter__(self) -> "ContainerInstanceManagementClient":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_location_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_location_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,132 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
+import functools
+from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
 import warnings
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
 from azure.mgmt.core.exceptions import ARMErrorFormat
+from msrest import Serializer
 
 from .. import models as _models
-
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
-
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+from .._vendor import _convert_request, _format_url_section
+T = TypeVar('T')
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+def build_list_usage_request(
+    subscription_id: str,
+    location: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/usages')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "location": _SERIALIZER.url("location", location, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_list_cached_images_request(
+    subscription_id: str,
+    location: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/cachedImages')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "location": _SERIALIZER.url("location", location, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_list_capabilities_request(
+    subscription_id: str,
+    location: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/capabilities')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "location": _SERIALIZER.url("location", location, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
 
 class LocationOperations(object):
     """LocationOperations operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
@@ -41,63 +142,59 @@
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list_usage(
         self,
-        location,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.UsageListResult"]
+        location: str,
+        **kwargs: Any
+    ) -> Iterable["_models.UsageListResult"]:
         """Get the usage for a subscription.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either UsageListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.UsageListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.UsageListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_usage.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_usage_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_usage.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_usage_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('UsageListResult', pipeline_response)
+            deserialized = self._deserialize("UsageListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -107,70 +204,69 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return ItemPaged(
             get_next, extract_data
         )
     list_usage.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/usages'}  # type: ignore
 
+    @distributed_trace
     def list_cached_images(
         self,
-        location,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.CachedImagesListResult"]
+        location: str,
+        **kwargs: Any
+    ) -> Iterable["_models.CachedImagesListResult"]:
         """Get the list of cached images.
 
         Get the list of cached images on specific OS type for a subscription in a region.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either CachedImagesListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.CachedImagesListResult]
+        :return: An iterator like instance of either CachedImagesListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.CachedImagesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CachedImagesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_cached_images.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_cached_images_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_cached_images.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_cached_images_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('CachedImagesListResult', pipeline_response)
+            deserialized = self._deserialize("CachedImagesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -180,70 +276,69 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return ItemPaged(
             get_next, extract_data
         )
     list_cached_images.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/cachedImages'}  # type: ignore
 
+    @distributed_trace
     def list_capabilities(
         self,
-        location,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.CapabilitiesListResult"]
+        location: str,
+        **kwargs: Any
+    ) -> Iterable["_models.CapabilitiesListResult"]:
         """Get the list of capabilities of the location.
 
         Get the list of CPU/memory/GPU capabilities of a region.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either CapabilitiesListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.CapabilitiesListResult]
+        :return: An iterator like instance of either CapabilitiesListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.CapabilitiesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CapabilitiesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_capabilities.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_capabilities_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_capabilities.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_capabilities_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('CapabilitiesListResult', pipeline_response)
+            deserialized = self._deserialize("CapabilitiesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -253,11 +348,12 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return ItemPaged(
             get_next, extract_data
         )
     list_capabilities.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/capabilities'}  # type: ignore
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
+import functools
+from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
 import warnings
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models as _models
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._operations import build_list_request
+T = TypeVar('T')
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
-
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-class Operations(object):
-    """Operations operations.
+class Operations:
+    """Operations async operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
     :ivar models: Alias to model classes used in this operation group.
     :type models: ~azure.mgmt.containerinstance.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer):
+    def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list(
         self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.OperationListResult"]
+        **kwargs: Any
+    ) -> AsyncIterable["_models.OperationListResult"]:
         """List the operations for Azure Container Instance service.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.OperationListResult]
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.OperationListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_request(
+                    template_url=self.list.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_request(
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize('OperationListResult', pipeline_response)
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
-            return deserialized.next_link or None, iter(list_of_elem)
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
+        async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(
+
+        return AsyncItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/providers/Microsoft.ContainerInstance/operations'}  # type: ignore
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/__init__.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_container_groups_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,398 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
+import functools
+from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, TypeVar, Union
 import warnings
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
+from msrest import Serializer
 
 from .. import models as _models
-
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, TypeVar, Union
-
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+from .._vendor import _convert_request, _format_url_section
+T = TypeVar('T')
+JSONType = Any
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+def build_list_request(
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/containerGroups')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_list_by_resource_group_request(
+    subscription_id: str,
+    resource_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_get_request(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_create_or_update_request_initial(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    *,
+    json: JSONType = None,
+    content: Any = None,
+    **kwargs: Any
+) -> HttpRequest:
+    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    if content_type is not None:
+        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="PUT",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        json=json,
+        content=content,
+        **kwargs
+    )
+
+
+def build_update_request(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    *,
+    json: JSONType = None,
+    content: Any = None,
+    **kwargs: Any
+) -> HttpRequest:
+    content_type = kwargs.pop('content_type', None)  # type: Optional[str]
+
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    if content_type is not None:
+        header_parameters['Content-Type'] = _SERIALIZER.header("content_type", content_type, 'str')
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="PATCH",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        json=json,
+        content=content,
+        **kwargs
+    )
+
+
+def build_delete_request_initial(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="DELETE",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_restart_request_initial(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/restart')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="POST",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_stop_request(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/stop')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="POST",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_start_request_initial(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/start')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="POST",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
+
+
+def build_get_outbound_network_dependencies_endpoints_request(
+    subscription_id: str,
+    resource_group_name: str,
+    container_group_name: str,
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/outboundNetworkDependenciesEndpoints')
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, 'str'),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, 'str'),
+        "containerGroupName": _SERIALIZER.url("container_group_name", container_group_name, 'str'),
+    }
+
+    url = _format_url_section(url, **path_format_arguments)
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
 
 class ContainerGroupsOperations(object):
     """ContainerGroupsOperations operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
@@ -43,63 +408,60 @@
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list(
         self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.ContainerGroupListResult"]
+        **kwargs: Any
+    ) -> Iterable["_models.ContainerGroupListResult"]:
         """Get a list of container groups in the specified subscription.
 
         Get a list of container groups in the specified subscription. This operation returns properties
         of each container group including containers, image registry credentials, restart policy, IP
         address type, OS type, state, and volumes.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ContainerGroupListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
+        :return: An iterator like instance of either ContainerGroupListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    template_url=self.list.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('ContainerGroupListResult', pipeline_response)
+            deserialized = self._deserialize("ContainerGroupListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -109,72 +471,71 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return ItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/containerGroups'}  # type: ignore
 
+    @distributed_trace
     def list_by_resource_group(
         self,
-        resource_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["_models.ContainerGroupListResult"]
+        resource_group_name: str,
+        **kwargs: Any
+    ) -> Iterable["_models.ContainerGroupListResult"]:
         """Get a list of container groups in the specified subscription and resource group.
 
         Get a list of container groups in a specified subscription and resource group. This operation
         returns properties of each container group including containers, image registry credentials,
         restart policy, IP address type, OS type, state, and volumes.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ContainerGroupListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
+        :return: An iterator like instance of either ContainerGroupListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_by_resource_group.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_by_resource_group_request(
+                    subscription_id=self._config.subscription_id,
+                    resource_group_name=resource_group_name,
+                    template_url=self.list_by_resource_group.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_by_resource_group_request(
+                    subscription_id=self._config.subscription_id,
+                    resource_group_name=resource_group_name,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize('ContainerGroupListResult', pipeline_response)
+            deserialized = self._deserialize("ContainerGroupListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -184,26 +545,27 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return ItemPaged(
             get_next, extract_data
         )
     list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups'}  # type: ignore
 
+    @distributed_trace
     def get(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.ContainerGroup"
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> "_models.ContainerGroup":
         """Get the properties of the specified container group.
 
         Gets the properties of the specified container group in the specified subscription and resource
         group. The operation returns the properties of each container group including containers, image
         registry credentials, restart policy, IP address type, OS type, state, and volumes.
 
         :param resource_group_name: The name of the resource group.
@@ -216,89 +578,70 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_get_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.get.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.get(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
     def _create_or_update_initial(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        container_group,  # type: "_models.ContainerGroup"
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.ContainerGroup"
+        resource_group_name: str,
+        container_group_name: str,
+        container_group: "_models.ContainerGroup",
+        **kwargs: Any
+    ) -> "_models.ContainerGroup":
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        content_type = kwargs.pop("content_type", "application/json")
-        accept = "application/json"
-
-        # Construct URL
-        url = self._create_or_update_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
-        body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(container_group, 'ContainerGroup')
-        body_content_kwargs['content'] = body_content
-        request = self._client.put(url, query_parameters, header_parameters, **body_content_kwargs)
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+
+        _json = self._serialize.body(container_group, 'ContainerGroup')
+
+        request = build_create_or_update_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            content_type=content_type,
+            json=_json,
+            template_url=self._create_or_update_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -308,98 +651,99 @@
         if response.status_code == 201:
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
+    @distributed_trace
     def begin_create_or_update(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        container_group,  # type: "_models.ContainerGroup"
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> LROPoller["_models.ContainerGroup"]
+        resource_group_name: str,
+        container_group_name: str,
+        container_group: "_models.ContainerGroup",
+        **kwargs: Any
+    ) -> LROPoller["_models.ContainerGroup"]:
         """Create or update container groups.
 
         Create or update container groups with specified configurations.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :param container_group: The properties of the container group to be created or updated.
         :type container_group: ~azure.mgmt.containerinstance.models.ContainerGroup
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
-        :return: An instance of LROPoller that returns either ContainerGroup or the result of cls(response)
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ContainerGroup or the result of
+         cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.containerinstance.models.ContainerGroup]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 container_group=container_group,
+                content_type=content_type,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
+            response = pipeline_response.http_response
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
-
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+    @distributed_trace
     def update(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        resource,  # type: "_models.Resource"
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.ContainerGroup"
+        resource_group_name: str,
+        container_group_name: str,
+        resource: "_models.Resource",
+        **kwargs: Any
+    ) -> "_models.ContainerGroup":
         """Update container groups.
 
         Updates container group tags with specified values.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
@@ -412,88 +756,69 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        content_type = kwargs.pop("content_type", "application/json")
-        accept = "application/json"
-
-        # Construct URL
-        url = self.update.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
-        body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(resource, 'Resource')
-        body_content_kwargs['content'] = body_content
-        request = self._client.patch(url, query_parameters, header_parameters, **body_content_kwargs)
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+
+        _json = self._serialize.body(resource, 'Resource')
+
+        request = build_update_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            content_type=content_type,
+            json=_json,
+            template_url=self.update.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
     def _delete_initial(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Optional["_models.ContainerGroup"]
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> Optional["_models.ContainerGroup"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.ContainerGroup"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
 
-        # Construct URL
-        url = self._delete_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
-
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_delete_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._delete_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -501,207 +826,192 @@
         if response.status_code == 200:
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
+    @distributed_trace
     def begin_delete(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> LROPoller["_models.ContainerGroup"]
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> LROPoller["_models.ContainerGroup"]:
         """Delete the specified container group.
 
         Delete the specified container group in the specified subscription and resource group. The
         operation does not delete other resources provided by the user, such as volumes.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
-        :return: An instance of LROPoller that returns either ContainerGroup or the result of cls(response)
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of LROPoller that returns either ContainerGroup or the result of
+         cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.containerinstance.models.ContainerGroup]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._delete_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
+            response = pipeline_response.http_response
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
-
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
     def _restart_initial(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self._restart_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_restart_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._restart_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _restart_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/restart'}  # type: ignore
 
+
+    @distributed_trace
     def begin_restart(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> LROPoller[None]
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> LROPoller[None]:
         """Restarts all containers in a container group.
 
         Restarts all containers in a container group in place. If container image has updates, new
         image will be downloaded.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._restart_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_restart.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/restart'}  # type: ignore
 
+    @distributed_trace
     def stop(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> None:
         """Stops all containers in a container group.
 
         Stops all containers in a container group. Compute resources will be deallocated and billing
         will stop.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
@@ -713,167 +1023,144 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.stop.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_stop_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.stop.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     stop.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/stop'}  # type: ignore
 
+
     def _start_initial(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self._start_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_start_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._start_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _start_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/start'}  # type: ignore
 
+
+    @distributed_trace
     def begin_start(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> LROPoller[None]
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> LROPoller[None]:
         """Starts all containers in a container group.
 
         Starts all containers in a container group. Compute resources will be allocated and billing
         will start.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
+         operation to not poll, or pass in your own initialized polling object for a personal polling
+         strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.PollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._start_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = ARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_start.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/start'}  # type: ignore
 
+    @distributed_trace
     def get_outbound_network_dependencies_endpoints(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> List[str]
+        resource_group_name: str,
+        container_group_name: str,
+        **kwargs: Any
+    ) -> List[str]:
         """Get all network dependencies for container group.
 
         Gets all the network dependencies for this container group to allow complete control of network
         setting and configuration. For container groups, this will always be an empty list.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
@@ -885,42 +1172,34 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType[List[str]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get_outbound_network_dependencies_endpoints.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_get_outbound_network_dependencies_endpoints_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.get_outbound_network_dependencies_endpoints.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.get(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('[str]', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     get_outbound_network_dependencies_endpoints.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/outboundNetworkDependenciesEndpoints'}  # type: ignore
+
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/operations/_containers_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_containers_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
+import functools
+from typing import Any, Callable, Dict, Generic, Optional, TypeVar
 import warnings
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models as _models
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._containers_operations import build_attach_request, build_execute_command_request, build_list_logs_request
+T = TypeVar('T')
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Optional, TypeVar
-
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-class ContainersOperations(object):
-    """ContainersOperations operations.
+class ContainersOperations:
+    """ContainersOperations async operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
     :ivar models: Alias to model classes used in this operation group.
     :type models: ~azure.mgmt.containerinstance.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer):
+    def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
-    def list_logs(
+    @distributed_trace_async
+    async def list_logs(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        container_name,  # type: str
-        tail=None,  # type: Optional[int]
-        timestamps=None,  # type: Optional[bool]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.Logs"
+        resource_group_name: str,
+        container_group_name: str,
+        container_name: str,
+        tail: Optional[int] = None,
+        timestamps: Optional[bool] = None,
+        **kwargs: Any
+    ) -> "_models.Logs":
         """Get the logs for a specified container instance.
 
         Get the logs for a specified container instance in a specified resource group and container
         group.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
@@ -77,64 +77,54 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Logs"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.list_logs.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-            'containerName': self._serialize.url("container_name", container_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-        if tail is not None:
-            query_parameters['tail'] = self._serialize.query("tail", tail, 'int')
-        if timestamps is not None:
-            query_parameters['timestamps'] = self._serialize.query("timestamps", timestamps, 'bool')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_list_logs_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            container_name=container_name,
+            tail=tail,
+            timestamps=timestamps,
+            template_url=self.list_logs.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.get(url, query_parameters, header_parameters)
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('Logs', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     list_logs.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/containers/{containerName}/logs'}  # type: ignore
 
-    def execute_command(
+
+    @distributed_trace_async
+    async def execute_command(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        container_name,  # type: str
-        container_exec_request,  # type: "_models.ContainerExecRequest"
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.ContainerExecResponse"
+        resource_group_name: str,
+        container_group_name: str,
+        container_name: str,
+        container_exec_request: "_models.ContainerExecRequest",
+        **kwargs: Any
+    ) -> "_models.ContainerExecResponse":
         """Executes a command in a specific container instance.
 
         Executes a command for a specific container instance in a specified resource group and
         container group.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
@@ -150,64 +140,56 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerExecResponse"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        content_type = kwargs.pop("content_type", "application/json")
-        accept = "application/json"
-
-        # Construct URL
-        url = self.execute_command.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-            'containerName': self._serialize.url("container_name", container_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
-        body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(container_exec_request, 'ContainerExecRequest')
-        body_content_kwargs['content'] = body_content
-        request = self._client.post(url, query_parameters, header_parameters, **body_content_kwargs)
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+
+        _json = self._serialize.body(container_exec_request, 'ContainerExecRequest')
+
+        request = build_execute_command_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            container_name=container_name,
+            content_type=content_type,
+            json=_json,
+            template_url=self.execute_command.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerExecResponse', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     execute_command.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/containers/{containerName}/exec'}  # type: ignore
 
-    def attach(
+
+    @distributed_trace_async
+    async def attach(
         self,
-        resource_group_name,  # type: str
-        container_group_name,  # type: str
-        container_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> "_models.ContainerAttachResponse"
+        resource_group_name: str,
+        container_group_name: str,
+        container_name: str,
+        **kwargs: Any
+    ) -> "_models.ContainerAttachResponse":
         """Attach to the output of a specific container instance.
 
         Attach to the output stream of a specific container instance in a specified resource group and
         container group.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
@@ -221,43 +203,35 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerAttachResponse"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
 
-        # Construct URL
-        url = self.attach.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-            'containerName': self._serialize.url("container_name", container_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
-
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_attach_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            container_name=container_name,
+            template_url=self.attach.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
-        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerAttachResponse', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     attach.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/containers/{containerName}/attach'}  # type: ignore
+
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_container_instance_management_client_enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,114 +2,109 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from enum import Enum, EnumMeta
+from enum import Enum
 from six import with_metaclass
+from azure.core import CaseInsensitiveEnumMeta
 
-class _CaseInsensitiveEnumMeta(EnumMeta):
-    def __getitem__(self, name):
-        return super().__getitem__(name.upper())
-
-    def __getattr__(cls, name):
-        """Return the enum member matching `name`
-        We use __getattr__ instead of descriptors or inserting into the enum
-        class' __dict__ in order to support `name` and `value` being both
-        properties for enum members (which live in the class' __dict__) and
-        enum members themselves.
-        """
-        try:
-            return cls._member_map_[name.upper()]
-        except KeyError:
-            raise AttributeError(name)
 
+class AutoGeneratedDomainNameLabelScope(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
+    """The value representing the security enum.
+    """
+
+    UNSECURE = "Unsecure"
+    TENANT_REUSE = "TenantReuse"
+    SUBSCRIPTION_REUSE = "SubscriptionReuse"
+    RESOURCE_GROUP_REUSE = "ResourceGroupReuse"
+    NOREUSE = "Noreuse"
 
-class ContainerGroupIpAddressType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerGroupIpAddressType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """Specifies if the IP is exposed to the public internet or private VNET.
     """
 
     PUBLIC = "Public"
     PRIVATE = "Private"
 
-class ContainerGroupNetworkProtocol(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerGroupNetworkProtocol(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The protocol associated with the port.
     """
 
     TCP = "TCP"
     UDP = "UDP"
 
-class ContainerGroupRestartPolicy(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerGroupRestartPolicy(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """Restart policy for all containers within the container group.
     
     
     * ``Always`` Always restart
     * ``OnFailure`` Restart on failure
     * ``Never`` Never restart
     """
 
     ALWAYS = "Always"
     ON_FAILURE = "OnFailure"
     NEVER = "Never"
 
-class ContainerGroupSku(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerGroupSku(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The container group SKU.
     """
 
     STANDARD = "Standard"
     DEDICATED = "Dedicated"
 
-class ContainerInstanceOperationsOrigin(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerInstanceOperationsOrigin(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The intended executor of the operation.
     """
 
     USER = "User"
     SYSTEM = "System"
 
-class ContainerNetworkProtocol(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ContainerNetworkProtocol(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The protocol associated with the port.
     """
 
     TCP = "TCP"
     UDP = "UDP"
 
-class GpuSku(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class GpuSku(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The SKU of the GPU resource.
     """
 
     K80 = "K80"
     P100 = "P100"
     V100 = "V100"
 
-class LogAnalyticsLogType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class LogAnalyticsLogType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The log type to be used.
     """
 
     CONTAINER_INSIGHTS = "ContainerInsights"
     CONTAINER_INSTANCE_LOGS = "ContainerInstanceLogs"
 
-class OperatingSystemTypes(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class OperatingSystemTypes(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The operating system type required by the containers in the container group.
     """
 
     WINDOWS = "Windows"
     LINUX = "Linux"
 
-class ResourceIdentityType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class ResourceIdentityType(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The type of identity used for the container group. The type 'SystemAssigned, UserAssigned'
     includes both an implicitly created identity and a set of user assigned identities. The type
     'None' will remove any identities from the container group.
     """
 
     SYSTEM_ASSIGNED = "SystemAssigned"
     USER_ASSIGNED = "UserAssigned"
     SYSTEM_ASSIGNED_USER_ASSIGNED = "SystemAssigned, UserAssigned"
     NONE = "None"
 
-class Scheme(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class Scheme(with_metaclass(CaseInsensitiveEnumMeta, str, Enum)):
     """The scheme.
     """
 
     HTTP = "http"
     HTTPS = "https"
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/models/_models_py3.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/models/_models_py3.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 
 class AzureFileVolume(msrest.serialization.Model):
     """The properties of the Azure File volume. Azure File shares are mounted as volumes.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param share_name: Required. The name of the Azure File share to be mounted as a volume.
-    :type share_name: str
-    :param read_only: The flag indicating whether the Azure File shared mounted as a volume is
+    :ivar share_name: Required. The name of the Azure File share to be mounted as a volume.
+    :vartype share_name: str
+    :ivar read_only: The flag indicating whether the Azure File shared mounted as a volume is
      read-only.
-    :type read_only: bool
-    :param storage_account_name: Required. The name of the storage account that contains the Azure
+    :vartype read_only: bool
+    :ivar storage_account_name: Required. The name of the storage account that contains the Azure
      File share.
-    :type storage_account_name: str
-    :param storage_account_key: The storage account access key used to access the Azure File share.
-    :type storage_account_key: str
+    :vartype storage_account_name: str
+    :ivar storage_account_key: The storage account access key used to access the Azure File share.
+    :vartype storage_account_key: str
     """
 
     _validation = {
         'share_name': {'required': True},
         'storage_account_name': {'required': True},
     }
 
@@ -47,30 +47,43 @@
         *,
         share_name: str,
         storage_account_name: str,
         read_only: Optional[bool] = None,
         storage_account_key: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword share_name: Required. The name of the Azure File share to be mounted as a volume.
+        :paramtype share_name: str
+        :keyword read_only: The flag indicating whether the Azure File shared mounted as a volume is
+         read-only.
+        :paramtype read_only: bool
+        :keyword storage_account_name: Required. The name of the storage account that contains the
+         Azure File share.
+        :paramtype storage_account_name: str
+        :keyword storage_account_key: The storage account access key used to access the Azure File
+         share.
+        :paramtype storage_account_key: str
+        """
         super(AzureFileVolume, self).__init__(**kwargs)
         self.share_name = share_name
         self.read_only = read_only
         self.storage_account_name = storage_account_name
         self.storage_account_key = storage_account_key
 
 
 class CachedImages(msrest.serialization.Model):
     """The cached image and OS type.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param os_type: Required. The OS type of the cached image.
-    :type os_type: str
-    :param image: Required. The cached image name.
-    :type image: str
+    :ivar os_type: Required. The OS type of the cached image.
+    :vartype os_type: str
+    :ivar image: Required. The cached image name.
+    :vartype image: str
     """
 
     _validation = {
         'os_type': {'required': True},
         'image': {'required': True},
     }
 
@@ -82,40 +95,52 @@
     def __init__(
         self,
         *,
         os_type: str,
         image: str,
         **kwargs
     ):
+        """
+        :keyword os_type: Required. The OS type of the cached image.
+        :paramtype os_type: str
+        :keyword image: Required. The cached image name.
+        :paramtype image: str
+        """
         super(CachedImages, self).__init__(**kwargs)
         self.os_type = os_type
         self.image = image
 
 
 class CachedImagesListResult(msrest.serialization.Model):
     """The response containing cached images.
 
-    :param value: The list of cached images.
-    :type value: list[~azure.mgmt.containerinstance.models.CachedImages]
-    :param next_link: The URI to fetch the next page of cached images.
-    :type next_link: str
+    :ivar value: The list of cached images.
+    :vartype value: list[~azure.mgmt.containerinstance.models.CachedImages]
+    :ivar next_link: The URI to fetch the next page of cached images.
+    :vartype next_link: str
     """
 
     _attribute_map = {
         'value': {'key': 'value', 'type': '[CachedImages]'},
         'next_link': {'key': 'nextLink', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["CachedImages"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword value: The list of cached images.
+        :paramtype value: list[~azure.mgmt.containerinstance.models.CachedImages]
+        :keyword next_link: The URI to fetch the next page of cached images.
+        :paramtype next_link: str
+        """
         super(CachedImagesListResult, self).__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class Capabilities(msrest.serialization.Model):
     """The regional capabilities.
@@ -154,14 +179,16 @@
         'capabilities': {'key': 'capabilities', 'type': 'CapabilitiesCapabilities'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(Capabilities, self).__init__(**kwargs)
         self.resource_type = None
         self.os_type = None
         self.location = None
         self.ip_address_type = None
         self.gpu = None
         self.capabilities = None
@@ -192,60 +219,68 @@
         'max_gpu_count': {'key': 'maxGpuCount', 'type': 'float'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(CapabilitiesCapabilities, self).__init__(**kwargs)
         self.max_memory_in_gb = None
         self.max_cpu = None
         self.max_gpu_count = None
 
 
 class CapabilitiesListResult(msrest.serialization.Model):
     """The response containing list of capabilities.
 
-    :param value: The list of capabilities.
-    :type value: list[~azure.mgmt.containerinstance.models.Capabilities]
-    :param next_link: The URI to fetch the next page of capabilities.
-    :type next_link: str
+    :ivar value: The list of capabilities.
+    :vartype value: list[~azure.mgmt.containerinstance.models.Capabilities]
+    :ivar next_link: The URI to fetch the next page of capabilities.
+    :vartype next_link: str
     """
 
     _attribute_map = {
         'value': {'key': 'value', 'type': '[Capabilities]'},
         'next_link': {'key': 'nextLink', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["Capabilities"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword value: The list of capabilities.
+        :paramtype value: list[~azure.mgmt.containerinstance.models.Capabilities]
+        :keyword next_link: The URI to fetch the next page of capabilities.
+        :paramtype next_link: str
+        """
         super(CapabilitiesListResult, self).__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class CloudErrorBody(msrest.serialization.Model):
     """An error response from the Container Instance service.
 
-    :param code: An identifier for the error. Codes are invariant and are intended to be consumed
+    :ivar code: An identifier for the error. Codes are invariant and are intended to be consumed
      programmatically.
-    :type code: str
-    :param message: A message describing the error, intended to be suitable for display in a user
+    :vartype code: str
+    :ivar message: A message describing the error, intended to be suitable for display in a user
      interface.
-    :type message: str
-    :param target: The target of the particular error. For example, the name of the property in
+    :vartype message: str
+    :ivar target: The target of the particular error. For example, the name of the property in
      error.
-    :type target: str
-    :param details: A list of additional details about the error.
-    :type details: list[~azure.mgmt.containerinstance.models.CloudErrorBody]
+    :vartype target: str
+    :ivar details: A list of additional details about the error.
+    :vartype details: list[~azure.mgmt.containerinstance.models.CloudErrorBody]
     """
 
     _attribute_map = {
         'code': {'key': 'code', 'type': 'str'},
         'message': {'key': 'message', 'type': 'str'},
         'target': {'key': 'target', 'type': 'str'},
         'details': {'key': 'details', 'type': '[CloudErrorBody]'},
@@ -256,14 +291,27 @@
         *,
         code: Optional[str] = None,
         message: Optional[str] = None,
         target: Optional[str] = None,
         details: Optional[List["CloudErrorBody"]] = None,
         **kwargs
     ):
+        """
+        :keyword code: An identifier for the error. Codes are invariant and are intended to be consumed
+         programmatically.
+        :paramtype code: str
+        :keyword message: A message describing the error, intended to be suitable for display in a user
+         interface.
+        :paramtype message: str
+        :keyword target: The target of the particular error. For example, the name of the property in
+         error.
+        :paramtype target: str
+        :keyword details: A list of additional details about the error.
+        :paramtype details: list[~azure.mgmt.containerinstance.models.CloudErrorBody]
+        """
         super(CloudErrorBody, self).__init__(**kwargs)
         self.code = code
         self.message = message
         self.target = target
         self.details = details
 
 
@@ -288,46 +336,48 @@
         'client_id': {'key': 'clientId', 'type': 'str'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(Components10Wh5UdSchemasContainergroupidentityPropertiesUserassignedidentitiesAdditionalproperties, self).__init__(**kwargs)
         self.principal_id = None
         self.client_id = None
 
 
 class Container(msrest.serialization.Model):
     """A container instance.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The user-provided name of the container instance.
-    :type name: str
-    :param image: Required. The name of the image used to create the container instance.
-    :type image: str
-    :param command: The commands to execute within the container instance in exec form.
-    :type command: list[str]
-    :param ports: The exposed ports on the container instance.
-    :type ports: list[~azure.mgmt.containerinstance.models.ContainerPort]
-    :param environment_variables: The environment variables to set in the container instance.
-    :type environment_variables: list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
+    :ivar name: Required. The user-provided name of the container instance.
+    :vartype name: str
+    :ivar image: Required. The name of the image used to create the container instance.
+    :vartype image: str
+    :ivar command: The commands to execute within the container instance in exec form.
+    :vartype command: list[str]
+    :ivar ports: The exposed ports on the container instance.
+    :vartype ports: list[~azure.mgmt.containerinstance.models.ContainerPort]
+    :ivar environment_variables: The environment variables to set in the container instance.
+    :vartype environment_variables: list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
     :ivar instance_view: The instance view of the container instance. Only valid in response.
     :vartype instance_view: ~azure.mgmt.containerinstance.models.ContainerPropertiesInstanceView
-    :param resources: Required. The resource requirements of the container instance.
-    :type resources: ~azure.mgmt.containerinstance.models.ResourceRequirements
-    :param volume_mounts: The volume mounts available to the container instance.
-    :type volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
-    :param liveness_probe: The liveness probe.
-    :type liveness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
-    :param readiness_probe: The readiness probe.
-    :type readiness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
+    :ivar resources: Required. The resource requirements of the container instance.
+    :vartype resources: ~azure.mgmt.containerinstance.models.ResourceRequirements
+    :ivar volume_mounts: The volume mounts available to the container instance.
+    :vartype volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
+    :ivar liveness_probe: The liveness probe.
+    :vartype liveness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
+    :ivar readiness_probe: The readiness probe.
+    :vartype readiness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
     """
 
     _validation = {
         'name': {'required': True},
         'image': {'required': True},
         'instance_view': {'readonly': True},
         'resources': {'required': True},
@@ -356,14 +406,35 @@
         ports: Optional[List["ContainerPort"]] = None,
         environment_variables: Optional[List["EnvironmentVariable"]] = None,
         volume_mounts: Optional[List["VolumeMount"]] = None,
         liveness_probe: Optional["ContainerProbe"] = None,
         readiness_probe: Optional["ContainerProbe"] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The user-provided name of the container instance.
+        :paramtype name: str
+        :keyword image: Required. The name of the image used to create the container instance.
+        :paramtype image: str
+        :keyword command: The commands to execute within the container instance in exec form.
+        :paramtype command: list[str]
+        :keyword ports: The exposed ports on the container instance.
+        :paramtype ports: list[~azure.mgmt.containerinstance.models.ContainerPort]
+        :keyword environment_variables: The environment variables to set in the container instance.
+        :paramtype environment_variables:
+         list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
+        :keyword resources: Required. The resource requirements of the container instance.
+        :paramtype resources: ~azure.mgmt.containerinstance.models.ResourceRequirements
+        :keyword volume_mounts: The volume mounts available to the container instance.
+        :paramtype volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
+        :keyword liveness_probe: The liveness probe.
+        :paramtype liveness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
+        :keyword readiness_probe: The readiness probe.
+        :paramtype readiness_probe: ~azure.mgmt.containerinstance.models.ContainerProbe
+        """
         super(Container, self).__init__(**kwargs)
         self.name = name
         self.image = image
         self.command = command
         self.ports = ports
         self.environment_variables = environment_variables
         self.instance_view = None
@@ -372,132 +443,161 @@
         self.liveness_probe = liveness_probe
         self.readiness_probe = readiness_probe
 
 
 class ContainerAttachResponse(msrest.serialization.Model):
     """The information for the output stream from container attach.
 
-    :param web_socket_uri: The uri for the output stream from the attach.
-    :type web_socket_uri: str
-    :param password: The password to the output stream from the attach. Send as an Authorization
+    :ivar web_socket_uri: The uri for the output stream from the attach.
+    :vartype web_socket_uri: str
+    :ivar password: The password to the output stream from the attach. Send as an Authorization
      header value when connecting to the websocketUri.
-    :type password: str
+    :vartype password: str
     """
 
     _attribute_map = {
         'web_socket_uri': {'key': 'webSocketUri', 'type': 'str'},
         'password': {'key': 'password', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         web_socket_uri: Optional[str] = None,
         password: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword web_socket_uri: The uri for the output stream from the attach.
+        :paramtype web_socket_uri: str
+        :keyword password: The password to the output stream from the attach. Send as an Authorization
+         header value when connecting to the websocketUri.
+        :paramtype password: str
+        """
         super(ContainerAttachResponse, self).__init__(**kwargs)
         self.web_socket_uri = web_socket_uri
         self.password = password
 
 
 class ContainerExec(msrest.serialization.Model):
     """The container execution command, for liveness or readiness probe.
 
-    :param command: The commands to execute within the container.
-    :type command: list[str]
+    :ivar command: The commands to execute within the container.
+    :vartype command: list[str]
     """
 
     _attribute_map = {
         'command': {'key': 'command', 'type': '[str]'},
     }
 
     def __init__(
         self,
         *,
         command: Optional[List[str]] = None,
         **kwargs
     ):
+        """
+        :keyword command: The commands to execute within the container.
+        :paramtype command: list[str]
+        """
         super(ContainerExec, self).__init__(**kwargs)
         self.command = command
 
 
 class ContainerExecRequest(msrest.serialization.Model):
     """The container exec request.
 
-    :param command: The command to be executed.
-    :type command: str
-    :param terminal_size: The size of the terminal.
-    :type terminal_size: ~azure.mgmt.containerinstance.models.ContainerExecRequestTerminalSize
+    :ivar command: The command to be executed.
+    :vartype command: str
+    :ivar terminal_size: The size of the terminal.
+    :vartype terminal_size: ~azure.mgmt.containerinstance.models.ContainerExecRequestTerminalSize
     """
 
     _attribute_map = {
         'command': {'key': 'command', 'type': 'str'},
         'terminal_size': {'key': 'terminalSize', 'type': 'ContainerExecRequestTerminalSize'},
     }
 
     def __init__(
         self,
         *,
         command: Optional[str] = None,
         terminal_size: Optional["ContainerExecRequestTerminalSize"] = None,
         **kwargs
     ):
+        """
+        :keyword command: The command to be executed.
+        :paramtype command: str
+        :keyword terminal_size: The size of the terminal.
+        :paramtype terminal_size: ~azure.mgmt.containerinstance.models.ContainerExecRequestTerminalSize
+        """
         super(ContainerExecRequest, self).__init__(**kwargs)
         self.command = command
         self.terminal_size = terminal_size
 
 
 class ContainerExecRequestTerminalSize(msrest.serialization.Model):
     """The size of the terminal.
 
-    :param rows: The row size of the terminal.
-    :type rows: int
-    :param cols: The column size of the terminal.
-    :type cols: int
+    :ivar rows: The row size of the terminal.
+    :vartype rows: int
+    :ivar cols: The column size of the terminal.
+    :vartype cols: int
     """
 
     _attribute_map = {
         'rows': {'key': 'rows', 'type': 'int'},
         'cols': {'key': 'cols', 'type': 'int'},
     }
 
     def __init__(
         self,
         *,
         rows: Optional[int] = None,
         cols: Optional[int] = None,
         **kwargs
     ):
+        """
+        :keyword rows: The row size of the terminal.
+        :paramtype rows: int
+        :keyword cols: The column size of the terminal.
+        :paramtype cols: int
+        """
         super(ContainerExecRequestTerminalSize, self).__init__(**kwargs)
         self.rows = rows
         self.cols = cols
 
 
 class ContainerExecResponse(msrest.serialization.Model):
     """The information for the container exec command.
 
-    :param web_socket_uri: The uri for the exec websocket.
-    :type web_socket_uri: str
-    :param password: The password to start the exec command.
-    :type password: str
+    :ivar web_socket_uri: The uri for the exec websocket.
+    :vartype web_socket_uri: str
+    :ivar password: The password to start the exec command.
+    :vartype password: str
     """
 
     _attribute_map = {
         'web_socket_uri': {'key': 'webSocketUri', 'type': 'str'},
         'password': {'key': 'password', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         web_socket_uri: Optional[str] = None,
         password: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword web_socket_uri: The uri for the exec websocket.
+        :paramtype web_socket_uri: str
+        :keyword password: The password to start the exec command.
+        :paramtype password: str
+        """
         super(ContainerExecResponse, self).__init__(**kwargs)
         self.web_socket_uri = web_socket_uri
         self.password = password
 
 
 class Resource(msrest.serialization.Model):
     """The Resource model definition.
@@ -506,20 +606,20 @@
 
     :ivar id: The resource id.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :param location: The resource location.
-    :type location: str
-    :param tags: A set of tags. The resource tags.
-    :type tags: dict[str, str]
-    :param zones: The zones for the container group.
-    :type zones: list[str]
+    :ivar location: The resource location.
+    :vartype location: str
+    :ivar tags: A set of tags. The resource tags.
+    :vartype tags: dict[str, str]
+    :ivar zones: The zones for the container group.
+    :vartype zones: list[str]
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
     }
@@ -537,14 +637,22 @@
         self,
         *,
         location: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
         zones: Optional[List[str]] = None,
         **kwargs
     ):
+        """
+        :keyword location: The resource location.
+        :paramtype location: str
+        :keyword tags: A set of tags. The resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword zones: The zones for the container group.
+        :paramtype zones: list[str]
+        """
         super(Resource, self).__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.location = location
         self.tags = tags
         self.zones = zones
@@ -559,60 +667,61 @@
 
     :ivar id: The resource id.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
-    :param location: The resource location.
-    :type location: str
-    :param tags: A set of tags. The resource tags.
-    :type tags: dict[str, str]
-    :param zones: The zones for the container group.
-    :type zones: list[str]
-    :param identity: The identity of the container group, if configured.
-    :type identity: ~azure.mgmt.containerinstance.models.ContainerGroupIdentity
+    :ivar location: The resource location.
+    :vartype location: str
+    :ivar tags: A set of tags. The resource tags.
+    :vartype tags: dict[str, str]
+    :ivar zones: The zones for the container group.
+    :vartype zones: list[str]
+    :ivar identity: The identity of the container group, if configured.
+    :vartype identity: ~azure.mgmt.containerinstance.models.ContainerGroupIdentity
     :ivar provisioning_state: The provisioning state of the container group. This only appears in
      the response.
     :vartype provisioning_state: str
-    :param containers: Required. The containers within the container group.
-    :type containers: list[~azure.mgmt.containerinstance.models.Container]
-    :param image_registry_credentials: The image registry credentials by which the container group
+    :ivar containers: Required. The containers within the container group.
+    :vartype containers: list[~azure.mgmt.containerinstance.models.Container]
+    :ivar image_registry_credentials: The image registry credentials by which the container group
      is created from.
-    :type image_registry_credentials:
+    :vartype image_registry_credentials:
      list[~azure.mgmt.containerinstance.models.ImageRegistryCredential]
-    :param restart_policy: Restart policy for all containers within the container group.
+    :ivar restart_policy: Restart policy for all containers within the container group.
     
     
      * ``Always`` Always restart
      * ``OnFailure`` Restart on failure
      * ``Never`` Never restart. Possible values include: "Always", "OnFailure", "Never".
-    :type restart_policy: str or ~azure.mgmt.containerinstance.models.ContainerGroupRestartPolicy
-    :param ip_address: The IP address type of the container group.
-    :type ip_address: ~azure.mgmt.containerinstance.models.IpAddress
-    :param os_type: Required. The operating system type required by the containers in the container
+    :vartype restart_policy: str or
+     ~azure.mgmt.containerinstance.models.ContainerGroupRestartPolicy
+    :ivar ip_address: The IP address type of the container group.
+    :vartype ip_address: ~azure.mgmt.containerinstance.models.IpAddress
+    :ivar os_type: Required. The operating system type required by the containers in the container
      group. Possible values include: "Windows", "Linux".
-    :type os_type: str or ~azure.mgmt.containerinstance.models.OperatingSystemTypes
-    :param volumes: The list of volumes that can be mounted by containers in this container group.
-    :type volumes: list[~azure.mgmt.containerinstance.models.Volume]
+    :vartype os_type: str or ~azure.mgmt.containerinstance.models.OperatingSystemTypes
+    :ivar volumes: The list of volumes that can be mounted by containers in this container group.
+    :vartype volumes: list[~azure.mgmt.containerinstance.models.Volume]
     :ivar instance_view: The instance view of the container group. Only valid in response.
     :vartype instance_view:
      ~azure.mgmt.containerinstance.models.ContainerGroupPropertiesInstanceView
-    :param diagnostics: The diagnostic information for a container group.
-    :type diagnostics: ~azure.mgmt.containerinstance.models.ContainerGroupDiagnostics
-    :param subnet_ids: The subnet resource IDs for a container group.
-    :type subnet_ids: list[~azure.mgmt.containerinstance.models.ContainerGroupSubnetId]
-    :param dns_config: The DNS config information for a container group.
-    :type dns_config: ~azure.mgmt.containerinstance.models.DnsConfiguration
-    :param sku: The SKU for a container group. Possible values include: "Standard", "Dedicated".
-    :type sku: str or ~azure.mgmt.containerinstance.models.ContainerGroupSku
-    :param encryption_properties: The encryption properties for a container group.
-    :type encryption_properties: ~azure.mgmt.containerinstance.models.EncryptionProperties
-    :param init_containers: The init containers for a container group.
-    :type init_containers: list[~azure.mgmt.containerinstance.models.InitContainerDefinition]
+    :ivar diagnostics: The diagnostic information for a container group.
+    :vartype diagnostics: ~azure.mgmt.containerinstance.models.ContainerGroupDiagnostics
+    :ivar subnet_ids: The subnet resource IDs for a container group.
+    :vartype subnet_ids: list[~azure.mgmt.containerinstance.models.ContainerGroupSubnetId]
+    :ivar dns_config: The DNS config information for a container group.
+    :vartype dns_config: ~azure.mgmt.containerinstance.models.DnsConfiguration
+    :ivar sku: The SKU for a container group. Possible values include: "Standard", "Dedicated".
+    :vartype sku: str or ~azure.mgmt.containerinstance.models.ContainerGroupSku
+    :ivar encryption_properties: The encryption properties for a container group.
+    :vartype encryption_properties: ~azure.mgmt.containerinstance.models.EncryptionProperties
+    :ivar init_containers: The init containers for a container group.
+    :vartype init_containers: list[~azure.mgmt.containerinstance.models.InitContainerDefinition]
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'provisioning_state': {'readonly': True},
@@ -662,14 +771,58 @@
         subnet_ids: Optional[List["ContainerGroupSubnetId"]] = None,
         dns_config: Optional["DnsConfiguration"] = None,
         sku: Optional[Union[str, "ContainerGroupSku"]] = None,
         encryption_properties: Optional["EncryptionProperties"] = None,
         init_containers: Optional[List["InitContainerDefinition"]] = None,
         **kwargs
     ):
+        """
+        :keyword location: The resource location.
+        :paramtype location: str
+        :keyword tags: A set of tags. The resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword zones: The zones for the container group.
+        :paramtype zones: list[str]
+        :keyword identity: The identity of the container group, if configured.
+        :paramtype identity: ~azure.mgmt.containerinstance.models.ContainerGroupIdentity
+        :keyword containers: Required. The containers within the container group.
+        :paramtype containers: list[~azure.mgmt.containerinstance.models.Container]
+        :keyword image_registry_credentials: The image registry credentials by which the container
+         group is created from.
+        :paramtype image_registry_credentials:
+         list[~azure.mgmt.containerinstance.models.ImageRegistryCredential]
+        :keyword restart_policy: Restart policy for all containers within the container group.
+        
+        
+         * ``Always`` Always restart
+         * ``OnFailure`` Restart on failure
+         * ``Never`` Never restart. Possible values include: "Always", "OnFailure", "Never".
+        :paramtype restart_policy: str or
+         ~azure.mgmt.containerinstance.models.ContainerGroupRestartPolicy
+        :keyword ip_address: The IP address type of the container group.
+        :paramtype ip_address: ~azure.mgmt.containerinstance.models.IpAddress
+        :keyword os_type: Required. The operating system type required by the containers in the
+         container group. Possible values include: "Windows", "Linux".
+        :paramtype os_type: str or ~azure.mgmt.containerinstance.models.OperatingSystemTypes
+        :keyword volumes: The list of volumes that can be mounted by containers in this container
+         group.
+        :paramtype volumes: list[~azure.mgmt.containerinstance.models.Volume]
+        :keyword diagnostics: The diagnostic information for a container group.
+        :paramtype diagnostics: ~azure.mgmt.containerinstance.models.ContainerGroupDiagnostics
+        :keyword subnet_ids: The subnet resource IDs for a container group.
+        :paramtype subnet_ids: list[~azure.mgmt.containerinstance.models.ContainerGroupSubnetId]
+        :keyword dns_config: The DNS config information for a container group.
+        :paramtype dns_config: ~azure.mgmt.containerinstance.models.DnsConfiguration
+        :keyword sku: The SKU for a container group. Possible values include: "Standard", "Dedicated".
+        :paramtype sku: str or ~azure.mgmt.containerinstance.models.ContainerGroupSku
+        :keyword encryption_properties: The encryption properties for a container group.
+        :paramtype encryption_properties: ~azure.mgmt.containerinstance.models.EncryptionProperties
+        :keyword init_containers: The init containers for a container group.
+        :paramtype init_containers: list[~azure.mgmt.containerinstance.models.InitContainerDefinition]
+        """
         super(ContainerGroup, self).__init__(location=location, tags=tags, zones=zones, **kwargs)
         self.identity = identity
         self.provisioning_state = None
         self.containers = containers
         self.image_registry_credentials = image_registry_credentials
         self.restart_policy = restart_policy
         self.ip_address = ip_address
@@ -683,28 +836,32 @@
         self.encryption_properties = encryption_properties
         self.init_containers = init_containers
 
 
 class ContainerGroupDiagnostics(msrest.serialization.Model):
     """Container group diagnostic information.
 
-    :param log_analytics: Container group log analytics information.
-    :type log_analytics: ~azure.mgmt.containerinstance.models.LogAnalytics
+    :ivar log_analytics: Container group log analytics information.
+    :vartype log_analytics: ~azure.mgmt.containerinstance.models.LogAnalytics
     """
 
     _attribute_map = {
         'log_analytics': {'key': 'logAnalytics', 'type': 'LogAnalytics'},
     }
 
     def __init__(
         self,
         *,
         log_analytics: Optional["LogAnalytics"] = None,
         **kwargs
     ):
+        """
+        :keyword log_analytics: Container group log analytics information.
+        :paramtype log_analytics: ~azure.mgmt.containerinstance.models.LogAnalytics
+        """
         super(ContainerGroupDiagnostics, self).__init__(**kwargs)
         self.log_analytics = log_analytics
 
 
 class ContainerGroupIdentity(msrest.serialization.Model):
     """Identity for the container group.
 
@@ -712,23 +869,23 @@
 
     :ivar principal_id: The principal id of the container group identity. This property will only
      be provided for a system assigned identity.
     :vartype principal_id: str
     :ivar tenant_id: The tenant id associated with the container group. This property will only be
      provided for a system assigned identity.
     :vartype tenant_id: str
-    :param type: The type of identity used for the container group. The type 'SystemAssigned,
+    :ivar type: The type of identity used for the container group. The type 'SystemAssigned,
      UserAssigned' includes both an implicitly created identity and a set of user assigned
      identities. The type 'None' will remove any identities from the container group. Possible
      values include: "SystemAssigned", "UserAssigned", "SystemAssigned, UserAssigned", "None".
-    :type type: str or ~azure.mgmt.containerinstance.models.ResourceIdentityType
-    :param user_assigned_identities: The list of user identities associated with the container
+    :vartype type: str or ~azure.mgmt.containerinstance.models.ResourceIdentityType
+    :ivar user_assigned_identities: The list of user identities associated with the container
      group. The user identity dictionary key references will be ARM resource ids in the form:
      '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
-    :type user_assigned_identities: dict[str,
+    :vartype user_assigned_identities: dict[str,
      ~azure.mgmt.containerinstance.models.Components10Wh5UdSchemasContainergroupidentityPropertiesUserassignedidentitiesAdditionalproperties]
     """
 
     _validation = {
         'principal_id': {'readonly': True},
         'tenant_id': {'readonly': True},
     }
@@ -743,42 +900,60 @@
     def __init__(
         self,
         *,
         type: Optional[Union[str, "ResourceIdentityType"]] = None,
         user_assigned_identities: Optional[Dict[str, "Components10Wh5UdSchemasContainergroupidentityPropertiesUserassignedidentitiesAdditionalproperties"]] = None,
         **kwargs
     ):
+        """
+        :keyword type: The type of identity used for the container group. The type 'SystemAssigned,
+         UserAssigned' includes both an implicitly created identity and a set of user assigned
+         identities. The type 'None' will remove any identities from the container group. Possible
+         values include: "SystemAssigned", "UserAssigned", "SystemAssigned, UserAssigned", "None".
+        :paramtype type: str or ~azure.mgmt.containerinstance.models.ResourceIdentityType
+        :keyword user_assigned_identities: The list of user identities associated with the container
+         group. The user identity dictionary key references will be ARM resource ids in the form:
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
+        :paramtype user_assigned_identities: dict[str,
+         ~azure.mgmt.containerinstance.models.Components10Wh5UdSchemasContainergroupidentityPropertiesUserassignedidentitiesAdditionalproperties]
+        """
         super(ContainerGroupIdentity, self).__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
         self.type = type
         self.user_assigned_identities = user_assigned_identities
 
 
 class ContainerGroupListResult(msrest.serialization.Model):
     """The container group list response that contains the container group properties.
 
-    :param value: The list of container groups.
-    :type value: list[~azure.mgmt.containerinstance.models.ContainerGroup]
-    :param next_link: The URI to fetch the next page of container groups.
-    :type next_link: str
+    :ivar value: The list of container groups.
+    :vartype value: list[~azure.mgmt.containerinstance.models.ContainerGroup]
+    :ivar next_link: The URI to fetch the next page of container groups.
+    :vartype next_link: str
     """
 
     _attribute_map = {
         'value': {'key': 'value', 'type': '[ContainerGroup]'},
         'next_link': {'key': 'nextLink', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["ContainerGroup"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword value: The list of container groups.
+        :paramtype value: list[~azure.mgmt.containerinstance.models.ContainerGroup]
+        :keyword next_link: The URI to fetch the next page of container groups.
+        :paramtype next_link: str
+        """
         super(ContainerGroupListResult, self).__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class ContainerGroupPropertiesInstanceView(msrest.serialization.Model):
     """The instance view of the container group. Only valid in response.
@@ -801,28 +976,30 @@
         'state': {'key': 'state', 'type': 'str'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(ContainerGroupPropertiesInstanceView, self).__init__(**kwargs)
         self.events = None
         self.state = None
 
 
 class ContainerGroupSubnetId(msrest.serialization.Model):
     """Container group subnet information.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param id: Required. Resource ID of virtual network and subnet.
-    :type id: str
-    :param name: Friendly name for the subnet.
-    :type name: str
+    :ivar id: Required. Resource ID of virtual network and subnet.
+    :vartype id: str
+    :ivar name: Friendly name for the subnet.
+    :vartype name: str
     """
 
     _validation = {
         'id': {'required': True},
     }
 
     _attribute_map = {
@@ -833,32 +1010,38 @@
     def __init__(
         self,
         *,
         id: str,
         name: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword id: Required. Resource ID of virtual network and subnet.
+        :paramtype id: str
+        :keyword name: Friendly name for the subnet.
+        :paramtype name: str
+        """
         super(ContainerGroupSubnetId, self).__init__(**kwargs)
         self.id = id
         self.name = name
 
 
 class ContainerHttpGet(msrest.serialization.Model):
     """The container Http Get settings, for liveness or readiness probe.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param path: The path to probe.
-    :type path: str
-    :param port: Required. The port number to probe.
-    :type port: int
-    :param scheme: The scheme. Possible values include: "http", "https".
-    :type scheme: str or ~azure.mgmt.containerinstance.models.Scheme
-    :param http_headers: The HTTP headers.
-    :type http_headers: list[~azure.mgmt.containerinstance.models.HttpHeader]
+    :ivar path: The path to probe.
+    :vartype path: str
+    :ivar port: Required. The port number to probe.
+    :vartype port: int
+    :ivar scheme: The scheme. Possible values include: "http", "https".
+    :vartype scheme: str or ~azure.mgmt.containerinstance.models.Scheme
+    :ivar http_headers: The HTTP headers.
+    :vartype http_headers: list[~azure.mgmt.containerinstance.models.HttpHeader]
     """
 
     _validation = {
         'port': {'required': True},
     }
 
     _attribute_map = {
@@ -873,30 +1056,40 @@
         *,
         port: int,
         path: Optional[str] = None,
         scheme: Optional[Union[str, "Scheme"]] = None,
         http_headers: Optional[List["HttpHeader"]] = None,
         **kwargs
     ):
+        """
+        :keyword path: The path to probe.
+        :paramtype path: str
+        :keyword port: Required. The port number to probe.
+        :paramtype port: int
+        :keyword scheme: The scheme. Possible values include: "http", "https".
+        :paramtype scheme: str or ~azure.mgmt.containerinstance.models.Scheme
+        :keyword http_headers: The HTTP headers.
+        :paramtype http_headers: list[~azure.mgmt.containerinstance.models.HttpHeader]
+        """
         super(ContainerHttpGet, self).__init__(**kwargs)
         self.path = path
         self.port = port
         self.scheme = scheme
         self.http_headers = http_headers
 
 
 class ContainerPort(msrest.serialization.Model):
     """The port exposed on the container instance.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param protocol: The protocol associated with the port. Possible values include: "TCP", "UDP".
-    :type protocol: str or ~azure.mgmt.containerinstance.models.ContainerNetworkProtocol
-    :param port: Required. The port number exposed within the container group.
-    :type port: int
+    :ivar protocol: The protocol associated with the port. Possible values include: "TCP", "UDP".
+    :vartype protocol: str or ~azure.mgmt.containerinstance.models.ContainerNetworkProtocol
+    :ivar port: Required. The port number exposed within the container group.
+    :vartype port: int
     """
 
     _validation = {
         'port': {'required': True},
     }
 
     _attribute_map = {
@@ -907,36 +1100,43 @@
     def __init__(
         self,
         *,
         port: int,
         protocol: Optional[Union[str, "ContainerNetworkProtocol"]] = None,
         **kwargs
     ):
+        """
+        :keyword protocol: The protocol associated with the port. Possible values include: "TCP",
+         "UDP".
+        :paramtype protocol: str or ~azure.mgmt.containerinstance.models.ContainerNetworkProtocol
+        :keyword port: Required. The port number exposed within the container group.
+        :paramtype port: int
+        """
         super(ContainerPort, self).__init__(**kwargs)
         self.protocol = protocol
         self.port = port
 
 
 class ContainerProbe(msrest.serialization.Model):
     """The container probe, for liveness or readiness.
 
-    :param exec_property: The execution command to probe.
-    :type exec_property: ~azure.mgmt.containerinstance.models.ContainerExec
-    :param http_get: The Http Get settings to probe.
-    :type http_get: ~azure.mgmt.containerinstance.models.ContainerHttpGet
-    :param initial_delay_seconds: The initial delay seconds.
-    :type initial_delay_seconds: int
-    :param period_seconds: The period seconds.
-    :type period_seconds: int
-    :param failure_threshold: The failure threshold.
-    :type failure_threshold: int
-    :param success_threshold: The success threshold.
-    :type success_threshold: int
-    :param timeout_seconds: The timeout seconds.
-    :type timeout_seconds: int
+    :ivar exec_property: The execution command to probe.
+    :vartype exec_property: ~azure.mgmt.containerinstance.models.ContainerExec
+    :ivar http_get: The Http Get settings to probe.
+    :vartype http_get: ~azure.mgmt.containerinstance.models.ContainerHttpGet
+    :ivar initial_delay_seconds: The initial delay seconds.
+    :vartype initial_delay_seconds: int
+    :ivar period_seconds: The period seconds.
+    :vartype period_seconds: int
+    :ivar failure_threshold: The failure threshold.
+    :vartype failure_threshold: int
+    :ivar success_threshold: The success threshold.
+    :vartype success_threshold: int
+    :ivar timeout_seconds: The timeout seconds.
+    :vartype timeout_seconds: int
     """
 
     _attribute_map = {
         'exec_property': {'key': 'exec', 'type': 'ContainerExec'},
         'http_get': {'key': 'httpGet', 'type': 'ContainerHttpGet'},
         'initial_delay_seconds': {'key': 'initialDelaySeconds', 'type': 'int'},
         'period_seconds': {'key': 'periodSeconds', 'type': 'int'},
@@ -953,14 +1153,30 @@
         initial_delay_seconds: Optional[int] = None,
         period_seconds: Optional[int] = None,
         failure_threshold: Optional[int] = None,
         success_threshold: Optional[int] = None,
         timeout_seconds: Optional[int] = None,
         **kwargs
     ):
+        """
+        :keyword exec_property: The execution command to probe.
+        :paramtype exec_property: ~azure.mgmt.containerinstance.models.ContainerExec
+        :keyword http_get: The Http Get settings to probe.
+        :paramtype http_get: ~azure.mgmt.containerinstance.models.ContainerHttpGet
+        :keyword initial_delay_seconds: The initial delay seconds.
+        :paramtype initial_delay_seconds: int
+        :keyword period_seconds: The period seconds.
+        :paramtype period_seconds: int
+        :keyword failure_threshold: The failure threshold.
+        :paramtype failure_threshold: int
+        :keyword success_threshold: The success threshold.
+        :paramtype success_threshold: int
+        :keyword timeout_seconds: The timeout seconds.
+        :paramtype timeout_seconds: int
+        """
         super(ContainerProbe, self).__init__(**kwargs)
         self.exec_property = exec_property
         self.http_get = http_get
         self.initial_delay_seconds = initial_delay_seconds
         self.period_seconds = period_seconds
         self.failure_threshold = failure_threshold
         self.success_threshold = success_threshold
@@ -996,14 +1212,16 @@
         'events': {'key': 'events', 'type': '[Event]'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(ContainerPropertiesInstanceView, self).__init__(**kwargs)
         self.restart_count = None
         self.current_state = None
         self.previous_state = None
         self.events = None
 
 
@@ -1041,33 +1259,35 @@
         'detail_status': {'key': 'detailStatus', 'type': 'str'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(ContainerState, self).__init__(**kwargs)
         self.state = None
         self.start_time = None
         self.exit_code = None
         self.finish_time = None
         self.detail_status = None
 
 
 class DnsConfiguration(msrest.serialization.Model):
     """DNS configuration for the container group.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name_servers: Required. The DNS servers for the container group.
-    :type name_servers: list[str]
-    :param search_domains: The DNS search domains for hostname lookup in the container group.
-    :type search_domains: str
-    :param options: The DNS options for the container group.
-    :type options: str
+    :ivar name_servers: Required. The DNS servers for the container group.
+    :vartype name_servers: list[str]
+    :ivar search_domains: The DNS search domains for hostname lookup in the container group.
+    :vartype search_domains: str
+    :ivar options: The DNS options for the container group.
+    :vartype options: str
     """
 
     _validation = {
         'name_servers': {'required': True},
     }
 
     _attribute_map = {
@@ -1080,31 +1300,39 @@
         self,
         *,
         name_servers: List[str],
         search_domains: Optional[str] = None,
         options: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword name_servers: Required. The DNS servers for the container group.
+        :paramtype name_servers: list[str]
+        :keyword search_domains: The DNS search domains for hostname lookup in the container group.
+        :paramtype search_domains: str
+        :keyword options: The DNS options for the container group.
+        :paramtype options: str
+        """
         super(DnsConfiguration, self).__init__(**kwargs)
         self.name_servers = name_servers
         self.search_domains = search_domains
         self.options = options
 
 
 class EncryptionProperties(msrest.serialization.Model):
     """The container group encryption properties.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param vault_base_url: Required. The keyvault base url.
-    :type vault_base_url: str
-    :param key_name: Required. The encryption key name.
-    :type key_name: str
-    :param key_version: Required. The encryption key version.
-    :type key_version: str
+    :ivar vault_base_url: Required. The keyvault base url.
+    :vartype vault_base_url: str
+    :ivar key_name: Required. The encryption key name.
+    :vartype key_name: str
+    :ivar key_version: Required. The encryption key version.
+    :vartype key_version: str
     """
 
     _validation = {
         'vault_base_url': {'required': True},
         'key_name': {'required': True},
         'key_version': {'required': True},
     }
@@ -1119,31 +1347,39 @@
         self,
         *,
         vault_base_url: str,
         key_name: str,
         key_version: str,
         **kwargs
     ):
+        """
+        :keyword vault_base_url: Required. The keyvault base url.
+        :paramtype vault_base_url: str
+        :keyword key_name: Required. The encryption key name.
+        :paramtype key_name: str
+        :keyword key_version: Required. The encryption key version.
+        :paramtype key_version: str
+        """
         super(EncryptionProperties, self).__init__(**kwargs)
         self.vault_base_url = vault_base_url
         self.key_name = key_name
         self.key_version = key_version
 
 
 class EnvironmentVariable(msrest.serialization.Model):
     """The environment variable to set within the container instance.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The name of the environment variable.
-    :type name: str
-    :param value: The value of the environment variable.
-    :type value: str
-    :param secure_value: The value of the secure environment variable.
-    :type secure_value: str
+    :ivar name: Required. The name of the environment variable.
+    :vartype name: str
+    :ivar value: The value of the environment variable.
+    :vartype value: str
+    :ivar secure_value: The value of the secure environment variable.
+    :vartype secure_value: str
     """
 
     _validation = {
         'name': {'required': True},
     }
 
     _attribute_map = {
@@ -1156,14 +1392,22 @@
         self,
         *,
         name: str,
         value: Optional[str] = None,
         secure_value: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The name of the environment variable.
+        :paramtype name: str
+        :keyword value: The value of the environment variable.
+        :paramtype value: str
+        :keyword secure_value: The value of the secure environment variable.
+        :paramtype secure_value: str
+        """
         super(EnvironmentVariable, self).__init__(**kwargs)
         self.name = name
         self.value = value
         self.secure_value = secure_value
 
 
 class Event(msrest.serialization.Model):
@@ -1203,36 +1447,38 @@
         'type': {'key': 'type', 'type': 'str'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(Event, self).__init__(**kwargs)
         self.count = None
         self.first_timestamp = None
         self.last_timestamp = None
         self.name = None
         self.message = None
         self.type = None
 
 
 class GitRepoVolume(msrest.serialization.Model):
     """Represents a volume that is populated with the contents of a git repository.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param directory: Target directory name. Must not contain or start with '..'.  If '.' is
+    :ivar directory: Target directory name. Must not contain or start with '..'.  If '.' is
      supplied, the volume directory will be the git repository.  Otherwise, if specified, the volume
      will contain the git repository in the subdirectory with the given name.
-    :type directory: str
-    :param repository: Required. Repository URL.
-    :type repository: str
-    :param revision: Commit hash for the specified revision.
-    :type revision: str
+    :vartype directory: str
+    :ivar repository: Required. Repository URL.
+    :vartype repository: str
+    :ivar revision: Commit hash for the specified revision.
+    :vartype revision: str
     """
 
     _validation = {
         'repository': {'required': True},
     }
 
     _attribute_map = {
@@ -1245,30 +1491,40 @@
         self,
         *,
         repository: str,
         directory: Optional[str] = None,
         revision: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword directory: Target directory name. Must not contain or start with '..'.  If '.' is
+         supplied, the volume directory will be the git repository.  Otherwise, if specified, the volume
+         will contain the git repository in the subdirectory with the given name.
+        :paramtype directory: str
+        :keyword repository: Required. Repository URL.
+        :paramtype repository: str
+        :keyword revision: Commit hash for the specified revision.
+        :paramtype revision: str
+        """
         super(GitRepoVolume, self).__init__(**kwargs)
         self.directory = directory
         self.repository = repository
         self.revision = revision
 
 
 class GpuResource(msrest.serialization.Model):
     """The GPU resource.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param count: Required. The count of the GPU resource.
-    :type count: int
-    :param sku: Required. The SKU of the GPU resource. Possible values include: "K80", "P100",
+    :ivar count: Required. The count of the GPU resource.
+    :vartype count: int
+    :ivar sku: Required. The SKU of the GPU resource. Possible values include: "K80", "P100",
      "V100".
-    :type sku: str or ~azure.mgmt.containerinstance.models.GpuSku
+    :vartype sku: str or ~azure.mgmt.containerinstance.models.GpuSku
     """
 
     _validation = {
         'count': {'required': True},
         'sku': {'required': True},
     }
 
@@ -1280,61 +1536,74 @@
     def __init__(
         self,
         *,
         count: int,
         sku: Union[str, "GpuSku"],
         **kwargs
     ):
+        """
+        :keyword count: Required. The count of the GPU resource.
+        :paramtype count: int
+        :keyword sku: Required. The SKU of the GPU resource. Possible values include: "K80", "P100",
+         "V100".
+        :paramtype sku: str or ~azure.mgmt.containerinstance.models.GpuSku
+        """
         super(GpuResource, self).__init__(**kwargs)
         self.count = count
         self.sku = sku
 
 
 class HttpHeader(msrest.serialization.Model):
     """The HTTP header.
 
-    :param name: The header name.
-    :type name: str
-    :param value: The header value.
-    :type value: str
+    :ivar name: The header name.
+    :vartype name: str
+    :ivar value: The header value.
+    :vartype value: str
     """
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'value': {'key': 'value', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         value: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword name: The header name.
+        :paramtype name: str
+        :keyword value: The header value.
+        :paramtype value: str
+        """
         super(HttpHeader, self).__init__(**kwargs)
         self.name = name
         self.value = value
 
 
 class ImageRegistryCredential(msrest.serialization.Model):
     """Image registry credential.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param server: Required. The Docker image registry server without a protocol such as "http" and
+    :ivar server: Required. The Docker image registry server without a protocol such as "http" and
      "https".
-    :type server: str
-    :param username: Required. The username for the private registry.
-    :type username: str
-    :param password: The password for the private registry.
-    :type password: str
-    :param identity: The identity for the private registry.
-    :type identity: str
-    :param identity_url: The identity URL for the private registry.
-    :type identity_url: str
+    :vartype server: str
+    :ivar username: Required. The username for the private registry.
+    :vartype username: str
+    :ivar password: The password for the private registry.
+    :vartype password: str
+    :ivar identity: The identity for the private registry.
+    :vartype identity: str
+    :ivar identity_url: The identity URL for the private registry.
+    :vartype identity_url: str
     """
 
     _validation = {
         'server': {'required': True},
         'username': {'required': True},
     }
 
@@ -1352,14 +1621,27 @@
         server: str,
         username: str,
         password: Optional[str] = None,
         identity: Optional[str] = None,
         identity_url: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword server: Required. The Docker image registry server without a protocol such as "http"
+         and "https".
+        :paramtype server: str
+        :keyword username: Required. The username for the private registry.
+        :paramtype username: str
+        :keyword password: The password for the private registry.
+        :paramtype password: str
+        :keyword identity: The identity for the private registry.
+        :paramtype identity: str
+        :keyword identity_url: The identity URL for the private registry.
+        :paramtype identity_url: str
+        """
         super(ImageRegistryCredential, self).__init__(**kwargs)
         self.server = server
         self.username = username
         self.password = password
         self.identity = identity
         self.identity_url = identity_url
 
@@ -1367,27 +1649,27 @@
 class InitContainerDefinition(msrest.serialization.Model):
     """The init container definition.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The name for the init container.
-    :type name: str
-    :param image: The image of the init container.
-    :type image: str
-    :param command: The command to execute within the init container in exec form.
-    :type command: list[str]
-    :param environment_variables: The environment variables to set in the init container.
-    :type environment_variables: list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
+    :ivar name: Required. The name for the init container.
+    :vartype name: str
+    :ivar image: The image of the init container.
+    :vartype image: str
+    :ivar command: The command to execute within the init container in exec form.
+    :vartype command: list[str]
+    :ivar environment_variables: The environment variables to set in the init container.
+    :vartype environment_variables: list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
     :ivar instance_view: The instance view of the init container. Only valid in response.
     :vartype instance_view:
      ~azure.mgmt.containerinstance.models.InitContainerPropertiesDefinitionInstanceView
-    :param volume_mounts: The volume mounts available to the init container.
-    :type volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
+    :ivar volume_mounts: The volume mounts available to the init container.
+    :vartype volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
     """
 
     _validation = {
         'name': {'required': True},
         'instance_view': {'readonly': True},
     }
 
@@ -1406,14 +1688,27 @@
         name: str,
         image: Optional[str] = None,
         command: Optional[List[str]] = None,
         environment_variables: Optional[List["EnvironmentVariable"]] = None,
         volume_mounts: Optional[List["VolumeMount"]] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The name for the init container.
+        :paramtype name: str
+        :keyword image: The image of the init container.
+        :paramtype image: str
+        :keyword command: The command to execute within the init container in exec form.
+        :paramtype command: list[str]
+        :keyword environment_variables: The environment variables to set in the init container.
+        :paramtype environment_variables:
+         list[~azure.mgmt.containerinstance.models.EnvironmentVariable]
+        :keyword volume_mounts: The volume mounts available to the init container.
+        :paramtype volume_mounts: list[~azure.mgmt.containerinstance.models.VolumeMount]
+        """
         super(InitContainerDefinition, self).__init__(**kwargs)
         self.name = name
         self.image = image
         self.command = command
         self.environment_variables = environment_variables
         self.instance_view = None
         self.volume_mounts = volume_mounts
@@ -1448,37 +1743,43 @@
         'events': {'key': 'events', 'type': '[Event]'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(InitContainerPropertiesDefinitionInstanceView, self).__init__(**kwargs)
         self.restart_count = None
         self.current_state = None
         self.previous_state = None
         self.events = None
 
 
 class IpAddress(msrest.serialization.Model):
     """IP address for the container group.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param ports: Required. The list of ports exposed on the container group.
-    :type ports: list[~azure.mgmt.containerinstance.models.Port]
-    :param type: Required. Specifies if the IP is exposed to the public internet or private VNET.
+    :ivar ports: Required. The list of ports exposed on the container group.
+    :vartype ports: list[~azure.mgmt.containerinstance.models.Port]
+    :ivar type: Required. Specifies if the IP is exposed to the public internet or private VNET.
      Possible values include: "Public", "Private".
-    :type type: str or ~azure.mgmt.containerinstance.models.ContainerGroupIpAddressType
-    :param ip: The IP exposed to the public internet.
-    :type ip: str
-    :param dns_name_label: The Dns name label for the IP.
-    :type dns_name_label: str
+    :vartype type: str or ~azure.mgmt.containerinstance.models.ContainerGroupIpAddressType
+    :ivar ip: The IP exposed to the public internet.
+    :vartype ip: str
+    :ivar dns_name_label: The Dns name label for the IP.
+    :vartype dns_name_label: str
+    :ivar dns_name_label_reuse_policy: The value representing the security enum. Possible values
+     include: "Unsecure", "TenantReuse", "SubscriptionReuse", "ResourceGroupReuse", "Noreuse".
+    :vartype dns_name_label_reuse_policy: str or
+     ~azure.mgmt.containerinstance.models.AutoGeneratedDomainNameLabelScope
     :ivar fqdn: The FQDN for the IP.
     :vartype fqdn: str
     """
 
     _validation = {
         'ports': {'required': True},
         'type': {'required': True},
@@ -1486,50 +1787,68 @@
     }
 
     _attribute_map = {
         'ports': {'key': 'ports', 'type': '[Port]'},
         'type': {'key': 'type', 'type': 'str'},
         'ip': {'key': 'ip', 'type': 'str'},
         'dns_name_label': {'key': 'dnsNameLabel', 'type': 'str'},
+        'dns_name_label_reuse_policy': {'key': 'dnsNameLabelReusePolicy', 'type': 'str'},
         'fqdn': {'key': 'fqdn', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         ports: List["Port"],
         type: Union[str, "ContainerGroupIpAddressType"],
         ip: Optional[str] = None,
         dns_name_label: Optional[str] = None,
+        dns_name_label_reuse_policy: Optional[Union[str, "AutoGeneratedDomainNameLabelScope"]] = None,
         **kwargs
     ):
+        """
+        :keyword ports: Required. The list of ports exposed on the container group.
+        :paramtype ports: list[~azure.mgmt.containerinstance.models.Port]
+        :keyword type: Required. Specifies if the IP is exposed to the public internet or private VNET.
+         Possible values include: "Public", "Private".
+        :paramtype type: str or ~azure.mgmt.containerinstance.models.ContainerGroupIpAddressType
+        :keyword ip: The IP exposed to the public internet.
+        :paramtype ip: str
+        :keyword dns_name_label: The Dns name label for the IP.
+        :paramtype dns_name_label: str
+        :keyword dns_name_label_reuse_policy: The value representing the security enum. Possible values
+         include: "Unsecure", "TenantReuse", "SubscriptionReuse", "ResourceGroupReuse", "Noreuse".
+        :paramtype dns_name_label_reuse_policy: str or
+         ~azure.mgmt.containerinstance.models.AutoGeneratedDomainNameLabelScope
+        """
         super(IpAddress, self).__init__(**kwargs)
         self.ports = ports
         self.type = type
         self.ip = ip
         self.dns_name_label = dns_name_label
+        self.dns_name_label_reuse_policy = dns_name_label_reuse_policy
         self.fqdn = None
 
 
 class LogAnalytics(msrest.serialization.Model):
     """Container group log analytics information.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param workspace_id: Required. The workspace id for log analytics.
-    :type workspace_id: str
-    :param workspace_key: Required. The workspace key for log analytics.
-    :type workspace_key: str
-    :param log_type: The log type to be used. Possible values include: "ContainerInsights",
+    :ivar workspace_id: Required. The workspace id for log analytics.
+    :vartype workspace_id: str
+    :ivar workspace_key: Required. The workspace key for log analytics.
+    :vartype workspace_key: str
+    :ivar log_type: The log type to be used. Possible values include: "ContainerInsights",
      "ContainerInstanceLogs".
-    :type log_type: str or ~azure.mgmt.containerinstance.models.LogAnalyticsLogType
-    :param metadata: Metadata for log analytics.
-    :type metadata: dict[str, str]
-    :param workspace_resource_id: The workspace resource id for log analytics.
-    :type workspace_resource_id: str
+    :vartype log_type: str or ~azure.mgmt.containerinstance.models.LogAnalyticsLogType
+    :ivar metadata: Metadata for log analytics.
+    :vartype metadata: dict[str, str]
+    :ivar workspace_resource_id: The workspace resource id for log analytics.
+    :vartype workspace_resource_id: str
     """
 
     _validation = {
         'workspace_id': {'required': True},
         'workspace_key': {'required': True},
     }
 
@@ -1547,57 +1866,74 @@
         workspace_id: str,
         workspace_key: str,
         log_type: Optional[Union[str, "LogAnalyticsLogType"]] = None,
         metadata: Optional[Dict[str, str]] = None,
         workspace_resource_id: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword workspace_id: Required. The workspace id for log analytics.
+        :paramtype workspace_id: str
+        :keyword workspace_key: Required. The workspace key for log analytics.
+        :paramtype workspace_key: str
+        :keyword log_type: The log type to be used. Possible values include: "ContainerInsights",
+         "ContainerInstanceLogs".
+        :paramtype log_type: str or ~azure.mgmt.containerinstance.models.LogAnalyticsLogType
+        :keyword metadata: Metadata for log analytics.
+        :paramtype metadata: dict[str, str]
+        :keyword workspace_resource_id: The workspace resource id for log analytics.
+        :paramtype workspace_resource_id: str
+        """
         super(LogAnalytics, self).__init__(**kwargs)
         self.workspace_id = workspace_id
         self.workspace_key = workspace_key
         self.log_type = log_type
         self.metadata = metadata
         self.workspace_resource_id = workspace_resource_id
 
 
 class Logs(msrest.serialization.Model):
     """The logs.
 
-    :param content: The content of the log.
-    :type content: str
+    :ivar content: The content of the log.
+    :vartype content: str
     """
 
     _attribute_map = {
         'content': {'key': 'content', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         content: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword content: The content of the log.
+        :paramtype content: str
+        """
         super(Logs, self).__init__(**kwargs)
         self.content = content
 
 
 class Operation(msrest.serialization.Model):
     """An operation for Azure Container Instance service.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The name of the operation.
-    :type name: str
-    :param display: Required. The display information of the operation.
-    :type display: ~azure.mgmt.containerinstance.models.OperationDisplay
-    :param properties: The additional properties.
-    :type properties: any
-    :param origin: The intended executor of the operation. Possible values include: "User",
+    :ivar name: Required. The name of the operation.
+    :vartype name: str
+    :ivar display: Required. The display information of the operation.
+    :vartype display: ~azure.mgmt.containerinstance.models.OperationDisplay
+    :ivar properties: The additional properties.
+    :vartype properties: any
+    :ivar origin: The intended executor of the operation. Possible values include: "User",
      "System".
-    :type origin: str or ~azure.mgmt.containerinstance.models.ContainerInstanceOperationsOrigin
+    :vartype origin: str or ~azure.mgmt.containerinstance.models.ContainerInstanceOperationsOrigin
     """
 
     _validation = {
         'name': {'required': True},
         'display': {'required': True},
     }
 
@@ -1613,32 +1949,44 @@
         *,
         name: str,
         display: "OperationDisplay",
         properties: Optional[Any] = None,
         origin: Optional[Union[str, "ContainerInstanceOperationsOrigin"]] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The name of the operation.
+        :paramtype name: str
+        :keyword display: Required. The display information of the operation.
+        :paramtype display: ~azure.mgmt.containerinstance.models.OperationDisplay
+        :keyword properties: The additional properties.
+        :paramtype properties: any
+        :keyword origin: The intended executor of the operation. Possible values include: "User",
+         "System".
+        :paramtype origin: str or
+         ~azure.mgmt.containerinstance.models.ContainerInstanceOperationsOrigin
+        """
         super(Operation, self).__init__(**kwargs)
         self.name = name
         self.display = display
         self.properties = properties
         self.origin = origin
 
 
 class OperationDisplay(msrest.serialization.Model):
     """The display information of the operation.
 
-    :param provider: The name of the provider of the operation.
-    :type provider: str
-    :param resource: The name of the resource type of the operation.
-    :type resource: str
-    :param operation: The friendly name of the operation.
-    :type operation: str
-    :param description: The description of the operation.
-    :type description: str
+    :ivar provider: The name of the provider of the operation.
+    :vartype provider: str
+    :ivar resource: The name of the resource type of the operation.
+    :vartype resource: str
+    :ivar operation: The friendly name of the operation.
+    :vartype operation: str
+    :ivar description: The description of the operation.
+    :vartype description: str
     """
 
     _attribute_map = {
         'provider': {'key': 'provider', 'type': 'str'},
         'resource': {'key': 'resource', 'type': 'str'},
         'operation': {'key': 'operation', 'type': 'str'},
         'description': {'key': 'description', 'type': 'str'},
@@ -1649,56 +1997,72 @@
         *,
         provider: Optional[str] = None,
         resource: Optional[str] = None,
         operation: Optional[str] = None,
         description: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword provider: The name of the provider of the operation.
+        :paramtype provider: str
+        :keyword resource: The name of the resource type of the operation.
+        :paramtype resource: str
+        :keyword operation: The friendly name of the operation.
+        :paramtype operation: str
+        :keyword description: The description of the operation.
+        :paramtype description: str
+        """
         super(OperationDisplay, self).__init__(**kwargs)
         self.provider = provider
         self.resource = resource
         self.operation = operation
         self.description = description
 
 
 class OperationListResult(msrest.serialization.Model):
     """The operation list response that contains all operations for Azure Container Instance service.
 
-    :param value: The list of operations.
-    :type value: list[~azure.mgmt.containerinstance.models.Operation]
-    :param next_link: The URI to fetch the next page of operations.
-    :type next_link: str
+    :ivar value: The list of operations.
+    :vartype value: list[~azure.mgmt.containerinstance.models.Operation]
+    :ivar next_link: The URI to fetch the next page of operations.
+    :vartype next_link: str
     """
 
     _attribute_map = {
         'value': {'key': 'value', 'type': '[Operation]'},
         'next_link': {'key': 'nextLink', 'type': 'str'},
     }
 
     def __init__(
         self,
         *,
         value: Optional[List["Operation"]] = None,
         next_link: Optional[str] = None,
         **kwargs
     ):
+        """
+        :keyword value: The list of operations.
+        :paramtype value: list[~azure.mgmt.containerinstance.models.Operation]
+        :keyword next_link: The URI to fetch the next page of operations.
+        :paramtype next_link: str
+        """
         super(OperationListResult, self).__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
 class Port(msrest.serialization.Model):
     """The port exposed on the container group.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param protocol: The protocol associated with the port. Possible values include: "TCP", "UDP".
-    :type protocol: str or ~azure.mgmt.containerinstance.models.ContainerGroupNetworkProtocol
-    :param port: Required. The port number.
-    :type port: int
+    :ivar protocol: The protocol associated with the port. Possible values include: "TCP", "UDP".
+    :vartype protocol: str or ~azure.mgmt.containerinstance.models.ContainerGroupNetworkProtocol
+    :ivar port: Required. The port number.
+    :vartype port: int
     """
 
     _validation = {
         'port': {'required': True},
     }
 
     _attribute_map = {
@@ -1709,28 +2073,35 @@
     def __init__(
         self,
         *,
         port: int,
         protocol: Optional[Union[str, "ContainerGroupNetworkProtocol"]] = None,
         **kwargs
     ):
+        """
+        :keyword protocol: The protocol associated with the port. Possible values include: "TCP",
+         "UDP".
+        :paramtype protocol: str or ~azure.mgmt.containerinstance.models.ContainerGroupNetworkProtocol
+        :keyword port: Required. The port number.
+        :paramtype port: int
+        """
         super(Port, self).__init__(**kwargs)
         self.protocol = protocol
         self.port = port
 
 
 class ResourceLimits(msrest.serialization.Model):
     """The resource limits.
 
-    :param memory_in_gb: The memory limit in GB of this container instance.
-    :type memory_in_gb: float
-    :param cpu: The CPU limit of this container instance.
-    :type cpu: float
-    :param gpu: The GPU limit of this container instance.
-    :type gpu: ~azure.mgmt.containerinstance.models.GpuResource
+    :ivar memory_in_gb: The memory limit in GB of this container instance.
+    :vartype memory_in_gb: float
+    :ivar cpu: The CPU limit of this container instance.
+    :vartype cpu: float
+    :ivar gpu: The GPU limit of this container instance.
+    :vartype gpu: ~azure.mgmt.containerinstance.models.GpuResource
     """
 
     _attribute_map = {
         'memory_in_gb': {'key': 'memoryInGB', 'type': 'float'},
         'cpu': {'key': 'cpu', 'type': 'float'},
         'gpu': {'key': 'gpu', 'type': 'GpuResource'},
     }
@@ -1739,31 +2110,39 @@
         self,
         *,
         memory_in_gb: Optional[float] = None,
         cpu: Optional[float] = None,
         gpu: Optional["GpuResource"] = None,
         **kwargs
     ):
+        """
+        :keyword memory_in_gb: The memory limit in GB of this container instance.
+        :paramtype memory_in_gb: float
+        :keyword cpu: The CPU limit of this container instance.
+        :paramtype cpu: float
+        :keyword gpu: The GPU limit of this container instance.
+        :paramtype gpu: ~azure.mgmt.containerinstance.models.GpuResource
+        """
         super(ResourceLimits, self).__init__(**kwargs)
         self.memory_in_gb = memory_in_gb
         self.cpu = cpu
         self.gpu = gpu
 
 
 class ResourceRequests(msrest.serialization.Model):
     """The resource requests.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param memory_in_gb: Required. The memory request in GB of this container instance.
-    :type memory_in_gb: float
-    :param cpu: Required. The CPU request of this container instance.
-    :type cpu: float
-    :param gpu: The GPU request of this container instance.
-    :type gpu: ~azure.mgmt.containerinstance.models.GpuResource
+    :ivar memory_in_gb: Required. The memory request in GB of this container instance.
+    :vartype memory_in_gb: float
+    :ivar cpu: Required. The CPU request of this container instance.
+    :vartype cpu: float
+    :ivar gpu: The GPU request of this container instance.
+    :vartype gpu: ~azure.mgmt.containerinstance.models.GpuResource
     """
 
     _validation = {
         'memory_in_gb': {'required': True},
         'cpu': {'required': True},
     }
 
@@ -1777,29 +2156,37 @@
         self,
         *,
         memory_in_gb: float,
         cpu: float,
         gpu: Optional["GpuResource"] = None,
         **kwargs
     ):
+        """
+        :keyword memory_in_gb: Required. The memory request in GB of this container instance.
+        :paramtype memory_in_gb: float
+        :keyword cpu: Required. The CPU request of this container instance.
+        :paramtype cpu: float
+        :keyword gpu: The GPU request of this container instance.
+        :paramtype gpu: ~azure.mgmt.containerinstance.models.GpuResource
+        """
         super(ResourceRequests, self).__init__(**kwargs)
         self.memory_in_gb = memory_in_gb
         self.cpu = cpu
         self.gpu = gpu
 
 
 class ResourceRequirements(msrest.serialization.Model):
     """The resource requirements.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param requests: Required. The resource requests of this container instance.
-    :type requests: ~azure.mgmt.containerinstance.models.ResourceRequests
-    :param limits: The resource limits of this container instance.
-    :type limits: ~azure.mgmt.containerinstance.models.ResourceLimits
+    :ivar requests: Required. The resource requests of this container instance.
+    :vartype requests: ~azure.mgmt.containerinstance.models.ResourceRequests
+    :ivar limits: The resource limits of this container instance.
+    :vartype limits: ~azure.mgmt.containerinstance.models.ResourceLimits
     """
 
     _validation = {
         'requests': {'required': True},
     }
 
     _attribute_map = {
@@ -1810,14 +2197,20 @@
     def __init__(
         self,
         *,
         requests: "ResourceRequests",
         limits: Optional["ResourceLimits"] = None,
         **kwargs
     ):
+        """
+        :keyword requests: Required. The resource requests of this container instance.
+        :paramtype requests: ~azure.mgmt.containerinstance.models.ResourceRequests
+        :keyword limits: The resource limits of this container instance.
+        :paramtype limits: ~azure.mgmt.containerinstance.models.ResourceLimits
+        """
         super(ResourceRequirements, self).__init__(**kwargs)
         self.requests = requests
         self.limits = limits
 
 
 class Usage(msrest.serialization.Model):
     """A single usage result.
@@ -1848,14 +2241,16 @@
         'name': {'key': 'name', 'type': 'UsageName'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(Usage, self).__init__(**kwargs)
         self.unit = None
         self.current_value = None
         self.limit = None
         self.name = None
 
 
@@ -1876,14 +2271,16 @@
         'value': {'key': 'value', 'type': '[Usage]'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(UsageListResult, self).__init__(**kwargs)
         self.value = None
 
 
 class UsageName(msrest.serialization.Model):
     """The name object of the resource.
 
@@ -1905,34 +2302,36 @@
         'localized_value': {'key': 'localizedValue', 'type': 'str'},
     }
 
     def __init__(
         self,
         **kwargs
     ):
+        """
+        """
         super(UsageName, self).__init__(**kwargs)
         self.value = None
         self.localized_value = None
 
 
 class Volume(msrest.serialization.Model):
     """The properties of the volume.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The name of the volume.
-    :type name: str
-    :param azure_file: The Azure File volume.
-    :type azure_file: ~azure.mgmt.containerinstance.models.AzureFileVolume
-    :param empty_dir: The empty directory volume.
-    :type empty_dir: any
-    :param secret: The secret volume.
-    :type secret: dict[str, str]
-    :param git_repo: The git repo volume.
-    :type git_repo: ~azure.mgmt.containerinstance.models.GitRepoVolume
+    :ivar name: Required. The name of the volume.
+    :vartype name: str
+    :ivar azure_file: The Azure File volume.
+    :vartype azure_file: ~azure.mgmt.containerinstance.models.AzureFileVolume
+    :ivar empty_dir: The empty directory volume.
+    :vartype empty_dir: any
+    :ivar secret: The secret volume.
+    :vartype secret: dict[str, str]
+    :ivar git_repo: The git repo volume.
+    :vartype git_repo: ~azure.mgmt.containerinstance.models.GitRepoVolume
     """
 
     _validation = {
         'name': {'required': True},
     }
 
     _attribute_map = {
@@ -1949,34 +2348,46 @@
         name: str,
         azure_file: Optional["AzureFileVolume"] = None,
         empty_dir: Optional[Any] = None,
         secret: Optional[Dict[str, str]] = None,
         git_repo: Optional["GitRepoVolume"] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The name of the volume.
+        :paramtype name: str
+        :keyword azure_file: The Azure File volume.
+        :paramtype azure_file: ~azure.mgmt.containerinstance.models.AzureFileVolume
+        :keyword empty_dir: The empty directory volume.
+        :paramtype empty_dir: any
+        :keyword secret: The secret volume.
+        :paramtype secret: dict[str, str]
+        :keyword git_repo: The git repo volume.
+        :paramtype git_repo: ~azure.mgmt.containerinstance.models.GitRepoVolume
+        """
         super(Volume, self).__init__(**kwargs)
         self.name = name
         self.azure_file = azure_file
         self.empty_dir = empty_dir
         self.secret = secret
         self.git_repo = git_repo
 
 
 class VolumeMount(msrest.serialization.Model):
     """The properties of the volume mount.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param name: Required. The name of the volume mount.
-    :type name: str
-    :param mount_path: Required. The path within the container where the volume should be mounted.
+    :ivar name: Required. The name of the volume mount.
+    :vartype name: str
+    :ivar mount_path: Required. The path within the container where the volume should be mounted.
      Must not contain colon (:).
-    :type mount_path: str
-    :param read_only: The flag indicating whether the volume mount is read-only.
-    :type read_only: bool
+    :vartype mount_path: str
+    :ivar read_only: The flag indicating whether the volume mount is read-only.
+    :vartype read_only: bool
     """
 
     _validation = {
         'name': {'required': True},
         'mount_path': {'required': True},
     }
 
@@ -1990,11 +2401,20 @@
         self,
         *,
         name: str,
         mount_path: str,
         read_only: Optional[bool] = None,
         **kwargs
     ):
+        """
+        :keyword name: Required. The name of the volume mount.
+        :paramtype name: str
+        :keyword mount_path: Required. The path within the container where the volume should be
+         mounted. Must not contain colon (:).
+        :paramtype mount_path: str
+        :keyword read_only: The flag indicating whether the volume mount is read-only.
+        :paramtype read_only: bool
+        """
         super(VolumeMount, self).__init__(**kwargs)
         self.name = name
         self.mount_path = mount_path
         self.read_only = read_only
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/__init__.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,7 +4,12 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._container_instance_management_client import ContainerInstanceManagementClient
 __all__ = ['ContainerInstanceManagementClient']
+
+# `._patch.py` is used for handwritten extensions to the generated code
+# Example: https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/customize_code/how-to-patch-sdk-code.md
+from ._patch import patch_sdk
+patch_sdk()
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_configuration.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,62 +6,63 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class ContainerInstanceManagementClientConfiguration(Configuration):
     """Configuration for ContainerInstanceManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
     :type subscription_id: str
     """
 
     def __init__(
         self,
-        credential: "AsyncTokenCredential",
+        credential: "TokenCredential",
         subscription_id: str,
         **kwargs: Any
     ) -> None:
+        super(ContainerInstanceManagementClientConfiguration, self).__init__(**kwargs)
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
-        super(ContainerInstanceManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-09-01"
+        self.api_version = "2021-10-01"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-containerinstance/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
-        **kwargs: Any
-    ) -> None:
+        **kwargs  # type: Any
+    ):
+        # type: (...) -> None
         self.user_agent_policy = kwargs.get('user_agent_policy') or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get('headers_policy') or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get('proxy_policy') or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get('logging_policy') or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get('http_logging_policy') or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get('retry_policy') or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get('retry_policy') or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get('custom_hook_policy') or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get('redirect_policy') or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get('redirect_policy') or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get('authentication_policy')
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = policies.AsyncBearerTokenCredentialPolicy(self.credential, *self.credential_scopes, **kwargs)
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(self.credential, *self.credential_scopes, **kwargs)
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/_container_instance_management_client.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/_container_instance_management_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,96 +2,102 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from copy import deepcopy
 from typing import Any, Optional, TYPE_CHECKING
 
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
-from azure.mgmt.core import AsyncARMPipelineClient
+from azure.core.rest import HttpRequest, HttpResponse
+from azure.mgmt.core import ARMPipelineClient
 from msrest import Deserializer, Serializer
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
-
+from . import models
 from ._configuration import ContainerInstanceManagementClientConfiguration
-from .operations import ContainerGroupsOperations
-from .operations import Operations
-from .operations import LocationOperations
-from .operations import ContainersOperations
-from .. import models
+from .operations import ContainerGroupsOperations, ContainersOperations, LocationOperations, Operations
 
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from azure.core.credentials import TokenCredential
 
-class ContainerInstanceManagementClient(object):
+class ContainerInstanceManagementClient:
     """ContainerInstanceManagementClient.
 
     :ivar container_groups: ContainerGroupsOperations operations
-    :vartype container_groups: azure.mgmt.containerinstance.aio.operations.ContainerGroupsOperations
+    :vartype container_groups: azure.mgmt.containerinstance.operations.ContainerGroupsOperations
     :ivar operations: Operations operations
-    :vartype operations: azure.mgmt.containerinstance.aio.operations.Operations
+    :vartype operations: azure.mgmt.containerinstance.operations.Operations
     :ivar location: LocationOperations operations
-    :vartype location: azure.mgmt.containerinstance.aio.operations.LocationOperations
+    :vartype location: azure.mgmt.containerinstance.operations.LocationOperations
     :ivar containers: ContainersOperations operations
-    :vartype containers: azure.mgmt.containerinstance.aio.operations.ContainersOperations
+    :vartype containers: azure.mgmt.containerinstance.operations.ContainersOperations
     :param credential: Credential needed for the client to connect to Azure.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
+    :type credential: ~azure.core.credentials.TokenCredential
+    :param subscription_id: Subscription credentials which uniquely identify Microsoft Azure
+     subscription. The subscription ID forms part of the URI for every service call.
     :type subscription_id: str
-    :param str base_url: Service URL
-    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+    :param base_url: Service URL. Default value is 'https://management.azure.com'.
+    :type base_url: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(
         self,
-        credential: "AsyncTokenCredential",
+        credential: "TokenCredential",
         subscription_id: str,
-        base_url: Optional[str] = None,
+        base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
-        if not base_url:
-            base_url = 'https://management.azure.com'
-        self._config = ContainerInstanceManagementClientConfiguration(credential, subscription_id, **kwargs)
-        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._config = ContainerInstanceManagementClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
-        self._serialize.client_side_validation = False
         self._deserialize = Deserializer(client_models)
+        self._serialize.client_side_validation = False
+        self.container_groups = ContainerGroupsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
+        self.location = LocationOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.containers = ContainersOperations(self._client, self._config, self._serialize, self._deserialize)
 
-        self.container_groups = ContainerGroupsOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.operations = Operations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.location = LocationOperations(
-            self._client, self._config, self._serialize, self._deserialize)
-        self.containers = ContainersOperations(
-            self._client, self._config, self._serialize, self._deserialize)
 
-    async def _send_request(self, http_request: HttpRequest, **kwargs: Any) -> AsyncHttpResponse:
+    def _send_request(
+        self,
+        request,  # type: HttpRequest
+        **kwargs: Any
+    ) -> HttpResponse:
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
+        For more information on this code flow, see https://aka.ms/azsdk/python/protocol/quickstart
+
+        :param request: The network request you want to make. Required.
+        :type request: ~azure.core.rest.HttpRequest
+        :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.pipeline.transport.AsyncHttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-        }
-        http_request.url = self._client.format_url(http_request.url, **path_format_arguments)
-        stream = kwargs.pop("stream", True)
-        pipeline_response = await self._client._pipeline.run(http_request, stream=stream, **kwargs)
-        return pipeline_response.http_response
-
-    async def close(self) -> None:
-        await self._client.close()
 
-    async def __aenter__(self) -> "ContainerInstanceManagementClient":
-        await self._client.__aenter__()
+        request_copy = deepcopy(request)
+        request_copy.url = self._client.format_url(request_copy.url)
+        return self._client.send_request(request_copy, **kwargs)
+
+    def close(self):
+        # type: () -> None
+        self._client.close()
+
+    def __enter__(self):
+        # type: () -> ContainerInstanceManagementClient
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details):
+        # type: (Any) -> None
+        self._client.__exit__(*exc_details)
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_location_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+import functools
 from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
 import warnings
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
-
+from ..._vendor import _convert_request
+from ...operations._location_operations import build_list_cached_images_request, build_list_capabilities_request, build_list_usage_request
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class LocationOperations:
     """LocationOperations async operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
@@ -37,62 +42,60 @@
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list_usage(
         self,
         location: str,
         **kwargs: Any
     ) -> AsyncIterable["_models.UsageListResult"]:
         """Get the usage for a subscription.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either UsageListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.UsageListResult]
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.UsageListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.UsageListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_usage.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_usage_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_usage.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_usage_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('UsageListResult', pipeline_response)
+            deserialized = self._deserialize("UsageListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -102,69 +105,69 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return AsyncItemPaged(
             get_next, extract_data
         )
     list_usage.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/usages'}  # type: ignore
 
+    @distributed_trace
     def list_cached_images(
         self,
         location: str,
         **kwargs: Any
     ) -> AsyncIterable["_models.CachedImagesListResult"]:
         """Get the list of cached images.
 
         Get the list of cached images on specific OS type for a subscription in a region.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either CachedImagesListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.CachedImagesListResult]
+        :return: An iterator like instance of either CachedImagesListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.CachedImagesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CachedImagesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_cached_images.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_cached_images_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_cached_images.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_cached_images_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('CachedImagesListResult', pipeline_response)
+            deserialized = self._deserialize("CachedImagesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -174,69 +177,69 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return AsyncItemPaged(
             get_next, extract_data
         )
     list_cached_images.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/cachedImages'}  # type: ignore
 
+    @distributed_trace
     def list_capabilities(
         self,
         location: str,
         **kwargs: Any
     ) -> AsyncIterable["_models.CapabilitiesListResult"]:
         """Get the list of capabilities of the location.
 
         Get the list of CPU/memory/GPU capabilities of a region.
 
         :param location: The identifier for the physical azure location.
         :type location: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either CapabilitiesListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.CapabilitiesListResult]
+        :return: An iterator like instance of either CapabilitiesListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.CapabilitiesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CapabilitiesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_capabilities.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'location': self._serialize.url("location", location, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_capabilities_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=self.list_capabilities.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_capabilities_request(
+                    subscription_id=self._config.subscription_id,
+                    location=location,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('CapabilitiesListResult', pipeline_response)
+            deserialized = self._deserialize("CapabilitiesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -246,11 +249,12 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return AsyncItemPaged(
             get_next, extract_data
         )
     list_capabilities.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/locations/{location}/capabilities'}  # type: ignore
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/operations/_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,134 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
+import functools
+from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
 import warnings
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
 from azure.mgmt.core.exceptions import ARMErrorFormat
+from msrest import Serializer
 
-from ... import models as _models
-
+from .. import models as _models
+from .._vendor import _convert_request
 T = TypeVar('T')
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+def build_list_request(
+    **kwargs: Any
+) -> HttpRequest:
+    api_version = "2021-10-01"
+    accept = "application/json"
+    # Construct URL
+    url = kwargs.pop("template_url", '/providers/Microsoft.ContainerInstance/operations')
+
+    # Construct parameters
+    query_parameters = kwargs.pop("params", {})  # type: Dict[str, Any]
+    query_parameters['api-version'] = _SERIALIZER.query("api_version", api_version, 'str')
+
+    # Construct headers
+    header_parameters = kwargs.pop("headers", {})  # type: Dict[str, Any]
+    header_parameters['Accept'] = _SERIALIZER.header("accept", accept, 'str')
+
+    return HttpRequest(
+        method="GET",
+        url=url,
+        params=query_parameters,
+        headers=header_parameters,
+        **kwargs
+    )
 
-class Operations:
-    """Operations async operations.
+class Operations(object):
+    """Operations operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
     :ivar models: Alias to model classes used in this operation group.
     :type models: ~azure.mgmt.containerinstance.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
     models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
+    def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list(
         self,
         **kwargs: Any
-    ) -> AsyncIterable["_models.OperationListResult"]:
+    ) -> Iterable["_models.OperationListResult"]:
         """List the operations for Azure Container Instance service.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.OperationListResult]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.containerinstance.models.OperationListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_request(
+                    template_url=self.list.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_request(
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize('OperationListResult', pipeline_response)
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(
+
+        return ItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/providers/Microsoft.ContainerInstance/operations'}  # type: ignore
```

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/__init__.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerinstance-9.1.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py` & `azure-mgmt-containerinstance-9.2.0/azure/mgmt/containerinstance/aio/operations/_container_groups_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+import functools
 from typing import Any, AsyncIterable, Callable, Dict, Generic, List, Optional, TypeVar, Union
 import warnings
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.rest import HttpRequest
+from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
-
+from ..._vendor import _convert_request
+from ...operations._container_groups_operations import build_create_or_update_request_initial, build_delete_request_initial, build_get_outbound_network_dependencies_endpoints_request, build_get_request, build_list_by_resource_group_request, build_list_request, build_restart_request_initial, build_start_request_initial, build_stop_request, build_update_request
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class ContainerGroupsOperations:
     """ContainerGroupsOperations async operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
@@ -39,62 +44,60 @@
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
+    @distributed_trace
     def list(
         self,
         **kwargs: Any
     ) -> AsyncIterable["_models.ContainerGroupListResult"]:
         """Get a list of container groups in the specified subscription.
 
         Get a list of container groups in the specified subscription. This operation returns properties
         of each container group including containers, image registry credentials, restart policy, IP
         address type, OS type, state, and volumes.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ContainerGroupListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
+        :return: An iterator like instance of either ContainerGroupListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    template_url=self.list.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('ContainerGroupListResult', pipeline_response)
+            deserialized = self._deserialize("ContainerGroupListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -104,71 +107,71 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return AsyncItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.ContainerInstance/containerGroups'}  # type: ignore
 
+    @distributed_trace
     def list_by_resource_group(
         self,
         resource_group_name: str,
         **kwargs: Any
     ) -> AsyncIterable["_models.ContainerGroupListResult"]:
         """Get a list of container groups in the specified subscription and resource group.
 
         Get a list of container groups in a specified subscription and resource group. This operation
         returns properties of each container group including containers, image registry credentials,
         restart policy, IP address type, OS type, state, and volumes.
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ContainerGroupListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
+        :return: An iterator like instance of either ContainerGroupListResult or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.containerinstance.models.ContainerGroupListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
         def prepare_request(next_link=None):
-            # Construct headers
-            header_parameters = {}  # type: Dict[str, Any]
-            header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
             if not next_link:
-                # Construct URL
-                url = self.list_by_resource_group.metadata['url']  # type: ignore
-                path_format_arguments = {
-                    'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-                    'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-                }
-                url = self._client.format_url(url, **path_format_arguments)
-                # Construct parameters
-                query_parameters = {}  # type: Dict[str, Any]
-                query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+                
+                request = build_list_by_resource_group_request(
+                    subscription_id=self._config.subscription_id,
+                    resource_group_name=resource_group_name,
+                    template_url=self.list_by_resource_group.metadata['url'],
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-                request = self._client.get(url, query_parameters, header_parameters)
             else:
-                url = next_link
-                query_parameters = {}  # type: Dict[str, Any]
-                request = self._client.get(url, query_parameters, header_parameters)
+                
+                request = build_list_by_resource_group_request(
+                    subscription_id=self._config.subscription_id,
+                    resource_group_name=resource_group_name,
+                    template_url=next_link,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize('ContainerGroupListResult', pipeline_response)
+            deserialized = self._deserialize("ContainerGroupListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
@@ -178,19 +181,21 @@
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
+
         return AsyncItemPaged(
             get_next, extract_data
         )
     list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups'}  # type: ignore
 
+    @distributed_trace_async
     async def get(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> "_models.ContainerGroup":
         """Get the properties of the specified container group.
@@ -209,88 +214,70 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
-
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
 
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_get_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.get.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.get(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         container_group_name: str,
         container_group: "_models.ContainerGroup",
         **kwargs: Any
     ) -> "_models.ContainerGroup":
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        content_type = kwargs.pop("content_type", "application/json")
-        accept = "application/json"
-
-        # Construct URL
-        url = self._create_or_update_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
-        body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(container_group, 'ContainerGroup')
-        body_content_kwargs['content'] = body_content
-        request = self._client.put(url, query_parameters, header_parameters, **body_content_kwargs)
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+
+        _json = self._serialize.body(container_group, 'ContainerGroup')
+
+        request = build_create_or_update_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            content_type=content_type,
+            json=_json,
+            template_url=self._create_or_update_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -300,16 +287,19 @@
         if response.status_code == 201:
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
+    @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         container_group_name: str,
         container_group: "_models.ContainerGroup",
         **kwargs: Any
     ) -> AsyncLROPoller["_models.ContainerGroup"]:
@@ -321,68 +311,68 @@
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :param container_group: The properties of the container group to be created or updated.
         :type container_group: ~azure.mgmt.containerinstance.models.ContainerGroup
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ContainerGroup or the result of cls(response)
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ContainerGroup or the result of
+         cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.containerinstance.models.ContainerGroup]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 container_group=container_group,
+                content_type=content_type,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
+            response = pipeline_response.http_response
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
-
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+    @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
         container_group_name: str,
         resource: "_models.Resource",
         **kwargs: Any
     ) -> "_models.ContainerGroup":
@@ -402,87 +392,69 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        content_type = kwargs.pop("content_type", "application/json")
-        accept = "application/json"
-
-        # Construct URL
-        url = self.update.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
-
-        body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(resource, 'Resource')
-        body_content_kwargs['content'] = body_content
-        request = self._client.patch(url, query_parameters, header_parameters, **body_content_kwargs)
+        content_type = kwargs.pop('content_type', "application/json")  # type: Optional[str]
+
+        _json = self._serialize.body(resource, 'Resource')
+
+        request = build_update_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            content_type=content_type,
+            json=_json,
+            template_url=self.update.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
     async def _delete_initial(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> Optional["_models.ContainerGroup"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.ContainerGroup"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
 
-        # Construct URL
-        url = self._delete_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
-
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_delete_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._delete_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -490,16 +462,19 @@
         if response.status_code == 200:
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
+
+    @distributed_trace_async
     async def begin_delete(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> AsyncLROPoller["_models.ContainerGroup"]:
         """Delete the specified container group.
@@ -509,111 +484,100 @@
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ContainerGroup or the result of cls(response)
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either ContainerGroup or the result of
+         cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.containerinstance.models.ContainerGroup]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ContainerGroup"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._delete_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
+            response = pipeline_response.http_response
             deserialized = self._deserialize('ContainerGroup', pipeline_response)
-
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}'}  # type: ignore
 
     async def _restart_initial(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self._restart_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_restart_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._restart_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _restart_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/restart'}  # type: ignore
 
+
+    @distributed_trace_async
     async def begin_restart(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Restarts all containers in a container group.
@@ -623,64 +587,61 @@
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._restart_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_restart.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/restart'}  # type: ignore
 
+    @distributed_trace_async
     async def stop(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> None:
         """Stops all containers in a container group.
@@ -698,91 +659,74 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.stop.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_stop_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.stop.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     stop.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/stop'}  # type: ignore
 
+
     async def _start_initial(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self._start_initial.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_start_request_initial(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self._start_initial.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.post(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _start_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/start'}  # type: ignore
 
+
+    @distributed_trace_async
     async def begin_start(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Starts all containers in a container group.
@@ -792,64 +736,61 @@
 
         :param resource_group_name: The name of the resource group.
         :type resource_group_name: str
         :param container_group_name: The name of the container group.
         :type container_group_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling.
-         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
+        polling = kwargs.pop('polling', True)  # type: Union[bool, azure.core.polling.AsyncPollingMethod]
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._start_initial(
                 resource_group_name=resource_group_name,
                 container_group_name=container_group_name,
                 cls=lambda x,y,z: x,
                 **kwargs
             )
-
         kwargs.pop('error_map', None)
-        kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output
             )
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+
     begin_start.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/start'}  # type: ignore
 
+    @distributed_trace_async
     async def get_outbound_network_dependencies_endpoints(
         self,
         resource_group_name: str,
         container_group_name: str,
         **kwargs: Any
     ) -> List[str]:
         """Get all network dependencies for container group.
@@ -867,42 +808,34 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType[List[str]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-09-01"
-        accept = "application/json"
-
-        # Construct URL
-        url = self.get_outbound_network_dependencies_endpoints.metadata['url']  # type: ignore
-        path_format_arguments = {
-            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
-            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
-            'containerGroupName': self._serialize.url("container_group_name", container_group_name, 'str'),
-        }
-        url = self._client.format_url(url, **path_format_arguments)
 
-        # Construct parameters
-        query_parameters = {}  # type: Dict[str, Any]
-        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
-
-        # Construct headers
-        header_parameters = {}  # type: Dict[str, Any]
-        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+        
+        request = build_get_outbound_network_dependencies_endpoints_request(
+            subscription_id=self._config.subscription_id,
+            resource_group_name=resource_group_name,
+            container_group_name=container_group_name,
+            template_url=self.get_outbound_network_dependencies_endpoints.metadata['url'],
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
 
-        request = self._client.get(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize('[str]', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
+
     get_outbound_network_dependencies_endpoints.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerInstance/containerGroups/{containerGroupName}/outboundNetworkDependenciesEndpoints'}  # type: ignore
+
```

## Comparing `azure-mgmt-containerinstance-9.1.0/tests/test_cli_mgmt_containerinstance.py` & `azure-mgmt-containerinstance-9.2.0/tests/disable_test_cli_mgmt_containerinstance.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerinstance-9.1.0/tests/disable_test_mgmt_containerinstance.py` & `azure-mgmt-containerinstance-9.2.0/tests/disable_test_mgmt_containerinstance.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerinstance-9.1.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml` & `azure-mgmt-containerinstance-9.2.0/tests/recordings/test_mgmt_containerinstance.test_container_instance.yaml`

 * *Files identical despite different names*

