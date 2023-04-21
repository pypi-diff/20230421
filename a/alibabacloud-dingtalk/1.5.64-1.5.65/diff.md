# Comparing `tmp/alibabacloud_dingtalk-1.5.64.tar.gz` & `tmp/alibabacloud_dingtalk-1.5.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.64.tar", last modified: Fri Apr 14 01:59:04 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-1.5.65.tar", last modified: Fri Apr 21 01:48:01 2023, max compression
```

## Comparing `alibabacloud_dingtalk-1.5.64.tar` & `alibabacloud_dingtalk-1.5.65.tar`

### file list

```diff
@@ -1,345 +1,353 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/
--rw-r--r--   0 root         (0) root         (0)    19039 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22962 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51882 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   179168 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21344 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44730 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18586 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22436 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81490 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140148 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134106 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   288074 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40908 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63666 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177626 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   583083 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3576 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131164 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   326662 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24154 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41993 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31362 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106693 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61834 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121561 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56162 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82298 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51372 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   127231 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260294 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   382552 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18716 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44885 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15642 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32114 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194896 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   555654 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7207 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29122 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47050 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   340246 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503096 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99276 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   149418 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50064 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53792 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40488 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    66172 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   196916 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   261579 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134506 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   276268 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127432 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   192831 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   401586 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   699718 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62504 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110186 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75706 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118345 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4334 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6225 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   273442 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   424209 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140236 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   310177 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4520 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9290 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9446 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69681 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   140857 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14767 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18751 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4336 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79392 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134254 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   268744 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   381405 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12612 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76078 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83510 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   454060 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731352 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54446 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   160887 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54782 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111368 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77806 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129784 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14978 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24607 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117228 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   154147 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45940 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    51039 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    39828 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6891 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67864 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137575 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68812 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   125156 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48952 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57536 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   233262 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   399779 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16002 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9973 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   118728 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171405 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71838 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91606 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50744 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    82767 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35104 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47649 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   322628 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499096 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28634 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25101 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40406 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105120 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   173162 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   389740 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9158 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31448 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30097 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60784 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   156671 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12502 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21548 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12290 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17800 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16936 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33576 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68340 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110827 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3124 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20769 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4608 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8329 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24540 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28057 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   154430 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385214 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3485 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   416280 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   688786 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11356 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2585 2023-04-14 01:59:04.000000 alibabacloud_dingtalk-1.5.64/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/
+-rw-r--r--   0 root         (0) root         (0)    19104 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22962 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51882 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   179168 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21344 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44730 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18586 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22436 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81490 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140148 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134106 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   288351 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40908 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63666 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177626 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   583083 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131164 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   326662 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24154 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41993 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31362 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106693 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61834 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121561 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56162 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82298 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51372 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   127231 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260294 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   384057 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18716 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44885 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32114 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194896 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   555654 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29122 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47050 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   340246 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503096 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99276 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   149418 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50064 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53792 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40488 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    66172 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196916 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   261579 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134506 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   276268 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127432 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   192831 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   401586 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   699718 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62504 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110186 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75706 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118345 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   273442 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   424209 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140236 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   310177 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4520 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9290 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9446 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69681 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   140857 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14767 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18751 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4336 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79392 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134254 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   268744 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   381405 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12612 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76078 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83510 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   454060 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731352 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54446 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   160887 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54782 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111368 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77806 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129784 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14978 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24607 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117228 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   154147 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45940 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    51039 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    39828 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6891 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67864 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137575 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68812 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   125156 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48952 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57536 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25914 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    72214 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233046 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   388907 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16002 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   118728 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171405 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71838 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91606 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50744 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    82767 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35104 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47649 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   322628 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499096 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28634 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25101 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40406 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105120 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   173162 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   389740 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9158 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31448 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12420 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30097 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60784 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   156671 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21548 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12290 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17800 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16936 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33576 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68340 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110827 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20769 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8329 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24540 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28057 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   154430 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385214 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   416280 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   688786 2023-04-21 01:48:00.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11618 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-21 01:48:01.000000 alibabacloud_dingtalk-1.5.65/setup.py
```

### Comparing `alibabacloud_dingtalk-1.5.64/ChangeLog.md` & `alibabacloud_dingtalk-1.5.65/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-14 Version: 1.5.64
+- Update AddOfficialAccountFollower.
+
 2023-04-11 Version: 1.5.63
 - Update AddOfficialAccountFollower.
 
 2023-04-07 Version: 1.5.62
 - Update AddOfficialAccountFollower.
 
 2023-04-04 Version: 1.5.61
