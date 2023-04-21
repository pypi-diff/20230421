# Comparing `tmp/azure-mgmt-containerservice-9.3.0.zip` & `tmp/azure-mgmt-containerservice-9.4.0.zip`

## zipinfo {}

```diff
@@ -1,324 +1,343 @@
-Zip file size: 688928 bytes, number of entries: 322
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/
--rw-r--r--  2.0 unx     3059 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/setup.py
--rw-r--r--  2.0 unx      107 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/MANIFEST.in
--rw-r--r--  2.0 unx      779 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/README.md
--rw-r--r--  2.0 unx       67 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/setup.cfg
--rw-r--r--  2.0 unx    18235 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/PKG-INFO
--rw-r--r--  2.0 unx    13291 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/CHANGELOG.md
--rw-r--r--  2.0 unx        1 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/not-zip-safe
--rw-r--r--  2.0 unx        1 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx    16493 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      101 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/requires.txt
--rw-r--r--  2.0 unx        6 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/top_level.txt
--rw-r--r--  2.0 unx    18235 b- defN 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/tests/recordings/
--rw-r--r--  2.0 unx     4345 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/tests/test_mgmt_containerservice.py
--rw-r--r--  2.0 unx    55188 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/tests/recordings/test_mgmt_containerservice.test_container.yaml
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/
--rw-r--r--  2.0 unx       64 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/
--rw-r--r--  2.0 unx       64 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/
--rw-r--r--  2.0 unx      428 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/models.py
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_configuration.py
--rw-r--r--  2.0 unx      492 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/__init__.py
--rw-r--r--  2.0 unx    22295 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_container_service_client.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py
--rw-r--r--  2.0 unx    79881 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py
--rw-r--r--  2.0 unx    78299 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py
--rw-r--r--  2.0 unx     8217 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py
--rw-r--r--  2.0 unx     6684 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py
--rw-r--r--  2.0 unx    56032 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/__init__.py
--rw-r--r--  2.0 unx     2413 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py
--rw-r--r--  2.0 unx    40581 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py
--rw-r--r--  2.0 unx    40228 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py
--rw-r--r--  2.0 unx     7706 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1434 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py
--rw-r--r--  2.0 unx     4018 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py
--rw-r--r--  2.0 unx    47466 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      644 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py
--rw-r--r--  2.0 unx     2219 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py
--rw-r--r--  2.0 unx    22111 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py
--rw-r--r--  2.0 unx    21964 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py
--rw-r--r--  2.0 unx     2012 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1024 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py
--rw-r--r--  2.0 unx     2765 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py
--rw-r--r--  2.0 unx    25682 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py
--rw-r--r--  2.0 unx      506 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py
--rw-r--r--  2.0 unx     2219 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py
--rw-r--r--  2.0 unx    22712 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py
--rw-r--r--  2.0 unx    22514 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py
--rw-r--r--  2.0 unx     2012 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1024 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py
--rw-r--r--  2.0 unx     2895 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py
--rw-r--r--  2.0 unx    25682 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py
--rw-r--r--  2.0 unx    79650 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py
--rw-r--r--  2.0 unx    78068 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py
--rw-r--r--  2.0 unx     8217 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py
--rw-r--r--  2.0 unx     6684 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py
--rw-r--r--  2.0 unx    52641 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py
--rw-r--r--  2.0 unx      506 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py
--rw-r--r--  2.0 unx     2219 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py
--rw-r--r--  2.0 unx    20398 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py
--rw-r--r--  2.0 unx    20265 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py
--rw-r--r--  2.0 unx     2012 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1024 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py
--rw-r--r--  2.0 unx     2590 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py
--rw-r--r--  2.0 unx    25682 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py
--rw-r--r--  2.0 unx    93791 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py
--rw-r--r--  2.0 unx    91559 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py
--rw-r--r--  2.0 unx     8656 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py
--rw-r--r--  2.0 unx     7698 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py
--rw-r--r--  2.0 unx    56032 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py
--rw-r--r--  2.0 unx    96307 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py
--rw-r--r--  2.0 unx    93893 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py
--rw-r--r--  2.0 unx     8640 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py
--rw-r--r--  2.0 unx     7834 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py
--rw-r--r--  2.0 unx    56371 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py
--rw-r--r--  2.0 unx    64569 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py
--rw-r--r--  2.0 unx    63518 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py
--rw-r--r--  2.0 unx     8043 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py
--rw-r--r--  2.0 unx     4791 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py
--rw-r--r--  2.0 unx    48456 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py
--rw-r--r--  2.0 unx    18303 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py
--rw-r--r--  2.0 unx    86200 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py
--rw-r--r--  2.0 unx    84239 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py
--rw-r--r--  2.0 unx     8334 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py
--rw-r--r--  2.0 unx     7208 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py
--rw-r--r--  2.0 unx    56032 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py
--rw-r--r--  2.0 unx      506 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py
--rw-r--r--  2.0 unx     2437 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py
--rw-r--r--  2.0 unx    43102 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py
--rw-r--r--  2.0 unx    42743 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py
--rw-r--r--  2.0 unx     7841 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1450 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py
--rw-r--r--  2.0 unx     4058 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py
--rw-r--r--  2.0 unx    47611 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      644 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py
--rw-r--r--  2.0 unx     3989 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py
--rw-r--r--  2.0 unx    20781 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py
--rw-r--r--  2.0 unx    20660 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py
--rw-r--r--  2.0 unx     2012 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1016 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py
--rw-r--r--  2.0 unx     2590 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py
--rw-r--r--  2.0 unx      619 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py
--rw-r--r--  2.0 unx    25586 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py
--rw-r--r--  2.0 unx      488 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/__init__.py
--rw-r--r--  2.0 unx     2108 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py
--rw-r--r--  2.0 unx    34321 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py
--rw-r--r--  2.0 unx    34082 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py
--rw-r--r--  2.0 unx     7742 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx      981 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py
--rw-r--r--  2.0 unx     3403 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py
--rw-r--r--  2.0 unx    24907 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py
--rw-r--r--  2.0 unx      596 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py
--rw-r--r--  2.0 unx    61836 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py
--rw-r--r--  2.0 unx    60806 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py
--rw-r--r--  2.0 unx     7861 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py
--rw-r--r--  2.0 unx     4494 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py
--rw-r--r--  2.0 unx    47466 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py
--rw-r--r--  2.0 unx    18137 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/__init__.py
--rw-r--r--  2.0 unx     3152 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py
--rw-r--r--  2.0 unx   103808 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py
--rw-r--r--  2.0 unx   101268 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py
--rw-r--r--  2.0 unx     9078 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py
--rw-r--r--  2.0 unx     8805 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py
--rw-r--r--  2.0 unx    17665 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py
--rw-r--r--  2.0 unx    61353 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      865 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py
--rw-r--r--  2.0 unx    86543 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py
--rw-r--r--  2.0 unx    84568 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py
--rw-r--r--  2.0 unx     8334 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py
--rw-r--r--  2.0 unx     7208 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py
--rw-r--r--  2.0 unx    56032 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py
--rw-r--r--  2.0 unx    74048 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py
--rw-r--r--  2.0 unx    72571 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py
--rw-r--r--  2.0 unx     8217 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py
--rw-r--r--  2.0 unx     5604 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py
--rw-r--r--  2.0 unx    48456 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/__init__.py
--rw-r--r--  2.0 unx     3152 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py
--rw-r--r--  2.0 unx   103388 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py
--rw-r--r--  2.0 unx   100758 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py
--rw-r--r--  2.0 unx     8989 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py
--rw-r--r--  2.0 unx     8769 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py
--rw-r--r--  2.0 unx    17665 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py
--rw-r--r--  2.0 unx    56371 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      865 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-02 03:18 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/
--rw-r--r--  2.0 unx     1993 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_configuration.py
--rw-r--r--  2.0 unx      498 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/version.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/__init__.py
--rw-r--r--  2.0 unx     2725 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py
--rw-r--r--  2.0 unx    91149 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py
--rw-r--r--  2.0 unx    88942 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py
--rw-r--r--  2.0 unx     8439 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py
--rw-r--r--  2.0 unx     1872 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py
--rw-r--r--  2.0 unx     7431 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py
--rw-r--r--  2.0 unx    56032 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py
--rw-r--r--  2.0 unx      730 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py
--rw-r--r--  2.0 unx     3957 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py
--rw-r--r--  2.0 unx    25197 b- defN 20-Sep-02 03:17 azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py
-322 files, 4227438 bytes uncompressed, 604402 bytes compressed:  85.7%
+Zip file size: 747672 bytes, number of entries: 341
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/
+-rw-r--r--  2.0 unx     3059 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/setup.py
+-rw-r--r--  2.0 unx      107 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/MANIFEST.in
+-rw-r--r--  2.0 unx      779 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/README.md
+-rw-r--r--  2.0 unx       67 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/setup.cfg
+-rw-r--r--  2.0 unx    19825 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/PKG-INFO
+-rw-r--r--  2.0 unx    14697 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/CHANGELOG.md
+-rw-r--r--  2.0 unx        1 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx        1 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx    17620 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      101 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/requires.txt
+-rw-r--r--  2.0 unx        6 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    19825 b- defN 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/tests/recordings/
+-rw-r--r--  2.0 unx     4345 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/tests/test_mgmt_containerservice.py
+-rw-r--r--  2.0 unx    51205 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/tests/recordings/test_mgmt_containerservice.test_container.yaml
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/
+-rw-r--r--  2.0 unx       64 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/
+-rw-r--r--  2.0 unx       64 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/
+-rw-r--r--  2.0 unx      428 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/models.py
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_configuration.py
+-rw-r--r--  2.0 unx      492 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/__init__.py
+-rw-r--r--  2.0 unx    25050 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_container_service_client.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py
+-rw-r--r--  2.0 unx    79881 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    78299 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py
+-rw-r--r--  2.0 unx     8217 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     6684 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py
+-rw-r--r--  2.0 unx    56032 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/__init__.py
+-rw-r--r--  2.0 unx     2413 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py
+-rw-r--r--  2.0 unx    40581 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py
+-rw-r--r--  2.0 unx    40228 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py
+-rw-r--r--  2.0 unx     7706 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1434 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py
+-rw-r--r--  2.0 unx     4018 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py
+-rw-r--r--  2.0 unx    47466 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      644 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py
+-rw-r--r--  2.0 unx     2219 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py
+-rw-r--r--  2.0 unx    22111 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py
+-rw-r--r--  2.0 unx    21964 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py
+-rw-r--r--  2.0 unx     2012 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1024 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py
+-rw-r--r--  2.0 unx     2765 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py
+-rw-r--r--  2.0 unx    25682 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py
+-rw-r--r--  2.0 unx      506 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py
+-rw-r--r--  2.0 unx     2219 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py
+-rw-r--r--  2.0 unx    22712 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py
+-rw-r--r--  2.0 unx    22514 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py
+-rw-r--r--  2.0 unx     2012 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1024 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py
+-rw-r--r--  2.0 unx     2895 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py
+-rw-r--r--  2.0 unx    25682 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/__init__.py
+-rw-r--r--  2.0 unx     3977 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/_container_service_client.py
+-rw-r--r--  2.0 unx   110899 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_models_py3.py
+-rw-r--r--  2.0 unx   108214 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_models.py
+-rw-r--r--  2.0 unx     9348 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     9260 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/__init__.py
+-rw-r--r--  2.0 unx    17665 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_private_endpoint_connections_operations.py
+-rw-r--r--  2.0 unx    69401 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx     1122 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/__init__.py
+-rw-r--r--  2.0 unx     4754 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_private_link_resources_operations.py
+-rw-r--r--  2.0 unx     5081 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_resolve_private_link_service_id_operations.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py
+-rw-r--r--  2.0 unx    79650 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    78068 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py
+-rw-r--r--  2.0 unx     8217 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     6684 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py
+-rw-r--r--  2.0 unx    52641 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py
+-rw-r--r--  2.0 unx      506 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py
+-rw-r--r--  2.0 unx     2219 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py
+-rw-r--r--  2.0 unx    20398 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py
+-rw-r--r--  2.0 unx    20265 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py
+-rw-r--r--  2.0 unx     2012 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1024 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py
+-rw-r--r--  2.0 unx     2590 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py
+-rw-r--r--  2.0 unx    25682 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py
+-rw-r--r--  2.0 unx    93791 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    91559 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py
+-rw-r--r--  2.0 unx     8656 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     7698 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py
+-rw-r--r--  2.0 unx    56032 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py
+-rw-r--r--  2.0 unx    96307 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    93893 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py
+-rw-r--r--  2.0 unx     8640 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     7834 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py
+-rw-r--r--  2.0 unx    56371 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py
+-rw-r--r--  2.0 unx    64569 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    63518 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py
+-rw-r--r--  2.0 unx     8043 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     4791 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py
+-rw-r--r--  2.0 unx    48456 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py
+-rw-r--r--  2.0 unx    18303 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py
+-rw-r--r--  2.0 unx    86200 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    84239 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py
+-rw-r--r--  2.0 unx     8334 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     7208 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py
+-rw-r--r--  2.0 unx    56032 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py
+-rw-r--r--  2.0 unx      506 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py
+-rw-r--r--  2.0 unx     2437 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py
+-rw-r--r--  2.0 unx    43102 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py
+-rw-r--r--  2.0 unx    42743 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py
+-rw-r--r--  2.0 unx     7841 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1450 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py
+-rw-r--r--  2.0 unx     4058 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py
+-rw-r--r--  2.0 unx    47611 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      644 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py
+-rw-r--r--  2.0 unx     3989 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/__init__.py
+-rw-r--r--  2.0 unx     2203 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py
+-rw-r--r--  2.0 unx    20781 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py
+-rw-r--r--  2.0 unx    20660 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py
+-rw-r--r--  2.0 unx     2012 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1016 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py
+-rw-r--r--  2.0 unx     2590 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py
+-rw-r--r--  2.0 unx      619 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py
+-rw-r--r--  2.0 unx    25586 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py
+-rw-r--r--  2.0 unx      488 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/__init__.py
+-rw-r--r--  2.0 unx     2108 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py
+-rw-r--r--  2.0 unx    34321 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    34082 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py
+-rw-r--r--  2.0 unx     7742 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx      981 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     3403 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py
+-rw-r--r--  2.0 unx    24907 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py
+-rw-r--r--  2.0 unx      596 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py
+-rw-r--r--  2.0 unx    61836 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    60806 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py
+-rw-r--r--  2.0 unx     7861 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     4494 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py
+-rw-r--r--  2.0 unx    47466 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py
+-rw-r--r--  2.0 unx    18137 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/__init__.py
+-rw-r--r--  2.0 unx     3152 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py
+-rw-r--r--  2.0 unx   103808 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py
+-rw-r--r--  2.0 unx   101268 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py
+-rw-r--r--  2.0 unx     9078 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     8805 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py
+-rw-r--r--  2.0 unx    17665 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py
+-rw-r--r--  2.0 unx    61353 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      865 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py
+-rw-r--r--  2.0 unx    86543 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    84568 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py
+-rw-r--r--  2.0 unx     8334 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     7208 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py
+-rw-r--r--  2.0 unx    56032 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py
+-rw-r--r--  2.0 unx    74048 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    72571 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py
+-rw-r--r--  2.0 unx     8217 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     5604 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py
+-rw-r--r--  2.0 unx    48456 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/__init__.py
+-rw-r--r--  2.0 unx     3152 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py
+-rw-r--r--  2.0 unx   103388 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py
+-rw-r--r--  2.0 unx   100758 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py
+-rw-r--r--  2.0 unx     8989 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     8769 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py
+-rw-r--r--  2.0 unx    17665 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py
+-rw-r--r--  2.0 unx    56371 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      865 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Sep-11 07:27 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/
+-rw-r--r--  2.0 unx     1993 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/_configuration.py
+-rw-r--r--  2.0 unx      498 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/version.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/__init__.py
+-rw-r--r--  2.0 unx     2725 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py
+-rw-r--r--  2.0 unx    91149 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py
+-rw-r--r--  2.0 unx    88942 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py
+-rw-r--r--  2.0 unx     8439 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py
+-rw-r--r--  2.0 unx     1872 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py
+-rw-r--r--  2.0 unx     7431 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py
+-rw-r--r--  2.0 unx    56032 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py
+-rw-r--r--  2.0 unx      730 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py
+-rw-r--r--  2.0 unx     3957 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py
+-rw-r--r--  2.0 unx    25197 b- defN 20-Sep-11 07:26 azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py
+341 files, 4605891 bytes uncompressed, 657912 bytes compressed:  85.7%
```

