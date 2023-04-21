# Comparing `tmp/cloud-governance-1.1.90.tar.gz` & `tmp/cloud-governance-1.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-governance-1.1.90.tar", last modified: Thu Apr 20 13:20:51 2023, max compression
+gzip compressed data, was "cloud-governance-1.1.91.tar", last modified: Fri Apr 21 21:03:23 2023, max compression
```

## Comparing `cloud-governance-1.1.90.tar` & `cloud-governance-1.1.91.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-20 13:20:51.835000 cloud-governance-1.1.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.819000 cloud-governance-1.1.90/cloud_governance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.819000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.819000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.819000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/google_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.823000 cloud-governance-1.1.90/cloud_governance/common/google_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/google_drive/google_drive_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/common/jira/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/jira/jira_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/common/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/ldap/ldap_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/common/mails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/mails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/mails/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/mails/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/mails/postfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/common/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/common/tool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/main/environment_variables_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/main/es_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/main/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/policy/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_in_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/empty_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/ip_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/monthly_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/s3_inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/skipped_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/policy/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/azure/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.827000 cloud-governance-1.1.90/cloud_governance/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    41752 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.831000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:20:51.819000 cloud-governance-1.1.90/cloud_governance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 13:20:51.000000 cloud-governance-1.1.90/cloud_governance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 13:20:51.835000 cloud-governance-1.1.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-20 13:20:34.000000 cloud-governance-1.1.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/short_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/common/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/aws/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/cost_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/gcp/google_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.211200 cloud-governance-1.1.91/cloud_governance/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/jira/jira_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/ldap/ldap_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/mails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/mails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/mails/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/mails/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/mails/postfix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/common/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/common/tool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/main/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/main/environment_variables_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/main/es_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/main/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.215201 cloud-governance-1.1.91/cloud_governance/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/cost_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ebs_in_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ebs_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/empty_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/ip_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/monthly_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/nat_gateway_unused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/s3_inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/skipped_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/aws/zombie_snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/azure/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/ibm/tag_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.219201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gitleaks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:03:23.207200 cloud-governance-1.1.91/cloud_governance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 21:03:23.000000 cloud-governance-1.1.91/cloud_governance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 21:03:23.223201 cloud-governance-1.1.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-21 21:03:04.000000 cloud-governance-1.1.91/setup.py
```

### Comparing `cloud-governance-1.1.90/LICENSE` & `cloud-governance-1.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/PKG-INFO` & `cloud-governance-1.1.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.90
+Version: 1.1.91
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.90/README.md` & `cloud-governance-1.1.91/README.md`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `cloud-governance-1.1.91/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/price.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/aws/utils/utils.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/gcp/google_account.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elastic_upload.py` & `cloud-governance-1.1.91/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/google_drive/google_drive_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/google_drive/upload_to_gsheet.py` & `cloud-governance-1.1.91/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/jira/jira.py` & `cloud-governance-1.1.91/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/jira/jira_operations.py` & `cloud-governance-1.1.91/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/ldap/ldap_search.py` & `cloud-governance-1.1.91/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/logger/logger_time_stamp.py` & `cloud-governance-1.1.91/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/mails/gmail.py` & `cloud-governance-1.1.91/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/mails/mail_message.py` & `cloud-governance-1.1.91/cloud_governance/common/mails/mail_message.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/common/mails/postfix.py` & `cloud-governance-1.1.91/cloud_governance/common/mails/postfix.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/main/environment_variables.py` & `cloud-governance-1.1.91/cloud_governance/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/main/es_uploader.py` & `cloud-governance-1.1.91/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/main/main.py` & `cloud-governance-1.1.91/cloud_governance/main/main.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/cost_billing_reports.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/cost_over_usage.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_in_use.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ebs_unattached.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_idle.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_run.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ec2_stop.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/empty_roles.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/ip_unattached.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/monthly_report.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/nat_gateway_unused.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/nat_gateway_unused.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/s3_inactive.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/skipped_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_cluster_resource.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/aws/zombie_snapshots.py` & `cloud-governance-1.1.91/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/azure/cost_billing_reports.py` & `cloud-governance-1.1.91/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/gcp/cost_billing_reports.py` & `cloud-governance-1.1.91/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/ibm/cost_billing_reports.py` & `cloud-governance-1.1.91/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `cloud-governance-1.1.91/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/ibm/ibm_cost_report.py` & `cloud-governance-1.1.91/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_baremetal.py` & `cloud-governance-1.1.91/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/ibm/tag_vm.py` & `cloud-governance-1.1.91/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,21 +224,21 @@
     def __validate_existing_tag(self, tags: list):
         """
         This method validates that permanent tag exists in tags list
         @param tags:
         @return:
         """
         check_tags = ['User', 'Project', 'Manager', 'Owner', 'Email']
+        tag_count = 0
         for tag in tags:
             if tag.get('Key') in check_tags:
+                tag_count += 1
                 if tag.get('Value') == 'NA':
                     return False
-            else:
-                return False
-        return True
+        return tag_count == len(check_tags)
 
     def update_cluster_tags(self, resources: list):
         """
         This method update the Cluster instance tags and returns the updated tags list ids.
         @param resources:
         @param queue:
         @return:
@@ -253,15 +253,16 @@
                 if tags:
                     # search that not exist permanent tags in the resource
                     if not self.__validate_existing_tag(tags):
                         for tag in tags:
                             if self.cluster_prefix in tag.get('Key'):
                                 add_tags = self.__append_input_tags()
                                 cluster_name = tag.get('Key').split('/')[-1]
-                                if cluster_name in cluster_instances:
+                                user = self.ec2_operations.get_tag_value_from_tags(tags=tags, tag_name='User')
+                                if cluster_name in cluster_instances and user and user != 'NA':
                                     add_tags = self.__filter_resource_tags_by_add_tags(tags=tags, search_tags=cluster_tags[cluster_name])
                                     if add_tags:
                                         cluster_instances[cluster_name].append(instance_id)
                                     break
                                 else:
                                     username = self.get_username(start_time=item.get('LaunchTime'), resource_id=instance_id, resource_type='AWS::EC2::Instance', tags=tags)
                                     if username:
@@ -288,15 +289,15 @@
                                         add_tags.extend(self._fill_na_tags())
                                     add_tags.append({'Key': 'LaunchTime',
                                                      'Value': self.get_date_from_date_time(item.get('LaunchTime'))})
                                     add_tags = self.remove_creation_date(add_tags)
                                     add_tags = self.__filter_resource_tags_by_add_tags(tags=item.get('Tags'),
                                                                                        search_tags=add_tags)
                                     if add_tags:
-                                        cluster_instances[cluster_name] = [instance_id]
+                                        cluster_instances.setdefault(cluster_name, []).append(instance_id)
                                         cluster_tags[cluster_name] = add_tags
                                     break
         for cluster_instance_name, instance_ids in cluster_instances.items():
             if self.dry_run == 'no':
                 try:
                     self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=instance_ids, tags=cluster_tags.get(cluster_instance_name))
                     logger.info(f'Cluster :: {cluster_instance_name} count: {len(instance_ids)} :: InstanceId :: {instance_ids} :: {cluster_tags.get(cluster_instance_name)}')
```

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,7 +214,23 @@
         """
         iam_username = self.get_user_name_from_name_tag(tags=tags, resource_name=resource_name)
         if not iam_username:
             iam_username = self.get_user_name_from_name_tag(resource_name=resource_name)
             if not iam_username:
                 return self._get_username_from_cloudtrail(start_time=start_time, resource_id=resource_id, resource_type=resource_type, end_time=end_time)
         return iam_username
+
+    def validate_existing_tag(self, tags: list):
+        """
+        This method validates that permanent tag exists in tags list
+        @param tags:
+        @return:
+        """
+        check_tags = ['User', 'Project', 'Manager', 'Owner', 'Email']
+        tag_count = 0
+        if tags:
+            for tag in tags:
+                if tag.get('Key') in check_tags:
+                    tag_count += 1
+                    if tag.get('Value') == 'NA':
+                        return False
+        return tag_count == len(check_tags)
```

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,23 +63,25 @@
         if not instances_list:
             instances_list = self._get_resource_data(resource_method=self._get_instances_data)
         instances_ids = []
         for instance in instances_list:
             for item in instance:
                 instance_id = item.get('InstanceId')
                 launch_time = item.get('LaunchTime')
-                add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=item.get('Tags'))
-                if add_tags:
-                    if self.dry_run == 'no':
-                        try:
-                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[instance_id], tags=add_tags)
-                            logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
-                        except Exception as err:
-                            logger.info(err)
-                    instances_ids.append(instance_id)
+                tags = item.get('Tags')
+                if not self.validate_existing_tag(tags=tags):
+                    add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=tags)
+                    if add_tags:
+                        if self.dry_run == 'no':
+                            try:
+                                self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[instance_id], tags=add_tags)
+                                logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
+                            except Exception as err:
+                                logger.info(err)
+                        instances_ids.append(instance_id)
         logger.info(f'non_cluster_ec2 count: {len(sorted(instances_ids))} {sorted(instances_ids)}')
         return sorted(instances_ids)
 
     def update_volumes(self, volumes_data: list = None):
         """
         This method updates the tags of non-cluster volumes
         @param volumes_data:
@@ -87,45 +89,46 @@
         """
         if not volumes_data:
             volumes_data = self._get_resource_data(resource_method=self.ec2_operations.get_volumes)
         volume_ids = []
         for volume in volumes_data:
             volume_id = volume.get('VolumeId')
             tags = volume.get('Tags')
-            username = self.get_username(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume', tags=tags)
-            search_tags = []
-            if not username:
-                get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
-                search_tags.extend(get_tags)
-            else:
-                search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume', tags=tags)
+                search_tags = []
+                if not username:
+                    get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
+                    search_tags.extend(get_tags)
                 else:
-                    search_tags.extend(user_tags)
-                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
-            else:
-                search_tags.extend(self._fill_na_tags())
-                search_tags.extend(self._append_input_tags())
-                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
-            if not self.__check_name_in_tags(volume.get('Tags')):
-                tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
-            if volume_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[volume_id], tags=volume_tags)
-                        logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                volume_ids.append(volume_id)
+                    search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
+                        search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+                else:
+                    search_tags.extend(self._fill_na_tags())
+                    search_tags.extend(self._append_input_tags())
+                    search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+                if not self.__check_name_in_tags(volume.get('Tags')):
+                    tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
+                if volume_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[volume_id], tags=volume_tags)
+                            logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    volume_ids.append(volume_id)
         logger.info(f'non_cluster_volumes count: {len(sorted(volume_ids))} {sorted(volume_ids)}')
         return sorted(volume_ids)
 
     def update_snapshots(self, snapshots: list = None):
         """
         This method updates the tags of  non-cluster snapshots
         @param snapshots:
@@ -133,57 +136,58 @@
         """
         if not snapshots:
             snapshots = self._get_resource_data(resource_method=self.ec2_operations.get_snapshots)
         snapshot_ids = []
         for snapshot in snapshots:
             snapshot_id = snapshot.get('SnapshotId')
             tags = snapshot.get('Tags')
-            username = self.get_username(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags)
-            if 'vm_import_image' in username:
-                start_time = snapshot.get('StartTime') + timedelta(seconds=5)
-                end_time = start_time + timedelta(minutes=30)
-                assume_username = self.get_username(start_time=start_time, resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags, end_time=end_time)
-                if assume_username:
-                    username = assume_username
-            search_tags = []
-            if not username:
-                if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
-                    image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
-                    if not username:
-                        instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
-                        instances = self._get_instances_data(instance_id)
-                        if instances:
-                            for item in instances:
-                                if item.get('InstanceId') == instance_id:
-                                    item_tags, username = self._get_tags_from_instance_item(instance_item=item)
-            else:
-                search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags)
+                if 'vm_import_image' in username:
+                    start_time = snapshot.get('StartTime') + timedelta(seconds=5)
+                    end_time = start_time + timedelta(minutes=30)
+                    assume_username = self.get_username(start_time=start_time, resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags, end_time=end_time)
+                    if assume_username:
+                        username = assume_username
+                search_tags = []
+                if not username:
+                    if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
+                        image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
+                        if not username:
+                            instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
+                            instances = self._get_instances_data(instance_id)
+                            if instances:
+                                for item in instances:
+                                    if item.get('InstanceId') == instance_id:
+                                        item_tags, username = self._get_tags_from_instance_item(instance_item=item)
                 else:
-                    search_tags.extend(user_tags)
-            else:
-                search_tags.extend(self._fill_na_tags())
-                search_tags.extend(self._append_input_tags())
-            if not self.__check_name_in_tags(snapshot.get('Tags')):
-                tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
-            snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
-            if snapshot_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[snapshot_id], tags=snapshot_tags)
-                        logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                snapshot_ids.append(snapshot_id)
+                    search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
+                else:
+                    search_tags.extend(self._fill_na_tags())
+                    search_tags.extend(self._append_input_tags())
+                if not self.__check_name_in_tags(snapshot.get('Tags')):
+                    tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
+                snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
+                if snapshot_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[snapshot_id], tags=snapshot_tags)
+                            logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    snapshot_ids.append(snapshot_id)
         logger.info(f'non_cluster_snapshot count: {len(sorted(snapshot_ids))} {sorted(snapshot_ids)}')
         return sorted(snapshot_ids)
 
     def update_ami(self, images: list = None):
         """
         This method update the tags of non-cluster Amazon Machine Images
         @param images:
@@ -194,34 +198,35 @@
             _, images = self.ec2_operations.scan_cluster_non_cluster_resources(images)
         image_ids = []
         for image in images:
             image_id = image.get('ImageId')
             tags = image.get('Tags')
             image_name = image.get('Name')
             start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
-            username = self.get_username(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami', tags=tags, resource_name=image_name)
-            search_tags = []
-            search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami', tags=tags, resource_name=image_name)
+                search_tags = []
+                search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
                 else:
-                    search_tags.extend(user_tags)
-            else:
-                search_tags.extend(self._fill_na_tags())
-            if not self.__check_name_in_tags(image.get('Tags')):
-                tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
-            image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
-            if image_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[image_id], tags=image_tags)
-                        logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                image_ids.append(image_id)
+                    search_tags.extend(self._fill_na_tags())
+                if not self.__check_name_in_tags(image.get('Tags')):
+                    tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
+                image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
+                if image_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[image_id], tags=image_tags)
+                            logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    image_ids.append(image_id)
         logger.info(f'non_cluster_amis count: {len(sorted(image_ids))} {sorted(image_ids)}')
         return sorted(image_ids)
```

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `cloud-governance-1.1.91/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance.egg-info/PKG-INFO` & `cloud-governance-1.1.91/cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.90
+Version: 1.1.91
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.90/cloud_governance.egg-info/SOURCES.txt` & `cloud-governance-1.1.91/cloud_governance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/cloud_governance.egg-info/requires.txt` & `cloud-governance-1.1.91/cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.90/setup.py` & `cloud-governance-1.1.91/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.90'
+__version__ = '1.1.91'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

