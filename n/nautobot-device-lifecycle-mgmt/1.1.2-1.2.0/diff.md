# Comparing `tmp/nautobot_device_lifecycle_mgmt-1.1.2.tar.gz` & `tmp/nautobot_device_lifecycle_mgmt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.1.2.tar", max compression
+gzip compressed data, was "nautobot_device_lifecycle_mgmt-1.2.0.tar", max compression
```

## Comparing `nautobot_device_lifecycle_mgmt-1.1.2.tar` & `nautobot_device_lifecycle_mgmt-1.2.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      591 2022-12-07 19:38:37.846341 nautobot_device_lifecycle_mgmt-1.1.2/LICENSE
--rw-r--r--   0        0        0     9140 2022-12-07 19:38:37.846341 nautobot_device_lifecycle_mgmt-1.1.2/README.md
--rw-r--r--   0        0        0     1418 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/__init__.py
--rw-r--r--   0        0        0      328 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/admin.py
--rw-r--r--   0        0        0       65 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/__init__.py
--rw-r--r--   0        0        0     2970 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
--rw-r--r--   0        0        0     9639 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/serializers.py
--rw-r--r--   0        0        0      926 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/urls.py
--rw-r--r--   0        0        0     3403 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/views.py
--rw-r--r--   0        0        0     2141 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/choices.py
--rw-r--r--   0        0        0     1188 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/const.py
--rw-r--r--   0        0        0    28481 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/filters.py
--rw-r--r--   0        0        0    39107 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/forms.py
--rw-r--r--   0        0        0      685 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/graphql/types.py
--rw-r--r--   0        0        0      327 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/jobs/__init__.py
--rw-r--r--   0        0        0     2909 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
--rw-r--r--   0        0        0     3060 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
--rw-r--r--   0        0        0     3449 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
--rw-r--r--   0        0        0     4319 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
--rw-r--r--   0        0        0     5580 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
--rw-r--r--   0        0        0     2378 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
--rw-r--r--   0        0        0     4405 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
--rw-r--r--   0        0        0     4794 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
--rw-r--r--   0        0        0     3131 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
--rw-r--r--   0        0        0     1123 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
--rw-r--r--   0        0        0      612 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
--rw-r--r--   0        0        0        0 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/__init__.py
--rw-r--r--   0        0        0    29682 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/models.py
--rw-r--r--   0        0        0    13356 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/navigation.py
--rw-r--r--   0        0        0     5407 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/signals.py
--rw-r--r--   0        0        0     2995 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/software.py
--rw-r--r--   0        0        0     8101 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/software_filters.py
--rw-r--r--   0        0        0    13830 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tables.py
--rw-r--r--   0        0        0     4326 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/template_content.py
--rw-r--r--   0        0        0     3761 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
--rw-r--r--   0        0        0     7902 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
--rw-r--r--   0        0        0     4090 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
--rw-r--r--   0        0        0     4362 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
--rw-r--r--   0        0        0      939 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
--rw-r--r--   0        0        0     1523 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
--rw-r--r--   0        0        0     5632 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
--rw-r--r--   0        0        0     2160 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
--rw-r--r--   0        0        0      513 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
--rw-r--r--   0        0        0     1113 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
--rw-r--r--   0        0        0      365 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
--rw-r--r--   0        0        0     5210 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
--rw-r--r--   0        0        0     7304 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
--rw-r--r--   0        0        0      263 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
--rw-r--r--   0        0        0     1917 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
--rw-r--r--   0        0        0       92 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
--rw-r--r--   0        0        0     5442 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
--rw-r--r--   0        0        0      251 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
--rw-r--r--   0        0        0       86 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
--rw-r--r--   0        0        0      392 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
--rw-r--r--   0        0        0     4234 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
--rw-r--r--   0        0        0     4313 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
--rw-r--r--   0        0        0     8623 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
--rw-r--r--   0        0        0      269 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
--rw-r--r--   0        0        0     1942 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
--rw-r--r--   0        0        0       96 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
--rw-r--r--   0        0        0     3257 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
--rw-r--r--   0        0        0      615 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
--rw-r--r--   0        0        0       67 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/__init__.py
--rw-r--r--   0        0        0     3705 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/conftest.py
--rw-r--r--   0        0        0    24710 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_api.py
--rw-r--r--   0        0        0    30041 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_filters.py
--rw-r--r--   0        0        0    23393 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_forms.py
--rw-r--r--   0        0        0    24237 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_model.py
--rw-r--r--   0        0        0    11840 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
--rw-r--r--   0        0        0    11406 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_views.py
--rw-r--r--   0        0        0     9524 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/urls.py
--rw-r--r--   0        0        0      423 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/utils.py
--rw-r--r--   0        0        0    40635 2022-12-07 19:38:37.862342 nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/views.py
--rw-r--r--   0        0        0     2471 2022-12-07 19:38:46.546438 nautobot_device_lifecycle_mgmt-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    10594 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.1.2/setup.py
--rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-04-21 15:38:36.765759 nautobot_device_lifecycle_mgmt-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4965 2023-04-21 15:38:36.765759 nautobot_device_lifecycle_mgmt-1.2.0/README.md
+-rw-r--r--   0        0        0     1418 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/admin.py
+-rw-r--r--   0        0        0       65 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/__init__.py
+-rw-r--r--   0        0        0     2970 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py
+-rw-r--r--   0        0        0     9639 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/serializers.py
+-rw-r--r--   0        0        0      926 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/urls.py
+-rw-r--r--   0        0        0     3403 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/views.py
+-rw-r--r--   0        0        0     2141 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/choices.py
+-rw-r--r--   0        0        0     1188 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/const.py
+-rw-r--r--   0        0        0    28481 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/filters.py
+-rw-r--r--   0        0        0    39107 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/forms.py
+-rw-r--r--   0        0        0      685 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/graphql/types.py
+-rw-r--r--   0        0        0      327 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/__init__.py
+-rw-r--r--   0        0        0     3191 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
+-rw-r--r--   0        0        0     3060 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
+-rw-r--r--   0        0        0     3449 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
+-rw-r--r--   0        0        0     4319 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
+-rw-r--r--   0        0        0     5580 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
+-rw-r--r--   0        0        0     2378 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
+-rw-r--r--   0        0        0     4405 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
+-rw-r--r--   0        0        0     4794 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
+-rw-r--r--   0        0        0     3131 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
+-rw-r--r--   0        0        0     1123 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
+-rw-r--r--   0        0        0      612 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/__init__.py
+-rw-r--r--   0        0        0    29626 2023-04-21 15:38:36.781759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/models.py
+-rw-r--r--   0        0        0    13356 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/navigation.py
+-rw-r--r--   0        0        0     5407 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/signals.py
+-rw-r--r--   0        0        0     2995 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software.py
+-rw-r--r--   0        0        0     8101 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software_filters.py
+-rw-r--r--   0        0        0    14122 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tables.py
+-rw-r--r--   0        0        0     4326 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/template_content.py
+-rw-r--r--   0        0        0     2094 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html
+-rw-r--r--   0        0        0     5904 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html
+-rw-r--r--   0        0        0     2429 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm.html
+-rw-r--r--   0        0        0     2613 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm.html
+-rw-r--r--   0        0        0      939 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
+-rw-r--r--   0        0        0     1523 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
+-rw-r--r--   0        0        0     5632 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
+-rw-r--r--   0        0        0     2160 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
+-rw-r--r--   0        0        0      513 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
+-rw-r--r--   0        0        0     1113 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
+-rw-r--r--   0        0        0      365 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
+-rw-r--r--   0        0        0     3447 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm.html
+-rw-r--r--   0        0        0     4705 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm.html
+-rw-r--r--   0        0        0      263 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
+-rw-r--r--   0        0        0     1917 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
+-rw-r--r--   0        0        0       92 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
+-rw-r--r--   0        0        0     3138 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html
+-rw-r--r--   0        0        0      251 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
+-rw-r--r--   0        0        0       86 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
+-rw-r--r--   0        0        0      392 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
+-rw-r--r--   0        0        0     4234 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
+-rw-r--r--   0        0        0     4313 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
+-rw-r--r--   0        0        0     5686 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html
+-rw-r--r--   0        0        0      269 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
+-rw-r--r--   0        0        0     1942 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
+-rw-r--r--   0        0        0       96 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
+-rw-r--r--   0        0        0     1599 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm.html
+-rw-r--r--   0        0        0      615 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
+-rw-r--r--   0        0        0       67 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/__init__.py
+-rw-r--r--   0        0        0     3933 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/conftest.py
+-rw-r--r--   0        0        0    24710 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_api.py
+-rw-r--r--   0        0        0     1535 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py
+-rw-r--r--   0        0        0    30041 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py
+-rw-r--r--   0        0        0    23393 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py
+-rw-r--r--   0        0        0    24237 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_model.py
+-rw-r--r--   0        0        0    11840 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
+-rw-r--r--   0        0        0    11615 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_views.py
+-rw-r--r--   0        0        0     9524 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/urls.py
+-rw-r--r--   0        0        0      423 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/utils.py
+-rw-r--r--   0        0        0    42336 2023-04-21 15:38:36.785759 nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/views.py
+-rw-r--r--   0        0        0     2771 2023-04-21 15:38:49.794005 nautobot_device_lifecycle_mgmt-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-1.2.0/PKG-INFO
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/LICENSE` & `nautobot_device_lifecycle_mgmt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/__init__.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     verbose_name = "Nautobot Device Lifecycle Management"
     version = __version__
     author = "Network to Code"
     author_email = "opensource@networktocode.com"
     description = "Manages device lifecycle of Nautobot Devices and Components."
     base_url = "nautobot-device-lifecycle-mgmt"
     required_settings = []