## zipnote {}

```diff
@@ -1,967 +1,1024 @@
-Filename: azure-mgmt-containerservice-9.3.0/
+Filename: azure-mgmt-containerservice-9.4.0/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/tests/
+Filename: azure-mgmt-containerservice-9.4.0/tests/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/
+Filename: azure-mgmt-containerservice-9.4.0/azure/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/setup.py
+Filename: azure-mgmt-containerservice-9.4.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/MANIFEST.in
+Filename: azure-mgmt-containerservice-9.4.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/README.md
+Filename: azure-mgmt-containerservice-9.4.0/README.md
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/setup.cfg
+Filename: azure-mgmt-containerservice-9.4.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/PKG-INFO
+Filename: azure-mgmt-containerservice-9.4.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/CHANGELOG.md
+Filename: azure-mgmt-containerservice-9.4.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/not-zip-safe
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/dependency_links.txt
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/SOURCES.txt
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/requires.txt
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/top_level.txt
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/PKG-INFO
+Filename: azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/tests/recordings/
+Filename: azure-mgmt-containerservice-9.4.0/tests/recordings/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/tests/test_mgmt_containerservice.py
+Filename: azure-mgmt-containerservice-9.4.0/tests/test_mgmt_containerservice.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/tests/recordings/test_mgmt_containerservice.test_container.yaml
+Filename: azure-mgmt-containerservice-9.4.0/tests/recordings/test_mgmt_containerservice.test_container.yaml
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_resolve_private_link_service_id_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_configuration.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/version.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/version.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/version.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/__init__.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-containerservice-9.3.0/setup.py` & `azure-mgmt-containerservice-9.4.0/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/README.md` & `azure-mgmt-containerservice-9.4.0/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/PKG-INFO` & `azure-mgmt-containerservice-9.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerservice
-Version: 9.3.0
+Version: 9.4.0
 Summary: Microsoft Azure Container Service Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -27,14 +27,37 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerservice%2FREADME.png)
         
         
         # Release History
         
+        ## 9.4.0 (2020-09-11)
+        
+        **Features**
+        
+          - Model ManagedClusterAgentPoolProfile has a new parameter power_state
+          - Model ManagedClusterAgentPoolProfile has a new parameter os_disk_type
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_empty_bulk_delete
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_local_storage
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_total_unready_percentage
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter ok_total_unready_count
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter expander
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_system_pods
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter new_pod_scale_up_delay
+          - Model AgentPool has a new parameter power_state
+          - Model AgentPool has a new parameter os_disk_type
+          - Model ManagedClusterAgentPoolProfileProperties has a new parameter power_state
+          - Model ManagedClusterAgentPoolProfileProperties has a new parameter os_disk_type
+          - Model ManagedCluster has a new parameter power_state
+          - Added operation ManagedClustersOperations.start
+          - Added operation ManagedClustersOperations.stop
+          - Added operation group ResolvePrivateLinkServiceIdOperations
+          - Added operation group PrivateLinkResourcesOperations
+        
         ## 9.3.0 (2020-08-24)
         
         **Features**
         
           - Model ManagedClusterWindowsProfile has a new parameter license_type
           - Added operation ManagedClustersOperations.upgrade_node_image_version
```