```

### Comparing `alibabacloud_dingtalk-1.5.64/LICENSE` & `alibabacloud_dingtalk-1.5.65/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/PKG-INFO` & `alibabacloud_dingtalk-1.5.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 1.5.64
+Version: 1.5.65
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.64/README-CN.md` & `alibabacloud_dingtalk-1.5.65/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/README.md` & `alibabacloud_dingtalk-1.5.65/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3278,14 +3278,15 @@
         gmt_create: int = None,
         gmt_modified: int = None,
         leave_code: str = None,
         leave_reason: str = None,
         leave_record_type: str = None,
         leave_status: str = None,
         leave_view_unit: str = None,
+        op_user_id: str = None,
         quota_id: str = None,
         record_id: str = None,
         record_num_per_day: int = None,
         record_num_per_hour: int = None,
         start_time: int = None,
         user_id: str = None,
     ):
@@ -3303,14 +3304,16 @@
         self.leave_reason = leave_reason
         # 假期记录类型。
         self.leave_record_type = leave_record_type
         # 请假状态。
         self.leave_status = leave_status
         # 显示单位。
         self.leave_view_unit = leave_view_unit
+        # 操作人userId。
+        self.op_user_id = op_user_id
         # 额度唯一标识。
         self.quota_id = quota_id
         # 假期记录唯一标识。
         self.record_id = record_id
         # 以天计算的消费额度。
         self.record_num_per_day = record_num_per_day
         # 以小时计算的消费额度。
@@ -3343,14 +3346,16 @@
             result['leaveReason'] = self.leave_reason
         if self.leave_record_type is not None:
             result['leaveRecordType'] = self.leave_record_type
         if self.leave_status is not None:
             result['leaveStatus'] = self.leave_status
         if self.leave_view_unit is not None:
             result['leaveViewUnit'] = self.leave_view_unit
+        if self.op_user_id is not None:
+            result['opUserId'] = self.op_user_id
         if self.quota_id is not None:
             result['quotaId'] = self.quota_id
         if self.record_id is not None:
             result['recordId'] = self.record_id
         if self.record_num_per_day is not None:
             result['recordNumPerDay'] = self.record_num_per_day
         if self.record_num_per_hour is not None:
@@ -3377,14 +3382,16 @@
             self.leave_reason = m.get('leaveReason')
         if m.get('leaveRecordType') is not None:
             self.leave_record_type = m.get('leaveRecordType')
         if m.get('leaveStatus') is not None:
             self.leave_status = m.get('leaveStatus')
         if m.get('leaveViewUnit') is not None:
             self.leave_view_unit = m.get('leaveViewUnit')
+        if m.get('opUserId') is not None:
+            self.op_user_id = m.get('opUserId')
         if m.get('quotaId') is not None:
             self.quota_id = m.get('quotaId')
         if m.get('recordId') is not None:
             self.record_id = m.get('recordId')
         if m.get('recordNumPerDay') is not None:
             self.record_num_per_day = m.get('recordNumPerDay')
         if m.get('recordNumPerHour') is not None:
```

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2949,30 +2949,65 @@
         if m.get('label') is not None:
             self.label = m.get('label')
         if m.get('value') is not None:
             self.value = m.get('value')
         return self
 
 
+class GetCardInfoResponseBodyExtensionCardContactInfoWorkPhone(TeaModel):
+    def __init__(
+        self,
+        label: str = None,
+        value: str = None,
+    ):
+        self.label = label
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label is not None:
+            result['label'] = self.label
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('label') is not None:
+            self.label = m.get('label')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
 class GetCardInfoResponseBodyExtensionCardContactInfo(TeaModel):
     def __init__(
         self,
         address: List[GetCardInfoResponseBodyExtensionCardContactInfoAddress] = None,
         email: List[GetCardInfoResponseBodyExtensionCardContactInfoEmail] = None,
         link: List[GetCardInfoResponseBodyExtensionCardContactInfoLink] = None,
         telephone: List[GetCardInfoResponseBodyExtensionCardContactInfoTelephone] = None,
+        work_phone: List[GetCardInfoResponseBodyExtensionCardContactInfoWorkPhone] = None,
     ):
         # 地址
         self.address = address
         # 邮箱
         self.email = email
         # 微信
         self.link = link
         # 电话
         self.telephone = telephone
+        self.work_phone = work_phone
 
     def validate(self):
         if self.address:
             for k in self.address:
                 if k:
                     k.validate()
         if self.email:
@@ -2983,14 +3018,18 @@
             for k in self.link:
                 if k:
                     k.validate()
         if self.telephone:
             for k in self.telephone:
                 if k:
                     k.validate()
+        if self.work_phone:
+            for k in self.work_phone:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -3006,14 +3045,18 @@
         if self.link is not None:
             for k in self.link:
                 result['link'].append(k.to_map() if k else None)
         result['telephone'] = []
         if self.telephone is not None:
             for k in self.telephone:
                 result['telephone'].append(k.to_map() if k else None)
+        result['workPhone'] = []
+        if self.work_phone is not None:
+            for k in self.work_phone:
+                result['workPhone'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.address = []
         if m.get('address') is not None:
             for k in m.get('address'):
@@ -3030,14 +3073,19 @@
                 temp_model = GetCardInfoResponseBodyExtensionCardContactInfoLink()
                 self.link.append(temp_model.from_map(k))
         self.telephone = []
         if m.get('telephone') is not None:
             for k in m.get('telephone'):
                 temp_model = GetCardInfoResponseBodyExtensionCardContactInfoTelephone()
                 self.telephone.append(temp_model.from_map(k))
+        self.work_phone = []
+        if m.get('workPhone') is not None:
+            for k in m.get('workPhone'):
+                temp_model = GetCardInfoResponseBodyExtensionCardContactInfoWorkPhone()
+                self.work_phone.append(temp_model.from_map(k))
         return self
 
 
 class GetCardInfoResponseBodyExtension(TeaModel):
     def __init__(
         self,
         card_contact_info: GetCardInfoResponseBodyExtensionCardContactInfo = None,
```

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2929,16 +2929,14 @@
         UtilClient.validate_model(request)
         user_id = OpenApiUtilClient.get_encode_param(user_id)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
