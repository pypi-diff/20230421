# Comparing `tmp/cakemail-openapi-1.9.0.tar.gz` & `tmp/cakemail-openapi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cakemail-openapi-1.9.0.tar", last modified: Wed Dec 22 14:15:42 2021, max compression
+gzip compressed data, was "cakemail-openapi-1.9.1.tar", last modified: Wed Dec 22 14:25:17 2021, max compression
```

## Comparing `cakemail-openapi-1.9.0.tar` & `cakemail-openapi-1.9.1.tar`

### file list

```diff
@@ -1,48 +1,350 @@
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:15:42.415899 cakemail-openapi-1.9.0/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      247 2021-12-22 14:15:42.415899 cakemail-openapi-1.9.0/PKG-INFO
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      393 2020-10-09 12:51:21.000000 cakemail-openapi-1.9.0/README.md
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:15:42.412899 cakemail-openapi-1.9.0/cakemail_openapi/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      820 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/__init__.py
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:15:42.415899 cakemail-openapi-1.9.0/cakemail_openapi/api/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      220 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/__init__.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9536 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/account_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    46087 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/action_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    80218 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/campaign_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    15212 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/campaign_blueprint_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    48317 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/contact_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    22306 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/custom_attribute_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    14358 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/domain_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    25322 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/form_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5556 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/links_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    39734 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/list_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    30282 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/log_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5750 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/logo_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    37950 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/report_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    28111 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/segment_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    34478 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/sender_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    43950 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/sub_account_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    15915 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/suppressed_email_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    15032 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/system_email_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    30266 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/template_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    11282 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/token_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5624 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/transactional_email_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    65891 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/user_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    29747 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/webhook_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    48103 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/workflow_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    20871 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api/workflow_blueprint_api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    37604 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/api_client.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    16566 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/configuration.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5126 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/exceptions.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    81950 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/model_utils.py
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:15:42.415899 cakemail-openapi-1.9.0/cakemail_openapi/models/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    22510 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/models/__init__.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    14252 2021-12-22 14:14:24.000000 cakemail-openapi-1.9.0/cakemail_openapi/rest.py
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:15:42.413899 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      247 2021-12-22 14:15:42.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/PKG-INFO
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1447 2021-12-22 14:15:42.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-12-22 14:15:42.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2020-09-30 13:55:19.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/not-zip-safe
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       36 2021-12-22 14:15:42.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/requires.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       17 2021-12-22 14:15:42.000000 cakemail-openapi-1.9.0/cakemail_openapi.egg-info/top_level.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       38 2021-12-22 14:15:42.415899 cakemail-openapi-1.9.0/setup.cfg
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      608 2021-12-22 14:11:21.000000 cakemail-openapi-1.9.0/setup.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:25:17.309519 cakemail-openapi-1.9.1/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      247 2021-12-22 14:25:17.309519 cakemail-openapi-1.9.1/PKG-INFO
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      393 2020-11-23 12:48:51.000000 cakemail-openapi-1.9.1/README.md
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:25:17.286519 cakemail-openapi-1.9.1/cakemail_openapi/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    25070 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/__init__.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:25:17.289519 cakemail-openapi-1.9.1/cakemail_openapi/api/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1560 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/__init__.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10349 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/account_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    56305 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/action_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    94470 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/campaign_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    16956 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/campaign_blueprint_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    60793 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/contact_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    26934 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/custom_attribute_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    15778 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/domain_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    29151 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/form_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6005 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/links_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    46397 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/list_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    39763 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/log_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6325 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/logo_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    48424 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/report_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    34837 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/segment_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    39615 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/sender_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    50830 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/sub_account_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    17735 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/suppressed_email_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    17134 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/system_email_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    34834 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/template_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12187 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/token_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6168 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/transactional_email_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    75999 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/user_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    34005 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/webhook_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    56989 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/workflow_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    23718 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api/workflow_blueprint_api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    26287 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/api_client.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12875 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/configuration.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3822 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/exceptions.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:25:17.309519 cakemail-openapi-1.9.1/cakemail_openapi/models/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    23147 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/__init__.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5018 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/accept_list_policy_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    14922 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3769 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_owner.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3419 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_owner_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10017 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_owner_user.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3521 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    17962 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_stat_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3561 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3078 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10250 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/account_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4450 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/accounts_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7159 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9557 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_blueprint.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2984 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_condition.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7801 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3612 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_default_email_settings.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4424 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_email_blueprint_settings.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5126 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_email_settings.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7755 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_log_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4459 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_logs_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10418 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    21565 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_stat_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3550 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9865 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4790 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_tracking.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2817 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/action_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4435 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/actions_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4902 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/activate_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4309 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/additional_email_header.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8512 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/address.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6704 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/address_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4661 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/api_schemas_requests_lists_webhook.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8506 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/api_services_webhooks_schemas_webhook.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4866 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/archive_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4798 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/archive_list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5710 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/archive_webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4527 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/audience.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4693 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/audience_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4184 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/audience_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4669 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/bad_request_message.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6533 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/body_create_token_token_post.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4518 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/body_refresh_token_token_put.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3960 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/browser_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3463 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_blueprint_id.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3604 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_blueprint_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8521 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_blueprint_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4600 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_blueprints_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9594 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10615 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_content_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    16230 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7774 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_link_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4579 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_links_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7810 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_log_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4489 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_logs_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3532 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    28181 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_stat_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3572 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3067 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    13236 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2906 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaign_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4465 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/campaigns_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4870 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/cancel_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4481 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/change_password.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3633 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/confirm_account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6326 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/confirm_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3959 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/confirm_sender.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4127 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/confirm_sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5616 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/confirm_user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4301 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/contact.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9076 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/contact_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3521 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/contact_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2913 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/contact_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4441 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/contacts_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2869 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/content_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2901 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/content_type_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    10755 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6980 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5592 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5736 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_attribute_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7346 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_campaign.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5652 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5474 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_contact_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4686 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_custom_attribute.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8499 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_form.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5556 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_form_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4913 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5628 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_segment_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5114 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_sender.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5604 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4314 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_suppressed_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5556 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6260 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_webhook.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4336 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5640 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/create_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4320 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attribute.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4100 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attribute_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3609 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attribute_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3000 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attribute_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4631 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attributes_data_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4561 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/custom_attributes_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4974 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/deactivate_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4813 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5592 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4830 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4813 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_contact_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4985 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_custom_attribute_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4762 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_form_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4762 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4813 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_segment_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4796 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4314 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_suppressed_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4830 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_template_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4762 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5640 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/delete_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2892 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/device_family_enum.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4536 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/device_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4381 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/domain_instruction_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5549 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/domains.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5908 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/domains_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4642 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/domains_instruction_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3521 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/domains_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2908 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/double_opt_in.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7617 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6903 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12842 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_log_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4444 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_logs_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7898 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_stat_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3557 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5260 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/email_tracking.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4141 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/encoding.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4200 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/encoding_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4562 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/event_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3832 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/event_type_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4653 2021-12-22 14:23:02.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/forbidden_message.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3502 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/forgot_my_password.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4830 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4076 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_content_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12867 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6782 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_redirections.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5281 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_redirections_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3488 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2853 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4040 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/form_urls_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4396 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/forms_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3522 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/get_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3544 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/get_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3607 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/http_bad_request_error.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3596 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/http_forbidden_error.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3629 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/http_unauthorized_error.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3445 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/http_validation_error.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4421 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/import_contact_data.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4324 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/import_contacts.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6265 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/import_contacts_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3272 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/languages.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5038 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/link_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3639 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/link_info_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3532 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/link_info_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4396 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/links_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6666 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    11144 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9597 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_log_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4429 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_logs_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5466 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_pages_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5281 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_redirections_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3488 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3964 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    14206 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_stat_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3528 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_stats_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7605 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3388 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_webhook_action.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4056 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4531 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_webhooks_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4492 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/list_workflows_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4405 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/lists_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3725 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/lock_workflow.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5102 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/lock_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2985 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/log_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4056 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/operating_system_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4514 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/pagination.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2854 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/password_grant_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9666 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4275 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6692 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_action.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7259 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_action_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4923 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_action_email_settings.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5572 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4870 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_action_tracking.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7194 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_campaign.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8327 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_campaign_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5632 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3776 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_contact.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5608 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_contact_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3524 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_domains.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4887 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_domains_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8064 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_form.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5536 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_form_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4897 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5608 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_segment_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7793 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_self_account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5584 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4832 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_template.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6379 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_template_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5632 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_template_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6570 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_tracking.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8461 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_user.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5536 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5318 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_webhook.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5650 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6717 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_workflow.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5620 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/patch_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4946 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/put_system_emails_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2870 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/rate_limit_period.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7016 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/redirections.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2865 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/refresh_grant_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4040 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/render_campaign_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3598 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/render_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4532 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/resend_account_verification_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4952 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/resend_confirmation_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4493 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/resend_user_verification_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3558 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/resend_verification_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4381 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/reset_password_confirm.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4309 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/reset_password_confirm_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5033 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/reset_password_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3799 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/reset_user_password.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4830 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/resume_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4803 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/schedule_campaign.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4902 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/schedule_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6266 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/segment.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9493 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/segment_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3521 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/segment_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4441 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/segments_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4750 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/send_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4101 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/send_test_action.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4768 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/send_test_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4089 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/send_test_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5616 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/send_test_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3591 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/sender.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4466 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/sender_and_name.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8330 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/sender_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3510 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/sender_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4426 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/senders_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2864 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/signature_hash_function.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4261 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/signature_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3993 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suppressed_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4219 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suppressed_email_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4549 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suppressed_emails_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5697 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suspend_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4886 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suspend_campaign_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5616 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/suspend_user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5125 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/system_email_template.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3567 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/system_emails_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6250 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/system_emails_templates.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5048 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6413 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_content.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6129 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_content_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4718 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_created.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4583 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_custom_attributes.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7525 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3391 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_id.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4325 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3532 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8233 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2913 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/template_type_enum.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4465 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/templates_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2871 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/test_email_type.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6271 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/token_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6470 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/tracking.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5675 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/tracking_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5751 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/un_archive_webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4831 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unarchive_list_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4704 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unauthorized_message.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3741 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unlock_workflow.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5134 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unlock_workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4993 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unsubscribe_contact_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5777 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/unsuspend_account_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6428 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/update_list.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6064 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/update_segment.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3970 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/update_sender.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3779 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/upload_logo.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4824 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/upload_logo_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5752 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/usage_limits.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5061 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/usage_limits_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8662 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4730 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user_confirmation.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12144 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user_full_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6669 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user_info.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3488 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     8613 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/user_summary_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4405 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/users_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3606 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/validate_domains_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4935 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/validation_error.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     5142 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/webhook_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2868 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/webhook_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     6735 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4257 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_audience.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     7813 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_blueprint.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3637 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_blueprint_action_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3595 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_blueprint_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4555 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_blueprints_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4361 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_from_blueprint.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     9604 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_response.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2872 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_status.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2930 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/models/workflow_trigger.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    12356 2021-12-22 14:23:03.000000 cakemail-openapi-1.9.1/cakemail_openapi/rest.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:25:17.287519 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      247 2021-12-22 14:25:17.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)    15776 2021-12-22 14:25:17.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-12-22 14:25:17.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-02-19 14:43:40.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       36 2021-12-22 14:25:17.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/requires.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       17 2021-12-22 14:25:17.000000 cakemail-openapi-1.9.1/cakemail_openapi.egg-info/top_level.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       38 2021-12-22 14:25:17.309519 cakemail-openapi-1.9.1/setup.cfg
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      608 2021-12-22 14:25:13.000000 cakemail-openapi-1.9.1/setup.py
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/api/logo_api.py` & `cakemail-openapi-1.9.1/cakemail_openapi/api/logo_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,158 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+from __future__ import absolute_import
+
 import re  # noqa: F401
-import sys  # noqa: F401
 
-from cakemail_openapi.api_client import ApiClient, Endpoint as _Endpoint
-from cakemail_openapi.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
+# python 2 and python 3 compatibility library
+import six
+
+from cakemail_openapi.api_client import ApiClient
+from cakemail_openapi.exceptions import (  # noqa: F401
+    ApiTypeError,
+    ApiValueError
 )