## Comparing `azure-mgmt-containerservice-9.3.0/CHANGELOG.md` & `azure-mgmt-containerservice-9.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Release History
 
+## 9.4.0 (2020-09-11)
+
+**Features**
+
+  - Model ManagedClusterAgentPoolProfile has a new parameter power_state
+  - Model ManagedClusterAgentPoolProfile has a new parameter os_disk_type
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_empty_bulk_delete
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_local_storage
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_total_unready_percentage
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter ok_total_unready_count
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter expander
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_system_pods
+  - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter new_pod_scale_up_delay
+  - Model AgentPool has a new parameter power_state
+  - Model AgentPool has a new parameter os_disk_type
+  - Model ManagedClusterAgentPoolProfileProperties has a new parameter power_state
+  - Model ManagedClusterAgentPoolProfileProperties has a new parameter os_disk_type
+  - Model ManagedCluster has a new parameter power_state
+  - Added operation ManagedClustersOperations.start
+  - Added operation ManagedClustersOperations.stop
+  - Added operation group ResolvePrivateLinkServiceIdOperations
+  - Added operation group PrivateLinkResourcesOperations
+
 ## 9.3.0 (2020-08-24)
 
 **Features**
 
   - Model ManagedClusterWindowsProfile has a new parameter license_type
   - Added operation ManagedClustersOperations.upgrade_node_image_version
```

## Comparing `azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/SOURCES.txt` & `azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,30 @@
 azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py
 azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py
 azure/mgmt/containerservice/v2020_07_01/operations/__init__.py
 azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py
 azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py
 azure/mgmt/containerservice/v2020_07_01/operations/_operations.py
 azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py
+azure/mgmt/containerservice/v2020_09_01/__init__.py
+azure/mgmt/containerservice/v2020_09_01/_configuration.py
+azure/mgmt/containerservice/v2020_09_01/_container_service_client.py
+azure/mgmt/containerservice/v2020_09_01/version.py
+azure/mgmt/containerservice/v2020_09_01/models/__init__.py
+azure/mgmt/containerservice/v2020_09_01/models/_container_service_client_enums.py
+azure/mgmt/containerservice/v2020_09_01/models/_models.py
+azure/mgmt/containerservice/v2020_09_01/models/_models_py3.py
+azure/mgmt/containerservice/v2020_09_01/models/_paged_models.py
+azure/mgmt/containerservice/v2020_09_01/operations/__init__.py
+azure/mgmt/containerservice/v2020_09_01/operations/_agent_pools_operations.py
+azure/mgmt/containerservice/v2020_09_01/operations/_managed_clusters_operations.py
+azure/mgmt/containerservice/v2020_09_01/operations/_operations.py
+azure/mgmt/containerservice/v2020_09_01/operations/_private_endpoint_connections_operations.py
+azure/mgmt/containerservice/v2020_09_01/operations/_private_link_resources_operations.py
+azure/mgmt/containerservice/v2020_09_01/operations/_resolve_private_link_service_id_operations.py
 azure_mgmt_containerservice.egg-info/PKG-INFO
 azure_mgmt_containerservice.egg-info/SOURCES.txt
 azure_mgmt_containerservice.egg-info/dependency_links.txt
 azure_mgmt_containerservice.egg-info/not-zip-safe
 azure_mgmt_containerservice.egg-info/requires.txt
 azure_mgmt_containerservice.egg-info/top_level.txt
 tests/test_mgmt_containerservice.py
```

## Comparing `azure-mgmt-containerservice-9.3.0/azure_mgmt_containerservice.egg-info/PKG-INFO` & `azure-mgmt-containerservice-9.4.0/azure_mgmt_containerservice.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-containerservice
-Version: 9.3.0
+Version: 9.4.0
 Summary: Microsoft Azure Container Service Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -27,14 +27,37 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-containerservice%2FREADME.png)
         
         
         # Release History
         
+        ## 9.4.0 (2020-09-11)
+        
+        **Features**
+        
+          - Model ManagedClusterAgentPoolProfile has a new parameter power_state
+          - Model ManagedClusterAgentPoolProfile has a new parameter os_disk_type
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_empty_bulk_delete
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_local_storage
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter max_total_unready_percentage
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter ok_total_unready_count
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter expander
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter skip_nodes_with_system_pods
+          - Model ManagedClusterPropertiesAutoScalerProfile has a new parameter new_pod_scale_up_delay
+          - Model AgentPool has a new parameter power_state
+          - Model AgentPool has a new parameter os_disk_type
+          - Model ManagedClusterAgentPoolProfileProperties has a new parameter power_state
+          - Model ManagedClusterAgentPoolProfileProperties has a new parameter os_disk_type
+          - Model ManagedCluster has a new parameter power_state
+          - Added operation ManagedClustersOperations.start
+          - Added operation ManagedClustersOperations.stop
+          - Added operation group ResolvePrivateLinkServiceIdOperations
+          - Added operation group PrivateLinkResourcesOperations
+        
         ## 9.3.0 (2020-08-24)
         
         **Features**
         
           - Model ManagedClusterWindowsProfile has a new parameter license_type
           - Added operation ManagedClustersOperations.upgrade_node_image_version
```

## Comparing `azure-mgmt-containerservice-9.3.0/tests/test_mgmt_containerservice.py` & `azure-mgmt-containerservice-9.4.0/tests/test_mgmt_containerservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             {
                 "address_prefix": "10.0.0.0/8"
             }
         ).result()
 
         return subnet.id
 
-    @ResourceGroupPreparer(location='westus')
+    @ResourceGroupPreparer(location='eastus')
     def test_container(self, resource_group, location):
         container_name = self.get_resource_name('pycontainer')
 
         if self.is_live:
             subnet_id = self.create_subet(resource_group.name, location)
         else:
             subnet_id = "<fake_id>"
@@ -67,15 +67,15 @@
             {
                 'location': location,
                 "orchestrator_profile": {
                     "orchestrator_type": "Swarm"
                 },
                 "master_profile": {
                     "count": 1,
-                    "dns_prefix": "MasterPrefixTest",
+                    "dns_prefix": "masterPrefixTest",
                     "vm_size": ContainerServiceVMSizeTypes.standard_d2_v2,
                     "vnet_subnet_id": subnet_id
                 },
                 "agent_pool_profiles": [{
                     "name": "agentpool0",
                     "count": 3,
                     "vm_size": "Standard_A2_v2",
```

## Comparing `azure-mgmt-containerservice-9.3.0/tests/recordings/test_mgmt_containerservice.test_container.yaml` & `azure-mgmt-containerservice-9.4.0/tests/recordings/test_mgmt_containerservice.test_container.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 interactions:
 - request:
-    body: '{"location": "westus", "properties": {"addressSpace": {"addressPrefixes":
+    body: '{"location": "eastus", "properties": {"addressSpace": {"addressPrefixes":
       ["10.0.0.0/8"]}}}'
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '91'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet?api-version=2019-09-01
   response:
     body:
-      string: "{\r\n  \"name\": \"vnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet\",\r\n
-        \ \"etag\": \"W/\\\"b182a2ff-c82c-47b5-9e49-23b7b361c1c5\\\"\",\r\n  \"type\":
-        \"Microsoft.Network/virtualNetworks\",\r\n  \"location\": \"westus\",\r\n
-        \ \"properties\": {\r\n    \"provisioningState\": \"Updating\",\r\n    \"resourceGuid\":
-        \"6f9803dd-30bf-425f-a547-6b073353818b\",\r\n    \"addressSpace\": {\r\n      \"addressPrefixes\":
-        [\r\n        \"10.0.0.0/8\"\r\n      ]\r\n    },\r\n    \"subnets\": [],\r\n
-        \   \"virtualNetworkPeerings\": [],\r\n    \"enableDdosProtection\": false,\r\n
-        \   \"enableVmProtection\": false\r\n  }\r\n}"
+      string: "{\r\n  \"name\": \"vnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet\"\
+        ,\r\n  \"etag\": \"W/\\\"08fb0046-6700-430f-bcff-544e82497380\\\"\",\r\n \
+        \ \"type\": \"Microsoft.Network/virtualNetworks\",\r\n  \"location\": \"eastus\"\
+        ,\r\n  \"properties\": {\r\n    \"provisioningState\": \"Updating\",\r\n \
+        \   \"resourceGuid\": \"cb7d273d-fd31-4b3c-a058-e0347e8f747b\",\r\n    \"\
+        addressSpace\": {\r\n      \"addressPrefixes\": [\r\n        \"10.0.0.0/8\"\
+        \r\n      ]\r\n    },\r\n    \"subnets\": [],\r\n    \"virtualNetworkPeerings\"\
+        : [],\r\n    \"enableDdosProtection\": false,\r\n    \"enableVmProtection\"\
+        : false\r\n  }\r\n}"
     headers:
       azure-asyncnotification:
       - Enabled
       azure-asyncoperation:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/westus/operations/4fded8ac-d3d6-49d7-8ad0-f20ab5161933?api-version=2020-05-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/eastus/operations/4ec8f1fa-71a0-468e-8c4f-ed855f3a178a?api-version=2019-09-01
       cache-control:
       - no-cache
       content-length:
       - '668'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:37 GMT
+      - Fri, 11 Sep 2020 06:52:47 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - 20f5db2b-5c4d-43d3-8408-3a3f2cb3bdd6
+      - 3e1c7127-7ce3-4e3c-b1ac-35e745ffb086
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1199'
+      - '1198'
     status:
       code: 201
       message: Created
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/westus/operations/4fded8ac-d3d6-49d7-8ad0-f20ab5161933?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/eastus/operations/4ec8f1fa-71a0-468e-8c4f-ed855f3a178a?api-version=2019-09-01
   response:
     body:
       string: "{\r\n  \"status\": \"Succeeded\"\r\n}"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '29'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:41 GMT
+      - Fri, 11 Sep 2020 06:52:53 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
@@ -99,53 +100,54 @@
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - 6d283600-8fc4-439e-a694-f35b22885348
+      - 6a0d9dec-5937-4a56-8d28-51e2cdea5b60
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet?api-version=2019-09-01
   response:
     body:
-      string: "{\r\n  \"name\": \"vnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet\",\r\n
-        \ \"etag\": \"W/\\\"a536b13a-070e-4e15-ae02-78eac30c1e3a\\\"\",\r\n  \"type\":
-        \"Microsoft.Network/virtualNetworks\",\r\n  \"location\": \"westus\",\r\n
-        \ \"properties\": {\r\n    \"provisioningState\": \"Succeeded\",\r\n    \"resourceGuid\":
-        \"6f9803dd-30bf-425f-a547-6b073353818b\",\r\n    \"addressSpace\": {\r\n      \"addressPrefixes\":
-        [\r\n        \"10.0.0.0/8\"\r\n      ]\r\n    },\r\n    \"subnets\": [],\r\n
-        \   \"virtualNetworkPeerings\": [],\r\n    \"enableDdosProtection\": false,\r\n
-        \   \"enableVmProtection\": false\r\n  }\r\n}"
+      string: "{\r\n  \"name\": \"vnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet\"\
+        ,\r\n  \"etag\": \"W/\\\"3cb82604-d0c6-4e9c-8407-0f0c1a71e00b\\\"\",\r\n \
+        \ \"type\": \"Microsoft.Network/virtualNetworks\",\r\n  \"location\": \"eastus\"\
+        ,\r\n  \"properties\": {\r\n    \"provisioningState\": \"Succeeded\",\r\n\
+        \    \"resourceGuid\": \"cb7d273d-fd31-4b3c-a058-e0347e8f747b\",\r\n    \"\
+        addressSpace\": {\r\n      \"addressPrefixes\": [\r\n        \"10.0.0.0/8\"\
+        \r\n      ]\r\n    },\r\n    \"subnets\": [],\r\n    \"virtualNetworkPeerings\"\
+        : [],\r\n    \"enableDdosProtection\": false,\r\n    \"enableVmProtection\"\
+        : false\r\n  }\r\n}"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '669'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:42 GMT
+      - Fri, 11 Sep 2020 06:52:53 GMT
       etag:
-      - W/"a536b13a-070e-4e15-ae02-78eac30c1e3a"
+      - W/"3cb82604-d0c6-4e9c-8407-0f0c1a71e00b"
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
@@ -154,15 +156,15 @@
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - e1810f50-8da4-4bab-92ca-8300a91c7671
+      - c1a83b98-f815-4e2f-b279-de89f6cffc27
     status:
       code: 200
       message: OK
 - request:
     body: '{"properties": {"addressPrefix": "10.0.0.0/8"}}'
     headers:
       Accept:
@@ -172,83 +174,83 @@
       Connection:
       - keep-alive
       Content-Length:
       - '47'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet?api-version=2019-09-01
   response:
     body:
-      string: "{\r\n  \"name\": \"v-subnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\r\n
-        \ \"etag\": \"W/\\\"49b10a00-f828-4275-8a82-9749e2cdb4b9\\\"\",\r\n  \"properties\":
-        {\r\n    \"provisioningState\": \"Updating\",\r\n    \"addressPrefix\": \"10.0.0.0/8\",\r\n
-        \   \"delegations\": [],\r\n    \"privateEndpointNetworkPolicies\": \"Enabled\",\r\n
-        \   \"privateLinkServiceNetworkPolicies\": \"Enabled\"\r\n  },\r\n  \"type\":
-        \"Microsoft.Network/virtualNetworks/subnets\"\r\n}"
+      string: "{\r\n  \"name\": \"v-subnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\r\n  \"etag\": \"W/\\\"8a13e125-c9fe-46d3-87f3-4a653cb43512\\\"\",\r\n \
+        \ \"properties\": {\r\n    \"provisioningState\": \"Updating\",\r\n    \"\
+        addressPrefix\": \"10.0.0.0/8\",\r\n    \"delegations\": [],\r\n    \"privateEndpointNetworkPolicies\"\
+        : \"Enabled\",\r\n    \"privateLinkServiceNetworkPolicies\": \"Enabled\"\r\
+        \n  },\r\n  \"type\": \"Microsoft.Network/virtualNetworks/subnets\"\r\n}"
     headers:
       azure-asyncoperation:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/westus/operations/589fe1ee-05ae-4419-8790-c73fd92971e7?api-version=2020-05-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/eastus/operations/e8cd31ba-47cf-4513-bc15-4a73392e4154?api-version=2019-09-01
       cache-control:
       - no-cache
       content-length:
       - '559'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:42 GMT
+      - Fri, 11 Sep 2020 06:52:53 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - bc3ed497-4563-45b5-90fb-fb851aba4333
+      - d3ccc644-7af1-4387-8cd7-7b21b1a0cdb7
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1198'
+      - '1197'
     status:
       code: 201
       message: Created
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/westus/operations/589fe1ee-05ae-4419-8790-c73fd92971e7?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/locations/eastus/operations/e8cd31ba-47cf-4513-bc15-4a73392e4154?api-version=2019-09-01
   response:
     body:
       string: "{\r\n  \"status\": \"Succeeded\"\r\n}"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '29'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:46 GMT
+      - Fri, 11 Sep 2020 06:52:58 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
@@ -257,51 +259,51 @@
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - c7e98bc5-b4ed-4cbc-a22a-e3f1903d150a
+      - 342cbfcd-d7ac-4efd-a685-618a55c60f01
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-network/11.0.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-network/7.0.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet?api-version=2020-05-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet?api-version=2019-09-01
   response:
     body:
-      string: "{\r\n  \"name\": \"v-subnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\r\n
-        \ \"etag\": \"W/\\\"5cde8c53-b782-4bc8-816b-6261d3c4a969\\\"\",\r\n  \"properties\":
-        {\r\n    \"provisioningState\": \"Succeeded\",\r\n    \"addressPrefix\": \"10.0.0.0/8\",\r\n
-        \   \"delegations\": [],\r\n    \"privateEndpointNetworkPolicies\": \"Enabled\",\r\n
-        \   \"privateLinkServiceNetworkPolicies\": \"Enabled\"\r\n  },\r\n  \"type\":
-        \"Microsoft.Network/virtualNetworks/subnets\"\r\n}"
+      string: "{\r\n  \"name\": \"v-subnet\",\r\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\r\n  \"etag\": \"W/\\\"0014a236-b412-4f6e-b559-c2d5035cbbfe\\\"\",\r\n \
+        \ \"properties\": {\r\n    \"provisioningState\": \"Succeeded\",\r\n    \"\
+        addressPrefix\": \"10.0.0.0/8\",\r\n    \"delegations\": [],\r\n    \"privateEndpointNetworkPolicies\"\
+        : \"Enabled\",\r\n    \"privateLinkServiceNetworkPolicies\": \"Enabled\"\r\
+        \n  },\r\n  \"type\": \"Microsoft.Network/virtualNetworks/subnets\"\r\n}"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '560'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Wed, 19 Aug 2020 08:23:46 GMT
+      - Fri, 11 Sep 2020 06:52:59 GMT
       etag:
-      - W/"5cde8c53-b782-4bc8-816b-6261d3c4a969"
+      - W/"0014a236-b412-4f6e-b559-c2d5035cbbfe"
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       - Microsoft-HTTPAPI/2.0
@@ -310,21 +312,21 @@
       transfer-encoding:
       - chunked
       vary:
       - Accept-Encoding
       x-content-type-options:
       - nosniff
       x-ms-arm-service-request-id:
-      - 1c56fb5e-e99d-447f-ae78-f3f7309e6551
+      - 638dec49-042b-4865-b26d-fcf75e1d9954
     status:
       code: 200
       message: OK
 - request:
-    body: 'b''b\''{"location": "westus", "properties": {"orchestratorProfile": {"orchestratorType":
-      "Swarm"}, "masterProfile": {"count": 1, "dnsPrefix": "MasterPrefixTest", "vmSize":
+    body: 'b''b\''{"location": "eastus", "properties": {"orchestratorProfile": {"orchestratorType":
+      "Swarm"}, "masterProfile": {"count": 1, "dnsPrefix": "masterPrefixTest", "vmSize":
       "Standard_D2_v2", "vnetSubnetID": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet"},
       "agentPoolProfiles": [{"name": "agentpool0", "count": 3, "vmSize": "Standard_A2_v2",
       "vnetSubnetID": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet"}],
       "linuxProfile": {"adminUsername": "acslinuxadmin", "ssh": {"publicKeys": [{"keyData":
       "ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
       azureuser@linuxvm"}]}}}}\'''''
     headers:
@@ -335,178 +337,91 @@
       Connection:
       - keep-alive
       Content-Length:
       - '1167'
       Content-Type:
       - application/json; charset=utf-8
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: PUT
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \ \"location\": \"westus\",\n  \"name\": \"pycontainer665810f8\",\n  \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\": {\n   \"provisioningState\":
-        \"Creating\",\n   \"orchestratorProfile\": {\n    \"orchestratorType\": \"Swarm\"\n
-        \  },\n   \"masterProfile\": {\n    \"count\": 1,\n    \"dnsPrefix\": \"MasterPrefixTest\",\n
-        \   \"vmSize\": \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \   \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\":
-        \"ManagedDisks\"\n   },\n   \"agentPoolProfiles\": [\n    {\n     \"name\":
-        \"agentpool0\",\n     \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n
-        \    \"dnsPrefix\": \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\":
-        \"ManagedDisks\",\n     \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \    \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"adminUsername\":
-        \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\": [\n      {\n       \"keyData\":
-        \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
+      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n  \"location\": \"eastus\",\n  \"name\": \"pycontainer665810f8\",\n  \"\
+        type\": \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\"\
+        : {\n   \"provisioningState\": \"Creating\",\n   \"orchestratorProfile\":\
+        \ {\n    \"orchestratorType\": \"Swarm\"\n   },\n   \"masterProfile\": {\n\
+        \    \"count\": 1,\n    \"dnsPrefix\": \"masterPrefixTest\",\n    \"vmSize\"\
+        : \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n    \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\"\
+        : \"ManagedDisks\"\n   },\n   \"agentPoolProfiles\": [\n    {\n     \"name\"\
+        : \"agentpool0\",\n     \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\"\
+        ,\n     \"dnsPrefix\": \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\"\
+        : \"ManagedDisks\",\n     \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n     \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"\
+        adminUsername\": \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\":\
+        \ [\n      {\n       \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
     headers:
       azure-asyncoperation:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
       cache-control:
       - no-cache
       content-length:
       - '1825'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:24:01 GMT
+      - Fri, 11 Sep 2020 06:53:10 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1199'
+      - '1196'
     status:
       code: 201
       message: Created
 - request:
     body: null
     headers:
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
-    method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
-  response:
-    body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
-    headers:
-      cache-control:
-      - no-cache
-      content-length:
-      - '125'
-      content-type:
-      - application/json
-      date:
-      - Wed, 19 Aug 2020 08:24:32 GMT
-      expires:
-      - '-1'
-      pragma:
-      - no-cache
-      server:
-      - nginx
-      strict-transport-security:
-      - max-age=31536000; includeSubDomains
-      transfer-encoding:
-      - chunked
-      vary:
-      - Accept-Encoding
-      x-content-type-options:
-      - nosniff
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - application/json
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
-    method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
-  response:
-    body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
-    headers:
-      cache-control:
-      - no-cache
-      content-length:
-      - '125'
-      content-type:
-      - application/json
-      date:
-      - Wed, 19 Aug 2020 08:25:02 GMT
-      expires:
-      - '-1'
-      pragma:
-      - no-cache
-      server:
-      - nginx
-      strict-transport-security:
-      - max-age=31536000; includeSubDomains
-      transfer-encoding:
-      - chunked
-      vary:
-      - Accept-Encoding
-      x-content-type-options:
-      - nosniff
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - application/json
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
+      string: "{\n  \"name\": \"71a486c8-5323-c449-b1c1-fa54de691405\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:53:09.6469992Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '125'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:25:32 GMT
+      - Fri, 11 Sep 2020 06:53:42 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -526,31 +441,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
+      string: "{\n  \"name\": \"71a486c8-5323-c449-b1c1-fa54de691405\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:53:09.6469992Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '125'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:26:03 GMT
+      - Fri, 11 Sep 2020 06:54:12 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -570,31 +485,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
+      string: "{\n  \"name\": \"71a486c8-5323-c449-b1c1-fa54de691405\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:53:09.6469992Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '125'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:26:34 GMT
+      - Fri, 11 Sep 2020 06:54:43 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -614,31 +529,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\"\n }"
+      string: "{\n  \"name\": \"71a486c8-5323-c449-b1c1-fa54de691405\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:53:09.6469992Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '125'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:04 GMT
+      - Fri, 11 Sep 2020 06:55:13 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -658,32 +573,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/542ea61f-c918-4de6-b18b-f736918f601b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/c886a471-2353-49c4-b1c1-fa54de691405?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"1fa62e54-18c9-e64d-b18b-f736918f601b\",\n  \"status\":
-        \"Succeeded\",\n  \"startTime\": \"2020-08-19T08:24:00.040365Z\",\n  \"endTime\":
-        \"2020-08-19T08:27:08.9557789Z\"\n }"
+      string: "{\n  \"name\": \"71a486c8-5323-c449-b1c1-fa54de691405\",\n  \"status\"\
+        : \"Succeeded\",\n  \"startTime\": \"2020-09-11T06:53:09.6469992Z\",\n  \"\
+        endTime\": \"2020-09-11T06:55:14.2030196Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '169'
+      - '170'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:34 GMT
+      - Fri, 11 Sep 2020 06:55:43 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -703,45 +618,46 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \ \"location\": \"westus\",\n  \"name\": \"pycontainer665810f8\",\n  \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\": {\n   \"provisioningState\":
-        \"Succeeded\",\n   \"orchestratorProfile\": {\n    \"orchestratorType\": \"Swarm\"\n
-        \  },\n   \"masterProfile\": {\n    \"count\": 1,\n    \"dnsPrefix\": \"MasterPrefixTest\",\n
-        \   \"vmSize\": \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \   \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\":
-        \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.westus.cloudapp.azure.com\"\n
-        \  },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\",\n
-        \    \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\":
-        \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n
-        \    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \    \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"adminUsername\":
-        \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\": [\n      {\n       \"keyData\":
-        \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
+      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n  \"location\": \"eastus\",\n  \"name\": \"pycontainer665810f8\",\n  \"\
+        type\": \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\"\
+        : {\n   \"provisioningState\": \"Succeeded\",\n   \"orchestratorProfile\"\
+        : {\n    \"orchestratorType\": \"Swarm\"\n   },\n   \"masterProfile\": {\n\
+        \    \"count\": 1,\n    \"dnsPrefix\": \"masterPrefixTest\",\n    \"vmSize\"\
+        : \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n    \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\"\
+        : \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.eastus.cloudapp.azure.com\"\
+        \n   },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\"\
+        ,\n     \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\"\
+        : \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n\
+        \     \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n     \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"\
+        adminUsername\": \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\":\
+        \ [\n      {\n       \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1884'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:35 GMT
+      - Fri, 11 Sep 2020 06:55:44 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -761,47 +677,48 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \ \"location\": \"westus\",\n  \"name\": \"pycontainer665810f8\",\n  \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\": {\n   \"provisioningState\":
-        \"Succeeded\",\n   \"orchestratorProfile\": {\n    \"orchestratorType\": \"Swarm\"\n
-        \  },\n   \"masterProfile\": {\n    \"count\": 1,\n    \"dnsPrefix\": \"MasterPrefixTest\",\n
-        \   \"vmSize\": \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \   \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\":
-        \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.westus.cloudapp.azure.com\"\n
-        \  },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\",\n
-        \    \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\":
-        \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n
-        \    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \    \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"adminUsername\":
-        \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\": [\n      {\n       \"keyData\":
-        \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
+      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n  \"location\": \"eastus\",\n  \"name\": \"pycontainer665810f8\",\n  \"\
+        type\": \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\"\
+        : {\n   \"provisioningState\": \"Succeeded\",\n   \"orchestratorProfile\"\
+        : {\n    \"orchestratorType\": \"Swarm\"\n   },\n   \"masterProfile\": {\n\
+        \    \"count\": 1,\n    \"dnsPrefix\": \"masterPrefixTest\",\n    \"vmSize\"\
+        : \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n    \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\"\
+        : \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.eastus.cloudapp.azure.com\"\
+        \n   },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\"\
+        ,\n     \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\"\
+        : \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n\
+        \     \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n     \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"\
+        adminUsername\": \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\":\
+        \ [\n      {\n       \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1884'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:36 GMT
+      - Fri, 11 Sep 2020 06:55:46 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -821,49 +738,49 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"value\": [\n   {\n    \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \   \"location\": \"westus\",\n    \"name\": \"pycontainer665810f8\",\n    \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n    \"properties\": {\n
-        \    \"provisioningState\": \"Succeeded\",\n     \"orchestratorProfile\":
-        {\n      \"orchestratorType\": \"Swarm\"\n     },\n     \"masterProfile\":
-        {\n      \"count\": 1,\n      \"dnsPrefix\": \"MasterPrefixTest\",\n      \"vmSize\":
-        \"Standard_D2_v2\",\n      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \     \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n      \"storageProfile\":
-        \"ManagedDisks\",\n      \"fqdn\": \"masterprefixtest.westus.cloudapp.azure.com\"\n
-        \    },\n     \"agentPoolProfiles\": [\n      {\n       \"name\": \"agentpool0\",\n
-        \      \"count\": 3,\n       \"vmSize\": \"Standard_A2_v2\",\n       \"dnsPrefix\":
-        \"\",\n       \"fqdn\": \"\",\n       \"storageProfile\": \"ManagedDisks\",\n
-        \      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \      \"osType\": \"Linux\"\n      }\n     ],\n     \"linuxProfile\": {\n
-        \     \"adminUsername\": \"acslinuxadmin\",\n      \"ssh\": {\n       \"publicKeys\":
-        [\n        {\n         \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n        }\n       ]\n      }\n     }\n    }\n   }\n  ]\n
-        }"
+      string: "{\n  \"value\": [\n   {\n    \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n    \"location\": \"eastus\",\n    \"name\": \"pycontainer665810f8\",\n\
+        \    \"type\": \"Microsoft.ContainerService/ContainerServices\",\n    \"properties\"\
+        : {\n     \"provisioningState\": \"Succeeded\",\n     \"orchestratorProfile\"\
+        : {\n      \"orchestratorType\": \"Swarm\"\n     },\n     \"masterProfile\"\
+        : {\n      \"count\": 1,\n      \"dnsPrefix\": \"masterPrefixTest\",\n   \
+        \   \"vmSize\": \"Standard_D2_v2\",\n      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n      \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n      \"storageProfile\"\
+        : \"ManagedDisks\",\n      \"fqdn\": \"masterprefixtest.eastus.cloudapp.azure.com\"\
+        \n     },\n     \"agentPoolProfiles\": [\n      {\n       \"name\": \"agentpool0\"\
+        ,\n       \"count\": 3,\n       \"vmSize\": \"Standard_A2_v2\",\n       \"\
+        dnsPrefix\": \"\",\n       \"fqdn\": \"\",\n       \"storageProfile\": \"\
+        ManagedDisks\",\n       \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n       \"osType\": \"Linux\"\n      }\n     ],\n     \"linuxProfile\":\
+        \ {\n      \"adminUsername\": \"acslinuxadmin\",\n      \"ssh\": {\n     \
+        \  \"publicKeys\": [\n        {\n         \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n        }\n       ]\n      }\n     }\n    }\n   }\n\
+        \  ]\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1993'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:37 GMT
+      - Fri, 11 Sep 2020 06:55:46 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -883,49 +800,49 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: GET
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/containerServices?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"value\": [\n   {\n    \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \   \"location\": \"westus\",\n    \"name\": \"pycontainer665810f8\",\n    \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n    \"properties\": {\n
-        \    \"provisioningState\": \"Succeeded\",\n     \"orchestratorProfile\":
-        {\n      \"orchestratorType\": \"Swarm\"\n     },\n     \"masterProfile\":
-        {\n      \"count\": 1,\n      \"dnsPrefix\": \"MasterPrefixTest\",\n      \"vmSize\":
-        \"Standard_D2_v2\",\n      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \     \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n      \"storageProfile\":
-        \"ManagedDisks\",\n      \"fqdn\": \"masterprefixtest.westus.cloudapp.azure.com\"\n
-        \    },\n     \"agentPoolProfiles\": [\n      {\n       \"name\": \"agentpool0\",\n
-        \      \"count\": 3,\n       \"vmSize\": \"Standard_A2_v2\",\n       \"dnsPrefix\":
-        \"\",\n       \"fqdn\": \"\",\n       \"storageProfile\": \"ManagedDisks\",\n
-        \      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \      \"osType\": \"Linux\"\n      }\n     ],\n     \"linuxProfile\": {\n
-        \     \"adminUsername\": \"acslinuxadmin\",\n      \"ssh\": {\n       \"publicKeys\":
-        [\n        {\n         \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n        }\n       ]\n      }\n     }\n    }\n   }\n  ]\n
-        }"
+      string: "{\n  \"value\": [\n   {\n    \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n    \"location\": \"eastus\",\n    \"name\": \"pycontainer665810f8\",\n\
+        \    \"type\": \"Microsoft.ContainerService/ContainerServices\",\n    \"properties\"\
+        : {\n     \"provisioningState\": \"Succeeded\",\n     \"orchestratorProfile\"\
+        : {\n      \"orchestratorType\": \"Swarm\"\n     },\n     \"masterProfile\"\
+        : {\n      \"count\": 1,\n      \"dnsPrefix\": \"masterPrefixTest\",\n   \
+        \   \"vmSize\": \"Standard_D2_v2\",\n      \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n      \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n      \"storageProfile\"\
+        : \"ManagedDisks\",\n      \"fqdn\": \"masterprefixtest.eastus.cloudapp.azure.com\"\
+        \n     },\n     \"agentPoolProfiles\": [\n      {\n       \"name\": \"agentpool0\"\
+        ,\n       \"count\": 3,\n       \"vmSize\": \"Standard_A2_v2\",\n       \"\
+        dnsPrefix\": \"\",\n       \"fqdn\": \"\",\n       \"storageProfile\": \"\
+        ManagedDisks\",\n       \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n       \"osType\": \"Linux\"\n      }\n     ],\n     \"linuxProfile\":\
+        \ {\n      \"adminUsername\": \"acslinuxadmin\",\n      \"ssh\": {\n     \
+        \  \"publicKeys\": [\n        {\n         \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n        }\n       ]\n      }\n     }\n    }\n   }\n\
+        \  ]\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
       - '1993'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:37 GMT
+      - Fri, 11 Sep 2020 06:55:47 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -947,53 +864,54 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
       accept-language:
       - en-US
     method: DELETE
     uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8?api-version=2017-07-01
   response:
     body:
-      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\",\n
-        \ \"location\": \"westus\",\n  \"name\": \"pycontainer665810f8\",\n  \"type\":
-        \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\": {\n   \"provisioningState\":
-        \"Deleting\",\n   \"orchestratorProfile\": {\n    \"orchestratorType\": \"Swarm\"\n
-        \  },\n   \"masterProfile\": {\n    \"count\": 1,\n    \"dnsPrefix\": \"MasterPrefixTest\",\n
-        \   \"vmSize\": \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \   \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\":
-        \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.westus.cloudapp.azure.com\"\n
-        \  },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\",\n
-        \    \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\":
-        \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n
-        \    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\",\n
-        \    \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"adminUsername\":
-        \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\": [\n      {\n       \"keyData\":
-        \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==
-        azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
+      string: "{\n  \"id\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.ContainerService/containerServices/pycontainer665810f8\"\
+        ,\n  \"location\": \"eastus\",\n  \"name\": \"pycontainer665810f8\",\n  \"\
+        type\": \"Microsoft.ContainerService/ContainerServices\",\n  \"properties\"\
+        : {\n   \"provisioningState\": \"Deleting\",\n   \"orchestratorProfile\":\
+        \ {\n    \"orchestratorType\": \"Swarm\"\n   },\n   \"masterProfile\": {\n\
+        \    \"count\": 1,\n    \"dnsPrefix\": \"masterPrefixTest\",\n    \"vmSize\"\
+        : \"Standard_D2_v2\",\n    \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n    \"firstConsecutiveStaticIP\": \"10.240.255.5\",\n    \"storageProfile\"\
+        : \"ManagedDisks\",\n    \"fqdn\": \"masterprefixtest.eastus.cloudapp.azure.com\"\
+        \n   },\n   \"agentPoolProfiles\": [\n    {\n     \"name\": \"agentpool0\"\
+        ,\n     \"count\": 3,\n     \"vmSize\": \"Standard_A2_v2\",\n     \"dnsPrefix\"\
+        : \"\",\n     \"fqdn\": \"\",\n     \"storageProfile\": \"ManagedDisks\",\n\
+        \     \"vnetSubnetID\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_mgmt_containerservice_test_container665810f8/providers/Microsoft.Network/virtualNetworks/vnet/subnets/v-subnet\"\
+        ,\n     \"osType\": \"Linux\"\n    }\n   ],\n   \"linuxProfile\": {\n    \"\
+        adminUsername\": \"acslinuxadmin\",\n    \"ssh\": {\n     \"publicKeys\":\
+        \ [\n      {\n       \"keyData\": \"ssh-rsa AAAAB3NzaC1yc2EAAAABJQAAAQEAlj9UC6+57XWVu0fd6zqXa256EU9EZdoLGE3TqdZqu9fvUvLQOX2G0d5DmFhDCyTmWLQUx3/ONQ9RotYmHGymBIPQcpx43nnxsuihAILcpGZ5NjCj4IOYnmhdULxN4ti7k00S+udqokrRYpmwt0N4NA4VT9cN+7uJDL8Opqa1FYu0CT/RqSW+3aoQ0nfGj11axoxM37FuOMZ/c7mBSxvuI9NsDmcDQOUmPXjlgNlxrLzf6VcjxnJh4AO83zbyLok37mW/C7CuNK4WowjPO1Ix2kqRHRxBrzxYZ9xqZPc8GpFTw/dxJEYdJ3xlitbOoBoDgrL5gSITv6ESlNqjPk6kHQ==\
+        \ azureuser@linuxvm\"\n      }\n     ]\n    }\n   }\n  }\n }"
     headers:
       azure-asyncoperation:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
       cache-control:
       - no-cache
       content-length:
       - '1883'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:27:39 GMT