-    min_version = "1.2.0"
+    min_version = "1.4.0"
     max_version = "1.9999"
     default_settings = {
         "expired_field": "end_of_support",
         "barchart_bar_width": 0.1,
         "barchart_width": 12,
         "barchart_height": 5,
     }
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/nested_serializers.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/serializers.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/urls.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/api/views.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/choices.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/const.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/const.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/filters.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/forms.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/graphql/types.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/graphql/types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Jobs for the CVE Tracking portion of the Device Lifecycle plugin."""
 from datetime import datetime
 
-from nautobot.extras.jobs import Job, StringVar
+from nautobot.extras.jobs import Job, StringVar, BooleanVar
 from nautobot.extras.models import Relationship, RelationshipAssociation
 
 from nautobot_device_lifecycle_mgmt.models import (
     CVELCM,
     VulnerabilityLCM,
 )
 
@@ -27,23 +27,28 @@
         required=False,
     )
 
     class Meta:  # pylint: disable=too-few-public-methods
         """Meta class for the job."""
 
         commit_default = True
+        field_order = ["published_after", "_task_queue", "debug", "_commit"]
+
+    debug = BooleanVar(description="Enable for more verbose logging.")
 
     def run(self, data, commit):  # pylint: disable=too-many-locals
         """Check if software assigned to each device is valid. If no software is assigned return warning message."""
         # Although the default is set on the class attribute for the UI, it doesn't default for the API
         published_after = data.get("published_after", "1970-01-01")
         cves = CVELCM.objects.filter(published_date__gte=datetime.fromisoformat(published_after))
         count_before = VulnerabilityLCM.objects.count()
 
         for cve in cves:
+            if data["debug"]:
+                self.log_info(obj=cve, message="Generating vulnerabilities for CVE {cve}")
             software_rels = RelationshipAssociation.objects.filter(relationship__slug="soft_cve", destination_id=cve.id)
             for soft_rel in software_rels:
 
                 # Loop through any device relationships
                 device_rels = soft_rel.source.get_relationships()["source"][
                     Relationship.objects.get(slug="device_soft")
                 ]
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/models.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,17 +306,17 @@
         return reverse("plugins:nautobot_device_lifecycle_mgmt:softwareimagelcm", kwargs={"pk": self.pk})
 
     def to_csv(self):
         """Return fields for bulk view."""
         return (
             self.image_file_name,
             self.software.id,
-            f'"{",".join(str(device_type["model"]) for device_type in self.device_types.values())}"',
-            f'"{",".join(str(inventory_item["id"]) for inventory_item in self.inventory_items.values())}"',
-            f'"{",".join(str(object_tag["slug"]) for object_tag in self.object_tags.values())}"',
+            ",".join(str(device_type["model"]) for device_type in self.device_types.values()),
+            ",".join(str(inventory_item["id"]) for inventory_item in self.inventory_items.values()),
+            ",".join(str(object_tag["slug"]) for object_tag in self.object_tags.values()),
             self.download_url,
             self.image_file_checksum,
             self.default_image,
         )
 
     objects = SoftwareImageLCMQuerySet.as_manager()
 
@@ -415,19 +415,19 @@
                 "Validated Software object with this Software and Valid Since and Valid Until dates already exists."
             )
 
     def to_csv(self):
         """Return fields for bulk view."""
         return (
             self.software.id,
-            f'"{",".join(str(device["name"]) for device in self.devices.values())}"',
-            f'"{",".join(str(device_type["model"]) for device_type in self.device_types.values())}"',
-            f'"{",".join(str(device_role["slug"]) for device_role in self.device_roles.values())}"',
-            f'"{",".join(str(inventory_item["id"]) for inventory_item in self.inventory_items.values())}"',
-            f'"{",".join(str(object_tag["slug"]) for object_tag in self.object_tags.values())}"',
+            ",".join(str(device["name"]) for device in self.devices.values()),
+            ",".join(str(device_type["model"]) for device_type in self.device_types.values()),
+            ",".join(str(device_role["slug"]) for device_role in self.device_roles.values()),
+            ",".join(str(inventory_item["id"]) for inventory_item in self.inventory_items.values()),
+            ",".join(str(object_tag["slug"]) for object_tag in self.object_tags.values()),
             self.start,
             self.end,
             self.preferred,
         )
 
     objects = ValidatedSoftwareLCMQuerySet.as_manager()
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/navigation.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/signals.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/software.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/software_filters.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tables.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,26 @@
             "device_platform",
             "release_date",
             "end_of_support",
             "long_term_support",
             "pre_release",
             "actions",
         )
+        default_columns = (
+            "pk",
+            "name",
+            "version",
+            "alias",
+            "device_platform",
+            "release_date",
+            "end_of_support",
+            "long_term_support",
+            "pre_release",
+            "actions",
+        )
 
 
 class SoftwareImageLCMTable(BaseTable):
     """Table for SoftwareImageLCM."""
 
     pk = ToggleColumn()
     name = tables.LinkColumn(
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/template_content.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,82 @@
-{% extends 'base.html' %}
-{% load buttons %}
-{% load custom_links %}
-{% load helpers %}
+{% extends 'generic/object_detail.html' %}
 
-{% block title %}{{ object }}{% endblock %}
+{% block masthead %}
+    <h2>{% block title %}{{ object }}{% endblock %}</h2>
+{% endblock masthead %}
 
-{% block header %}
-    <div class="row noprint">
-        <div class="col-sm-12 col-md-12">
-            <ol class="breadcrumb">
-                <li><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_list' %}">Contract Point-of-Contacts</a></li>
-                <li><a>{{ object }}</a></li>
-            </ol>
-        </div>
-    </div>
-    <div class="pull-right noprint">
-        {% if perms.nautobot_device_lifecycle_mgmt.change_contactlcm %}
-            {% edit_button object %}
-        {% endif %}
-        {% if perms.nautobot_device_lifecycle_mgmt.delete_contactlcm %}
-            {% delete_button object %}
-        {% endif %}
-    </div>
-    <h2>Contact: {{ object }}</h2>
-        {% include 'inc/created_updated.html' with obj=object %}
-    <div class="pull-right noprint">
-        {% custom_links object %}
-    </div>
-    <ul class="nav nav-tabs">
-        <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-            <a href="{{ object.get_absolute_url }}">Contact</a>
-        </li>
-        <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_changelog' pk=object.id %}">Change Log</a>
-        </li>
-    </ul>
+{% block extra_buttons %}
+    {% if perms.nautobot_device_lifecycle_mgmt.add_softwareimagelcm and active_tab == 'software-images' %}
+        <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwareimagelcm_add' %}?software={{ object.pk }}" class="btn btn-success">
+            <span class="mdi mdi-plus-thick" aria-hidden="true"></span>
+            Add a Software Image
+        </a>
+    {% endif %}
+{% endblock extra_buttons %}
+
+{% block extra_nav_tabs %}
+    <li role="presentation"{% if active_tab == 'software-images' %} class="active"{% endif %}>
+        <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:software_software_images' pk=object.pk %}">Software Images <span class="badge">{{ object.get_software_images.count }}</span></a>
+    </li>
 {% endblock %}
 
-{% block content %}
-<div class="row">
-    <div class="col-md-8">
-        <div class="panel panel-default">
-            <div class="panel-heading">
-                <strong>Contact</strong>
-            </div>
-            <table class="table table-hover panel-body attr-table">
-                <tr>
-                    <td>Name</td>
-                    <td>{{ object.name }}</td>
-                </tr>
-                <tr>
-                    <td>Address</td>
-                    <td>{% if object.address %}
-                        <div class="pull-right noprint">
-                            <a href="https://maps.google.com/?q={{ object.address|urlencode }}" target="_blank" class="btn btn-primary btn-xs">
-                                <i class="mdi mdi-map-marker"></i> Map it
-                            </a>
-                        </div>
-                        <span>{{ object.address|linebreaksbr }}</span>
-                        {% else %} &mdash; {% endif %}
-                    </td>
-                </tr>
-                <tr>
-                    <td>Phone</td>
-                    <td>{{ object.phone|placeholder }}</td>
-                </tr>
-                <tr>
-                    <td>E-Mail</td>
-                    <td>{% if object.email %} <a href="mailto:{{ object.email }}">{{ object.email }}</a>{% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>PoC Type</td>
-                    <td>{{ object.type }}</td>
-                </tr>
-                <tr>
-                    <td>Assign to Contract</td>
-                    <td><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm' pk=object.contract.id %}">{{ object.contract.name }}</a></td>
-                </tr>
-                <tr>
-                    <td>Priority</td>
-                    <td>{{ object.priority }}</td>
-                </tr>
-                <tr>
-                    <td>Comments</td>
-                    <td>{% if object.comments %}<pre>{{ object.comments|placeholder  }}</pre>{% else %} &mdash; {% endif %}</td>
-                </tr>
-            </table>
+{% block content_left_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Software</strong>
         </div>
-        {% include 'inc/custom_fields_panel.html' %}
-        {% include 'inc/relationships_panel.html' %}
-        {% include 'extras/inc/tags_panel.html' with tags=object.tags.all %}
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>Device Platform</td>
+                <td>
+                    {% if object.device_platform %}
+                        <a href="{% url 'dcim:platform' slug=object.device_platform.slug %}">{{ object.device_platform }}</a>
+                    {% else %}
+                        &mdash;
+                    {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Software Version</td>
+                <td>{{ object.version }}</td>
+            </tr>
+            <tr>
+                <td>Release Date</td>
+                <td>{{ object.release_date }}</td>
+            </tr>
+            <tr>
+                <td>End of Support</td>
+                <td>{{ object.end_of_support }}</td>
+            </tr>
+            <tr>
+                <td>Documentation URL</td>
+                <td>
+                {% if object.documentation_url %}
+                    <a href="{{ object.documentation_url }}">{{ object.documentation_url }}</a>
+                {% else %}
+                    <span class="text-muted">&mdash;</span>
+                {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Long Term Support</td>
+                <td>
+                {% if object.long_term_support is True %}
+                    <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                {% else %}
+                    <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Pre Release</td>
+                <td>
+                {% if object.pre_release is True %}
+                    <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                {% else %}
+                    <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                {% endif %}
+                </td>
+            </tr>
+        </table>
     </div>
-</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,33 +1,23 @@
-{% extends 'base.html' %} {% load buttons %} {% load custom_links %} {% load
-helpers %} {% block title %}{{ object }}{% endblock %} {% block header %}
-   1. Contract_Point-of-Contacts
-   2. {{ object }}
-{% if perms.nautobot_device_lifecycle_mgmt.change_contactlcm %} {% edit_button
-object %} {% endif %} {% if
-perms.nautobot_device_lifecycle_mgmt.delete_contactlcm %} {% delete_button
-object %} {% endif %}
-***** Contact: {{ object }} *****
-{% include 'inc/created_updated.html' with obj=object %}
-{% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Contact
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
-{% endblock %} {% block content %}
-Contact
-Name      {{ object.name }}
-          {% if object.address %}
-Address    Map_it
-          {{ object.address|linebreaksbr }} {% else %} — {% endif %}
-Phone     {{ object.phone|placeholder }}
-E-Mail    {% if object.email %} {{_object.email_}}{% else %} — {% endif
-          %}
-PoC Type  {{ object.type }}
-Assign to {{_object.contract.name_}}
-Contract
-Priority  {{ object.priority }}
-          {% if object.comments %}
-Comments  {{ object.comments|placeholder  }}
-          {% else %} — {% endif %}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% include 'extras/inc/tags_panel.html' with
-tags=object.tags.all %}
+{% extends 'generic/object_detail.html' %} {% block masthead %}
+***** {% block title %}{{ object }}{% endblock %} *****
+{% endblock masthead %} {% block extra_buttons %} {% if
+perms.nautobot_device_lifecycle_mgmt.add_softwareimagelcm and active_tab ==
+'software-images' %} _Add_a_Software_Image {% endif %} {% endblock
+extra_buttons %} {% block extra_nav_tabs %}
+% if active_tab == 'software-images' %} class="active"{% endif %}> Software
+Images_{{_object.get_software_images.count_}}
+{% endblock %} {% block content_left_page %}
+Software
+Device        {% if object.device_platform %} {{_object.device_platform_}} {% else %} — {%
+Platform      endif %}
+Software      {{ object.version }}
+Version
+Release Date  {{ object.release_date }}
+End of        {{ object.end_of_support }}
+Support
+Documentation {% if object.documentation_url %} {{_object.documentation_url_}} {% else %} — {%
+URL           endif %}
+Long Term     {% if object.long_term_support is True %}  {% else %}  {% endif %}
+Support
+Pre Release   {% if object.pre_release is True %}  {% else %}  {% endif %}
 {% endblock %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,187 +1,149 @@
-{% extends 'base.html' %}
-{% load buttons %}
-{% load custom_links %}
+{% extends 'generic/object_detail.html' %}
 {% load helpers %}
 {% load humanize %}
 
-{% block title %}{{ object }}{% endblock %}
+{% block masthead %}
+    <h2>Contract: {% block title %}{{ object }}{% endblock %}</h2>
+{% endblock masthead %}
 
-{% block header %}
-    <div class="row noprint">
-        <div class="col-sm-12 col-md-12">
-            <ol class="breadcrumb">
-                <li><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm_list' %}">Contracts</a></li>
-                <li><a>{{ object }}</a></li>
-            </ol>
+{% block content_left_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Contract</strong>
         </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr style="font-weight: bold">
+                <td>Name</td>
+                <td>{{ object.name }}</td>
+            </tr>
+            <tr>
+                <td>Provider</td>
+                <td>
+                    <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:providerlcm' pk=object.provider.id %}">
+                        {{ object.provider }}
+                    </a>
+                </td>
+            </tr>
+            <tr>
+                <td>Start Date</td>
+                <td>{% if object.start %} {{ object.start }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>End Date</td>
+                <td>{% if object.end %} {{ object.end }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>Cost</td>
+                <td>{% if object.cost %} {{ object.cost | intcomma }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>Currency</td>
+                <td>{% if object.currency %} {{ object.currency }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>Support Level</td>
+                <td>{% if object.support_level %} {{ object.support_level }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>Contract Type</td>
+                <td>{% if object.contract_type %} {{ object.contract_type }} {% else %} &mdash; {% endif %}</td>
+            </tr>
+            <tr>
+                <td>Comments</td>
+                <td>{% if object.comments %}<pre>{{ object.comments|placeholder  }}</pre>{% else %} &mdash; {% endif %}</td>
+            </tr>
+        </table>
     </div>
-    <div class="pull-right noprint">
-        {% if perms.nautobot_device_lifecycle_mgmt.change_contractlcm %}
-            {% edit_button object %}
-        {% endif %}
-        {% if perms.nautobot_device_lifecycle_mgmt.delete_contractlcm %}
-            {% delete_button object %}
-        {% endif %}
-    </div>
-    <h2>Contract: {{ object }}</h2>
-        {% include 'inc/created_updated.html' with obj=object %}
-    <div class="pull-right noprint">
-        {% custom_links object %}
-    </div>
-    <ul class="nav nav-tabs">
-        <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-            <a href="{{ object.get_absolute_url }}">Contract</a>
-        </li>
-        <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm_changelog' pk=object.id %}">Change Log</a>
-        </li>
-    </ul>
 {% endblock %}
 
-{% block content %}
-<div class="row">
-    <div class="col-md-6">
-        <div class="panel panel-default">
-            <div class="panel-heading">
-                <strong>Contract</strong>
-            </div>
-            <table class="table table-hover panel-body attr-table">
-                <tr style="font-weight: bold">
-                    <td>Name</td>
-                    <td>{{ object.name }}</td>
-                </tr>
-                <tr>
-                    <td>Provider</td>
-                    <td>
-                        <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:providerlcm' pk=object.provider.id %}">
-                            {{ object.provider }}
-                        </a>
-                    </td>
-                </tr>
-                <tr>
-                    <td>Start Date</td>
-                    <td>{% if object.start %} {{ object.start }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>End Date</td>
-                    <td>{% if object.end %} {{ object.end }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>Cost</td>
-                    <td>{% if object.cost %} {{ object.cost | intcomma }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>Currency</td>
-                    <td>{% if object.currency %} {{ object.currency }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>Support Level</td>
-                    <td>{% if object.support_level %} {{ object.support_level }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>Contract Type</td>
-                    <td>{% if object.contract_type %} {{ object.contract_type }} {% else %} &mdash; {% endif %}</td>
-                </tr>
-                <tr>
-                    <td>Comments</td>
-                    <td>{% if object.comments %}<pre>{{ object.comments|placeholder  }}</pre>{% else %} &mdash; {% endif %}</td>
-                </tr>
-            </table>
+{% block content_right_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Escalation Contacts</strong>
         </div>
-        {% include 'inc/custom_fields_panel.html' %}
-        {% include 'inc/relationships_panel.html' %}
-        {% include 'extras/inc/tags_panel.html' with tags=object.tags.all %}
-    </div>
-    <div class="col-md-6">
-        <div class="panel panel-default">
-            <div class="panel-heading">
-                <strong>Escalation Contacts</strong>
-            </div>
-            <table class="table table-hover panel-body attr-table">
-                <thead>
-                <tr>
-                    <th style="width: 5%"></th>
-                    <th>Name</th>
-                    <th>E-Mail</th>
-                    <th>Phone</th>
-                    <th>Tier</th>
-                </tr>
-                </thead>
-                <tbody>
-                {% if not contacts %}
-                <tr>
-                    <td colspan="5" class="text-muted text-center">
-                        No contacts defined. Click the 'Add PoC' button below to add contacts.
-                    </td>
-                </tr>
-                {% endif %}
-                {% for contact in contacts %}
-                <tr>
-                    <td style="width: 5%">
-                        {% if contact.type == "Primary" %}
-                        <span class="mdi mdi-star" data-toggle="tooltip" title="Primary Contact"></span>
-                        {% endif %}
-                    </td>
-                    <td><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm' pk=contact.id %}">{{ contact.name }}</a></td>
-                    <td>
-                        {% if contact.email %}
-                        <a href="mailto:{{ contact.email }}">{{ contact.email }}</a>
-                        {% else %}&mdash;{% endif %}
-                    </td>
-                    <td>{{ contact.phone|placeholder }}</td>
-                    <td>{{ contact.type }}</td>
-                </tr>
-                {% endfor %}
-                </tbody>
-            </table>
-            <div class="panel-footer text-right no-print">
-                <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_add' %}?contract={{ object.id }}&return_url={% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm' pk=object.pk %}" class="btn btn-primary btn-xs">
-                    <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Contact
-                </a>
-            </div>
+        <table class="table table-hover panel-body attr-table">
+            <thead>
+            <tr>
+                <th style="width: 5%"></th>
+                <th>Name</th>
+                <th>E-Mail</th>
+                <th>Phone</th>
+                <th>Tier</th>
+            </tr>
+            </thead>
+            <tbody>
+            {% if not contacts %}
+            <tr>
+                <td colspan="5" class="text-muted text-center">
+                    No contacts defined. Click the 'Add PoC' button below to add contacts.
+                </td>
+            </tr>
+            {% endif %}
+            {% for contact in contacts %}
+            <tr>
+                <td style="width: 5%">
+                    {% if contact.type == "Primary" %}
+                    <span class="mdi mdi-star" data-toggle="tooltip" title="Primary Contact"></span>
+                    {% endif %}
+                </td>
+                <td><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm' pk=contact.id %}">{{ contact.name }}</a></td>
+                <td>
+                    {% if contact.email %}
+                    <a href="mailto:{{ contact.email }}">{{ contact.email }}</a>
+                    {% else %}&mdash;{% endif %}
+                </td>
+                <td>{{ contact.phone|placeholder }}</td>
+                <td>{{ contact.type }}</td>
+            </tr>
+            {% endfor %}
+            </tbody>
+        </table>
+        <div class="panel-footer text-right no-print">
+            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_add' %}?contract={{ object.id }}&return_url={% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm' pk=object.pk %}" class="btn btn-primary btn-xs">
+                <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Contact
+            </a>
         </div>
+    </div>
 
-        <div class="panel panel-default">
-            <div class="panel-heading">
-                <strong>Service Contract Owner</strong>
-            </div>
-            <table class="table table-hover panel-body attr-table">
-                <thead>
-                <tr>
-                    <th style="width: 5%"></th>
-                    <th>Name</th>
-                    <th>E-Mail</th>
-                    <th>Phone</th>
-                </tr>
-                </thead>
-                <tbody>
-                {% if not owners %}
-                <tr>
-                    <td colspan="5" class="text-muted text-center">
-                        No contract owner defined. Click the 'Add Owner' button below to add an owner.
-                    </td>
-                </tr>
-                {% endif %}
-                {% for contact in owners %}
-                <tr>
-                    <td style="width: 5%"></td>
-                    <td><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm' pk=contact.id %}">{{ contact.name }}</a></td>
-                    <td>
-                        {% if contact.email %}
-                        <a href="mailto:{{ contact.email }}">{{ contact.email }}</a>
-                        {% else %}&mdash{% endif %}
-                    </td>
-                    <td>{{ contact.phone|placeholder }}</td>
-                </tr>
-                {% endfor %}
-                </tbody>
-            </table>
-            <div class="panel-footer text-right no-print">
-                <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_add' %}?type=Owner&contract={{ object.id }}&return_url={% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm' pk=object.pk %}" class="btn btn-primary btn-xs">
-                    <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Owner
-                </a>
-            </div>
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Service Contract Owner</strong>
+        </div>
+        <table class="table table-hover panel-body attr-table">
+            <thead>
+            <tr>
+                <th style="width: 5%"></th>
+                <th>Name</th>
+                <th>E-Mail</th>
+                <th>Phone</th>
+            </tr>
+            </thead>
+            <tbody>
+            {% if not owners %}
+            <tr>
+                <td colspan="5" class="text-muted text-center">
+                    No contract owner defined. Click the 'Add Owner' button below to add an owner.
+                </td>
+            </tr>
+            {% endif %}
+            {% for contact in owners %}
+            <tr>
+                <td style="width: 5%"></td>
+                <td><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm' pk=contact.id %}">{{ contact.name }}</a></td>
+                <td>
+                    {% if contact.email %}
+                    <a href="mailto:{{ contact.email }}">{{ contact.email }}</a>
+                    {% else %}&mdash{% endif %}
+                </td>
+                <td>{{ contact.phone|placeholder }}</td>
+            </tr>
+            {% endfor %}
+            </tbody>
+        </table>
+        <div class="panel-footer text-right no-print">
+            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:contactlcm_add' %}?type=Owner&contract={{ object.id }}&return_url={% url 'plugins:nautobot_device_lifecycle_mgmt:contractlcm' pk=object.pk %}" class="btn btn-primary btn-xs">
+                <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Owner
+            </a>
         </div>
     </div>
-</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,22 +1,11 @@
-{% extends 'base.html' %} {% load buttons %} {% load custom_links %} {% load
-helpers %} {% load humanize %} {% block title %}{{ object }}{% endblock %} {%
-block header %}
-   1. Contracts
-   2. {{ object }}
-{% if perms.nautobot_device_lifecycle_mgmt.change_contractlcm %} {% edit_button
-object %} {% endif %} {% if
-perms.nautobot_device_lifecycle_mgmt.delete_contractlcm %} {% delete_button
-object %} {% endif %}
-***** Contract: {{ object }} *****
-{% include 'inc/created_updated.html' with obj=object %}
-{% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Contract
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
-{% endblock %} {% block content %}
+{% extends 'generic/object_detail.html' %} {% load helpers %} {% load humanize
+%} {% block masthead %}
+***** Contract: {% block title %}{{ object }}{% endblock %} *****
+{% endblock masthead %} {% block content_left_page %}
 Contract
 Name     {{ object.name }}
 Provider {{_object.provider_}}
 Start    {% if object.start %} {{ object.start }} {% else %} — {% endif %}
 Date
 End Date {% if object.end %} {{ object.end }} {% else %} — {% endif %}
 Cost     {% if object.cost %} {{ object.cost | intcomma }} {% else %} — {% endif %}
@@ -24,17 +13,15 @@
 Support  {% if object.support_level %} {{ object.support_level }} {% else %} — {% endif
 Level    %}
 Contract {% if object.contract_type %} {{ object.contract_type }} {% else %} — {% endif
 Type     %}
          {% if object.comments %}
 Comments {{ object.comments|placeholder  }}
          {% else %} — {% endif %}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% include 'extras/inc/tags_panel.html' with
-tags=object.tags.all %}
+{% endblock %} {% block content_right_page %}
 Escalation Contacts
              Name         E-Mail                                                           Phone                     Tier
 No contacts defined. Click the 'Add PoC' button below to add contacts.
 {% if        {                                                                             {                         {
 contact.type {            {% if contact.email %} {{_contact.email_}} {% else %}—{% endif {                         {
 == "Primary" contact.name %}                                                               contact.phone|placeholder contact.type
 %}  {% endif }}                                                                            }}                        }}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,162 @@
-{% extends 'base.html' %}
-{% load plugins %}
-{% load buttons %}
-{% load custom_links %}
-{% load helpers %}
+{% extends 'generic/object_detail.html' %}
 
-{% block title %}{{ object }}{% endblock %}
+{% block masthead %}
+    <h2>{% block title %}{{ object }}{% endblock %}</h2>
+{% endblock masthead %}
 
-{% block header %}
-    <div class="row noprint">
-        <div class="col-sm-8 col-md-9">
-            <ol class="breadcrumb">
-                <li><a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwarelcm_list' %}">Software</a></li>
-                <li><a>{{ object }}</a></li>
-            </ol>
+{% block content_left_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>ValidatedSoftware</strong>
         </div>
-        <div class="col-sm-4 col-md-3">
-            <form action="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwarelcm_list' %}" method="get">
-                <div class="input-group">
-                    <input type="text" name="q" class="form-control" />
-                    <span class="input-group-btn">
-                        <button type="submit" class="btn btn-primary">
-                            <span class="mdi mdi-magnify" aria-hidden="true"></span> Search
-                        </button>
-                    </span>
-                </div>
-            </form>
-        </div>
-    </div>
-    <div class="pull-right noprint">
-        {% plugin_buttons object %}
-        {% if perms.nautobot_device_lifecycle_mgmt.add_softwareimagelcm and active_tab == 'software-images' %}
-            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwareimagelcm_add' %}?software={{ object.pk }}" class="btn btn-success">
-                <span class="mdi mdi-plus-thick" aria-hidden="true"></span>
-                Add a Software Image
-            </a>
-        {% endif %}
-        {% if perms.nautobot_device_lifecycle_mgmt.change_softwarelcm %}
-            {% edit_button object %}
-        {% endif %}
-        {% if perms.nautobot_device_lifecycle_mgmt.delete_softwarelcm %}
-            {% delete_button object %}
-        {% endif %}
-    </div>
-    <h2>{{ object }}</h2>
-        {% include 'inc/created_updated.html' with obj=object %}
-    <div class="pull-right noprint">
-        {% custom_links object %}
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>Software Version</td>
+                <td>
+                    {% if object.software %}
+                        <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwarelcm' pk=object.software.pk %}">{{ object.software }}</a>
+                    {% else %}
+                        &mdash;
+                    {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Valid Start</td>
+                <td>{{ object.start }}</td>
+            </tr>
+            <tr>
+                <td>Valid End</td>
+                <td>
+                    {% if object.end %}
+                        {{ object.end }}
+                    {% else %}
+                        &mdash;
+                    {% endif %}
+                </td>
+            </tr>
+                <td>Valid Now</td>
+                <td>
+                {% if object.valid is True %}
+                    <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                {% else %}
+                    <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>Preferred Version</td>
+                <td>
+                {% if object.preferred is True %}
+                    <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                {% else %}
+                    <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                {% endif %}
+                </td>
+            </tr>
+        </table>
     </div>
-    <ul class="nav nav-tabs">
-        <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-            <a href="{{ object.get_absolute_url }}">Software</a>
-        </li>
-        <li role="presentation"{% if active_tab == 'software-images' %} class="active"{% endif %}>
-            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:software_software_images' pk=object.pk %}">Software Images <span class="badge">{{ object.get_software_images.count }}</span></a>
-        </li>
-        <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-            <a href="{% url 'plugins:nautobot_device_lifecycle_mgmt:softwarelcm_changelog' pk=object.id %}">Change Log</a>
-        </li>
-    </ul>
 {% endblock %}
 
-{% block content %}
-<div class="row">
-    <div class="col-md-6">
-        <div class="panel panel-default">
-            <div class="panel-heading">
-                <strong>Software</strong>
-            </div>
-            <table class="table table-hover panel-body attr-table">
-                <tr>
-                    <td>Device Platform</td>
-                    <td>
-                        {% if object.device_platform %}
-                            <a href="{% url 'dcim:platform' slug=object.device_platform.slug %}">{{ object.device_platform }}</a>
-                        {% else %}
-                            &mdash;
-                        {% endif %}
-                    </td>
-                </tr>
-                <tr>
-                    <td>Software Version</td>
-                    <td>{{ object.version }}</td>
-                </tr>
-                <tr>
-                    <td>Release Date</td>
-                    <td>{{ object.release_date }}</td>
-                </tr>
-                <tr>
-                    <td>End of Support</td>
-                    <td>{{ object.end_of_support }}</td>
-                </tr>
-                <tr>
-                    <td>Documentation URL</td>
-                    <td>
-                    {% if object.documentation_url %}
-                        <a href="{{ object.documentation_url }}">{{ object.documentation_url }}</a>
-                    {% else %}
-                     <span class="text-muted">&mdash;</span>
-                    {% endif %}
-                    </td>
-                </tr>
-                <tr>
-                    <td>Long Term Support</td>
-                    <td>
-                    {% if object.long_term_support is True %}
-                        <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
-                    {% else %}
-                        <span class="text-danger"><i class="mdi mdi-close"></i></span>
-                    {% endif %}
-                    </td>
-                </tr>
-                <tr>
-                    <td>Pre Release</td>
-                    <td>
-                    {% if object.pre_release is True %}
-                        <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
-                    {% else %}
-                        <span class="text-danger"><i class="mdi mdi-close"></i></span>
-                    {% endif %}
-                    </td>
-                </tr>
-            </table>
+{% block content_right_page %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Device assignments</strong>
+        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>
+                    Devices
+                </td>
+                <td>
+                    {% if object.devices.all %}
+                    <ul>
+                        {% for device in object.devices.all %}
+                            <li><a href="{{ device.get_absolute_url }}">{{ device }}</a></li>
+                        {% endfor %}
+                    </ul>
+                    {% else %}
+                        <span class="text-muted">None</span>
+                    {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>
+                    Device Types
+                </td>
+                <td>
+                    {% if object.device_types.all %}
+                    <ul>
+                        {% for device_type in object.device_types.all %}
+                            <li><a href="{{ device_type.get_absolute_url }}">{{ device_type }}</a></li>
+                        {% endfor %}
+                    </ul>
+                    {% else %}
+                        <span class="text-muted">None</span>
+                    {% endif %}
+                </td>
+            </tr>
+            <tr>
+                <td>
+                    Device Roles
+                </td>
+                <td>
+                    {% if object.device_roles.all %}
+                    <ul>
+                        {% for role in object.device_roles.all %}
+                            <li><a href="{{ role.get_absolute_url }}">{{ role }}</a></li>
+                        {% endfor %}
+                    </ul>
+                    {% else %}
+                        <span class="text-muted">None</span>
+                    {% endif %}
+                </td>
+            </tr>
+        </table>
+    </div>
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Inventory Items assignments</strong>
         </div>
-        {% include 'inc/custom_fields_panel.html' %}
-        {% include 'inc/relationships_panel.html' %}
-        {% include 'extras/inc/tags_panel.html' with tags=object.tags.all %}
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>
+                    Inventory Items
+                </td>
+                <td>
+                    {% if object.inventory_items.all %}
+                    <ul>
+                        {% for inventory_item in object.inventory_items.all %}
+                            <li><a href="{{ inventory_item.get_absolute_url }}">{{ inventory_item }}</a></li>
+                        {% endfor %}
+                    </ul>
+                    {% else %}
+                        <span class="text-muted">None</span>
+                    {% endif %}
+                </td>
+            </tr>
+        </table>
     </div>
-</div>
-{% endblock %}
+    <div class="panel panel-default">
+        <div class="panel-heading">
+            <strong>Object Tags assignments</strong>
+        </div>
+        <table class="table table-hover panel-body attr-table">
+            <tr>
+                <td>
+                    Object Tags
+                </td>
+                <td>
+                    {% if object.object_tags.all %}
+                    <ul>
+                        {% for object_tag in object.object_tags.all %}
+                            <li><a href="{{ object_tag.get_absolute_url }}">{{ object_tag }}</a></li>
+                        {% endfor %}
+                    </ul>
+                    {% else %}
+                        <span class="text-muted">None</span>
+                    {% endif %}
+                </td>
+            </tr>
+        </table>
+    </div>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,38 +1,41 @@
-{% extends 'base.html' %} {% load plugins %} {% load buttons %} {% load
-custom_links %} {% load helpers %} {% block title %}{{ object }}{% endblock %}
-{% block header %}
-   1. Software
-   2. {{ object }}
-[q                   ]    Search
-{% plugin_buttons object %} {% if
-perms.nautobot_device_lifecycle_mgmt.add_softwareimagelcm and active_tab ==
-'software-images' %} _Add_a_Software_Image {% endif %} {% if
-perms.nautobot_device_lifecycle_mgmt.change_softwarelcm %} {% edit_button
-object %} {% endif %} {% if
-perms.nautobot_device_lifecycle_mgmt.delete_softwarelcm %} {% delete_button
-object %} {% endif %}
-***** {{ object }} *****
-{% include 'inc/created_updated.html' with obj=object %}
-{% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Software
-% if active_tab == 'software-images' %} class="active"{% endif %}> Software
-Images_{{_object.get_software_images.count_}}
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
-{% endblock %} {% block content %}
-Software
-Device        {% if object.device_platform %} {{_object.device_platform_}} {% else %} — {%
-Platform      endif %}
-Software      {{ object.version }}
+{% extends 'generic/object_detail.html' %} {% block masthead %}
+***** {% block title %}{{ object }}{% endblock %} *****
+{% endblock masthead %} {% block content_left_page %}
+ValidatedSoftware
+Software  {% if object.software %} {{_object.software_}} {% else %} — {% endif
+Version   %}
+Valid     {{ object.start }}
+Start
+Valid End {% if object.end %} {{ object.end }} {% else %} — {% endif %}
+Preferred {% if object.preferred is True %}  {% else %}  {% endif %}
 Version
-Release Date  {{ object.release_date }}
-End of        {{ object.end_of_support }}
-Support
-Documentation {% if object.documentation_url %} {{_object.documentation_url_}} {% else %} — {%
-URL           endif %}
-Long Term     {% if object.long_term_support is True %}  {% else %}  {% endif %}
-Support
-Pre Release   {% if object.pre_release is True %}  {% else %}  {% endif %}
-{% include 'inc/custom_fields_panel.html' %} {% include 'inc/
-relationships_panel.html' %} {% include 'extras/inc/tags_panel.html' with
-tags=object.tags.all %}
+{% endblock %} {% block content_right_page %}
+Device assignments
+             {% if object.devices.all %}
+                 * {% for device in object.devices.all %}
+Devices          * {{_device_}}
+                 * {% endfor %}
+             {% else %} None {% endif %}
+             {% if object.device_types.all %}
+                 * {% for device_type in object.device_types.all %}
+Device Types     * {{_device_type_}}
+                 * {% endfor %}
+             {% else %} None {% endif %}
+             {% if object.device_roles.all %}
+                 * {% for role in object.device_roles.all %}
+Device Roles     * {{_role_}}
+                 * {% endfor %}
+             {% else %} None {% endif %}
+Inventory Items assignments
+                {% if object.inventory_items.all %}
+                    * {% for inventory_item in object.inventory_items.all %}
+Inventory Items     * {{_inventory_item_}}
+                    * {% endfor %}
+                {% else %} None {% endif %}
+Object Tags assignments
+            {% if object.object_tags.all %}
+                * {% for object_tag in object.object_tags.all %}
+Object Tags     * {{_object_tag_}}
+                * {% endfor %}
+            {% else %} None {% endif %}
 {% endblock %}
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/conftest.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,27 @@
 def create_cves():
     """Create CVELCM items for tests."""
     cves = (
         CVELCM.objects.create(
             name="CVE-2021-1391",
             published_date="2021-03-24",
             link="https://www.cvedetails.com/cve/CVE-2021-1391/",
+            description="A vulnerability in the dragonite debugger of Cisco IOS XE Software",
         ),
         CVELCM.objects.create(
             name="CVE-2021-44228",
             published_date="2021-12-10",
             link="https://www.cvedetails.com/cve/CVE-2021-44228/",
+            description="Apache Log4j2 2.0-beta9 through 2.15.0",
         ),
         CVELCM.objects.create(
             name="CVE-2020-27134",
             published_date="2020-12-11",
             link="https://www.cvedetails.com/cve/CVE-2020-27134/",
+            description="Multiple vulnerabilities in Cisco Jabber",
         ),
     )
     return cves
 
 
 def create_softwares():
     """Create SoftwareLCM items for tests."""
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_api.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_filters.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_forms.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_model.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/tests/test_views.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,29 @@
 
     @classmethod
     def setUpTestData(cls):
         """Create a superuser and token for API calls."""
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
         device_types = tuple(
             DeviceType.objects.create(model=model, slug=model, manufacturer=manufacturer)
-            for model in ["c9300-24", "c9300-48", "c9500-24", "c9200-24", "c9200-48"]
+            for model in ["c9300-24", "c9300-48", "c9500-24", "c9500-48", "c9200-24", "c9200-48"]
         )
 
         HardwareLCM.objects.create(device_type=device_types[0], end_of_sale=datetime.date(2021, 4, 1))
         HardwareLCM.objects.create(device_type=device_types[1], end_of_sale=datetime.date(2021, 4, 1))
+        HardwareLCM.objects.create(device_type=device_types[2], end_of_sale=datetime.date(2021, 4, 1))
 
         cls.form_data = {
-            "device_type": device_types[2].id,
+            "device_type": device_types[3].id,
             "end_of_sale": datetime.date(2021, 4, 1),
             "end_of_support": datetime.date(2024, 4, 1),
         }
         cls.csv_data = (
             "device_type,end_of_sale,end_of_support,end_of_sw_releases,end_of_security_patches,documentation_url",
-            "c9500-24, 2021-10-06, 2022-10-06, 2025-10-06, 2026-10-06, https://cisco.com/eox",
+            "c9500-48, 2021-10-06, 2022-10-06, 2025-10-06, 2026-10-06, https://cisco.com/eox",
             "c9200-24, 2022-10-06, 2023-10-06, 2025-10-06, 2026-10-06, https://cisco.com/eox",
             "c9200-48, 2023-10-06, 2024-10-06, 2025-10-06, 2026-10-06, https://cisco.com/eox",
         )
 
     def test_has_advanced_tab(self):
         pass
 
@@ -204,20 +205,15 @@
         "slug": "test-1",
         "published_date": datetime.date(2022, 1, 1),
         "link": "https://www.cvedetails.com/cve/CVE-2022-0001/",
     }
 
     @classmethod
     def setUpTestData(cls):
-        CVELCM.objects.create(
-            name="CVE-2021-1391", published_date="2021-03-24", link="https://www.cvedetails.com/cve/CVE-2021-1391/"
-        )
-        CVELCM.objects.create(
-            name="CVE-2021-34699", published_date="2021-09-23", link="https://www.cvedetails.com/cve/CVE-2021-34699/"
-        )
+        create_cves()
 
     def test_bulk_import_objects_with_constrained_permission(self):
         pass
 
     def test_bulk_import_objects_with_permission(self):
         pass
 
@@ -243,21 +239,30 @@
     model = VulnerabilityLCM
 
     @classmethod
     def setUpTestData(cls):
         devices = create_devices()
         softwares = create_softwares()
         cves = create_cves()
-        for i, cve in enumerate(cves):
-            VulnerabilityLCM.objects.create(cve=cve, software=softwares[i], device=devices[i])
 
         vuln_ct = ContentType.objects.get_for_model(VulnerabilityLCM)
-        status = Status.objects.create(name="Exempt", slug="exempt", color="4caf50", description="This unit is exempt.")
-        status.content_types.set([vuln_ct])
-        cls.bulk_edit_data = {"status": status.id}
+
+        exempt_status = Status.objects.create(
+            name="Exempt", slug="exempt", color="4caf50", description="This unit is exempt."
+        )
+        exempt_status.content_types.set([vuln_ct])
+        cls.bulk_edit_data = {"status": exempt_status.id}
+
+        forced_status = Status.objects.create(
+            name="Forced", slug="forced", color="4caf50", description="This unit is forced."
+        )
+        forced_status.content_types.set([vuln_ct])
+
+        for i, cve in enumerate(cves):
+            VulnerabilityLCM.objects.create(cve=cve, software=softwares[i], device=devices[i], status=forced_status)
 
     def test_bulk_import_objects_with_constrained_permission(self):
         pass
 
     def test_bulk_import_objects_with_permission(self):
         pass
 
@@ -294,31 +299,32 @@
 
     model = SoftwareImageLCM
 
     @classmethod
     def setUpTestData(cls):
         softwares = create_softwares()
         manufacturer = Manufacturer.objects.create(name="Cisco", slug="cisco")
-        device_type = DeviceType.objects.create(manufacturer=manufacturer, model="6509-E", slug="6509-e")
+        device_type1 = DeviceType.objects.create(manufacturer=manufacturer, model="6509", slug="6509")
+        device_type2 = DeviceType.objects.create(manufacturer=manufacturer, model="6509-E", slug="6509-e")
 
-        SoftwareImageLCM.objects.create(
+        softimage = SoftwareImageLCM.objects.create(
             image_file_name="ios15.1.2m.img",
             software=softwares[0],
             download_url="ftp://images.local/cisco/ios15.1.2m.img",
             image_file_checksum="441rfabd75b0512r7fde7a7a66faa596",
             default_image=True,
         )
-        softimage = SoftwareImageLCM.objects.create(
+        softimage.device_types.set([device_type1, device_type2])
+        SoftwareImageLCM.objects.create(
             image_file_name="ios4.22.9m.img",
             software=softwares[1],
             download_url="ftp://images.local/cisco/ios4.22.9m.img",
             image_file_checksum="58arfabd75b051fr7fde7a7ac6faa3fv",
             default_image=False,
         )
-        softimage.device_types.set([device_type])
 
         cls.form_data = {
             "image_file_name": "eos_4.21m.swi",
             "software": softwares[-1].id,
             "download_url": "ftp://images.local/arista/eos_4.21m.swi",
             "image_file_checksum": "78arfabd75b0fa2vzas1e7a7ac6faa3fc",
             "default_image": True,
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/urls.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/nautobot_device_lifecycle_mgmt/views.py` & `nautobot_device_lifecycle_mgmt-1.2.0/nautobot_device_lifecycle_mgmt/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Views implementation for the Lifecycle Management plugin."""
 import base64