-from cakemail_openapi.model.http_bad_request_error import HTTPBadRequestError
-from cakemail_openapi.model.http_validation_error import HTTPValidationError
-from cakemail_openapi.model.upload_logo import UploadLogo
-from cakemail_openapi.model.upload_logo_response import UploadLogoResponse
 
 
 class LogoApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.upload_default_logo_endpoint = _Endpoint(
-            settings={
-                'response_type': (UploadLogoResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/logos/default',
-                'operation_id': 'upload_default_logo',
-                'http_method': 'PUT',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'upload_logo',
-                    'account_id',
-                ],
-                'required': [
-                    'upload_logo',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'upload_logo':
-                        (UploadLogo,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'upload_logo': 'body',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
 
-    def upload_default_logo(
-        self,
-        upload_logo,
-        **kwargs
-    ):
+    def upload_default_logo(self, upload_logo, **kwargs):  # noqa: E501
         """Upload a default logo  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.upload_default_logo(upload_logo, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            upload_logo (UploadLogo):
+        :param async_req bool: execute request asynchronously
+        :param UploadLogo upload_logo: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: UploadLogoResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.upload_default_logo_with_http_info(upload_logo, **kwargs)  # noqa: E501
+
+    def upload_default_logo_with_http_info(self, upload_logo, **kwargs):  # noqa: E501
+        """Upload a default logo  # noqa: E501
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            UploadLogoResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.upload_default_logo_with_http_info(upload_logo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param UploadLogo upload_logo: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(UploadLogoResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['upload_logo'] = \
-            upload_logo
-        return self.upload_default_logo_endpoint.call_with_http_info(**kwargs)
 
+        local_var_params = locals()
+
+        all_params = [
+            'upload_logo',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method upload_default_logo" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'upload_logo' is set
+        if self.api_client.client_side_validation and ('upload_logo' not in local_var_params or  # noqa: E501
+                                                        local_var_params['upload_logo'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `upload_logo` when calling `upload_default_logo`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'upload_logo' in local_var_params:
+            body_params = local_var_params['upload_logo']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/logos/default', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='UploadLogoResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/api/sender_api.py` & `cakemail-openapi-1.9.1/cakemail_openapi/api/sender_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,965 +1,887 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+from __future__ import absolute_import
+
 import re  # noqa: F401
-import sys  # noqa: F401
 
-from cakemail_openapi.api_client import ApiClient, Endpoint as _Endpoint
-from cakemail_openapi.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
+# python 2 and python 3 compatibility library
+import six
+
+from cakemail_openapi.api_client import ApiClient
+from cakemail_openapi.exceptions import (  # noqa: F401
+    ApiTypeError,
+    ApiValueError
 )
-from cakemail_openapi.model.confirm_sender import ConfirmSender
-from cakemail_openapi.model.confirm_sender_response import ConfirmSenderResponse
-from cakemail_openapi.model.create_sender import CreateSender
-from cakemail_openapi.model.create_sender_response import CreateSenderResponse
-from cakemail_openapi.model.delete_sender_response import DeleteSenderResponse
-from cakemail_openapi.model.http_bad_request_error import HTTPBadRequestError
-from cakemail_openapi.model.http_validation_error import HTTPValidationError
-from cakemail_openapi.model.patch_sender_response import PatchSenderResponse
-from cakemail_openapi.model.resend_confirmation_email_response import ResendConfirmationEmailResponse
-from cakemail_openapi.model.sender_response import SenderResponse
-from cakemail_openapi.model.senders_response import SendersResponse
-from cakemail_openapi.model.update_sender import UpdateSender
 
 
 class SenderApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.confirm_sender_endpoint = _Endpoint(
-            settings={
-                'response_type': (ConfirmSenderResponse,),
-                'auth': [],
-                'endpoint_path': '/brands/default/senders/confirm-email',
-                'operation_id': 'confirm_sender',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'confirm_sender',
-                ],
-                'required': [
-                    'confirm_sender',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'confirm_sender':
-                        (ConfirmSender,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'confirm_sender': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.create_sender_endpoint = _Endpoint(
-            settings={
-                'response_type': (CreateSenderResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders',
-                'operation_id': 'create_sender',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'create_sender',
-                    'account_id',
-                ],
-                'required': [
-                    'create_sender',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'create_sender':
-                        (CreateSender,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'create_sender': 'body',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.delete_sender_endpoint = _Endpoint(
-            settings={
-                'response_type': (DeleteSenderResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders/{sender_id}',
-                'operation_id': 'delete_sender',
-                'http_method': 'DELETE',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sender_id',
-                    'account_id',
-                ],
-                'required': [
-                    'sender_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sender_id':
-                        (str,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'sender_id': 'sender_id',
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'sender_id': 'path',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.get_sender_endpoint = _Endpoint(
-            settings={
-                'response_type': (SenderResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders/{sender_id}',
-                'operation_id': 'get_sender',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sender_id',
-                    'account_id',
-                ],
-                'required': [
-                    'sender_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sender_id':
-                        (str,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'sender_id': 'sender_id',
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'sender_id': 'path',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.list_senders_endpoint = _Endpoint(
-            settings={
-                'response_type': (SendersResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders',
-                'operation_id': 'list_senders',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'page',
-                    'per_page',
-                    'account_id',
-                    'with_count',
-                    'sort',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'page',
-                    'per_page',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('page',): {
-
-                        'inclusive_minimum': 1,
-                    },
-                    ('per_page',): {
-
-                        'inclusive_minimum': 1,
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'page':
-                        (int,),
-                    'per_page':
-                        (int,),
-                    'account_id':
-                        (int,),
-                    'with_count':
-                        (bool,),
-                    'sort':
-                        (str,),
-                },
-                'attribute_map': {
-                    'page': 'page',
-                    'per_page': 'per_page',
-                    'account_id': 'account_id',
-                    'with_count': 'with_count',
-                    'sort': 'sort',
-                },
-                'location_map': {
-                    'page': 'query',
-                    'per_page': 'query',
-                    'account_id': 'query',
-                    'with_count': 'query',
-                    'sort': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-        self.patch_sender_endpoint = _Endpoint(
-            settings={
-                'response_type': (PatchSenderResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders/{sender_id}',
-                'operation_id': 'patch_sender',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sender_id',
-                    'update_sender',
-                    'account_id',
-                ],
-                'required': [
-                    'sender_id',
-                    'update_sender',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sender_id':
-                        (str,),
-                    'update_sender':
-                        (UpdateSender,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'sender_id': 'sender_id',
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'sender_id': 'path',
-                    'update_sender': 'body',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.resend_confirmation_email_endpoint = _Endpoint(
-            settings={
-                'response_type': (ResendConfirmationEmailResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/senders/{sender_id}/resend-confirmation-email',
-                'operation_id': 'resend_confirmation_email',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sender_id',
-                    'account_id',
-                ],
-                'required': [
-                    'sender_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sender_id':
-                        (str,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'sender_id': 'sender_id',
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'sender_id': 'path',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
 
-    def confirm_sender(
-        self,
-        confirm_sender,
-        **kwargs
-    ):
+    def confirm_sender(self, confirm_sender, **kwargs):  # noqa: E501
         """Confirm a sender  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.confirm_sender(confirm_sender, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            confirm_sender (ConfirmSender):
+        :param async_req bool: execute request asynchronously
+        :param ConfirmSender confirm_sender: (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ConfirmSenderResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.confirm_sender_with_http_info(confirm_sender, **kwargs)  # noqa: E501
+
+    def confirm_sender_with_http_info(self, confirm_sender, **kwargs):  # noqa: E501
+        """Confirm a sender  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.confirm_sender_with_http_info(confirm_sender, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            ConfirmSenderResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param ConfirmSender confirm_sender: (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ConfirmSenderResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['confirm_sender'] = \
-            confirm_sender
-        return self.confirm_sender_endpoint.call_with_http_info(**kwargs)
-
-    def create_sender(
-        self,
-        create_sender,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'confirm_sender'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method confirm_sender" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'confirm_sender' is set
+        if self.api_client.client_side_validation and ('confirm_sender' not in local_var_params or  # noqa: E501
+                                                        local_var_params['confirm_sender'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `confirm_sender` when calling `confirm_sender`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'confirm_sender' in local_var_params:
+            body_params = local_var_params['confirm_sender']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders/confirm-email', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ConfirmSenderResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def create_sender(self, create_sender, **kwargs):  # noqa: E501
         """Add a sender  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.create_sender(create_sender, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            create_sender (CreateSender):
+        :param async_req bool: execute request asynchronously
+        :param CreateSender create_sender: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: CreateSenderResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_sender_with_http_info(create_sender, **kwargs)  # noqa: E501
+
+    def create_sender_with_http_info(self, create_sender, **kwargs):  # noqa: E501
+        """Add a sender  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_sender_with_http_info(create_sender, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CreateSenderResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param CreateSender create_sender: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(CreateSenderResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['create_sender'] = \
-            create_sender
-        return self.create_sender_endpoint.call_with_http_info(**kwargs)
-
-    def delete_sender(
-        self,
-        sender_id,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'create_sender',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_sender" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'create_sender' is set
+        if self.api_client.client_side_validation and ('create_sender' not in local_var_params or  # noqa: E501
+                                                        local_var_params['create_sender'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `create_sender` when calling `create_sender`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'create_sender' in local_var_params:
+            body_params = local_var_params['create_sender']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='CreateSenderResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_sender(self, sender_id, **kwargs):  # noqa: E501
         """Delete a sender  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.delete_sender(sender_id, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            sender_id (str):
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: DeleteSenderResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_sender_with_http_info(sender_id, **kwargs)  # noqa: E501
+
+    def delete_sender_with_http_info(self, sender_id, **kwargs):  # noqa: E501
+        """Delete a sender  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_sender_with_http_info(sender_id, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            DeleteSenderResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(DeleteSenderResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sender_id'] = \
-            sender_id
-        return self.delete_sender_endpoint.call_with_http_info(**kwargs)
-
-    def get_sender(
-        self,
-        sender_id,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'sender_id',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_sender" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'sender_id' is set
+        if self.api_client.client_side_validation and ('sender_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['sender_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `sender_id` when calling `delete_sender`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'sender_id' in local_var_params:
+            path_params['sender_id'] = local_var_params['sender_id']  # noqa: E501
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders/{sender_id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='DeleteSenderResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_sender(self, sender_id, **kwargs):  # noqa: E501
         """Show a sender details  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_sender(sender_id, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            sender_id (str):
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SenderResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_sender_with_http_info(sender_id, **kwargs)  # noqa: E501
+
+    def get_sender_with_http_info(self, sender_id, **kwargs):  # noqa: E501
+        """Show a sender details  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_sender_with_http_info(sender_id, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            SenderResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SenderResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sender_id'] = \
-            sender_id
-        return self.get_sender_endpoint.call_with_http_info(**kwargs)
-
-    def list_senders(
-        self,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'sender_id',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_sender" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'sender_id' is set
+        if self.api_client.client_side_validation and ('sender_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['sender_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `sender_id` when calling `get_sender`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'sender_id' in local_var_params:
+            path_params['sender_id'] = local_var_params['sender_id']  # noqa: E501
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders/{sender_id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SenderResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def list_senders(self, **kwargs):  # noqa: E501
         """Show all senders  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.list_senders(async_req=True)
         >>> result = thread.get()
 
+        :param async_req bool: execute request asynchronously
+        :param int page:
+        :param int per_page:
+        :param int account_id:
+        :param bool with_count:
+        :param str sort: Sort term and direction, using syntax `[-|+]term`.  Valid terms:   - `name`   - `email`   - `confirmed`
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SendersResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.list_senders_with_http_info(**kwargs)  # noqa: E501
+
+    def list_senders_with_http_info(self, **kwargs):  # noqa: E501
+        """Show all senders  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_senders_with_http_info(async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            page (int): [optional] if omitted the server will use the default value of 1
-            per_page (int): [optional] if omitted the server will use the default value of 50
-            account_id (int): [optional]
-            with_count (bool): [optional] if omitted the server will use the default value of False
-            sort (str): Sort term and direction, using syntax `[-|+]term`.  Valid terms:   - `name`   - `email`   - `confirmed`. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            SendersResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param int page:
+        :param int per_page:
+        :param int account_id:
+        :param bool with_count:
+        :param str sort: Sort term and direction, using syntax `[-|+]term`.  Valid terms:   - `name`   - `email`   - `confirmed`
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SendersResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.list_senders_endpoint.call_with_http_info(**kwargs)
-
-    def patch_sender(
-        self,
-        sender_id,
-        update_sender,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'page',
+            'per_page',
+            'account_id',
+            'with_count',
+            'sort'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_senders" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        if self.api_client.client_side_validation and 'page' in local_var_params and local_var_params['page'] < 1:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_senders`, must be a value greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'per_page' in local_var_params and local_var_params['per_page'] < 1:  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `per_page` when calling `list_senders`, must be a value greater than or equal to `1`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
+            query_params.append(('page', local_var_params['page']))  # noqa: E501
+        if 'per_page' in local_var_params and local_var_params['per_page'] is not None:  # noqa: E501
+            query_params.append(('per_page', local_var_params['per_page']))  # noqa: E501
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+        if 'with_count' in local_var_params and local_var_params['with_count'] is not None:  # noqa: E501
+            query_params.append(('with_count', local_var_params['with_count']))  # noqa: E501
+        if 'sort' in local_var_params and local_var_params['sort'] is not None:  # noqa: E501
+            query_params.append(('sort', local_var_params['sort']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SendersResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def patch_sender(self, sender_id, update_sender, **kwargs):  # noqa: E501
         """Update a sender  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.patch_sender(sender_id, update_sender, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            sender_id (str):
-            update_sender (UpdateSender):
-
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            PatchSenderResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param UpdateSender update_sender: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PatchSenderResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sender_id'] = \
-            sender_id
-        kwargs['update_sender'] = \
-            update_sender
-        return self.patch_sender_endpoint.call_with_http_info(**kwargs)
-
-    def resend_confirmation_email(
-        self,
-        sender_id,
-        **kwargs
-    ):
-        """Resend confirmation email  # noqa: E501
+        kwargs['_return_http_data_only'] = True
+        return self.patch_sender_with_http_info(sender_id, update_sender, **kwargs)  # noqa: E501
+
+    def patch_sender_with_http_info(self, sender_id, update_sender, **kwargs):  # noqa: E501
+        """Update a sender  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.patch_sender_with_http_info(sender_id, update_sender, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param UpdateSender update_sender: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PatchSenderResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'sender_id',
+            'update_sender',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method patch_sender" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'sender_id' is set
+        if self.api_client.client_side_validation and ('sender_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['sender_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `sender_id` when calling `patch_sender`")  # noqa: E501
+        # verify the required parameter 'update_sender' is set
+        if self.api_client.client_side_validation and ('update_sender' not in local_var_params or  # noqa: E501
+                                                        local_var_params['update_sender'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `update_sender` when calling `patch_sender`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'sender_id' in local_var_params:
+            path_params['sender_id'] = local_var_params['sender_id']  # noqa: E501
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'update_sender' in local_var_params:
+            body_params = local_var_params['update_sender']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders/{sender_id}', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PatchSenderResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def resend_confirmation_email(self, sender_id, **kwargs):  # noqa: E501
+        """Resend confirmation email  # noqa: E501
 
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
         >>> thread = api.resend_confirmation_email(sender_id, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            sender_id (str):
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ResendConfirmationEmailResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.resend_confirmation_email_with_http_info(sender_id, **kwargs)  # noqa: E501
+
+    def resend_confirmation_email_with_http_info(self, sender_id, **kwargs):  # noqa: E501
+        """Resend confirmation email  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.resend_confirmation_email_with_http_info(sender_id, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            ResendConfirmationEmailResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param str sender_id: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ResendConfirmationEmailResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sender_id'] = \
-            sender_id
-        return self.resend_confirmation_email_endpoint.call_with_http_info(**kwargs)
 
+        local_var_params = locals()
+
+        all_params = [
+            'sender_id',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method resend_confirmation_email" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'sender_id' is set
+        if self.api_client.client_side_validation and ('sender_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['sender_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `sender_id` when calling `resend_confirmation_email`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'sender_id' in local_var_params:
+            path_params['sender_id'] = local_var_params['sender_id']  # noqa: E501
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/senders/{sender_id}/resend-confirmation-email', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ResendConfirmationEmailResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/api/system_email_api.py` & `cakemail-openapi-1.9.1/cakemail_openapi/api/system_email_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,416 +1,393 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+from __future__ import absolute_import
+
 import re  # noqa: F401
-import sys  # noqa: F401
 
-from cakemail_openapi.api_client import ApiClient, Endpoint as _Endpoint
-from cakemail_openapi.model_utils import (  # noqa: F401
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_and_convert_types
+# python 2 and python 3 compatibility library
+import six
+
+from cakemail_openapi.api_client import ApiClient
+from cakemail_openapi.exceptions import (  # noqa: F401
+    ApiTypeError,
+    ApiValueError
 )
-from cakemail_openapi.model.http_bad_request_error import HTTPBadRequestError
-from cakemail_openapi.model.http_validation_error import HTTPValidationError
-from cakemail_openapi.model.put_system_emails_response import PutSystemEmailsResponse
-from cakemail_openapi.model.system_emails_response import SystemEmailsResponse
-from cakemail_openapi.model.system_emails_templates import SystemEmailsTemplates
 
 
 class SystemEmailApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.patch_system_emails_endpoint = _Endpoint(
-            settings={
-                'response_type': (PutSystemEmailsResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/system-emails',
-                'operation_id': 'patch_system_emails',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'system_emails_templates',
-                    'account_id',
-                ],
-                'required': [
-                    'system_emails_templates',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'system_emails_templates':
-                        (SystemEmailsTemplates,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'system_emails_templates': 'body',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.set_system_emails_endpoint = _Endpoint(
-            settings={
-                'response_type': (PutSystemEmailsResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/system-emails',
-                'operation_id': 'set_system_emails',
-                'http_method': 'PUT',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'system_emails_templates',
-                    'account_id',
-                ],
-                'required': [
-                    'system_emails_templates',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'system_emails_templates':
-                        (SystemEmailsTemplates,),
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'system_emails_templates': 'body',
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-        self.show_system_emails_endpoint = _Endpoint(
-            settings={
-                'response_type': (SystemEmailsResponse,),
-                'auth': [
-                    'OAuth2PasswordBearer'
-                ],
-                'endpoint_path': '/brands/default/system-emails',
-                'operation_id': 'show_system_emails',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'account_id',
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'account_id':
-                        (int,),
-                },
-                'attribute_map': {
-                    'account_id': 'account_id',
-                },
-                'location_map': {
-                    'account_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
 
-    def patch_system_emails(
-        self,
-        system_emails_templates,
-        **kwargs
-    ):
+    def patch_system_emails(self, system_emails_templates, **kwargs):  # noqa: E501
         """Update system emails configuration  # noqa: E501
 
         Partially update system emails configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.patch_system_emails(system_emails_templates, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            system_emails_templates (SystemEmailsTemplates):
+        :param async_req bool: execute request asynchronously
+        :param SystemEmailsTemplates system_emails_templates: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PutSystemEmailsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.patch_system_emails_with_http_info(system_emails_templates, **kwargs)  # noqa: E501
+
+    def patch_system_emails_with_http_info(self, system_emails_templates, **kwargs):  # noqa: E501
+        """Update system emails configuration  # noqa: E501
+
+        Partially update system emails configuration  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.patch_system_emails_with_http_info(system_emails_templates, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            PutSystemEmailsResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param SystemEmailsTemplates system_emails_templates: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PutSystemEmailsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['system_emails_templates'] = \
-            system_emails_templates
-        return self.patch_system_emails_endpoint.call_with_http_info(**kwargs)
-
-    def set_system_emails(
-        self,
-        system_emails_templates,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'system_emails_templates',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method patch_system_emails" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'system_emails_templates' is set
+        if self.api_client.client_side_validation and ('system_emails_templates' not in local_var_params or  # noqa: E501
+                                                        local_var_params['system_emails_templates'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `system_emails_templates` when calling `patch_system_emails`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'system_emails_templates' in local_var_params:
+            body_params = local_var_params['system_emails_templates']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/system-emails', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PutSystemEmailsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def set_system_emails(self, system_emails_templates, **kwargs):  # noqa: E501
         """Set system emails configuration  # noqa: E501
 
         Set system emails configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.set_system_emails(system_emails_templates, async_req=True)
         >>> result = thread.get()
 
-        Args:
-            system_emails_templates (SystemEmailsTemplates):
+        :param async_req bool: execute request asynchronously
+        :param SystemEmailsTemplates system_emails_templates: (required)
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PutSystemEmailsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.set_system_emails_with_http_info(system_emails_templates, **kwargs)  # noqa: E501
+
+    def set_system_emails_with_http_info(self, system_emails_templates, **kwargs):  # noqa: E501
+        """Set system emails configuration  # noqa: E501
+
+        Set system emails configuration  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_system_emails_with_http_info(system_emails_templates, async_req=True)
+        >>> result = thread.get()
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            PutSystemEmailsResponse
-                If the method is called asynchronously, returns the request
-                thread.
+        :param async_req bool: execute request asynchronously
+        :param SystemEmailsTemplates system_emails_templates: (required)
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PutSystemEmailsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['system_emails_templates'] = \
-            system_emails_templates
-        return self.set_system_emails_endpoint.call_with_http_info(**kwargs)
-
-    def show_system_emails(
-        self,
-        **kwargs
-    ):
+
+        local_var_params = locals()
+
+        all_params = [
+            'system_emails_templates',
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method set_system_emails" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'system_emails_templates' is set
+        if self.api_client.client_side_validation and ('system_emails_templates' not in local_var_params or  # noqa: E501
+                                                        local_var_params['system_emails_templates'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `system_emails_templates` when calling `set_system_emails`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'system_emails_templates' in local_var_params:
+            body_params = local_var_params['system_emails_templates']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/system-emails', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PutSystemEmailsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def show_system_emails(self, **kwargs):  # noqa: E501
         """Show system emails configuration  # noqa: E501
 
         Show system emails configuration  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.show_system_emails(async_req=True)
         >>> result = thread.get()
 
+        :param async_req bool: execute request asynchronously
+        :param int account_id:
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SystemEmailsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.show_system_emails_with_http_info(**kwargs)  # noqa: E501
 
-        Keyword Args:
-            account_id (int): [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            SystemEmailsResponse
-                If the method is called asynchronously, returns the request
-                thread.
+    def show_system_emails_with_http_info(self, **kwargs):  # noqa: E501
+        """Show system emails configuration  # noqa: E501
+
+        Show system emails configuration  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.show_system_emails_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int account_id:
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SystemEmailsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
         """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.show_system_emails_endpoint.call_with_http_info(**kwargs)
 
+        local_var_params = locals()
+
+        all_params = [
+            'account_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method show_system_emails" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'account_id' in local_var_params and local_var_params['account_id'] is not None:  # noqa: E501
+            query_params.append(('account_id', local_var_params['account_id']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['OAuth2PasswordBearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/brands/default/system-emails', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SystemEmailsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/api_client.py` & `cakemail-openapi-1.9.1/cakemail_openapi/api_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,37 @@
+# coding: utf-8
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
+from __future__ import absolute_import
 
-import json
 import atexit
+import datetime
+from dateutil.parser import parse
+import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
-import io
 import os
 import re
-import typing
-from urllib.parse import quote
-from urllib3.fields import RequestField
+import tempfile
 
+# python 2 and python 3 compatibility library
+import six
+from six.moves.urllib.parse import quote
 
-from cakemail_openapi import rest
 from cakemail_openapi.configuration import Configuration
-from cakemail_openapi.exceptions import ApiTypeError, ApiValueError, ApiException
-from cakemail_openapi.model_utils import (
-    ModelNormal,
-    ModelSimple,
-    ModelComposed,
-    check_allowed_values,
-    check_validations,
-    date,
-    datetime,
-    deserialize_file,
-    file_type,
-    model_to_dict,
-    none_type,
-    validate_and_convert_types
-)
+import cakemail_openapi.models
+from cakemail_openapi import rest
+from cakemail_openapi.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -57,14 +48,25 @@
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
     :param pool_threads: The number of threads to use for async requests
         to the API. More threads means more concurrent API requests.
     """
 
+    PRIMITIVE_TYPES = (float, bool, bytes, six.text_type) + six.integer_types
+    NATIVE_TYPES_MAPPING = {
+        'int': int,
+        'long': int if six.PY3 else long,  # noqa: F821
+        'float': float,
+        'str': str,
+        'bool': bool,
+        'date': datetime.date,
+        'datetime': datetime.datetime,
+        'object': object,
+    }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
                  cookie=None, pool_threads=1):
         if configuration is None:
             configuration = Configuration.get_default_copy()
         self.configuration = configuration
@@ -73,14 +75,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -111,33 +114,19 @@
     def user_agent(self, value):
         self.default_headers['User-Agent'] = value
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
-        self,
-        resource_path: str,
-        method: str,
-        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        body: typing.Optional[typing.Any] = None,
-        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
-        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
-        auth_settings: typing.Optional[typing.List[str]] = None,
-        _return_http_data_only: typing.Optional[bool] = None,
-        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
-        _preload_content: bool = True,
-        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
-        _host: typing.Optional[str] = None,
-        _check_type: typing.Optional[bool] = None,
-        _content_type: typing.Optional[str] = None
-    ):
+            self, resource_path, method, path_params=None,
+            query_params=None, header_params=None, body=None, post_params=None,
+            files=None, response_type=None, auth_settings=None,
+            _return_http_data_only=None, collection_formats=None,
+            _preload_content=True, _request_timeout=None, _host=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -168,26 +157,22 @@
         # post parameters
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
             post_params.extend(self.files_parameters(files))
-            if header_params['Content-Type'].startswith("multipart"):
-                post_params = self.parameters_to_multipart(post_params,
-                                                          (dict) )
+
+        # auth setting
+        self.update_params_for_auth(header_params, query_params, auth_settings)
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
-        # auth setting
-        self.update_params_for_auth(header_params, query_params,
-                                    auth_settings, resource_path, method, body)
-
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
         else:
             # use server/host defined in path or operation instead
             url = _host + resource_path
 
@@ -195,241 +180,210 @@
             # perform request and return response
             response_data = self.request(
                 method, url, query_params=query_params, headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout)
         except ApiException as e:
-            e.body = e.body.decode('utf-8')
+            e.body = e.body.decode('utf-8') if six.PY3 else e.body
             raise e
 
+        content_type = response_data.getheader('content-type')
+
         self.last_response = response_data
 
         return_data = response_data
 
         if not _preload_content:
-            return (return_data)
             return return_data
 
+        if six.PY3 and response_type not in ["file", "bytes"]:
+            match = None
+            if content_type is not None:
+                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
+            encoding = match.group(1) if match else "utf-8"
+            response_data.data = response_data.data.decode(encoding)
+
         # deserialize response data
         if response_type:
-            if response_type != (file_type,):
-                encoding = "utf-8"
-                content_type = response_data.getheader('content-type')
-                if content_type is not None:
-                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
-                    if match:
-                        encoding = match.group(1)
-                response_data.data = response_data.data.decode(encoding)
-
-            return_data = self.deserialize(
-                response_data,
-                response_type,
-                _check_type
-            )
+            return_data = self.deserialize(response_data, response_type)
         else:
             return_data = None
 
         if _return_http_data_only:
             return (return_data)
         else:
             return (return_data, response_data.status,
                     response_data.getheaders())
 
-    def parameters_to_multipart(self, params, collection_types):
-        """Get parameters as list of tuples, formatting as json if value is collection_types
+    def sanitize_for_serialization(self, obj):
+        """Builds a JSON POST object.
 
-        :param params: Parameters as list of two-tuples
-        :param dict collection_types: Parameter collection types
-        :return: Parameters as list of tuple or urllib3.fields.RequestField
-        """
-        new_params = []
-        if collection_types is None:
-            collection_types = (dict)
-        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
-            if isinstance(v, collection_types): # v is instance of collection_type, formatting as application/json
-                 v = json.dumps(v, ensure_ascii=False).encode("utf-8")
-                 field = RequestField(k, v)
-                 field.make_multipart(content_type="application/json; charset=utf-8")
-                 new_params.append(field)
-            else:
-                 new_params.append((k, v))
-        return new_params
-
-    @classmethod
-    def sanitize_for_serialization(cls, obj):
-        """Prepares data for transmission before it is sent with the rest client
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
-        If obj is io.IOBase, return the bytes
+
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
-        if isinstance(obj, (ModelNormal, ModelComposed)):
-            return {
-                key: cls.sanitize_for_serialization(val) for key, val in model_to_dict(obj, serialize=True).items()
-            }
-        elif isinstance(obj, io.IOBase):
-            return cls.get_file_data_and_close_file(obj)
-        elif isinstance(obj, (str, int, float, none_type, bool)):
+        if obj is None:
+            return None
+        elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
-        elif isinstance(obj, (datetime, date)):
+        elif isinstance(obj, list):
+            return [self.sanitize_for_serialization(sub_obj)
+                    for sub_obj in obj]
+        elif isinstance(obj, tuple):
+            return tuple(self.sanitize_for_serialization(sub_obj)
+                         for sub_obj in obj)
+        elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
-        elif isinstance(obj, ModelSimple):
-            return cls.sanitize_for_serialization(obj.value)
-        elif isinstance(obj, (list, tuple)):
-            return [cls.sanitize_for_serialization(item) for item in obj]
+
         if isinstance(obj, dict):
-            return {key: cls.sanitize_for_serialization(val) for key, val in obj.items()}
-        raise ApiValueError('Unable to prepare type {} for serialization'.format(obj.__class__.__name__))
+            obj_dict = obj
+        else:
+            # Convert model obj to dict except
+            # attributes `openapi_types`, `attribute_map`
+            # and attributes which value is not None.
+            # Convert attribute name to json key in
+            # model definition for request.
+            obj_dict = {obj.attribute_map[attr]: getattr(obj, attr)
+                        for attr, _ in six.iteritems(obj.openapi_types)
+                        if getattr(obj, attr) is not None}
 
-    def deserialize(self, response, response_type, _check_type):
+        return {key: self.sanitize_for_serialization(val)
+                for key, val in six.iteritems(obj_dict)}
+
+    def deserialize(self, response, response_type):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
-        :param response_type: For the response, a tuple containing:
-            valid classes
-            a list containing valid classes (for list schemas)
-            a dict containing a tuple of valid classes as the value
-            Example values:
-            (str,)
-            (Pet,)
-            (float, none_type)
-            ([int, none_type],)
-            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
-        :param _check_type: boolean, whether to check the types of the data
-            received from the server
-        :type _check_type: bool
+        :param response_type: class literal for
+            deserialized object, or string of class name.
 
         :return: deserialized object.
         """
         # handle file downloading
         # save response body into a tmp file and return the instance
-        if response_type == (file_type,):
-            content_disposition = response.getheader("Content-Disposition")
-            return deserialize_file(response.data, self.configuration,
-                                    content_disposition=content_disposition)
+        if response_type == "file":
+            return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            received_data = json.loads(response.data)
+            data = json.loads(response.data)
         except ValueError:
-            received_data = response.data
+            data = response.data
+
+        return self.__deserialize(data, response_type)
+
+    def __deserialize(self, data, klass):
+        """Deserializes dict, list, str into an object.
+
+        :param data: dict, list or str.
+        :param klass: class literal, or string of class name.
+
+        :return: object.
+        """
+        if data is None:
+            return None
+
+        if type(klass) == str:
+            if klass.startswith('list['):
+                sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
+                return [self.__deserialize(sub_data, sub_kls)
+                        for sub_data in data]
+
+            if klass.startswith('dict('):
+                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+                return {k: self.__deserialize(v, sub_kls)
+                        for k, v in six.iteritems(data)}
+
+            # convert str to class
+            if klass in self.NATIVE_TYPES_MAPPING:
+                klass = self.NATIVE_TYPES_MAPPING[klass]
+            else:
+                klass = getattr(cakemail_openapi.models, klass)
+
+        if klass in self.PRIMITIVE_TYPES:
+            return self.__deserialize_primitive(data, klass)
+        elif klass == object:
+            return self.__deserialize_object(data)
+        elif klass == datetime.date:
+            return self.__deserialize_date(data)
+        elif klass == datetime.datetime:
+            return self.__deserialize_datetime(data)
+        else:
+            return self.__deserialize_model(data, klass)
 
-        # store our data under the key of 'received_data' so users have some
-        # context if they are deserializing a string and the data type is wrong
-        deserialized_data = validate_and_convert_types(
-            received_data,
-            response_type,
-            ['received_data'],
-            True,
-            _check_type,
-            configuration=self.configuration
-        )
-        return deserialized_data
-
-    def call_api(
-        self,
-        resource_path: str,
-        method: str,
-        path_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        query_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        header_params: typing.Optional[typing.Dict[str, typing.Any]] = None,
-        body: typing.Optional[typing.Any] = None,
-        post_params: typing.Optional[typing.List[typing.Tuple[str, typing.Any]]] = None,
-        files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None,
-        response_type: typing.Optional[typing.Tuple[typing.Any]] = None,
-        auth_settings: typing.Optional[typing.List[str]] = None,
-        async_req: typing.Optional[bool] = None,
-        _return_http_data_only: typing.Optional[bool] = None,
-        collection_formats: typing.Optional[typing.Dict[str, str]] = None,
-        _preload_content: bool = True,
-        _request_timeout: typing.Optional[typing.Union[int, float, typing.Tuple]] = None,
-        _host: typing.Optional[str] = None,
-        _check_type: typing.Optional[bool] = None
-    ):
+    def call_api(self, resource_path, method,
+                 path_params=None, query_params=None, header_params=None,
+                 body=None, post_params=None, files=None,
+                 response_type=None, auth_settings=None, async_req=None,
+                 _return_http_data_only=None, collection_formats=None,
+                 _preload_content=True, _request_timeout=None, _host=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
         :param header_params: Header parameters to be
             placed in the request header.
         :param body: Request body.
         :param post_params dict: Request post form parameters,
             for `application/x-www-form-urlencoded`, `multipart/form-data`.
         :param auth_settings list: Auth Settings names for the request.
-        :param response_type: For the response, a tuple containing:
-            valid classes
-            a list containing valid classes (for list schemas)
-            a dict containing a tuple of valid classes as the value
-            Example values:
-            (str,)
-            (Pet,)
-            (float, none_type)
-            ([int, none_type],)
-            ({str: (bool, str, int, float, date, datetime, str, none_type)},)
-        :param files: key -> field name, value -> a list of open file
-            objects for `multipart/form-data`.
-        :type files: dict
+        :param response: Response data type.
+        :param files dict: key -> filename, value -> filepath,
+            for `multipart/form-data`.
         :param async_req bool: execute request asynchronously
-        :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param collection_formats: dict of collection formats for path, query,
             header, and post parameters.
-        :type collection_formats: dict, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _check_type: boolean describing if the data back from the server
-            should have its type checked.
-        :type _check_type: bool, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
                                    response_type, auth_settings,
                                    _return_http_data_only, collection_formats,
-                                   _preload_content, _request_timeout, _host,
-                                   _check_type)
+                                   _preload_content, _request_timeout, _host)
 
         return self.pool.apply_async(self.__call_api, (resource_path,
                                                        method, path_params,
                                                        query_params,
                                                        header_params, body,
                                                        post_params, files,
                                                        response_type,
                                                        auth_settings,
                                                        _return_http_data_only,
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
-                                                       _host, _check_type))
+                                                       _host))
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(url,
@@ -443,18 +397,16 @@
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          headers=headers)
         elif method == "OPTIONS":
             return self.rest_client.OPTIONS(url,
                                             query_params=query_params,
                                             headers=headers,
-                                            post_params=post_params,
                                             _preload_content=_preload_content,
-                                            _request_timeout=_request_timeout,
-                                            body=body)
+                                            _request_timeout=_request_timeout)
         elif method == "POST":
             return self.rest_client.POST(url,
                                          query_params=query_params,
                                          headers=headers,
                                          post_params=post_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
@@ -494,15 +446,15 @@
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
         new_params = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+        for k, v in six.iteritems(params) if isinstance(params, dict) else params:  # noqa: E501
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, value) for value in v)
                 else:
                     if collection_format == 'ssv':
                         delimiter = ' '
@@ -514,50 +466,35 @@
                         delimiter = ','
                     new_params.append(
                         (k, delimiter.join(str(value) for value in v)))
             else:
                 new_params.append((k, v))
         return new_params
 
-    @staticmethod
-    def get_file_data_and_close_file(file_instance: io.IOBase) -> bytes:
-        file_data = file_instance.read()
-        file_instance.close()
-        return file_data
-
-    def files_parameters(self, files: typing.Optional[typing.Dict[str, typing.List[io.IOBase]]] = None):
+    def files_parameters(self, files=None):
         """Builds form parameters.
 
-        :param files: None or a dict with key=param_name and
-            value is a list of open file objects
-        :return: List of tuples of form parameters with file data
+        :param files: File parameters.
+        :return: Form parameters with files.
         """
-        if files is None:
-            return []
-
         params = []
-        for param_name, file_instances in files.items():
-            if file_instances is None:
-                # if the file field is nullable, skip None values
-                continue
-            for file_instance in file_instances:
-                if file_instance is None:
-                    # if the file field is nullable, skip None values
+
+        if files:
+            for k, v in six.iteritems(files):
+                if not v:
                     continue
-                if file_instance.closed is True:
-                    raise ApiValueError(
-                        "Cannot read a closed file. The passed in file_type "
-                        "for %s must be open." % param_name
-                    )
-                filename = os.path.basename(file_instance.name)
-                filedata = self.get_file_data_and_close_file(file_instance)
-                mimetype = (mimetypes.guess_type(filename)[0] or
-                            'application/octet-stream')
-                params.append(
-                    tuple([param_name, tuple([filename, filedata, mimetype])]))
+                file_names = v if type(v) is list else [v]
+                for n in file_names:
+                    with open(n, 'rb') as f:
+                        filename = os.path.basename(f.name)
+                        filedata = f.read()
+                        mimetype = (mimetypes.guess_type(filename)[0] or
+                                    'application/octet-stream')
+                        params.append(
+                            tuple([k, tuple([filename, filedata, mimetype])]))
 
         return params
 
     def select_header_accept(self, accepts):
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
@@ -569,296 +506,161 @@
         accepts = [x.lower() for x in accepts]
 
         if 'application/json' in accepts:
             return 'application/json'
         else:
             return ', '.join(accepts)
 
-    def select_header_content_type(self, content_types, method=None, body=None):
+    def select_header_content_type(self, content_types):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
-        :param method: http method (e.g. POST, PATCH).
-        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
             return 'application/json'
 
         content_types = [x.lower() for x in content_types]
 
-        if (method == 'PATCH' and
-                'application/json-patch+json' in content_types and
-                isinstance(body, list)):
-            return 'application/json-patch+json'
-
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, queries, auth_settings,
-                               resource_path, method, body):
+    def update_params_for_auth(self, headers, querys, auth_settings):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
-        :param queries: Query parameters tuple list to be updated.
+        :param querys: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
-        :param resource_path: A string representation of the HTTP request resource path.
-        :param method: A string representation of the HTTP request method.
-        :param body: A object representing the body of the HTTP request.
-            The object type is the return value of _encoder.default().
         """
         if not auth_settings:
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
                 if auth_setting['in'] == 'cookie':
                     headers['Cookie'] = auth_setting['value']
                 elif auth_setting['in'] == 'header':
-                    if auth_setting['type'] != 'http-signature':
-                        headers[auth_setting['key']] = auth_setting['value']
+                    headers[auth_setting['key']] = auth_setting['value']
                 elif auth_setting['in'] == 'query':
-                    queries.append((auth_setting['key'], auth_setting['value']))
+                    querys.append((auth_setting['key'], auth_setting['value']))
                 else:
                     raise ApiValueError(
                         'Authentication token must be in `query` or `header`'
                     )
 
+    def __deserialize_file(self, response):
+        """Deserializes body to file
 
-class Endpoint(object):
-    def __init__(self, settings=None, params_map=None, root_map=None,
-                 headers_map=None, api_client=None, callable=None):
-        """Creates an endpoint
-
-        Args:
-            settings (dict): see below key value pairs
-                'response_type' (tuple/None): response type
-                'auth' (list): a list of auth type keys
-                'endpoint_path' (str): the endpoint path
-                'operation_id' (str): endpoint string identifier
-                'http_method' (str): POST/PUT/PATCH/GET etc
-                'servers' (list): list of str servers that this endpoint is at
-            params_map (dict): see below key value pairs
-                'all' (list): list of str endpoint parameter names
-                'required' (list): list of required parameter names
-                'nullable' (list): list of nullable parameter names
-                'enum' (list): list of parameters with enum values
-                'validation' (list): list of parameters with validations
-            root_map
-                'validations' (dict): the dict mapping endpoint parameter tuple
-                    paths to their validation dictionaries
-                'allowed_values' (dict): the dict mapping endpoint parameter
-                    tuple paths to their allowed_values (enum) dictionaries
-                'openapi_types' (dict): param_name to openapi type
-                'attribute_map' (dict): param_name to camelCase name
-                'location_map' (dict): param_name to  'body', 'file', 'form',
-                    'header', 'path', 'query'
-                collection_format_map (dict): param_name to `csv` etc.
-            headers_map (dict): see below key value pairs
-                'accept' (list): list of Accept header strings
-                'content_type' (list): list of Content-Type header strings
-            api_client (ApiClient) api client instance
-            callable (function): the function which is invoked when the
-                Endpoint is called
-        """
-        self.settings = settings
-        self.params_map = params_map
-        self.params_map['all'].extend([
-            'async_req',
-            '_host_index',
-            '_preload_content',
-            '_request_timeout',
-            '_return_http_data_only',
-            '_check_input_type',
-            '_check_return_type',
-            '_content_type'
-        ])
-        self.params_map['nullable'].extend(['_request_timeout'])
-        self.validations = root_map['validations']
-        self.allowed_values = root_map['allowed_values']
-        self.openapi_types = root_map['openapi_types']
-        extra_types = {
-            'async_req': (bool,),
-            '_host_index': (none_type, int),
-            '_preload_content': (bool,),
-            '_request_timeout': (none_type, float, (float,), [float], int, (int,), [int]),
-            '_return_http_data_only': (bool,),
-            '_check_input_type': (bool,),
-            '_check_return_type': (bool,),
-            '_content_type': (none_type, str)
-        }
-        self.openapi_types.update(extra_types)
-        self.attribute_map = root_map['attribute_map']
-        self.location_map = root_map['location_map']
-        self.collection_format_map = root_map['collection_format_map']
-        self.headers_map = headers_map
-        self.api_client = api_client
-        self.callable = callable
-
-    def __validate_inputs(self, kwargs):
-        for param in self.params_map['enum']:
-            if param in kwargs:
-                check_allowed_values(
-                    self.allowed_values,
-                    (param,),
-                    kwargs[param]
-                )
+        Saves response body into a file in a temporary folder,
+        using the filename from the `Content-Disposition` header if provided.
 
-        for param in self.params_map['validation']:
-            if param in kwargs:
-                check_validations(
-                    self.validations,
-                    (param,),
-                    kwargs[param],
-                    configuration=self.api_client.configuration
-                )
+        :param response:  RESTResponse.
+        :return: file path.
+        """
+        fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
+        os.close(fd)
+        os.remove(path)
 
-        if kwargs['_check_input_type'] is False:
-            return
+        content_disposition = response.getheader("Content-Disposition")
+        if content_disposition:
+            filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
+                                 content_disposition).group(1)
+            path = os.path.join(os.path.dirname(path), filename)
 
-        for key, value in kwargs.items():
-            fixed_val = validate_and_convert_types(
-                value,
-                self.openapi_types[key],
-                [key],
-                False,
-                kwargs['_check_input_type'],
-                configuration=self.api_client.configuration
-            )
-            kwargs[key] = fixed_val
+        with open(path, "wb") as f:
+            f.write(response.data)
 
-    def __gather_params(self, kwargs):
-        params = {
-            'body': None,
-            'collection_format': {},
-            'file': {},
-            'form': [],
-            'header': {},
-            'path': {},
-            'query': []
-        }
-
-        for param_name, param_value in kwargs.items():
-            param_location = self.location_map.get(param_name)
-            if param_location is None:
-                continue
-            if param_location:
-                if param_location == 'body':
-                    params['body'] = param_value
-                    continue
-                base_name = self.attribute_map[param_name]
-                if (param_location == 'form' and
-                        self.openapi_types[param_name] == (file_type,)):
-                    params['file'][param_name] = [param_value]
-                elif (param_location == 'form' and
-                        self.openapi_types[param_name] == ([file_type],)):
-                    # param_value is already a list
-                    params['file'][param_name] = param_value
-                elif param_location in {'form', 'query'}:
-                    param_value_full = (base_name, param_value)
-                    params[param_location].append(param_value_full)
-                if param_location not in {'form', 'query'}:
-                    params[param_location][base_name] = param_value
-                collection_format = self.collection_format_map.get(param_name)
-                if collection_format:
-                    params['collection_format'][base_name] = collection_format
+        return path
 
-        return params
+    def __deserialize_primitive(self, data, klass):
+        """Deserializes string to primitive type.
 
-    def __call__(self, *args, **kwargs):
-        """ This method is invoked when endpoints are called
-        Example:
+        :param data: str.
+        :param klass: class literal.
 
-        api_instance = AccountApi()
-        api_instance.get_self_account  # this is an instance of the class Endpoint
-        api_instance.get_self_account()  # this invokes api_instance.get_self_account.__call__()
-        which then invokes the callable functions stored in that endpoint at
-        api_instance.get_self_account.callable or self.callable in this class
+        :return: int, long, float, str, bool.
+        """
+        try:
+            return klass(data)
+        except UnicodeEncodeError:
+            return six.text_type(data)
+        except TypeError:
+            return data
 
+    def __deserialize_object(self, value):
+        """Return an original value.
+
+        :return: object.
         """
-        return self.callable(self, *args, **kwargs)
+        return value
 
-    def call_with_http_info(self, **kwargs):
+    def __deserialize_date(self, string):
+        """Deserializes string to date.
 
+        :param string: str.
+        :return: date.
+        """
         try:
-            index = self.api_client.configuration.server_operation_index.get(
-                self.settings['operation_id'], self.api_client.configuration.server_index
-            ) if kwargs['_host_index'] is None else kwargs['_host_index']
-            server_variables = self.api_client.configuration.server_operation_variables.get(
-                self.settings['operation_id'], self.api_client.configuration.server_variables
-            )
-            _host = self.api_client.configuration.get_host_from_settings(
-                index, variables=server_variables, servers=self.settings['servers']
+            return parse(string).date()
+        except ImportError:
+            return string
+        except ValueError:
+            raise rest.ApiException(
+                status=0,
+                reason="Failed to parse `{0}` as date object".format(string)
             )
-        except IndexError:
-            if self.settings['servers']:
-                raise ApiValueError(
-                    "Invalid host index. Must be 0 <= index < %s" %
-                    len(self.settings['servers'])
-                )
-            _host = None
 
-        for key, value in kwargs.items():
-            if key not in self.params_map['all']:
-                raise ApiTypeError(
-                    "Got an unexpected parameter '%s'"
-                    " to method `%s`" %
-                    (key, self.settings['operation_id'])
-                )
-            # only throw this nullable ApiValueError if _check_input_type
-            # is False, if _check_input_type==True we catch this case
-            # in self.__validate_inputs
-            if (key not in self.params_map['nullable'] and value is None
-                    and kwargs['_check_input_type'] is False):
-                raise ApiValueError(
-                    "Value may not be None for non-nullable parameter `%s`"
-                    " when calling `%s`" %
-                    (key, self.settings['operation_id'])
-                )
+    def __deserialize_datetime(self, string):
+        """Deserializes string to datetime.
 
-        for key in self.params_map['required']:
-            if key not in kwargs.keys():
-                raise ApiValueError(
-                    "Missing the required parameter `%s` when calling "
-                    "`%s`" % (key, self.settings['operation_id'])
-                )
+        The string should be in iso8601 datetime format.
 
-        self.__validate_inputs(kwargs)
-
-        params = self.__gather_params(kwargs)
+        :param string: str.
+        :return: datetime.
+        """
+        try:
+            return parse(string)
+        except ImportError:
+            return string
+        except ValueError:
+            raise rest.ApiException(
+                status=0,
+                reason=(
+                    "Failed to parse `{0}` as datetime object"
+                    .format(string)
+                )
+            )
 
-        accept_headers_list = self.headers_map['accept']
-        if accept_headers_list:
-            params['header']['Accept'] = self.api_client.select_header_accept(
-                accept_headers_list)
+    def __deserialize_model(self, data, klass):
+        """Deserializes list or dict to model.
 
-        if kwargs.get('_content_type'):
-            params['header']['Content-Type'] = kwargs['_content_type']
-        else:
-            content_type_headers_list = self.headers_map['content_type']
-            if content_type_headers_list:
-                if params['body'] != "":
-                    header_list = self.api_client.select_header_content_type(
-                        content_type_headers_list, self.settings['http_method'],
-                        params['body'])
-                    params['header']['Content-Type'] = header_list
-
-        return self.api_client.call_api(
-            self.settings['endpoint_path'], self.settings['http_method'],
-            params['path'],
-            params['query'],
-            params['header'],
-            body=params['body'],
-            post_params=params['form'],
-            files=params['file'],
-            response_type=self.settings['response_type'],
-            auth_settings=self.settings['auth'],
-            async_req=kwargs['async_req'],
-            _check_type=kwargs['_check_return_type'],
-            _return_http_data_only=kwargs['_return_http_data_only'],
-            _preload_content=kwargs['_preload_content'],
-            _request_timeout=kwargs['_request_timeout'],
-            _host=_host,
-            collection_formats=params['collection_format'])
+        :param data: dict, list.
+        :param klass: class literal.
+        :return: model object.
+        """
+        has_discriminator = False
+        if (hasattr(klass, 'get_real_child_model')
+                and klass.discriminator_value_class_map):
+            has_discriminator = True
+
+        if not klass.openapi_types and has_discriminator is False:
+            return data
+
+        kwargs = {}
+        if (data is not None and
+                klass.openapi_types is not None and
+                isinstance(data, (list, dict))):
+            for attr, attr_type in six.iteritems(klass.openapi_types):
+                if klass.attribute_map[attr] in data:
+                    value = data[klass.attribute_map[attr]]
+                    kwargs[attr] = self.__deserialize(value, attr_type)
+
+        instance = klass(**kwargs)
+
+        if has_discriminator:
+            klass_name = instance.get_real_child_model(data)
+            if klass_name:
+                instance = self.__deserialize(data, klass_name)
+        return instance
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/configuration.py` & `cakemail-openapi-1.9.1/cakemail_openapi/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+from __future__ import absolute_import
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
-from cakemail_openapi.exceptions import ApiValueError
-
+import six
+from six.moves import http_client as httplib
 
-JSON_SCHEMA_VALIDATION_KEYWORDS = {
-    'multipleOf', 'maximum', 'exclusiveMaximum',
-    'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
-}
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
@@ -47,72 +45,34 @@
          implementation.
       2. The client was generated using an older version of the OpenAPI document
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
-    :param server_index: Index to servers configuration.
-    :param server_variables: Mapping with string values to replace variables in
-      templated server configuration. The validation of enums is performed for
-      variables with defined enum values before.
-    :param server_operation_index: Mapping from operation ID to an index to server
-      configuration.
-    :param server_operation_variables: Mapping from operation ID to a mapping with
-      string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
 
     :Example:
     """
 
     _default = None
 
-    def __init__(self, host=None,
+    def __init__(self, host="https://api.cakemail.dev",
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
-                 disabled_client_side_validations="",
-                 server_index=None, server_variables=None,
-                 server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://api.cakemail.dev" if host is None else host
+        self.host = host
         """Default Base url
         """
-        self.server_index = 0 if server_index is None and host is None else server_index
-        self.server_operation_index = server_operation_index or {}
-        """Default server index
-        """
-        self.server_variables = server_variables or {}
-        self.server_operation_variables = server_operation_variables or {}
-        """Default server variables
-        """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
             self.api_key = api_key
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
@@ -125,15 +85,17 @@
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
-        self.disabled_client_side_validations = disabled_client_side_validations
+        self.access_token = None
+        """access token for OAuth/Bearer
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("cakemail_openapi")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -152,15 +114,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -176,32 +138,26 @@
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
-        # Enable client side validation
+        # Disable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
-        self.socket_options = None
-
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
                 setattr(result, k, copy.deepcopy(v, memo))
@@ -210,21 +166,14 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
@@ -271,15 +220,15 @@
         """
         self.__logger_file = value
         if self.__logger_file:
             # If set logging file,
             # then add file handler and remove stream handler.
             self.logger_file_handler = logging.FileHandler(self.__logger_file)
             self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.addHandler(self.logger_file_handler)
 
     @property
     def debug(self):
         """Debug status
 
         :param value: The debug status, True or False.
@@ -293,25 +242,25 @@
 
         :param value: The debug status, True or False.
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
-            for _, logger in self.logger.items():
+            for _, logger in six.iteritems(self.logger):
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -328,24 +277,23 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
-    def get_api_key_with_prefix(self, identifier, alias=None):
+    def get_api_key_with_prefix(self, identifier):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
-        :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
+        key = self.api_key.get(identifier)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
@@ -399,56 +347,41 @@
         return [
             {
                 'url': "https://api.cakemail.dev",
                 'description': "No description provided",
             }
         ]
 
-    def get_host_from_settings(self, index, variables=None, servers=None):
+    def get_host_from_settings(self, index, variables=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
-        :param servers: an array of host settings or None
         :return: URL based on host settings
         """
-        if index is None:
-            return self._base_path
-
         variables = {} if variables is None else variables
-        servers = self.get_host_settings() if servers is None else servers
+        servers = self.get_host_settings()
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
                 "Invalid index {0} when selecting the host settings. "
                 "Must be less than {1}".format(index, len(servers)))
 
         url = server['url']
 
         # go through variables and replace placeholders
-        for variable_name, variable in server.get('variables', {}).items():
+        for variable_name, variable in server['variables'].items():
             used_value = variables.get(
                 variable_name, variable['default_value'])
 
             if 'enum_values' in variable \
                     and used_value not in variable['enum_values']:
                 raise ValueError(
                     "The variable `{0}` in the host URL has invalid value "
                     "{1}. Must be {2}.".format(
                         variable_name, variables[variable_name],
                         variable['enum_values']))
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
-
-    @property
-    def host(self):
-        """Return generated host."""
-        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
-
-    @host.setter
-    def host(self, value):
-        """Fix base path."""
-        self._base_path = value
-        self.server_index = None
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/exceptions.py` & `cakemail-openapi-1.9.1/cakemail_openapi/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+import six
+
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
     def __init__(self, msg, path_to_item=None, valid_classes=None,
@@ -56,33 +60,14 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
-class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Raised when an attribute reference or assignment fails.
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiAttributeError, self).__init__(full_msg)
-
-
 class ApiKeyError(OpenApiException, KeyError):
     def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -120,40 +105,16 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
-        if isinstance(pth, int):
+        if isinstance(pth, six.integer_types):
             result += "[{0}]".format(pth)
         else:
             result += "['{0}']".format(pth)
     return result
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/models/__init__.py` & `cakemail-openapi-1.9.1/cakemail_openapi/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,310 +1,319 @@
+# coding: utf-8
+
 # flake8: noqa
+"""
+    Cakemail API
+
+    The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
+
+    The version of the OpenAPI document: 1.9.0
+    Generated by: https://openapi-generator.tech
+"""
+
 
-# import all models into this package
-# if you have many models here with many references from one model to another this may
-# raise a RecursionError
-# to avoid this, import only the models that you directly need like:
-# from from cakemail_openapi.model.pet import Pet
-# or import this package, but before doing it, use:
-# import sys
-# sys.setrecursionlimit(n)
+from __future__ import absolute_import
 
-from cakemail_openapi.model.accept_list_policy_response import AcceptListPolicyResponse
-from cakemail_openapi.model.account_full_response import AccountFullResponse
-from cakemail_openapi.model.account_owner import AccountOwner
-from cakemail_openapi.model.account_owner_response import AccountOwnerResponse
-from cakemail_openapi.model.account_owner_user import AccountOwnerUser
-from cakemail_openapi.model.account_response import AccountResponse
-from cakemail_openapi.model.account_stat_response import AccountStatResponse
-from cakemail_openapi.model.account_stats_response import AccountStatsResponse
-from cakemail_openapi.model.account_status import AccountStatus
-from cakemail_openapi.model.account_summary_response import AccountSummaryResponse
-from cakemail_openapi.model.accounts_response import AccountsResponse
-from cakemail_openapi.model.action import Action
-from cakemail_openapi.model.action_blueprint import ActionBlueprint
-from cakemail_openapi.model.action_condition import ActionCondition
-from cakemail_openapi.model.action_content import ActionContent
-from cakemail_openapi.model.action_default_email_settings import ActionDefaultEmailSettings
-from cakemail_openapi.model.action_email_blueprint_settings import ActionEmailBlueprintSettings
-from cakemail_openapi.model.action_email_settings import ActionEmailSettings
-from cakemail_openapi.model.action_log_response import ActionLogResponse
-from cakemail_openapi.model.action_logs_response import ActionLogsResponse
-from cakemail_openapi.model.action_response import ActionResponse
-from cakemail_openapi.model.action_stat_response import ActionStatResponse
-from cakemail_openapi.model.action_stats_response import ActionStatsResponse
-from cakemail_openapi.model.action_summary_response import ActionSummaryResponse
-from cakemail_openapi.model.action_tracking import ActionTracking
-from cakemail_openapi.model.action_type import ActionType
-from cakemail_openapi.model.actions_response import ActionsResponse
-from cakemail_openapi.model.activate_workflow_response import ActivateWorkflowResponse
-from cakemail_openapi.model.additional_email_header import AdditionalEmailHeader
-from cakemail_openapi.model.address import Address
-from cakemail_openapi.model.address_response import AddressResponse
-from cakemail_openapi.model.api_schemas_requests_lists_webhook import ApiSchemasRequestsListsWebhook
-from cakemail_openapi.model.api_services_webhooks_schemas_webhook import ApiServicesWebhooksSchemasWebhook
-from cakemail_openapi.model.archive_campaign_response import ArchiveCampaignResponse
-from cakemail_openapi.model.archive_list_response import ArchiveListResponse
-from cakemail_openapi.model.archive_webhook_response import ArchiveWebhookResponse
-from cakemail_openapi.model.audience import Audience
-from cakemail_openapi.model.audience_response import AudienceResponse
-from cakemail_openapi.model.audience_summary_response import AudienceSummaryResponse
-from cakemail_openapi.model.bad_request_message import BadRequestMessage
-from cakemail_openapi.model.browser_info import BrowserInfo
-from cakemail_openapi.model.campaign_blueprint_id import CampaignBlueprintId
-from cakemail_openapi.model.campaign_blueprint_response import CampaignBlueprintResponse
-from cakemail_openapi.model.campaign_blueprint_summary_response import CampaignBlueprintSummaryResponse
-from cakemail_openapi.model.campaign_blueprints_response import CampaignBlueprintsResponse
-from cakemail_openapi.model.campaign_content import CampaignContent
-from cakemail_openapi.model.campaign_content_response import CampaignContentResponse
-from cakemail_openapi.model.campaign_full_response import CampaignFullResponse
-from cakemail_openapi.model.campaign_link_stats_response import CampaignLinkStatsResponse
-from cakemail_openapi.model.campaign_links_stats_response import CampaignLinksStatsResponse
-from cakemail_openapi.model.campaign_log_response import CampaignLogResponse
-from cakemail_openapi.model.campaign_logs_response import CampaignLogsResponse
-from cakemail_openapi.model.campaign_response import CampaignResponse
-from cakemail_openapi.model.campaign_stat_response import CampaignStatResponse
-from cakemail_openapi.model.campaign_stats_response import CampaignStatsResponse
-from cakemail_openapi.model.campaign_status import CampaignStatus
-from cakemail_openapi.model.campaign_summary_response import CampaignSummaryResponse
-from cakemail_openapi.model.campaign_type import CampaignType
-from cakemail_openapi.model.campaigns_response import CampaignsResponse
-from cakemail_openapi.model.cancel_campaign_response import CancelCampaignResponse
-from cakemail_openapi.model.change_password import ChangePassword
-from cakemail_openapi.model.confirm_account import ConfirmAccount
-from cakemail_openapi.model.confirm_account_response import ConfirmAccountResponse
-from cakemail_openapi.model.confirm_sender import ConfirmSender
-from cakemail_openapi.model.confirm_sender_response import ConfirmSenderResponse
-from cakemail_openapi.model.confirm_user_response import ConfirmUserResponse
-from cakemail_openapi.model.contact import Contact
-from cakemail_openapi.model.contact_full_response import ContactFullResponse
-from cakemail_openapi.model.contact_response import ContactResponse
-from cakemail_openapi.model.contact_status import ContactStatus
-from cakemail_openapi.model.contacts_response import ContactsResponse
-from cakemail_openapi.model.content_type import ContentType
-from cakemail_openapi.model.content_type_response import ContentTypeResponse
-from cakemail_openapi.model.create_account import CreateAccount
-from cakemail_openapi.model.create_account_response import CreateAccountResponse
-from cakemail_openapi.model.create_action_response import CreateActionResponse
-from cakemail_openapi.model.create_attribute_response import CreateAttributeResponse
-from cakemail_openapi.model.create_campaign import CreateCampaign
-from cakemail_openapi.model.create_campaign_response import CreateCampaignResponse
-from cakemail_openapi.model.create_contact_response import CreateContactResponse
-from cakemail_openapi.model.create_custom_attribute import CreateCustomAttribute
-from cakemail_openapi.model.create_form import CreateForm
-from cakemail_openapi.model.create_form_response import CreateFormResponse
-from cakemail_openapi.model.create_list_response import CreateListResponse
-from cakemail_openapi.model.create_segment_response import CreateSegmentResponse
-from cakemail_openapi.model.create_sender import CreateSender
-from cakemail_openapi.model.create_sender_response import CreateSenderResponse
-from cakemail_openapi.model.create_suppressed_email_response import CreateSuppressedEmailResponse
-from cakemail_openapi.model.create_user_response import CreateUserResponse
-from cakemail_openapi.model.create_webhook import CreateWebhook
-from cakemail_openapi.model.create_webhook_response import CreateWebhookResponse
-from cakemail_openapi.model.create_workflow_response import CreateWorkflowResponse
-from cakemail_openapi.model.custom_attribute import CustomAttribute
-from cakemail_openapi.model.custom_attribute_full_response import CustomAttributeFullResponse
-from cakemail_openapi.model.custom_attribute_response import CustomAttributeResponse
-from cakemail_openapi.model.custom_attribute_type import CustomAttributeType
-from cakemail_openapi.model.custom_attributes_data_response import CustomAttributesDataResponse
-from cakemail_openapi.model.custom_attributes_response import CustomAttributesResponse
-from cakemail_openapi.model.deactivate_workflow_response import DeactivateWorkflowResponse
-from cakemail_openapi.model.delete_account_response import DeleteAccountResponse
-from cakemail_openapi.model.delete_action_response import DeleteActionResponse
-from cakemail_openapi.model.delete_campaign_response import DeleteCampaignResponse
-from cakemail_openapi.model.delete_contact_response import DeleteContactResponse
-from cakemail_openapi.model.delete_custom_attribute_response import DeleteCustomAttributeResponse
-from cakemail_openapi.model.delete_form_response import DeleteFormResponse
-from cakemail_openapi.model.delete_list_response import DeleteListResponse
-from cakemail_openapi.model.delete_segment_response import DeleteSegmentResponse
-from cakemail_openapi.model.delete_sender_response import DeleteSenderResponse
-from cakemail_openapi.model.delete_suppressed_email_response import DeleteSuppressedEmailResponse
-from cakemail_openapi.model.delete_template_response import DeleteTemplateResponse
-from cakemail_openapi.model.delete_user_response import DeleteUserResponse
-from cakemail_openapi.model.delete_workflow_response import DeleteWorkflowResponse
-from cakemail_openapi.model.device_family_enum import DeviceFamilyEnum
-from cakemail_openapi.model.device_info import DeviceInfo
-from cakemail_openapi.model.domain_instruction_response import DomainInstructionResponse
-from cakemail_openapi.model.domains import Domains
-from cakemail_openapi.model.domains_full_response import DomainsFullResponse
-from cakemail_openapi.model.domains_instruction_response import DomainsInstructionResponse
-from cakemail_openapi.model.domains_response import DomainsResponse
-from cakemail_openapi.model.double_opt_in import DoubleOptIn
-from cakemail_openapi.model.email import Email
-from cakemail_openapi.model.email_content import EmailContent
-from cakemail_openapi.model.email_log_response import EmailLogResponse
-from cakemail_openapi.model.email_logs_response import EmailLogsResponse
-from cakemail_openapi.model.email_stat_response import EmailStatResponse
-from cakemail_openapi.model.email_stats_response import EmailStatsResponse
-from cakemail_openapi.model.email_tracking import EmailTracking
-from cakemail_openapi.model.encoding import Encoding
-from cakemail_openapi.model.encoding_response import EncodingResponse
-from cakemail_openapi.model.event_type import EventType
-from cakemail_openapi.model.event_type_response import EventTypeResponse
-from cakemail_openapi.model.forbidden_message import ForbiddenMessage
-from cakemail_openapi.model.forgot_my_password import ForgotMyPassword
-from cakemail_openapi.model.form_content import FormContent
-from cakemail_openapi.model.form_content_response import FormContentResponse
-from cakemail_openapi.model.form_full_response import FormFullResponse
-from cakemail_openapi.model.form_redirections import FormRedirections
-from cakemail_openapi.model.form_redirections_response import FormRedirectionsResponse
-from cakemail_openapi.model.form_response import FormResponse
-from cakemail_openapi.model.form_status import FormStatus
-from cakemail_openapi.model.form_urls_response import FormUrlsResponse
-from cakemail_openapi.model.forms_response import FormsResponse
-from cakemail_openapi.model.get_action_response import GetActionResponse
-from cakemail_openapi.model.get_workflow_response import GetWorkflowResponse
-from cakemail_openapi.model.http_bad_request_error import HTTPBadRequestError
-from cakemail_openapi.model.http_forbidden_error import HTTPForbiddenError
-from cakemail_openapi.model.http_unauthorized_error import HTTPUnauthorizedError
-from cakemail_openapi.model.http_validation_error import HTTPValidationError
-from cakemail_openapi.model.import_contact_data import ImportContactData
-from cakemail_openapi.model.import_contacts import ImportContacts
-from cakemail_openapi.model.import_contacts_response import ImportContactsResponse
-from cakemail_openapi.model.languages import Languages
-from cakemail_openapi.model.link_full_response import LinkFullResponse
-from cakemail_openapi.model.link_info_full_response import LinkInfoFullResponse
-from cakemail_openapi.model.link_info_response import LinkInfoResponse
-from cakemail_openapi.model.links_response import LinksResponse
-from cakemail_openapi.model.list import List
-from cakemail_openapi.model.list_full_response import ListFullResponse
-from cakemail_openapi.model.list_log_response import ListLogResponse
-from cakemail_openapi.model.list_logs_response import ListLogsResponse
-from cakemail_openapi.model.list_pages_response import ListPagesResponse
-from cakemail_openapi.model.list_redirections_response import ListRedirectionsResponse
-from cakemail_openapi.model.list_response import ListResponse
-from cakemail_openapi.model.list_sender_response import ListSenderResponse
-from cakemail_openapi.model.list_stat_response import ListStatResponse
-from cakemail_openapi.model.list_stats_response import ListStatsResponse
-from cakemail_openapi.model.list_summary_response import ListSummaryResponse
-from cakemail_openapi.model.list_webhook_action import ListWebhookAction
-from cakemail_openapi.model.list_webhook_response import ListWebhookResponse
-from cakemail_openapi.model.list_webhooks_response import ListWebhooksResponse
-from cakemail_openapi.model.list_workflows_response import ListWorkflowsResponse
-from cakemail_openapi.model.lists_response import ListsResponse
-from cakemail_openapi.model.lock_workflow import LockWorkflow
-from cakemail_openapi.model.lock_workflow_response import LockWorkflowResponse
-from cakemail_openapi.model.log_type import LogType
-from cakemail_openapi.model.operating_system_info import OperatingSystemInfo
-from cakemail_openapi.model.pagination import Pagination
-from cakemail_openapi.model.patch_account import PatchAccount
-from cakemail_openapi.model.patch_account_response import PatchAccountResponse
-from cakemail_openapi.model.patch_action import PatchAction
-from cakemail_openapi.model.patch_action_content import PatchActionContent
-from cakemail_openapi.model.patch_action_email_settings import PatchActionEmailSettings
-from cakemail_openapi.model.patch_action_response import PatchActionResponse
-from cakemail_openapi.model.patch_action_tracking import PatchActionTracking
-from cakemail_openapi.model.patch_campaign import PatchCampaign
-from cakemail_openapi.model.patch_campaign_content import PatchCampaignContent
-from cakemail_openapi.model.patch_campaign_response import PatchCampaignResponse
-from cakemail_openapi.model.patch_contact import PatchContact
-from cakemail_openapi.model.patch_contact_response import PatchContactResponse
-from cakemail_openapi.model.patch_domains import PatchDomains
-from cakemail_openapi.model.patch_domains_response import PatchDomainsResponse
-from cakemail_openapi.model.patch_form import PatchForm
-from cakemail_openapi.model.patch_form_response import PatchFormResponse
-from cakemail_openapi.model.patch_list_response import PatchListResponse
-from cakemail_openapi.model.patch_segment_response import PatchSegmentResponse
-from cakemail_openapi.model.patch_self_account import PatchSelfAccount
-from cakemail_openapi.model.patch_sender_response import PatchSenderResponse
-from cakemail_openapi.model.patch_template import PatchTemplate
-from cakemail_openapi.model.patch_template_content import PatchTemplateContent
-from cakemail_openapi.model.patch_template_response import PatchTemplateResponse
-from cakemail_openapi.model.patch_tracking import PatchTracking
-from cakemail_openapi.model.patch_user import PatchUser
-from cakemail_openapi.model.patch_user_response import PatchUserResponse
-from cakemail_openapi.model.patch_webhook import PatchWebhook
-from cakemail_openapi.model.patch_webhook_response import PatchWebhookResponse
-from cakemail_openapi.model.patch_workflow import PatchWorkflow
-from cakemail_openapi.model.patch_workflow_response import PatchWorkflowResponse
-from cakemail_openapi.model.put_system_emails_response import PutSystemEmailsResponse
-from cakemail_openapi.model.rate_limit_period import RateLimitPeriod
-from cakemail_openapi.model.redirections import Redirections
-from cakemail_openapi.model.render_campaign_full_response import RenderCampaignFullResponse
-from cakemail_openapi.model.render_campaign_response import RenderCampaignResponse
-from cakemail_openapi.model.resend_account_verification_email_response import ResendAccountVerificationEmailResponse
-from cakemail_openapi.model.resend_confirmation_email_response import ResendConfirmationEmailResponse
-from cakemail_openapi.model.resend_user_verification_email_response import ResendUserVerificationEmailResponse
-from cakemail_openapi.model.resend_verification_email import ResendVerificationEmail
-from cakemail_openapi.model.reset_password_confirm import ResetPasswordConfirm
-from cakemail_openapi.model.reset_password_confirm_response import ResetPasswordConfirmResponse
-from cakemail_openapi.model.reset_password_response import ResetPasswordResponse
-from cakemail_openapi.model.reset_user_password import ResetUserPassword
-from cakemail_openapi.model.resume_campaign_response import ResumeCampaignResponse
-from cakemail_openapi.model.schedule_campaign import ScheduleCampaign
-from cakemail_openapi.model.schedule_campaign_response import ScheduleCampaignResponse
-from cakemail_openapi.model.segment import Segment
-from cakemail_openapi.model.segment_full_response import SegmentFullResponse
-from cakemail_openapi.model.segment_response import SegmentResponse
-from cakemail_openapi.model.segments_response import SegmentsResponse
-from cakemail_openapi.model.send_email_response import SendEmailResponse
-from cakemail_openapi.model.send_test_action import SendTestAction
-from cakemail_openapi.model.send_test_action_response import SendTestActionResponse
-from cakemail_openapi.model.send_test_email import SendTestEmail
-from cakemail_openapi.model.send_test_email_response import SendTestEmailResponse
-from cakemail_openapi.model.sender import Sender
-from cakemail_openapi.model.sender_and_name import SenderAndName
-from cakemail_openapi.model.sender_full_response import SenderFullResponse
-from cakemail_openapi.model.sender_response import SenderResponse
-from cakemail_openapi.model.senders_response import SendersResponse
-from cakemail_openapi.model.signature_hash_function import SignatureHashFunction
-from cakemail_openapi.model.signature_info import SignatureInfo
-from cakemail_openapi.model.suppressed_email import SuppressedEmail
-from cakemail_openapi.model.suppressed_email_response import SuppressedEmailResponse
-from cakemail_openapi.model.suppressed_emails_response import SuppressedEmailsResponse
-from cakemail_openapi.model.suspend_account_response import SuspendAccountResponse
-from cakemail_openapi.model.suspend_campaign_response import SuspendCampaignResponse
-from cakemail_openapi.model.suspend_user_response import SuspendUserResponse
-from cakemail_openapi.model.system_email_template import SystemEmailTemplate
-from cakemail_openapi.model.system_emails_response import SystemEmailsResponse
-from cakemail_openapi.model.system_emails_templates import SystemEmailsTemplates
-from cakemail_openapi.model.template import Template
-from cakemail_openapi.model.template_content import TemplateContent
-from cakemail_openapi.model.template_content_response import TemplateContentResponse
-from cakemail_openapi.model.template_created import TemplateCreated
-from cakemail_openapi.model.template_custom_attributes import TemplateCustomAttributes
-from cakemail_openapi.model.template_full_response import TemplateFullResponse
-from cakemail_openapi.model.template_id import TemplateId
-from cakemail_openapi.model.template_info import TemplateInfo
-from cakemail_openapi.model.template_response import TemplateResponse
-from cakemail_openapi.model.template_summary_response import TemplateSummaryResponse
-from cakemail_openapi.model.template_type_enum import TemplateTypeEnum
-from cakemail_openapi.model.templates_response import TemplatesResponse
-from cakemail_openapi.model.test_email_type import TestEmailType
-from cakemail_openapi.model.token_response import TokenResponse
-from cakemail_openapi.model.tracking import Tracking
-from cakemail_openapi.model.tracking_response import TrackingResponse
-from cakemail_openapi.model.un_archive_webhook_response import UnArchiveWebhookResponse
-from cakemail_openapi.model.unarchive_list_response import UnarchiveListResponse
-from cakemail_openapi.model.unauthorized_message import UnauthorizedMessage
-from cakemail_openapi.model.unlock_workflow import UnlockWorkflow
-from cakemail_openapi.model.unlock_workflow_response import UnlockWorkflowResponse
-from cakemail_openapi.model.unsubscribe_contact_response import UnsubscribeContactResponse
-from cakemail_openapi.model.unsuspend_account_response import UnsuspendAccountResponse
-from cakemail_openapi.model.update_list import UpdateList
-from cakemail_openapi.model.update_segment import UpdateSegment
-from cakemail_openapi.model.update_sender import UpdateSender
-from cakemail_openapi.model.upload_logo import UploadLogo
-from cakemail_openapi.model.upload_logo_response import UploadLogoResponse
-from cakemail_openapi.model.usage_limits import UsageLimits
-from cakemail_openapi.model.usage_limits_response import UsageLimitsResponse
-from cakemail_openapi.model.user import User
-from cakemail_openapi.model.user_confirmation import UserConfirmation
-from cakemail_openapi.model.user_full_response import UserFullResponse
-from cakemail_openapi.model.user_info import UserInfo
-from cakemail_openapi.model.user_response import UserResponse
-from cakemail_openapi.model.user_summary_response import UserSummaryResponse
-from cakemail_openapi.model.users_response import UsersResponse
-from cakemail_openapi.model.validate_domains_response import ValidateDomainsResponse
-from cakemail_openapi.model.validation_error import ValidationError
-from cakemail_openapi.model.webhook_response import WebhookResponse
-from cakemail_openapi.model.webhook_status import WebhookStatus
-from cakemail_openapi.model.workflow import Workflow
-from cakemail_openapi.model.workflow_audience import WorkflowAudience
-from cakemail_openapi.model.workflow_blueprint import WorkflowBlueprint
-from cakemail_openapi.model.workflow_blueprint_action_response import WorkflowBlueprintActionResponse
-from cakemail_openapi.model.workflow_blueprint_response import WorkflowBlueprintResponse
-from cakemail_openapi.model.workflow_blueprints_response import WorkflowBlueprintsResponse
-from cakemail_openapi.model.workflow_from_blueprint import WorkflowFromBlueprint
-from cakemail_openapi.model.workflow_response import WorkflowResponse
-from cakemail_openapi.model.workflow_status import WorkflowStatus
-from cakemail_openapi.model.workflow_trigger import WorkflowTrigger
+# import models into model package
+from cakemail_openapi.models.accept_list_policy_response import AcceptListPolicyResponse
+from cakemail_openapi.models.account_full_response import AccountFullResponse
+from cakemail_openapi.models.account_owner import AccountOwner
+from cakemail_openapi.models.account_owner_response import AccountOwnerResponse
+from cakemail_openapi.models.account_owner_user import AccountOwnerUser
+from cakemail_openapi.models.account_response import AccountResponse
+from cakemail_openapi.models.account_stat_response import AccountStatResponse
+from cakemail_openapi.models.account_stats_response import AccountStatsResponse
+from cakemail_openapi.models.account_status import AccountStatus
+from cakemail_openapi.models.account_summary_response import AccountSummaryResponse
+from cakemail_openapi.models.accounts_response import AccountsResponse
+from cakemail_openapi.models.action import Action
+from cakemail_openapi.models.action_blueprint import ActionBlueprint
+from cakemail_openapi.models.action_condition import ActionCondition
+from cakemail_openapi.models.action_content import ActionContent
+from cakemail_openapi.models.action_default_email_settings import ActionDefaultEmailSettings
+from cakemail_openapi.models.action_email_blueprint_settings import ActionEmailBlueprintSettings
+from cakemail_openapi.models.action_email_settings import ActionEmailSettings
+from cakemail_openapi.models.action_log_response import ActionLogResponse
+from cakemail_openapi.models.action_logs_response import ActionLogsResponse
+from cakemail_openapi.models.action_response import ActionResponse
+from cakemail_openapi.models.action_stat_response import ActionStatResponse
+from cakemail_openapi.models.action_stats_response import ActionStatsResponse
+from cakemail_openapi.models.action_summary_response import ActionSummaryResponse
+from cakemail_openapi.models.action_tracking import ActionTracking
+from cakemail_openapi.models.action_type import ActionType
+from cakemail_openapi.models.actions_response import ActionsResponse
+from cakemail_openapi.models.activate_workflow_response import ActivateWorkflowResponse
+from cakemail_openapi.models.additional_email_header import AdditionalEmailHeader
+from cakemail_openapi.models.address import Address
+from cakemail_openapi.models.address_response import AddressResponse
+from cakemail_openapi.models.api_schemas_requests_lists_webhook import ApiSchemasRequestsListsWebhook
+from cakemail_openapi.models.api_services_webhooks_schemas_webhook import ApiServicesWebhooksSchemasWebhook
+from cakemail_openapi.models.archive_campaign_response import ArchiveCampaignResponse
+from cakemail_openapi.models.archive_list_response import ArchiveListResponse
+from cakemail_openapi.models.archive_webhook_response import ArchiveWebhookResponse
+from cakemail_openapi.models.audience import Audience
+from cakemail_openapi.models.audience_response import AudienceResponse
+from cakemail_openapi.models.audience_summary_response import AudienceSummaryResponse
+from cakemail_openapi.models.bad_request_message import BadRequestMessage
+from cakemail_openapi.models.body_create_token_token_post import BodyCreateTokenTokenPost
+from cakemail_openapi.models.body_refresh_token_token_put import BodyRefreshTokenTokenPut
+from cakemail_openapi.models.browser_info import BrowserInfo
+from cakemail_openapi.models.campaign_blueprint_id import CampaignBlueprintId
+from cakemail_openapi.models.campaign_blueprint_response import CampaignBlueprintResponse
+from cakemail_openapi.models.campaign_blueprint_summary_response import CampaignBlueprintSummaryResponse
+from cakemail_openapi.models.campaign_blueprints_response import CampaignBlueprintsResponse
+from cakemail_openapi.models.campaign_content import CampaignContent
+from cakemail_openapi.models.campaign_content_response import CampaignContentResponse
+from cakemail_openapi.models.campaign_full_response import CampaignFullResponse
+from cakemail_openapi.models.campaign_link_stats_response import CampaignLinkStatsResponse
+from cakemail_openapi.models.campaign_links_stats_response import CampaignLinksStatsResponse
+from cakemail_openapi.models.campaign_log_response import CampaignLogResponse
+from cakemail_openapi.models.campaign_logs_response import CampaignLogsResponse
+from cakemail_openapi.models.campaign_response import CampaignResponse
+from cakemail_openapi.models.campaign_stat_response import CampaignStatResponse
+from cakemail_openapi.models.campaign_stats_response import CampaignStatsResponse
+from cakemail_openapi.models.campaign_status import CampaignStatus
+from cakemail_openapi.models.campaign_summary_response import CampaignSummaryResponse
+from cakemail_openapi.models.campaign_type import CampaignType
+from cakemail_openapi.models.campaigns_response import CampaignsResponse
+from cakemail_openapi.models.cancel_campaign_response import CancelCampaignResponse
+from cakemail_openapi.models.change_password import ChangePassword
+from cakemail_openapi.models.confirm_account import ConfirmAccount
+from cakemail_openapi.models.confirm_account_response import ConfirmAccountResponse
+from cakemail_openapi.models.confirm_sender import ConfirmSender
+from cakemail_openapi.models.confirm_sender_response import ConfirmSenderResponse
+from cakemail_openapi.models.confirm_user_response import ConfirmUserResponse
+from cakemail_openapi.models.contact import Contact
+from cakemail_openapi.models.contact_full_response import ContactFullResponse
+from cakemail_openapi.models.contact_response import ContactResponse
+from cakemail_openapi.models.contact_status import ContactStatus
+from cakemail_openapi.models.contacts_response import ContactsResponse
+from cakemail_openapi.models.content_type import ContentType
+from cakemail_openapi.models.content_type_response import ContentTypeResponse
+from cakemail_openapi.models.create_account import CreateAccount
+from cakemail_openapi.models.create_account_response import CreateAccountResponse
+from cakemail_openapi.models.create_action_response import CreateActionResponse
+from cakemail_openapi.models.create_attribute_response import CreateAttributeResponse
+from cakemail_openapi.models.create_campaign import CreateCampaign
+from cakemail_openapi.models.create_campaign_response import CreateCampaignResponse
+from cakemail_openapi.models.create_contact_response import CreateContactResponse
+from cakemail_openapi.models.create_custom_attribute import CreateCustomAttribute
+from cakemail_openapi.models.create_form import CreateForm
+from cakemail_openapi.models.create_form_response import CreateFormResponse
+from cakemail_openapi.models.create_list_response import CreateListResponse
+from cakemail_openapi.models.create_segment_response import CreateSegmentResponse
+from cakemail_openapi.models.create_sender import CreateSender
+from cakemail_openapi.models.create_sender_response import CreateSenderResponse
+from cakemail_openapi.models.create_suppressed_email_response import CreateSuppressedEmailResponse
+from cakemail_openapi.models.create_user_response import CreateUserResponse
+from cakemail_openapi.models.create_webhook import CreateWebhook
+from cakemail_openapi.models.create_webhook_response import CreateWebhookResponse
+from cakemail_openapi.models.create_workflow_response import CreateWorkflowResponse
+from cakemail_openapi.models.custom_attribute import CustomAttribute
+from cakemail_openapi.models.custom_attribute_full_response import CustomAttributeFullResponse
+from cakemail_openapi.models.custom_attribute_response import CustomAttributeResponse
+from cakemail_openapi.models.custom_attribute_type import CustomAttributeType
+from cakemail_openapi.models.custom_attributes_data_response import CustomAttributesDataResponse
+from cakemail_openapi.models.custom_attributes_response import CustomAttributesResponse
+from cakemail_openapi.models.deactivate_workflow_response import DeactivateWorkflowResponse
+from cakemail_openapi.models.delete_account_response import DeleteAccountResponse
+from cakemail_openapi.models.delete_action_response import DeleteActionResponse
+from cakemail_openapi.models.delete_campaign_response import DeleteCampaignResponse
+from cakemail_openapi.models.delete_contact_response import DeleteContactResponse
+from cakemail_openapi.models.delete_custom_attribute_response import DeleteCustomAttributeResponse
+from cakemail_openapi.models.delete_form_response import DeleteFormResponse
+from cakemail_openapi.models.delete_list_response import DeleteListResponse
+from cakemail_openapi.models.delete_segment_response import DeleteSegmentResponse
+from cakemail_openapi.models.delete_sender_response import DeleteSenderResponse
+from cakemail_openapi.models.delete_suppressed_email_response import DeleteSuppressedEmailResponse
+from cakemail_openapi.models.delete_template_response import DeleteTemplateResponse
+from cakemail_openapi.models.delete_user_response import DeleteUserResponse
+from cakemail_openapi.models.delete_workflow_response import DeleteWorkflowResponse
+from cakemail_openapi.models.device_family_enum import DeviceFamilyEnum
+from cakemail_openapi.models.device_info import DeviceInfo
+from cakemail_openapi.models.domain_instruction_response import DomainInstructionResponse
+from cakemail_openapi.models.domains import Domains
+from cakemail_openapi.models.domains_full_response import DomainsFullResponse
+from cakemail_openapi.models.domains_instruction_response import DomainsInstructionResponse
+from cakemail_openapi.models.domains_response import DomainsResponse
+from cakemail_openapi.models.double_opt_in import DoubleOptIn
+from cakemail_openapi.models.email import Email
+from cakemail_openapi.models.email_content import EmailContent
+from cakemail_openapi.models.email_log_response import EmailLogResponse
+from cakemail_openapi.models.email_logs_response import EmailLogsResponse
+from cakemail_openapi.models.email_stat_response import EmailStatResponse
+from cakemail_openapi.models.email_stats_response import EmailStatsResponse
+from cakemail_openapi.models.email_tracking import EmailTracking
+from cakemail_openapi.models.encoding import Encoding
+from cakemail_openapi.models.encoding_response import EncodingResponse
+from cakemail_openapi.models.event_type import EventType
+from cakemail_openapi.models.event_type_response import EventTypeResponse
+from cakemail_openapi.models.forbidden_message import ForbiddenMessage
+from cakemail_openapi.models.forgot_my_password import ForgotMyPassword
+from cakemail_openapi.models.form_content import FormContent
+from cakemail_openapi.models.form_content_response import FormContentResponse
+from cakemail_openapi.models.form_full_response import FormFullResponse
+from cakemail_openapi.models.form_redirections import FormRedirections
+from cakemail_openapi.models.form_redirections_response import FormRedirectionsResponse
+from cakemail_openapi.models.form_response import FormResponse
+from cakemail_openapi.models.form_status import FormStatus
+from cakemail_openapi.models.form_urls_response import FormUrlsResponse
+from cakemail_openapi.models.forms_response import FormsResponse
+from cakemail_openapi.models.get_action_response import GetActionResponse
+from cakemail_openapi.models.get_workflow_response import GetWorkflowResponse
+from cakemail_openapi.models.http_bad_request_error import HTTPBadRequestError
+from cakemail_openapi.models.http_forbidden_error import HTTPForbiddenError
+from cakemail_openapi.models.http_unauthorized_error import HTTPUnauthorizedError
+from cakemail_openapi.models.http_validation_error import HTTPValidationError
+from cakemail_openapi.models.import_contact_data import ImportContactData
+from cakemail_openapi.models.import_contacts import ImportContacts
+from cakemail_openapi.models.import_contacts_response import ImportContactsResponse
+from cakemail_openapi.models.languages import Languages
+from cakemail_openapi.models.link_full_response import LinkFullResponse
+from cakemail_openapi.models.link_info_full_response import LinkInfoFullResponse
+from cakemail_openapi.models.link_info_response import LinkInfoResponse
+from cakemail_openapi.models.links_response import LinksResponse
+from cakemail_openapi.models.list import List
+from cakemail_openapi.models.list_full_response import ListFullResponse
+from cakemail_openapi.models.list_log_response import ListLogResponse
+from cakemail_openapi.models.list_logs_response import ListLogsResponse
+from cakemail_openapi.models.list_pages_response import ListPagesResponse
+from cakemail_openapi.models.list_redirections_response import ListRedirectionsResponse
+from cakemail_openapi.models.list_response import ListResponse
+from cakemail_openapi.models.list_sender_response import ListSenderResponse
+from cakemail_openapi.models.list_stat_response import ListStatResponse
+from cakemail_openapi.models.list_stats_response import ListStatsResponse
+from cakemail_openapi.models.list_summary_response import ListSummaryResponse
+from cakemail_openapi.models.list_webhook_action import ListWebhookAction
+from cakemail_openapi.models.list_webhook_response import ListWebhookResponse
+from cakemail_openapi.models.list_webhooks_response import ListWebhooksResponse
+from cakemail_openapi.models.list_workflows_response import ListWorkflowsResponse
+from cakemail_openapi.models.lists_response import ListsResponse
+from cakemail_openapi.models.lock_workflow import LockWorkflow
+from cakemail_openapi.models.lock_workflow_response import LockWorkflowResponse
+from cakemail_openapi.models.log_type import LogType
+from cakemail_openapi.models.operating_system_info import OperatingSystemInfo
+from cakemail_openapi.models.pagination import Pagination
+from cakemail_openapi.models.password_grant_type import PasswordGrantType
+from cakemail_openapi.models.patch_account import PatchAccount
+from cakemail_openapi.models.patch_account_response import PatchAccountResponse
+from cakemail_openapi.models.patch_action import PatchAction
+from cakemail_openapi.models.patch_action_content import PatchActionContent
+from cakemail_openapi.models.patch_action_email_settings import PatchActionEmailSettings
+from cakemail_openapi.models.patch_action_response import PatchActionResponse
+from cakemail_openapi.models.patch_action_tracking import PatchActionTracking
+from cakemail_openapi.models.patch_campaign import PatchCampaign
+from cakemail_openapi.models.patch_campaign_content import PatchCampaignContent
+from cakemail_openapi.models.patch_campaign_response import PatchCampaignResponse
+from cakemail_openapi.models.patch_contact import PatchContact
+from cakemail_openapi.models.patch_contact_response import PatchContactResponse
+from cakemail_openapi.models.patch_domains import PatchDomains
+from cakemail_openapi.models.patch_domains_response import PatchDomainsResponse
+from cakemail_openapi.models.patch_form import PatchForm
+from cakemail_openapi.models.patch_form_response import PatchFormResponse
+from cakemail_openapi.models.patch_list_response import PatchListResponse
+from cakemail_openapi.models.patch_segment_response import PatchSegmentResponse
+from cakemail_openapi.models.patch_self_account import PatchSelfAccount
+from cakemail_openapi.models.patch_sender_response import PatchSenderResponse
+from cakemail_openapi.models.patch_template import PatchTemplate
+from cakemail_openapi.models.patch_template_content import PatchTemplateContent
+from cakemail_openapi.models.patch_template_response import PatchTemplateResponse
+from cakemail_openapi.models.patch_tracking import PatchTracking
+from cakemail_openapi.models.patch_user import PatchUser
+from cakemail_openapi.models.patch_user_response import PatchUserResponse
+from cakemail_openapi.models.patch_webhook import PatchWebhook
+from cakemail_openapi.models.patch_webhook_response import PatchWebhookResponse
+from cakemail_openapi.models.patch_workflow import PatchWorkflow
+from cakemail_openapi.models.patch_workflow_response import PatchWorkflowResponse
+from cakemail_openapi.models.put_system_emails_response import PutSystemEmailsResponse
+from cakemail_openapi.models.rate_limit_period import RateLimitPeriod
+from cakemail_openapi.models.redirections import Redirections
+from cakemail_openapi.models.refresh_grant_type import RefreshGrantType
+from cakemail_openapi.models.render_campaign_full_response import RenderCampaignFullResponse
+from cakemail_openapi.models.render_campaign_response import RenderCampaignResponse
+from cakemail_openapi.models.resend_account_verification_email_response import ResendAccountVerificationEmailResponse
+from cakemail_openapi.models.resend_confirmation_email_response import ResendConfirmationEmailResponse
+from cakemail_openapi.models.resend_user_verification_email_response import ResendUserVerificationEmailResponse
+from cakemail_openapi.models.resend_verification_email import ResendVerificationEmail
+from cakemail_openapi.models.reset_password_confirm import ResetPasswordConfirm
+from cakemail_openapi.models.reset_password_confirm_response import ResetPasswordConfirmResponse
+from cakemail_openapi.models.reset_password_response import ResetPasswordResponse
+from cakemail_openapi.models.reset_user_password import ResetUserPassword
+from cakemail_openapi.models.resume_campaign_response import ResumeCampaignResponse
+from cakemail_openapi.models.schedule_campaign import ScheduleCampaign
+from cakemail_openapi.models.schedule_campaign_response import ScheduleCampaignResponse
+from cakemail_openapi.models.segment import Segment
+from cakemail_openapi.models.segment_full_response import SegmentFullResponse
+from cakemail_openapi.models.segment_response import SegmentResponse
+from cakemail_openapi.models.segments_response import SegmentsResponse
+from cakemail_openapi.models.send_email_response import SendEmailResponse
+from cakemail_openapi.models.send_test_action import SendTestAction
+from cakemail_openapi.models.send_test_action_response import SendTestActionResponse
+from cakemail_openapi.models.send_test_email import SendTestEmail
+from cakemail_openapi.models.send_test_email_response import SendTestEmailResponse
+from cakemail_openapi.models.sender import Sender
+from cakemail_openapi.models.sender_and_name import SenderAndName
+from cakemail_openapi.models.sender_full_response import SenderFullResponse
+from cakemail_openapi.models.sender_response import SenderResponse
+from cakemail_openapi.models.senders_response import SendersResponse
+from cakemail_openapi.models.signature_hash_function import SignatureHashFunction
+from cakemail_openapi.models.signature_info import SignatureInfo
+from cakemail_openapi.models.suppressed_email import SuppressedEmail
+from cakemail_openapi.models.suppressed_email_response import SuppressedEmailResponse
+from cakemail_openapi.models.suppressed_emails_response import SuppressedEmailsResponse
+from cakemail_openapi.models.suspend_account_response import SuspendAccountResponse
+from cakemail_openapi.models.suspend_campaign_response import SuspendCampaignResponse
+from cakemail_openapi.models.suspend_user_response import SuspendUserResponse
+from cakemail_openapi.models.system_email_template import SystemEmailTemplate
+from cakemail_openapi.models.system_emails_response import SystemEmailsResponse
+from cakemail_openapi.models.system_emails_templates import SystemEmailsTemplates
+from cakemail_openapi.models.template import Template
+from cakemail_openapi.models.template_content import TemplateContent
+from cakemail_openapi.models.template_content_response import TemplateContentResponse
+from cakemail_openapi.models.template_created import TemplateCreated
+from cakemail_openapi.models.template_custom_attributes import TemplateCustomAttributes
+from cakemail_openapi.models.template_full_response import TemplateFullResponse
+from cakemail_openapi.models.template_id import TemplateId
+from cakemail_openapi.models.template_info import TemplateInfo
+from cakemail_openapi.models.template_response import TemplateResponse
+from cakemail_openapi.models.template_summary_response import TemplateSummaryResponse
+from cakemail_openapi.models.template_type_enum import TemplateTypeEnum
+from cakemail_openapi.models.templates_response import TemplatesResponse
+from cakemail_openapi.models.test_email_type import TestEmailType
+from cakemail_openapi.models.token_response import TokenResponse
+from cakemail_openapi.models.tracking import Tracking
+from cakemail_openapi.models.tracking_response import TrackingResponse
+from cakemail_openapi.models.un_archive_webhook_response import UnArchiveWebhookResponse
+from cakemail_openapi.models.unarchive_list_response import UnarchiveListResponse
+from cakemail_openapi.models.unauthorized_message import UnauthorizedMessage
+from cakemail_openapi.models.unlock_workflow import UnlockWorkflow
+from cakemail_openapi.models.unlock_workflow_response import UnlockWorkflowResponse
+from cakemail_openapi.models.unsubscribe_contact_response import UnsubscribeContactResponse
+from cakemail_openapi.models.unsuspend_account_response import UnsuspendAccountResponse
+from cakemail_openapi.models.update_list import UpdateList
+from cakemail_openapi.models.update_segment import UpdateSegment
+from cakemail_openapi.models.update_sender import UpdateSender
+from cakemail_openapi.models.upload_logo import UploadLogo
+from cakemail_openapi.models.upload_logo_response import UploadLogoResponse
+from cakemail_openapi.models.usage_limits import UsageLimits
+from cakemail_openapi.models.usage_limits_response import UsageLimitsResponse
+from cakemail_openapi.models.user import User
+from cakemail_openapi.models.user_confirmation import UserConfirmation
+from cakemail_openapi.models.user_full_response import UserFullResponse
+from cakemail_openapi.models.user_info import UserInfo
+from cakemail_openapi.models.user_response import UserResponse
+from cakemail_openapi.models.user_summary_response import UserSummaryResponse
+from cakemail_openapi.models.users_response import UsersResponse
+from cakemail_openapi.models.validate_domains_response import ValidateDomainsResponse
+from cakemail_openapi.models.validation_error import ValidationError
+from cakemail_openapi.models.webhook_response import WebhookResponse
+from cakemail_openapi.models.webhook_status import WebhookStatus
+from cakemail_openapi.models.workflow import Workflow
+from cakemail_openapi.models.workflow_audience import WorkflowAudience
+from cakemail_openapi.models.workflow_blueprint import WorkflowBlueprint
+from cakemail_openapi.models.workflow_blueprint_action_response import WorkflowBlueprintActionResponse
+from cakemail_openapi.models.workflow_blueprint_response import WorkflowBlueprintResponse
+from cakemail_openapi.models.workflow_blueprints_response import WorkflowBlueprintsResponse
+from cakemail_openapi.models.workflow_from_blueprint import WorkflowFromBlueprint
+from cakemail_openapi.models.workflow_response import WorkflowResponse
+from cakemail_openapi.models.workflow_status import WorkflowStatus
+from cakemail_openapi.models.workflow_trigger import WorkflowTrigger
```

### Comparing `cakemail-openapi-1.9.0/cakemail_openapi/rest.py` & `cakemail-openapi-1.9.1/cakemail_openapi/rest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+# coding: utf-8
+
 """
     Cakemail API
 
     The Cakemail API exposes multiple APIs including Authentication, Marketing, Contact, Transactional, Analytic, Content, Account and Partner.  # noqa: E501
 
     The version of the OpenAPI document: 1.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+from __future__ import absolute_import
+
 import io
 import json
 import logging
 import re
 import ssl
-from urllib.parse import urlencode
-from urllib.parse import urlparse
-from urllib.request import proxy_bypass_environment
+
+import certifi
+# python 2 and python 3 compatibility library
+import six
+from six.moves.urllib.parse import urlencode
 import urllib3
-import ipaddress
 
-from cakemail_openapi.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from cakemail_openapi.exceptions import ApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
 
@@ -53,49 +58,53 @@
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
+        # ca_certs
+        if configuration.ssl_ca_cert:
+            ca_certs = configuration.ssl_ca_cert
+        else:
+            # if not set certificate file, use Mozilla's root certificates.
+            ca_certs = certifi.where()
+
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
-        if configuration.socket_options is not None:
-            addition_pool_args['socket_options'] = configuration.socket_options
-
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
-        if configuration.proxy and not should_bypass_proxies(configuration.host, no_proxy=configuration.no_proxy or ''):
+        if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
+                ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
                 **addition_pool_args
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
+                ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
@@ -128,30 +137,30 @@
             )
 
         post_params = post_params or {}
         headers = headers or {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif (isinstance(_request_timeout, tuple) and
                   len(_request_timeout) == 2):
                 timeout = urllib3.Timeout(
                     connect=_request_timeout[0], read=_request_timeout[1])
 
+        if 'Content-Type' not in headers:
+            headers['Content-Type'] = 'application/json'
+
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
-                if (method != 'DELETE') and ('Content-Type' not in headers):
-                    headers['Content-Type'] = 'application/json'
                 if query_params:
                     url += '?' + urlencode(query_params)
-                if ('Content-Type' not in headers) or (re.search('json', headers['Content-Type'], re.IGNORECASE)):
+                if re.search('json', headers['Content-Type'], re.IGNORECASE):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
                         preload_content=_preload_content,
@@ -208,26 +217,14 @@
         if _preload_content:
             r = RESTResponse(r)
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
-            if r.status == 401:
-                raise UnauthorizedException(http_resp=r)
-
-            if r.status == 403:
-                raise ForbiddenException(http_resp=r)
-
-            if r.status == 404:
-                raise NotFoundException(http_resp=r)
-
-            if 500 <= r.status <= 599:
-                raise ServiceException(http_resp=r)
-
             raise ApiException(http_resp=r)
 
         return r
 
     def GET(self, url, headers=None, query_params=None, _preload_content=True,
             _request_timeout=None):
         return self.request("GET", url,
@@ -288,59 +285,7 @@
         return self.request("PATCH", url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
-
-# end of class RESTClientObject
-def is_ipv4(target):
-    """ Test if IPv4 address or not
-    """
-    try:
-       chk = ipaddress.IPv4Address(target)
-       return True
-    except ipaddress.AddressValueError:
-       return False
-
-def in_ipv4net(target, net):
-    """ Test if target belongs to given IPv4 network
-    """
-    try:
-        nw = ipaddress.IPv4Network(net)
-        ip = ipaddress.IPv4Address(target)
-        if ip in nw:
-            return True
-        return False
-    except ipaddress.AddressValueError:
-        return False
-    except ipaddress.NetmaskValueError:
-        return False
-
-def should_bypass_proxies(url, no_proxy=None):
-    """ Yet another requests.should_bypass_proxies
-    Test if proxies should not be used for a particular url.
-    """
-
-    parsed = urlparse(url)
-
-    # special cases
-    if parsed.hostname in [None, '']:
-        return True
-
-    # special cases
-    if no_proxy in [None , '']:
-        return False
-    if no_proxy == '*':
-        return True
-
-    no_proxy = no_proxy.lower().replace(' ','');
-    entries = (
-        host for host in no_proxy.split(',') if host
-    )
-
-    if is_ipv4(parsed.hostname):
-        for item in entries:
-           if in_ipv4net(parsed.hostname, item):
-               return True
-    return proxy_bypass_environment(parsed.hostname, {'no': no_proxy} )
```

### Comparing `cakemail-openapi-1.9.0/setup.py` & `cakemail-openapi-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'urllib3',
     'certifi',
     'python-dateutil'
 ]
 
 setup(
     name='cakemail-openapi',
-    version='1.9.0',
+    version='1.9.1',
     description='OpenAPI generated client for Cakemail Next-gen API',
     python_requires='>=3.6',
     url='https://github.com/cakemail/cakemail-openapi-python',
     license='MIT',
     packages=[
         'cakemail_openapi',
         'cakemail_openapi.api',
```