+      - Fri, 11 Sep 2020 06:55:48 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operationresults/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operationresults/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
@@ -1009,119 +927,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
-    method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
-  response:
-    body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
-    headers:
-      cache-control:
-      - no-cache
-      content-length:
-      - '124'
-      content-type:
-      - application/json
-      date:
-      - Wed, 19 Aug 2020 08:28:11 GMT
-      expires:
-      - '-1'
-      pragma:
-      - no-cache
-      server:
-      - nginx
-      strict-transport-security:
-      - max-age=31536000; includeSubDomains
-      transfer-encoding:
-      - chunked
-      vary:
-      - Accept-Encoding
-      x-content-type-options:
-      - nosniff
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - application/json
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
-    method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
-  response:
-    body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
-    headers:
-      cache-control:
-      - no-cache
-      content-length:
-      - '124'
-      content-type:
-      - application/json
-      date:
-      - Wed, 19 Aug 2020 08:28:41 GMT
-      expires:
-      - '-1'
-      pragma:
-      - no-cache
-      server:
-      - nginx
-      strict-transport-security:
-      - max-age=31536000; includeSubDomains
-      transfer-encoding:
-      - chunked
-      vary:
-      - Accept-Encoding
-      x-content-type-options:
-      - nosniff
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - application/json
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:29:11 GMT
+      - Fri, 11 Sep 2020 06:56:18 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1141,31 +971,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:29:42 GMT
+      - Fri, 11 Sep 2020 06:56:49 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1185,31 +1015,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:30:12 GMT
+      - Fri, 11 Sep 2020 06:57:19 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1229,31 +1059,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:30:43 GMT
+      - Fri, 11 Sep 2020 06:57:50 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1273,31 +1103,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:31:14 GMT
+      - Fri, 11 Sep 2020 06:58:20 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1317,31 +1147,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:31:44 GMT
+      - Fri, 11 Sep 2020 06:58:50 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1361,31 +1191,31 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"InProgress\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"InProgress\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '124'
+      - '126'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:32:14 GMT
+      - Fri, 11 Sep 2020 06:59:20 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
@@ -1405,32 +1235,32 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python/3.8.2 (Windows-10-10.0.19041-SP0) msrest/0.6.17 msrest_azure/0.6.3
-        azure-mgmt-containerservice/9.2.0 Azure-SDK-For-Python
+      - python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic) msrest/0.6.10
+        msrest_azure/0.6.2 azure-mgmt-containerservice/9.4.0 Azure-SDK-For-Python
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/westus/operations/777c8d51-9bd0-4fc4-82f4-316c24bf465b?api-version=2016-03-30
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.ContainerService/locations/eastus/operations/d5e1637b-16cf-4b9c-86cc-3ca91a767b8a?api-version=2016-03-30
   response:
     body:
-      string: "{\n  \"name\": \"518d7c77-d09b-c44f-82f4-316c24bf465b\",\n  \"status\":
-        \"Succeeded\",\n  \"startTime\": \"2020-08-19T08:27:39.89089Z\",\n  \"endTime\":
-        \"2020-08-19T08:32:27.6567614Z\"\n }"
+      string: "{\n  \"name\": \"7b63e1d5-cf16-9c4b-86cc-3ca91a767b8a\",\n  \"status\"\
+        : \"Succeeded\",\n  \"startTime\": \"2020-09-11T06:55:47.9961378Z\",\n  \"\
+        endTime\": \"2020-09-11T06:59:37.2974788Z\"\n }"
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '168'
+      - '170'
       content-type:
       - application/json
       date:
-      - Wed, 19 Aug 2020 08:32:44 GMT
+      - Fri, 11 Sep 2020 06:59:51 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - nginx
       strict-transport-security:
```

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/_container_service_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     :param str api_version: API version to use if no profile is provided, or if
      missing in profile.
     :param str base_url: Service URL
     :param profile: A profile definition, from KnownProfiles to dict.
     :type profile: azure.profiles.KnownProfiles
     """
 
-    DEFAULT_API_VERSION = '2020-07-01'
+    DEFAULT_API_VERSION = '2020-09-01'
     _PROFILE_TAG = "azure.mgmt.containerservice.ContainerServiceClient"
     LATEST_PROFILE = ProfileDefinition({
         _PROFILE_TAG: {
             None: DEFAULT_API_VERSION,
             'container_services': '2017-07-01',
             'open_shift_managed_clusters': '2019-04-30',
         }},
@@ -89,14 +89,15 @@
            * 2019-11-01: :mod:`v2019_11_01.models<azure.mgmt.containerservice.v2019_11_01.models>`
            * 2020-01-01: :mod:`v2020_01_01.models<azure.mgmt.containerservice.v2020_01_01.models>`
            * 2020-02-01: :mod:`v2020_02_01.models<azure.mgmt.containerservice.v2020_02_01.models>`
            * 2020-03-01: :mod:`v2020_03_01.models<azure.mgmt.containerservice.v2020_03_01.models>`
            * 2020-04-01: :mod:`v2020_04_01.models<azure.mgmt.containerservice.v2020_04_01.models>`
            * 2020-06-01: :mod:`v2020_06_01.models<azure.mgmt.containerservice.v2020_06_01.models>`
            * 2020-07-01: :mod:`v2020_07_01.models<azure.mgmt.containerservice.v2020_07_01.models>`
+           * 2020-09-01: :mod:`v2020_09_01.models<azure.mgmt.containerservice.v2020_09_01.models>`
         """
         if api_version == '2017-07-01':
             from .v2017_07_01 import models
             return models
         elif api_version == '2018-03-31':
             from .v2018_03_31 import models
             return models
@@ -147,14 +148,17 @@
             return models
         elif api_version == '2020-06-01':
             from .v2020_06_01 import models
             return models
         elif api_version == '2020-07-01':
             from .v2020_07_01 import models
             return models
+        elif api_version == '2020-09-01':
+            from .v2020_09_01 import models
+            return models
         raise NotImplementedError("APIVersion {} is not available".format(api_version))
 
     @property
     def agent_pools(self):
         """Instance depends on the API version:
 
            * 2019-02-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2019_02_01.operations.AgentPoolsOperations>`