-        if not UtilClient.is_unset(request.role_types):
-            query['roleTypes'] = request.role_types
         if not UtilClient.is_unset(request.tql):
             query['tql'] = request.tql
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -2961,16 +2959,14 @@
         UtilClient.validate_model(request)
         user_id = OpenApiUtilClient.get_encode_param(user_id)
         query = {}
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
-        if not UtilClient.is_unset(request.role_types):
-            query['roleTypes'] = request.role_types
         if not UtilClient.is_unset(request.tql):
             query['tql'] = request.tql
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
```

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1778,15 +1778,15 @@
 class CreateProjectCustomfieldStatusRequestValue(TeaModel):
     def __init__(
         self,
         fieldvalue_id: str = None,
         meta_string: str = None,
         title: str = None,
     ):
-        # 字段值id。
+        # 字段值id,当自定义字段是work类型该id表示文件id，当自定义字段是commongroup类型该id表示分类id，其他类型无意义。
         self.fieldvalue_id = fieldvalue_id
         # 字段值元信息(json格式)。
         self.meta_string = meta_string
         # 字段值渲染值。
         self.title = title
 
     def validate(self):
@@ -8914,24 +8914,21 @@
 
 
 class SearchUserTaskRequest(TeaModel):
     def __init__(
         self,
         max_results: int = None,
         next_token: str = None,
-        role_types: str = None,
         tql: str = None,
     ):
-        # 每页返回最大数量。默认10，最大100。
+        # 每页返回最大数量。默认10，最大300。
         self.max_results = max_results
         # 分页标，从上一次请求结果中获取。
         self.next_token = next_token
-        # 用户的任务角色, creator,executor,involveMember 中的一个或多个,以 ','拼接。例如：creator,executor。
-        self.role_types = role_types
-        # tql，参考项目内的tql使用说明。
+        # 企业下任务搜索TQL语句。
         self.tql = tql
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8939,376 +8936,75 @@
             return _map
 
         result = dict()
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
-        if self.role_types is not None:
-            result['roleTypes'] = self.role_types
         if self.tql is not None:
             result['tql'] = self.tql
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
-        if m.get('roleTypes') is not None:
-            self.role_types = m.get('roleTypes')
         if m.get('tql') is not None:
             self.tql = m.get('tql')
         return self
 
 
-class SearchUserTaskResponseBodyResultCustomfieldsValue(TeaModel):
-    def __init__(
-        self,
-        fieldvalue_id: str = None,
-        meta_string: str = None,
-        title: str = None,
-    ):
-        # 字段值ID。
-        self.fieldvalue_id = fieldvalue_id
-        # 字段值元属性。
-        self.meta_string = meta_string
-        # 字段值内容。
-        self.title = title
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.fieldvalue_id is not None:
-            result['fieldvalueId'] = self.fieldvalue_id
-        if self.meta_string is not None:
-            result['metaString'] = self.meta_string
-        if self.title is not None:
-            result['title'] = self.title
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('fieldvalueId') is not None:
-            self.fieldvalue_id = m.get('fieldvalueId')
-        if m.get('metaString') is not None:
-            self.meta_string = m.get('metaString')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        return self
-
-
-class SearchUserTaskResponseBodyResultCustomfields(TeaModel):
-    def __init__(
-        self,
-        customfield_id: str = None,
-        type: str = None,
-        value: List[SearchUserTaskResponseBodyResultCustomfieldsValue] = None,
-    ):
-        # 自定义字段ID。
-        self.customfield_id = customfield_id
-        # 自定义字段类型。
-        self.type = type
-        # 字段值集合。
-        self.value = value
-
-    def validate(self):
-        if self.value:
-            for k in self.value:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.customfield_id is not None:
-            result['customfieldId'] = self.customfield_id
-        if self.type is not None:
-            result['type'] = self.type
-        result['value'] = []
-        if self.value is not None:
-            for k in self.value:
-                result['value'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('customfieldId') is not None:
-            self.customfield_id = m.get('customfieldId')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        self.value = []
-        if m.get('value') is not None:
-            for k in m.get('value'):
-                temp_model = SearchUserTaskResponseBodyResultCustomfieldsValue()
-                self.value.append(temp_model.from_map(k))
-        return self
-
-
-class SearchUserTaskResponseBodyResult(TeaModel):
-    def __init__(
-        self,
-        accomplish_time: str = None,
-        ancestor_ids: List[str] = None,
-        content: str = None,
-        created: str = None,
-        creator_id: str = None,
-        customfields: List[SearchUserTaskResponseBodyResultCustomfields] = None,
-        due_date: str = None,
-        executor_id: str = None,
-        involve_members: List[str] = None,
-        is_archived: bool = None,
-        is_done: bool = None,
-        note: str = None,
-        parent_task_id: str = None,
-        priority: int = None,
-        project_id: str = None,
-        recurrence: List[str] = None,
-        scenariofieldconfig_id: str = None,
-        sprint_id: str = None,
-        stage_id: str = None,
-        start_date: str = None,
-        story_point: str = None,
-        tag_ids: List[str] = None,
-        task_id: str = None,
-        task_list_id: str = None,
-        unique_id: str = None,
-        updated: str = None,
-        visible: str = None,
-    ):
-        # 任务完成时间(UTC)。
-        self.accomplish_time = accomplish_time
-        # 祖先任务ID列表。
-        self.ancestor_ids = ancestor_ids
-        # 任务标题。
-        self.content = content
-        # 创建时间(UTC)。
-        self.created = created
-        # 创建人ID。
-        self.creator_id = creator_id
-        # 自定义字段值集合。
-        self.customfields = customfields
-        # 任务截止时间(UTC)。
-        self.due_date = due_date
-        # 执行人ID。
-        self.executor_id = executor_id
-        # 参与者ID集合。
-        self.involve_members = involve_members
-        # 是否任务放入回收站。
-        self.is_archived = is_archived
-        # 是否任务已完成。
-        self.is_done = is_done
-        # 任务备注。
-        self.note = note
-        # 父任务ID。
-        self.parent_task_id = parent_task_id
-        # 任务优先级。
-        self.priority = priority
-        # 项目ID。
-        self.project_id = project_id
-        # 重复规则列表。
-        self.recurrence = recurrence
-        # 任务类型ID。
-        self.scenariofieldconfig_id = scenariofieldconfig_id
-        # 迭代ID。
-        self.sprint_id = sprint_id
-        # 任务列ID。
-        self.stage_id = stage_id
-        # 任务开始时间(UTC)。
-        self.start_date = start_date
-        # StoryPoint。
-        self.story_point = story_point
-        # 标签ID集合。
-        self.tag_ids = tag_ids
-        # 任务状态ID。
-        self.task_id = task_id
-        # 任务列表ID。
-        self.task_list_id = task_list_id
-        # 任务数字ID。
-        self.unique_id = unique_id
-        # 更新时间(UTC)。
-        self.updated = updated
-        # 任务隐私性，'involves'表达仅参与者可见; 'members'表达项目成员可见。
-        self.visible = visible
-
-    def validate(self):
-        if self.customfields:
-            for k in self.customfields:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.accomplish_time is not None:
-            result['accomplishTime'] = self.accomplish_time
-        if self.ancestor_ids is not None:
-            result['ancestorIds'] = self.ancestor_ids
-        if self.content is not None:
-            result['content'] = self.content
-        if self.created is not None:
-            result['created'] = self.created
-        if self.creator_id is not None:
-            result['creatorId'] = self.creator_id
-        result['customfields'] = []
-        if self.customfields is not None:
-            for k in self.customfields:
-                result['customfields'].append(k.to_map() if k else None)
-        if self.due_date is not None:
-            result['dueDate'] = self.due_date
-        if self.executor_id is not None:
-            result['executorId'] = self.executor_id
-        if self.involve_members is not None:
-            result['involveMembers'] = self.involve_members
-        if self.is_archived is not None:
-            result['isArchived'] = self.is_archived
-        if self.is_done is not None:
-            result['isDone'] = self.is_done
-        if self.note is not None:
-            result['note'] = self.note
-        if self.parent_task_id is not None:
-            result['parentTaskId'] = self.parent_task_id
-        if self.priority is not None:
-            result['priority'] = self.priority
-        if self.project_id is not None:
-            result['projectId'] = self.project_id
-        if self.recurrence is not None:
-            result['recurrence'] = self.recurrence
-        if self.scenariofieldconfig_id is not None:
-            result['scenariofieldconfigId'] = self.scenariofieldconfig_id
-        if self.sprint_id is not None:
-            result['sprintId'] = self.sprint_id
-        if self.stage_id is not None:
-            result['stageId'] = self.stage_id
-        if self.start_date is not None:
-            result['startDate'] = self.start_date
-        if self.story_point is not None:
-            result['storyPoint'] = self.story_point
-        if self.tag_ids is not None:
-            result['tagIds'] = self.tag_ids
-        if self.task_id is not None:
-            result['taskId'] = self.task_id
-        if self.task_list_id is not None:
-            result['taskListId'] = self.task_list_id
-        if self.unique_id is not None:
-            result['uniqueId'] = self.unique_id
-        if self.updated is not None:
-            result['updated'] = self.updated
-        if self.visible is not None:
-            result['visible'] = self.visible
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('accomplishTime') is not None:
-            self.accomplish_time = m.get('accomplishTime')
-        if m.get('ancestorIds') is not None:
-            self.ancestor_ids = m.get('ancestorIds')
-        if m.get('content') is not None:
-            self.content = m.get('content')
-        if m.get('created') is not None:
-            self.created = m.get('created')
-        if m.get('creatorId') is not None:
-            self.creator_id = m.get('creatorId')
-        self.customfields = []
-        if m.get('customfields') is not None:
-            for k in m.get('customfields'):
-                temp_model = SearchUserTaskResponseBodyResultCustomfields()
-                self.customfields.append(temp_model.from_map(k))
-        if m.get('dueDate') is not None:
-            self.due_date = m.get('dueDate')
-        if m.get('executorId') is not None:
-            self.executor_id = m.get('executorId')
-        if m.get('involveMembers') is not None:
-            self.involve_members = m.get('involveMembers')
-        if m.get('isArchived') is not None:
-            self.is_archived = m.get('isArchived')
-        if m.get('isDone') is not None:
-            self.is_done = m.get('isDone')
-        if m.get('note') is not None:
-            self.note = m.get('note')
-        if m.get('parentTaskId') is not None:
-            self.parent_task_id = m.get('parentTaskId')
-        if m.get('priority') is not None:
-            self.priority = m.get('priority')
-        if m.get('projectId') is not None:
-            self.project_id = m.get('projectId')
-        if m.get('recurrence') is not None:
-            self.recurrence = m.get('recurrence')
-        if m.get('scenariofieldconfigId') is not None:
-            self.scenariofieldconfig_id = m.get('scenariofieldconfigId')
-        if m.get('sprintId') is not None:
-            self.sprint_id = m.get('sprintId')
-        if m.get('stageId') is not None:
-            self.stage_id = m.get('stageId')
-        if m.get('startDate') is not None:
-            self.start_date = m.get('startDate')
-        if m.get('storyPoint') is not None:
-            self.story_point = m.get('storyPoint')
-        if m.get('tagIds') is not None:
-            self.tag_ids = m.get('tagIds')
-        if m.get('taskId') is not None:
-            self.task_id = m.get('taskId')
-        if m.get('taskListId') is not None:
-            self.task_list_id = m.get('taskListId')
-        if m.get('uniqueId') is not None:
-            self.unique_id = m.get('uniqueId')
-        if m.get('updated') is not None:
-            self.updated = m.get('updated')
-        if m.get('visible') is not None:
-            self.visible = m.get('visible')
-        return self
-
-
 class SearchUserTaskResponseBody(TeaModel):
     def __init__(
         self,
-        result: List[SearchUserTaskResponseBodyResult] = None,
+        next_token: str = None,
+        request_id: str = None,
+        result: List[str] = None,
+        total_size: int = None,
     ):
-        # 任务详情集合。
+        # 分页标，供分页使用，下一页token。
+        self.next_token = next_token
+        # 请求 ID，请求异常时可提供此 ID，进行问题排查。
+        self.request_id = request_id
+        # 任务ID列表。
         self.result = result
+        # 任务总数。
+        self.total_size = total_size
 
     def validate(self):
-        if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['result'] = []
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
         if self.result is not None:
-            for k in self.result:
-                result['result'].append(k.to_map() if k else None)
+            result['result'] = self.result
+        if self.total_size is not None:
+            result['totalSize'] = self.total_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.result = []
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
         if m.get('result') is not None:
-            for k in m.get('result'):
-                temp_model = SearchUserTaskResponseBodyResult()
-                self.result.append(temp_model.from_map(k))
+            self.result = m.get('result')
+        if m.get('totalSize') is not None:
+            self.total_size = m.get('totalSize')
         return self
 
 
 class SearchUserTaskResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -12349,15 +12045,15 @@
 
 class UpdateTaskPriorityResponseBodyResult(TeaModel):
     def __init__(
         self,
         priority: int = None,
         updated: str = None,
     ):
-        # 优先级。
+        # 优先级，默认的优先级包含：-10、0、1、2，含义分别为较低、普通、紧急、非常紧急。
         self.priority = priority
         # 更新时间。
         self.updated = updated
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 1.5.64
+Version: 1.5.65
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-1.5.64/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-1.5.65/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,17 @@
 alibabacloud_dingtalk/exclusive_1_0/models.py
 alibabacloud_dingtalk/finance_1_0/__init__.py
 alibabacloud_dingtalk/finance_1_0/client.py
 alibabacloud_dingtalk/finance_1_0/models.py
 alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
 alibabacloud_dingtalk/flashmeeting_1_0/client.py
 alibabacloud_dingtalk/flashmeeting_1_0/models.py
+alibabacloud_dingtalk/gateway_1_0/__init__.py
+alibabacloud_dingtalk/gateway_1_0/client.py
+alibabacloud_dingtalk/gateway_1_0/models.py
 alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
 alibabacloud_dingtalk/group_blackboard_1_0/client.py
 alibabacloud_dingtalk/group_blackboard_1_0/models.py
 alibabacloud_dingtalk/h3yun_1_0/__init__.py
 alibabacloud_dingtalk/h3yun_1_0/client.py
 alibabacloud_dingtalk/h3yun_1_0/models.py
 alibabacloud_dingtalk/h5package_1_0/__init__.py
@@ -175,14 +178,17 @@
 alibabacloud_dingtalk/okr_1_0/models.py
 alibabacloud_dingtalk/org_culture_1_0/__init__.py
 alibabacloud_dingtalk/org_culture_1_0/client.py
 alibabacloud_dingtalk/org_culture_1_0/models.py
 alibabacloud_dingtalk/package_1_0/__init__.py
 alibabacloud_dingtalk/package_1_0/client.py
 alibabacloud_dingtalk/package_1_0/models.py
+alibabacloud_dingtalk/pedia_1_0/__init__.py
+alibabacloud_dingtalk/pedia_1_0/client.py
+alibabacloud_dingtalk/pedia_1_0/models.py
 alibabacloud_dingtalk/project_1_0/__init__.py
 alibabacloud_dingtalk/project_1_0/client.py
 alibabacloud_dingtalk/project_1_0/models.py
 alibabacloud_dingtalk/project_integration_1_0/__init__.py
 alibabacloud_dingtalk/project_integration_1_0/client.py
 alibabacloud_dingtalk/project_integration_1_0/models.py
 alibabacloud_dingtalk/rcs_call_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-1.5.64/setup.py` & `alibabacloud_dingtalk-1.5.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 14/04/2023
+Created on 21/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

