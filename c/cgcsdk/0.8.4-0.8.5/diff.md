# Comparing `tmp/cgcsdk-0.8.4.tar.gz` & `tmp/cgcsdk-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.4.tar", last modified: Tue Apr 18 11:51:35 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.5.tar", last modified: Fri Apr 21 11:28:58 2023, max compression
```

## Comparing `cgcsdk-0.8.4.tar` & `cgcsdk-0.8.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.988383 cgcsdk-0.8.4/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.4/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-04-18 11:51:35.986386 cgcsdk-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.766142 cgcsdk-0.8.4/cgc/
--rw-rw-rw-   0        0        0      234 2023-04-18 11:50:11.000000 cgcsdk-0.8.4/cgc/.env
--rw-rw-rw-   0        0        0     3406 2023-04-18 11:49:37.000000 cgcsdk-0.8.4/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-04-18 11:39:07.000000 cgcsdk-0.8.4/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.780357 cgcsdk-0.8.4/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.791841 cgcsdk-0.8.4/cgc/commands/auth/
--rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.4/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.4/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.4/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.803944 cgcsdk-0.8.4/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     1995 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/cgc_cmd_responses.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.820703 cgcsdk-0.8.4/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.4/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.827167 cgcsdk-0.8.4/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.4/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.836414 cgcsdk-0.8.4/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.4/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.844664 cgcsdk-0.8.4/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.863759 cgcsdk-0.8.4/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.4/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.4/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.879037 cgcsdk-0.8.4/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7189 2023-04-18 10:58:34.000000 cgcsdk-0.8.4/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.4/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     1499 2023-04-18 10:58:48.000000 cgcsdk-0.8.4/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.885283 cgcsdk-0.8.4/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.891504 cgcsdk-0.8.4/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.4/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.916348 cgcsdk-0.8.4/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.4/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.4/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.944682 cgcsdk-0.8.4/cgc/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.4/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.4/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.955294 cgcsdk-0.8.4/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.4/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.967605 cgcsdk-0.8.4/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.4/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.4/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.4/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.4/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.4/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.4/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.4/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.4/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:51:35.982965 cgcsdk-0.8.4/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 11:51:35.000000 cgcsdk-0.8.4/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 11:51:35.988975 cgcsdk-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.495473 cgcsdk-0.8.5/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.5/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-04-21 11:28:58.494476 cgcsdk-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.233253 cgcsdk-0.8.5/cgc/
+-rw-rw-rw-   0        0        0      234 2023-04-21 11:23:47.000000 cgcsdk-0.8.5/cgc/.env
+-rw-rw-rw-   0        0        0     3518 2023-04-21 11:25:14.000000 cgcsdk-0.8.5/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-04-18 11:39:07.000000 cgcsdk-0.8.5/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.252297 cgcsdk-0.8.5/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.268926 cgcsdk-0.8.5/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.288411 cgcsdk-0.8.5/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.5/cgc/commands/cgc_cmd_responses.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.307542 cgcsdk-0.8.5/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.314019 cgcsdk-0.8.5/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.5/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.319918 cgcsdk-0.8.5/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.5/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.326249 cgcsdk-0.8.5/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.341671 cgcsdk-0.8.5/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.360074 cgcsdk-0.8.5/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.5/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.5/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     1499 2023-04-18 10:58:48.000000 cgcsdk-0.8.5/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.367139 cgcsdk-0.8.5/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.374972 cgcsdk-0.8.5/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.5/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.406579 cgcsdk-0.8.5/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.441933 cgcsdk-0.8.5/cgc/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.450100 cgcsdk-0.8.5/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.5/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.464623 cgcsdk-0.8.5/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.5/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.5/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.5/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.5/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.491014 cgcsdk-0.8.5/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2418 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:28:58.496458 cgcsdk-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.5/setup.py
```

### Comparing `cgcsdk-0.8.4/PKG-INFO` & `cgcsdk-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.4/cgc/CHANGELOG.md` & `cgcsdk-0.8.5/cgc/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 
+## 0.8.5
+
+Release on Apr 21, 2023.
+
+* update for cgc status: resource_keys in cgc_status_response
+
 ## 0.8.4
 
 Release on Apr 18, 2023.
 
-* minor import fix
+* fix regarding missing imports
 
 ## 0.8.3
 
 Release on Apr 18, 2023.
 
 * minor db sdk update
 * added restart optional parameter to client
```

### Comparing `cgcsdk-0.8.4/cgc/cgc.py` & `cgcsdk-0.8.5/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.5/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.5/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.5/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.5/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.5/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.5/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.5/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.5/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.5/cgc/commands/cgc_cmd_responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         # "V100",
         "Count",
         "",
         "nvme",
         "ssd",
     ]
     resource_keys = [
-        "limits.cpu",
-        "limits.memory",
+        "requests.cpu",
+        "requests.memory",
         "requests.nvidia.com/gpu",
-        "comtegra.cloud/a100",
-        "comtegra.cloud/a5000",
-        # "comtegra.cloud/v100",
+        "requests.comtegra.cloud/a100",
+        "requests.comtegra.cloud/a5000",
+        # "requests.comtegra.cloud/v100",
         "persistentvolumeclaims",
         "requests.storage",
         "nvme-rwx.storageclass.storage.k8s.io/requests.storage",
         "ssd-rwx.storageclass.storage.k8s.io/requests.storage",
     ]
 
     resources_available_list = []
```

### Comparing `cgcsdk-0.8.4/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.5/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.5/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.5/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.5/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.5/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.8.5/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.5/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.5/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.5/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.5/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/sdk/handlers.py` & `cgcsdk-0.8.5/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/sdk/mongodb.py` & `cgcsdk-0.8.5/cgc/sdk/mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,21 +177,23 @@
         # print("collection   : {}.{}".format(d["ns"]["db"], d["ns"]["coll"]))
         # try:
         #     print("doc          : {}".format(d["fullDocument"]))
         # except KeyError:
         #     pass
 
 
-def get_mongo_access(app_name: str, password: str, restart: bool = False):
+def get_mongo_access(
+    app_name: str, password: str, database: str = "db", restart: bool = False
+):
     global _mongo_access
 
     def init_access():
         global _mongo_access
         _mongo_access = MongoConnector(
-            database_name="db",
+            database_name=database,
             hosts=f"{app_name}:27017",
             username="admin",
             password=password,
         )
 
     try:
         if not isinstance(_mongo_access, MongoConnector) or restart:
```

### Comparing `cgcsdk-0.8.4/cgc/sdk/postgresql.py` & `cgcsdk-0.8.5/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/sdk/redis.py` & `cgcsdk-0.8.5/cgc/sdk/redis.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/server.crt` & `cgcsdk-0.8.5/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/telemetry/basic.py` & `cgcsdk-0.8.5/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/__init__.py` & `cgcsdk-0.8.5/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.5/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/tests/responses_tests.py` & `cgcsdk-0.8.5/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/click_group.py` & `cgcsdk-0.8.5/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/config_utils.py` & `cgcsdk-0.8.5/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.5/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.5/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.5/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.5/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.5/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.5/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/message_utils.py` & `cgcsdk-0.8.5/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.5/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/requests_helper.py` & `cgcsdk-0.8.5/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/response_utils.py` & `cgcsdk-0.8.5/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgc/utils/version_control.py` & `cgcsdk-0.8.5/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.5/cgcsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.4/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.5/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.4/setup.py` & `cgcsdk-0.8.5/setup.py`

 * *Files identical despite different names*