@@ -165,14 +169,15 @@
            * 2019-11-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2019_11_01.operations.AgentPoolsOperations>`
            * 2020-01-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_01_01.operations.AgentPoolsOperations>`
            * 2020-02-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_02_01.operations.AgentPoolsOperations>`
            * 2020-03-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_03_01.operations.AgentPoolsOperations>`
            * 2020-04-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_04_01.operations.AgentPoolsOperations>`
            * 2020-06-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_06_01.operations.AgentPoolsOperations>`
            * 2020-07-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_07_01.operations.AgentPoolsOperations>`
+           * 2020-09-01: :class:`AgentPoolsOperations<azure.mgmt.containerservice.v2020_09_01.operations.AgentPoolsOperations>`
         """
         api_version = self._get_api_version('agent_pools')
         if api_version == '2019-02-01':
             from .v2019_02_01.operations import AgentPoolsOperations as OperationClass
         elif api_version == '2019-04-01':
             from .v2019_04_01.operations import AgentPoolsOperations as OperationClass
         elif api_version == '2019-06-01':
@@ -191,14 +196,16 @@
             from .v2020_03_01.operations import AgentPoolsOperations as OperationClass
         elif api_version == '2020-04-01':
             from .v2020_04_01.operations import AgentPoolsOperations as OperationClass
         elif api_version == '2020-06-01':
             from .v2020_06_01.operations import AgentPoolsOperations as OperationClass
         elif api_version == '2020-07-01':
             from .v2020_07_01.operations import AgentPoolsOperations as OperationClass
+        elif api_version == '2020-09-01':
+            from .v2020_09_01.operations import AgentPoolsOperations as OperationClass
         else:
             raise NotImplementedError("APIVersion {} is not available".format(api_version))
         return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def container_services(self):
         """Instance depends on the API version:
@@ -226,14 +233,15 @@
            * 2019-11-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2019_11_01.operations.ManagedClustersOperations>`
            * 2020-01-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_01_01.operations.ManagedClustersOperations>`
            * 2020-02-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_02_01.operations.ManagedClustersOperations>`
            * 2020-03-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_03_01.operations.ManagedClustersOperations>`
            * 2020-04-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_04_01.operations.ManagedClustersOperations>`
            * 2020-06-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_06_01.operations.ManagedClustersOperations>`
            * 2020-07-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_07_01.operations.ManagedClustersOperations>`