+import inspect
 import io
 import logging
 import urllib
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 import numpy as np
 
 from django.db.models import Q, F, Count, ExpressionWrapper, FloatField
 from django_tables2 import RequestConfig
 
+from nautobot.core.forms import SearchForm
 from nautobot.core.views import generic
 from nautobot.dcim.models import Device
 from nautobot.utilities.paginator import EnhancedPaginator, get_paginate_count
 from nautobot.utilities.views import ContentTypePermissionRequiredMixin
 from nautobot_device_lifecycle_mgmt import choices
 from nautobot_device_lifecycle_mgmt.models import (
     HardwareLCM,
@@ -200,14 +202,29 @@
     action_buttons = (
         "add",
         "import",
         "export",
     )
     template_name = "nautobot_device_lifecycle_mgmt/softwarelcm_list.html"
 
+    def extra_context(self):
+        """Changes "Softwares" => "Software"."""
+        # TODO: Remove the dynamic check for 'q_placeholder' once we dropped the support for Nautobot < 1.5.0
+        if "q_placeholder" in inspect.signature(SearchForm.__init__).parameters:
+            search_form = SearchForm(data=self.request.GET, q_placeholder="Search Software")
+        else:
+            search_form = SearchForm(data=self.request.GET)
+
+        return {
+            **super().extra_context(),
+            "search_form": search_form,
+            "title": "Software",
+            "verbose_name_plural": "Software",
+        }
+
 
 class SoftwareLCMView(generic.ObjectView):
     """SoftwareLCM Detail view."""
 
     queryset = SoftwareLCM.objects.prefetch_related("device_platform")
 
     def get_extra_context(self, request, instance):
@@ -216,14 +233,16 @@
         if softwareimages.exists():
             softwareimages_table = SoftwareImageLCMTable(data=softwareimages, user=request.user, orderable=False)
         else:
             softwareimages_table = None
 
         extra_context = {
             "softwareimages_table": softwareimages_table,
+            "title": "Software",
+            "verbose_name_plural": "Software",
         }
 
         return extra_context
 
 
 class SoftwareLCMCreateView(generic.ObjectEditView):
     """SoftwareLCM Create view."""
@@ -358,20 +377,43 @@
     action_buttons = (
         "add",
         "import",
         "export",
     )
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html"
 
+    def extra_context(self):
+        """Changes "Softwares" => "Software"."""
+        # TODO: Remove the dynamic check for 'q_placeholder' once we dropped the support for Nautobot < 1.5.0
+        if "q_placeholder" in inspect.signature(SearchForm.__init__).parameters:
+            search_form = SearchForm(data=self.request.GET, q_placeholder="Search Validated Software")
+        else:
+            search_form = SearchForm(data=self.request.GET)
+
+        return {
+            **super().extra_context(),
+            "search_form": search_form,
+            "title": "Validated Software",
+            "verbose_name_plural": "Validated Software",
+        }
+
 
 class ValidatedSoftwareLCMView(generic.ObjectView):
     """ValidatedSoftware Detail view."""
 
     queryset = ValidatedSoftwareLCM.objects.all()
 
+    def get_extra_context(self, *args, **kwargs):
+        """Changes "Softwares" => "Software"."""
+        return {
+            **super().get_extra_context(*args, **kwargs),
+            "title": "Validated Software",
+            "verbose_name_plural": "Validated Software",
+        }
+
 
 class ValidatedSoftwareLCMEditView(generic.ObjectEditView):
     """ValidatedSoftware Create view."""
 
     queryset = ValidatedSoftwareLCM.objects.all()
     model_form = ValidatedSoftwareLCMForm
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html"
```

### Comparing `nautobot_device_lifecycle_mgmt-1.1.2/pyproject.toml` & `nautobot_device_lifecycle_mgmt-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-device-lifecycle-mgmt"
-version = "v1.1.2"
+version = "v1.2.0"
 description = "Manages device lifecycles for platforms and software."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 repository = "https://github.com/nautobot/nautobot-plugin-device-lifecycle-mgmt"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -16,15 +16,15 @@
     { include = "nautobot_device_lifecycle_mgmt" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pycountry = "^22.3.5"
 matplotlib = "^3.3.4"
-nautobot = "^1.2.0"
+nautobot = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 invoke = "*"
 black = "*"
 bandit = "*"
 pylint = "*"
 pylint-django = "*"
@@ -36,14 +36,23 @@
 coverage = "*"
 django-extensions = "*"
 time-machine = "*"
 yamllint = "*"
 mysqlclient = "*"
 python-dotenv = "*"
 Markdown = "*"
+# Rendering docs to HTML
+mkdocs = "1.3.1"
+# Material for MkDocs theme
+mkdocs-material = "8.3.0"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
+mkdocstrings = "0.19"
+mkdocstrings-python = "0.7.1"
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 include = '\.pyi?$'
 exclude = '''
 (
```