+           * 2020-09-01: :class:`ManagedClustersOperations<azure.mgmt.containerservice.v2020_09_01.operations.ManagedClustersOperations>`
         """
         api_version = self._get_api_version('managed_clusters')
         if api_version == '2018-03-31':
             from .v2018_03_31.operations import ManagedClustersOperations as OperationClass
         elif api_version == '2018-08-01-preview':
             from .v2018_08_01_preview.operations import ManagedClustersOperations as OperationClass
         elif api_version == '2019-02-01':
@@ -256,14 +264,16 @@
             from .v2020_03_01.operations import ManagedClustersOperations as OperationClass
         elif api_version == '2020-04-01':
             from .v2020_04_01.operations import ManagedClustersOperations as OperationClass
         elif api_version == '2020-06-01':
             from .v2020_06_01.operations import ManagedClustersOperations as OperationClass
         elif api_version == '2020-07-01':
             from .v2020_07_01.operations import ManagedClustersOperations as OperationClass
+        elif api_version == '2020-09-01':
+            from .v2020_09_01.operations import ManagedClustersOperations as OperationClass
         else:
             raise NotImplementedError("APIVersion {} is not available".format(api_version))
         return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def open_shift_managed_clusters(self):
         """Instance depends on the API version:
@@ -300,14 +310,15 @@
            * 2019-11-01: :class:`Operations<azure.mgmt.containerservice.v2019_11_01.operations.Operations>`
            * 2020-01-01: :class:`Operations<azure.mgmt.containerservice.v2020_01_01.operations.Operations>`
            * 2020-02-01: :class:`Operations<azure.mgmt.containerservice.v2020_02_01.operations.Operations>`
            * 2020-03-01: :class:`Operations<azure.mgmt.containerservice.v2020_03_01.operations.Operations>`
            * 2020-04-01: :class:`Operations<azure.mgmt.containerservice.v2020_04_01.operations.Operations>`
            * 2020-06-01: :class:`Operations<azure.mgmt.containerservice.v2020_06_01.operations.Operations>`
            * 2020-07-01: :class:`Operations<azure.mgmt.containerservice.v2020_07_01.operations.Operations>`
+           * 2020-09-01: :class:`Operations<azure.mgmt.containerservice.v2020_09_01.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2018-03-31':
             from .v2018_03_31.operations import Operations as OperationClass
         elif api_version == '2018-08-01-preview':
             from .v2018_08_01_preview.operations import Operations as OperationClass
         elif api_version == '2019-02-01':
@@ -330,26 +341,57 @@
             from .v2020_03_01.operations import Operations as OperationClass
         elif api_version == '2020-04-01':
             from .v2020_04_01.operations import Operations as OperationClass
         elif api_version == '2020-06-01':
             from .v2020_06_01.operations import Operations as OperationClass
         elif api_version == '2020-07-01':
             from .v2020_07_01.operations import Operations as OperationClass
+        elif api_version == '2020-09-01':
+            from .v2020_09_01.operations import Operations as OperationClass
         else:
             raise NotImplementedError("APIVersion {} is not available".format(api_version))
         return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def private_endpoint_connections(self):
         """Instance depends on the API version:
 
            * 2020-06-01: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.containerservice.v2020_06_01.operations.PrivateEndpointConnectionsOperations>`
            * 2020-07-01: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.containerservice.v2020_07_01.operations.PrivateEndpointConnectionsOperations>`
+           * 2020-09-01: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.containerservice.v2020_09_01.operations.PrivateEndpointConnectionsOperations>`
         """
         api_version = self._get_api_version('private_endpoint_connections')
         if api_version == '2020-06-01':
             from .v2020_06_01.operations import PrivateEndpointConnectionsOperations as OperationClass
         elif api_version == '2020-07-01':
             from .v2020_07_01.operations import PrivateEndpointConnectionsOperations as OperationClass
+        elif api_version == '2020-09-01':
+            from .v2020_09_01.operations import PrivateEndpointConnectionsOperations as OperationClass
+        else:
+            raise NotImplementedError("APIVersion {} is not available".format(api_version))
+        return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
+
+    @property
+    def private_link_resources(self):
+        """Instance depends on the API version:
+
+           * 2020-09-01: :class:`PrivateLinkResourcesOperations<azure.mgmt.containerservice.v2020_09_01.operations.PrivateLinkResourcesOperations>`
+        """
+        api_version = self._get_api_version('private_link_resources')
+        if api_version == '2020-09-01':
+            from .v2020_09_01.operations import PrivateLinkResourcesOperations as OperationClass
+        else:
+            raise NotImplementedError("APIVersion {} is not available".format(api_version))
+        return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
+
+    @property
+    def resolve_private_link_service_id(self):
+        """Instance depends on the API version:
+
+           * 2020-09-01: :class:`ResolvePrivateLinkServiceIdOperations<azure.mgmt.containerservice.v2020_09_01.operations.ResolvePrivateLinkServiceIdOperations>`
+        """
+        api_version = self._get_api_version('resolve_private_link_service_id')
+        if api_version == '2020-09-01':
+            from .v2020_09_01.operations import ResolvePrivateLinkServiceIdOperations as OperationClass
         else:
             raise NotImplementedError("APIVersion {} is not available".format(api_version))
         return OperationClass(self._client, self.config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
```

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_03_31/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_09_30_preview/operations/_open_shift_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_10_27_preview/operations/_open_shift_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_09_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_08_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/operations/_open_shift_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_09_30_preview/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_03_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_04_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_11_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2018_08_01_preview/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/operations/_open_shift_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_04_30/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/_container_services_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2017_07_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_02_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_07_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_01_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2019_06_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_configuration.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_06_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/_container_service_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_container_service_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/_paged_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_managed_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-containerservice-9.3.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py` & `azure-mgmt-containerservice-9.4.0/azure/mgmt/containerservice/v2020_02_01/operations/_agent_pools_operations.py`

 * *Files identical despite different names*

