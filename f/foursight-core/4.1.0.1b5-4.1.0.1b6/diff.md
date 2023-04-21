# Comparing `tmp/foursight_core-4.1.0.1b5.tar.gz` & `tmp/foursight_core-4.1.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.1b5.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.1b6.tar", max compression
```

## Comparing `foursight_core-4.1.0.1b5.tar` & `foursight_core-4.1.0.1b6.tar`

### file list

```diff
@@ -1,135 +1,140 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:08:59.753994 foursight_core-4.1.0.1b5/LICENSE.txt
--rw-r--r--   0        0        0    10825 2022-11-20 13:33:58.544911 foursight_core-4.1.0.1b5/foursight_core/'
--rw-r--r--   0        0        0        0 2022-09-07 10:08:59.760120 foursight_core-4.1.0.1b5/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-03-30 11:22:44.920863 foursight_core-4.1.0.1b5/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0     8523 2023-02-23 17:12:48.834947 foursight_core-4.1.0.1b5/foursight_core/adfasdfad
--rw-r--r--   0        0        0       69 2023-04-16 14:05:52.759877 foursight_core-4.1.0.1b5/foursight_core/app.py
--rw-r--r--   0        0        0   105730 2023-04-16 14:04:58.418881 foursight_core-4.1.0.1b5/foursight_core/app_utils.py
--rw-r--r--   0        0        0   101241 2022-12-02 19:01:09.085977 foursight_core-4.1.0.1b5/foursight_core/app_utils.py---
--rw-r--r--   0        0        0    97799 2022-11-22 14:52:55.397982 foursight_core-4.1.0.1b5/foursight_core/app_utils.py-deb
--rw-r--r--   0        0        0    97949 2022-11-23 13:18:09.708092 foursight_core-4.1.0.1b5/foursight_core/app_utils.py-debug
--rw-r--r--   0        0        0   101943 2023-03-29 22:48:31.801408 foursight_core-4.1.0.1b5/foursight_core/app_utils.py-debugg
--rw-r--r--   0        0        0    12620 2022-11-30 14:04:39.423857 foursight_core-4.1.0.1b5/foursight_core/asdf
--rw-r--r--   0        0        0     2571 2023-03-30 11:22:44.922092 foursight_core-4.1.0.1b5/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2022-09-07 10:08:59.760846 foursight_core-4.1.0.1b5/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2022-09-07 10:08:59.760916 foursight_core-4.1.0.1b5/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-03-31 17:00:42.022944 foursight_core-4.1.0.1b5/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-03-30 11:22:44.922592 foursight_core-4.1.0.1b5/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-10 14:14:30.704500 foursight_core-4.1.0.1b5/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-03-31 17:00:42.023738 foursight_core-4.1.0.1b5/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-03-31 17:00:42.024190 foursight_core-4.1.0.1b5/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-03-31 17:00:42.024311 foursight_core-4.1.0.1b5/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2022-09-07 10:08:59.761273 foursight_core-4.1.0.1b5/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-03-30 11:22:44.922849 foursight_core-4.1.0.1b5/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-03-30 11:22:44.923050 foursight_core-4.1.0.1b5/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2022-09-07 10:08:59.761552 foursight_core-4.1.0.1b5/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-03-31 17:00:42.024438 foursight_core-4.1.0.1b5/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-03-31 17:00:42.024598 foursight_core-4.1.0.1b5/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11437 2022-11-20 14:31:38.983954 foursight_core-4.1.0.1b5/foursight_core/d
--rw-r--r--   0        0        0    11929 2023-03-31 17:00:42.024812 foursight_core-4.1.0.1b5/foursight_core/decorators.py
--rw-r--r--   0        0        0    12565 2022-11-28 19:43:36.821773 foursight_core-4.1.0.1b5/foursight_core/decorators.py-new
--rw-r--r--   0        0        0    15050 2023-03-31 17:00:42.025145 foursight_core-4.1.0.1b5/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-16 04:32:00.359540 foursight_core-4.1.0.1b5/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-03-31 17:00:42.025932 foursight_core-4.1.0.1b5/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2022-09-07 10:08:59.762246 foursight_core-4.1.0.1b5/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-10 14:14:30.704795 foursight_core-4.1.0.1b5/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-10 14:14:30.705142 foursight_core-4.1.0.1b5/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-03-31 17:00:42.026791 foursight_core-4.1.0.1b5/foursight_core/mapping.json
--rw-r--r--   0        0        0    95074 2022-11-15 14:26:15.846985 foursight_core-4.1.0.1b5/foursight_core/okk
--rw-r--r--   0        0        0     1014 2023-03-30 11:22:44.924884 foursight_core-4.1.0.1b5/foursight_core/package.py
--rw-r--r--   0        0        0     4846 2022-10-18 15:27:01.122701 foursight_core-4.1.0.1b5/foursight_core/react/api/'
--rw-r--r--   0        0        0    26281 2022-12-06 19:54:26.692542 foursight_core-4.1.0.1b5/foursight_core/react/api/:w
--rw-r--r--   0        0        0     5122 2022-10-19 18:25:39.526281 foursight_core-4.1.0.1b5/foursight_core/react/api/]:w
--rw-r--r--   0        0        0    16866 2022-10-19 15:30:53.424281 foursight_core-4.1.0.1b5/foursight_core/react/api/adsfa
--rw-r--r--   0        0        0    46462 2022-11-19 15:11:20.178519 foursight_core-4.1.0.1b5/foursight_core/react/api/alkd
--rw-r--r--   0        0        0    32044 2022-10-21 15:56:11.928913 foursight_core-4.1.0.1b5/foursight_core/react/api/asav
--rw-r--r--   0        0        0    28883 2022-10-19 18:32:59.913329 foursight_core-4.1.0.1b5/foursight_core/react/api/asdf
--rw-r--r--   0        0        0    12150 2022-12-08 18:15:25.696290 foursight_core-4.1.0.1b5/foursight_core/react/api/asdff
--rw-r--r--   0        0        0    13838 2023-04-16 14:05:39.122944 foursight_core-4.1.0.1b5/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0    14143 2023-03-31 15:18:53.676413 foursight_core-4.1.0.1b5/foursight_core/react/api/auth.py-deb
--rw-r--r--   0        0        0     7091 2023-04-16 14:14:05.368090 foursight_core-4.1.0.1b5/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0     1163 2022-12-26 13:33:51.355358 foursight_core-4.1.0.1b5/foursight_core/react/api/aws_logs.py
--rw-r--r--   0        0        0    23203 2023-03-31 17:00:42.028111 foursight_core-4.1.0.1b5/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-03-31 17:00:42.028307 foursight_core-4.1.0.1b5/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-03-31 17:00:42.028636 foursight_core-4.1.0.1b5/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-03-31 17:00:42.029013 foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    30044 2023-01-03 14:40:15.527405 foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py---
--rw-r--r--   0        0        0    28530 2022-12-07 15:57:38.726495 foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py-new
--rw-r--r--   0        0        0    20652 2023-03-31 17:00:42.029767 foursight_core-4.1.0.1b5/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3459 2023-04-18 14:46:47.694282 foursight_core-4.1.0.1b5/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5745 2023-03-31 17:00:42.030106 foursight_core-4.1.0.1b5/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-03-31 17:00:42.030271 foursight_core-4.1.0.1b5/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-03-31 17:00:42.030388 foursight_core-4.1.0.1b5/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4783 2023-03-31 17:00:42.030600 foursight_core-4.1.0.1b5/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0    58991 2022-12-25 17:24:38.880437 foursight_core-4.1.0.1b5/foursight_core/react/api/foo
--rw-r--r--   0        0        0     3257 2023-03-31 17:00:42.030761 foursight_core-4.1.0.1b5/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0    13097 2022-11-07 19:29:38.049301 foursight_core-4.1.0.1b5/foursight_core/react/api/hama
--rw-r--r--   0        0        0    44446 2022-11-18 16:41:20.868752 foursight_core-4.1.0.1b5/foursight_core/react/api/hmm
--rw-r--r--   0        0        0     3516 2023-03-31 17:00:42.030910 foursight_core-4.1.0.1b5/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-03-31 17:00:42.031263 foursight_core-4.1.0.1b5/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0    14646 2022-10-23 19:06:03.352206 foursight_core-4.1.0.1b5/foursight_core/react/api/ok
--rw-r--r--   0        0        0    27126 2022-12-07 16:03:28.375164 foursight_core-4.1.0.1b5/foursight_core/react/api/oklk
--rw-r--r--   0        0        0    17397 2022-10-19 18:57:09.208083 foursight_core-4.1.0.1b5/foursight_core/react/api/okok
--rw-r--r--   0        0        0    15418 2022-10-23 19:08:13.968538 foursight_core-4.1.0.1b5/foursight_core/react/api/okokok
--rw-r--r--   0        0        0    37016 2022-11-12 14:03:53.287757 foursight_core-4.1.0.1b5/foursight_core/react/api/okokokok
--rw-r--r--   0        0        0    39205 2022-11-12 19:00:46.033390 foursight_core-4.1.0.1b5/foursight_core/react/api/okokokokok
--rw-r--r--   0        0        0    29102 2022-12-07 19:03:24.489085 foursight_core-4.1.0.1b5/foursight_core/react/api/ot
--rw-r--r--   0        0        0    75413 2023-04-18 17:19:33.151602 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    45701 2022-10-21 14:29:00.904736 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-
--rw-r--r--   0        0        0    30313 2022-10-21 17:36:32.520832 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py--
--rw-r--r--   0        0        0    71345 2023-01-23 23:30:44.383522 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py----
--rw-r--r--   0        0        0    46990 2022-11-22 14:51:44.189069 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-deb
--rw-r--r--   0        0        0    24458 2022-10-22 23:24:49.505751 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-saaave
--rw-r--r--   0        0        0    11336 2023-04-10 14:14:40.711249 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0    11721 2023-03-31 15:18:58.965799 foursight_core-4.1.0.1b5/foursight_core/react/api/react_api_base.py-deb
--rw-r--r--   0        0        0    10435 2022-10-22 23:25:02.692255 foursight_core-4.1.0.1b5/foursight_core/react/api/react_app.py-saaave
--rw-r--r--   0        0        0     8025 2023-03-31 17:00:42.033249 foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0     5576 2022-10-19 22:12:16.865537 foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_utils.py-
--rw-r--r--   0        0        0     7471 2022-10-22 19:19:42.543417 foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_utils.py.save
--rw-r--r--   0        0        0    31570 2023-04-16 23:01:06.114489 foursight_core-4.1.0.1b5/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0    12876 2022-10-22 19:00:58.268720 foursight_core-4.1.0.1b5/foursight_core/react/api/react_routes.py.save
--rw-r--r--   0        0        0     4861 2023-03-31 17:00:42.034179 foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0     5027 2022-10-17 22:40:41.733498 foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py-bak
--rw-r--r--   0        0        0     4206 2022-10-17 22:47:29.529384 foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py-debug
--rw-r--r--   0        0        0    56415 2022-12-15 17:41:55.903970 foursight_core-4.1.0.1b5/foursight_core/react/api/sa
--rw-r--r--   0        0        0    42517 2022-11-15 20:10:51.305457 foursight_core-4.1.0.1b5/foursight_core/react/api/sav
--rw-r--r--   0        0        0    16885 2022-10-19 15:44:40.693752 foursight_core-4.1.0.1b5/foursight_core/react/api/save
--rw-r--r--   0        0        0    17391 2023-04-18 12:55:08.320992 foursight_core-4.1.0.1b5/foursight_core/react/api/x
--rw-r--r--   0        0        0    31785 2022-10-21 15:29:37.208969 foursight_core-4.1.0.1b5/foursight_core/react/api/xx
--rw-r--r--   0        0        0    56739 2022-12-15 20:17:56.533252 foursight_core-4.1.0.1b5/foursight_core/react/api/xxy
--rw-r--r--   0        0        0     5921 2022-10-21 16:32:06.326758 foursight_core-4.1.0.1b5/foursight_core/react/api/xyz
--rw-r--r--   0        0        0      806 2023-03-31 17:00:42.034293 foursight_core-4.1.0.1b5/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-18 19:45:20.310593 foursight_core-4.1.0.1b5/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-18 19:45:20.308051 foursight_core-4.1.0.1b5/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-18 19:45:10.488505 foursight_core-4.1.0.1b5/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-18 19:45:20.206108 foursight_core-4.1.0.1b5/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1919947 2023-04-18 19:45:20.206339 foursight_core-4.1.0.1b5/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-03-31 17:00:42.046642 foursight_core-4.1.0.1b5/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-03-31 17:00:42.047578 foursight_core-4.1.0.1b5/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-03-31 17:00:42.047831 foursight_core-4.1.0.1b5/foursight_core/run_result.py
--rw-r--r--   0        0        0    22924 2022-11-21 20:22:40.475142 foursight_core-4.1.0.1b5/foursight_core/run_result.py-deb
--rw-r--r--   0        0        0     6330 2023-03-31 17:00:42.048014 foursight_core-4.1.0.1b5/foursight_core/s3_connection.py
--rw-r--r--   0        0        0    95791 2022-11-15 19:33:17.290307 foursight_core-4.1.0.1b5/foursight_core/sav
--rw-r--r--   0        0        0     5282 2023-03-31 17:00:42.048163 foursight_core-4.1.0.1b5/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     6458 2022-11-04 14:38:30.182413 foursight_core-4.1.0.1b5/foursight_core/schedule_decorator.py-
--rw-r--r--   0        0        0     1402 2023-03-31 17:00:42.048268 foursight_core-4.1.0.1b5/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-03-31 17:00:42.048339 foursight_core-4.1.0.1b5/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0       65 2022-11-14 16:31:57.489442 foursight_core-4.1.0.1b5/foursight_core/scripts/p
--rw-r--r--   0        0        0      797 2022-11-17 17:02:52.436871 foursight_core-4.1.0.1b5/foursight_core/scripts/save/decrypt_accounts_file.py
--rw-r--r--   0        0        0      801 2022-11-17 17:02:55.810728 foursight_core-4.1.0.1b5/foursight_core/scripts/save/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-03-31 17:00:42.048769 foursight_core-4.1.0.1b5/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-03-30 11:23:29.553404 foursight_core-4.1.0.1b5/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-03-30 11:26:56.704948 foursight_core-4.1.0.1b5/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-10 14:14:30.716241 foursight_core-4.1.0.1b5/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2022-09-07 10:08:59.763471 foursight_core-4.1.0.1b5/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-03-30 11:28:21.582264 foursight_core-4.1.0.1b5/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2022-09-07 10:08:59.763671 foursight_core-4.1.0.1b5/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-03-30 11:26:56.705625 foursight_core-4.1.0.1b5/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-03-30 11:26:56.705764 foursight_core-4.1.0.1b5/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-03-30 11:26:56.706033 foursight_core-4.1.0.1b5/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-03-30 11:26:56.706216 foursight_core-4.1.0.1b5/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1489 2023-03-29 22:45:57.789020 foursight_core-4.1.0.1b5/foursight_core/x
--rw-r--r--   0        0        0      231 2023-02-23 19:48:15.449939 foursight_core-4.1.0.1b5/foursight_core/x.py]
--rw-r--r--   0        0        0     1531 2023-04-18 19:48:01.206841 foursight_core-4.1.0.1b5/pyproject.toml
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b5/setup.py
--rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:08:59.753994 foursight_core-4.1.0.1b6/LICENSE.txt
+-rw-r--r--   0        0        0    10825 2022-11-20 13:33:58.544911 foursight_core-4.1.0.1b6/foursight_core/'
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.760120 foursight_core-4.1.0.1b6/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-03-30 11:22:44.920863 foursight_core-4.1.0.1b6/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0     8523 2023-02-23 17:12:48.834947 foursight_core-4.1.0.1b6/foursight_core/adfasdfad
+-rw-r--r--   0        0        0       69 2023-04-16 14:05:52.759877 foursight_core-4.1.0.1b6/foursight_core/app.py
+-rw-r--r--   0        0        0   105730 2023-04-16 14:04:58.418881 foursight_core-4.1.0.1b6/foursight_core/app_utils.py
+-rw-r--r--   0        0        0   101241 2022-12-02 19:01:09.085977 foursight_core-4.1.0.1b6/foursight_core/app_utils.py---
+-rw-r--r--   0        0        0    97799 2022-11-22 14:52:55.397982 foursight_core-4.1.0.1b6/foursight_core/app_utils.py-deb
+-rw-r--r--   0        0        0    97949 2022-11-23 13:18:09.708092 foursight_core-4.1.0.1b6/foursight_core/app_utils.py-debug
+-rw-r--r--   0        0        0   101943 2023-03-29 22:48:31.801408 foursight_core-4.1.0.1b6/foursight_core/app_utils.py-debugg
+-rw-r--r--   0        0        0    12620 2022-11-30 14:04:39.423857 foursight_core-4.1.0.1b6/foursight_core/asdf
+-rw-r--r--   0        0        0     2571 2023-03-30 11:22:44.922092 foursight_core-4.1.0.1b6/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2022-09-07 10:08:59.760846 foursight_core-4.1.0.1b6/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2022-09-07 10:08:59.760916 foursight_core-4.1.0.1b6/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-03-31 17:00:42.022944 foursight_core-4.1.0.1b6/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-03-30 11:22:44.922592 foursight_core-4.1.0.1b6/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-20 18:26:30.344734 foursight_core-4.1.0.1b6/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-03-31 17:00:42.023738 foursight_core-4.1.0.1b6/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-03-31 17:00:42.024190 foursight_core-4.1.0.1b6/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-03-31 17:00:42.024311 foursight_core-4.1.0.1b6/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.761273 foursight_core-4.1.0.1b6/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-30 11:22:44.922849 foursight_core-4.1.0.1b6/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-03-30 11:22:44.923050 foursight_core-4.1.0.1b6/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2022-09-07 10:08:59.761552 foursight_core-4.1.0.1b6/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-03-31 17:00:42.024438 foursight_core-4.1.0.1b6/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-03-31 17:00:42.024598 foursight_core-4.1.0.1b6/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0     1292 2023-04-19 11:31:51.999612 foursight_core-4.1.0.1b6/foursight_core/checks/x
+-rw-r--r--   0        0        0    11437 2022-11-20 14:31:38.983954 foursight_core-4.1.0.1b6/foursight_core/d
+-rw-r--r--   0        0        0    11929 2023-03-31 17:00:42.024812 foursight_core-4.1.0.1b6/foursight_core/decorators.py
+-rw-r--r--   0        0        0    12565 2022-11-28 19:43:36.821773 foursight_core-4.1.0.1b6/foursight_core/decorators.py-new
+-rw-r--r--   0        0        0    15050 2023-03-31 17:00:42.025145 foursight_core-4.1.0.1b6/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-16 04:32:00.359540 foursight_core-4.1.0.1b6/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-03-31 17:00:42.025932 foursight_core-4.1.0.1b6/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2022-09-07 10:08:59.762246 foursight_core-4.1.0.1b6/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-10 14:14:30.704795 foursight_core-4.1.0.1b6/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-10 14:14:30.705142 foursight_core-4.1.0.1b6/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-03-31 17:00:42.026791 foursight_core-4.1.0.1b6/foursight_core/mapping.json
+-rw-r--r--   0        0        0    95074 2022-11-15 14:26:15.846985 foursight_core-4.1.0.1b6/foursight_core/okk
+-rw-r--r--   0        0        0     1014 2023-03-30 11:22:44.924884 foursight_core-4.1.0.1b6/foursight_core/package.py
+-rw-r--r--   0        0        0     4846 2022-10-18 15:27:01.122701 foursight_core-4.1.0.1b6/foursight_core/react/api/'
+-rw-r--r--   0        0        0    26281 2022-12-06 19:54:26.692542 foursight_core-4.1.0.1b6/foursight_core/react/api/:w
+-rw-r--r--   0        0        0     5122 2022-10-19 18:25:39.526281 foursight_core-4.1.0.1b6/foursight_core/react/api/]:w
+-rw-r--r--   0        0        0    11106 2023-04-19 14:18:32.307677 foursight_core-4.1.0.1b6/foursight_core/react/api/a
+-rw-r--r--   0        0        0    16866 2022-10-19 15:30:53.424281 foursight_core-4.1.0.1b6/foursight_core/react/api/adsfa
+-rw-r--r--   0        0        0    46462 2022-11-19 15:11:20.178519 foursight_core-4.1.0.1b6/foursight_core/react/api/alkd
+-rw-r--r--   0        0        0    32044 2022-10-21 15:56:11.928913 foursight_core-4.1.0.1b6/foursight_core/react/api/asav
+-rw-r--r--   0        0        0    28883 2022-10-19 18:32:59.913329 foursight_core-4.1.0.1b6/foursight_core/react/api/asdf
+-rw-r--r--   0        0        0     2582 2023-04-19 15:51:21.736937 foursight_core-4.1.0.1b6/foursight_core/react/api/asdfasdf
+-rw-r--r--   0        0        0    12150 2022-12-08 18:15:25.696290 foursight_core-4.1.0.1b6/foursight_core/react/api/asdff
+-rw-r--r--   0        0        0    17014 2023-04-21 20:17:58.353284 foursight_core-4.1.0.1b6/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0    14143 2023-03-31 15:18:53.676413 foursight_core-4.1.0.1b6/foursight_core/react/api/auth.py-deb
+-rw-r--r--   0        0        0     7091 2023-04-16 14:14:05.368090 foursight_core-4.1.0.1b6/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0     1163 2022-12-26 13:33:51.355358 foursight_core-4.1.0.1b6/foursight_core/react/api/aws_logs.py
+-rw-r--r--   0        0        0    23203 2023-03-31 17:00:42.028111 foursight_core-4.1.0.1b6/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-03-31 17:00:42.028307 foursight_core-4.1.0.1b6/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-03-31 17:00:42.028636 foursight_core-4.1.0.1b6/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-03-31 17:00:42.029013 foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    30044 2023-01-03 14:40:15.527405 foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py---
+-rw-r--r--   0        0        0    28530 2022-12-07 15:57:38.726495 foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py-new
+-rw-r--r--   0        0        0    20652 2023-03-31 17:00:42.029767 foursight_core-4.1.0.1b6/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3459 2023-04-18 14:46:47.694282 foursight_core-4.1.0.1b6/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     5745 2023-03-31 17:00:42.030106 foursight_core-4.1.0.1b6/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-03-31 17:00:42.030271 foursight_core-4.1.0.1b6/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-03-31 17:00:42.030388 foursight_core-4.1.0.1b6/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4878 2023-04-21 20:12:47.966508 foursight_core-4.1.0.1b6/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0    58991 2022-12-25 17:24:38.880437 foursight_core-4.1.0.1b6/foursight_core/react/api/foo
+-rw-r--r--   0        0        0     3257 2023-03-31 17:00:42.030761 foursight_core-4.1.0.1b6/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0    13097 2022-11-07 19:29:38.049301 foursight_core-4.1.0.1b6/foursight_core/react/api/hama
+-rw-r--r--   0        0        0    44446 2022-11-18 16:41:20.868752 foursight_core-4.1.0.1b6/foursight_core/react/api/hmm
+-rw-r--r--   0        0        0     3516 2023-03-31 17:00:42.030910 foursight_core-4.1.0.1b6/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-03-31 17:00:42.031263 foursight_core-4.1.0.1b6/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0    14646 2022-10-23 19:06:03.352206 foursight_core-4.1.0.1b6/foursight_core/react/api/ok
+-rw-r--r--   0        0        0    27126 2022-12-07 16:03:28.375164 foursight_core-4.1.0.1b6/foursight_core/react/api/oklk
+-rw-r--r--   0        0        0    17397 2022-10-19 18:57:09.208083 foursight_core-4.1.0.1b6/foursight_core/react/api/okok
+-rw-r--r--   0        0        0    15418 2022-10-23 19:08:13.968538 foursight_core-4.1.0.1b6/foursight_core/react/api/okokok
+-rw-r--r--   0        0        0    37016 2022-11-12 14:03:53.287757 foursight_core-4.1.0.1b6/foursight_core/react/api/okokokok
+-rw-r--r--   0        0        0    39205 2022-11-12 19:00:46.033390 foursight_core-4.1.0.1b6/foursight_core/react/api/okokokokok
+-rw-r--r--   0        0        0    29102 2022-12-07 19:03:24.489085 foursight_core-4.1.0.1b6/foursight_core/react/api/ot
+-rw-r--r--   0        0        0     3862 2023-04-21 03:15:59.228651 foursight_core-4.1.0.1b6/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    77827 2023-04-21 20:10:16.814770 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    45701 2022-10-21 14:29:00.904736 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-
+-rw-r--r--   0        0        0    30313 2022-10-21 17:36:32.520832 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py--
+-rw-r--r--   0        0        0    71345 2023-01-23 23:30:44.383522 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py----
+-rw-r--r--   0        0        0    46990 2022-11-22 14:51:44.189069 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-deb
+-rw-r--r--   0        0        0    24458 2022-10-22 23:24:49.505751 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-saaave
+-rw-r--r--   0        0        0    11353 2023-04-21 19:21:13.190302 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0    11721 2023-03-31 15:18:58.965799 foursight_core-4.1.0.1b6/foursight_core/react/api/react_api_base.py-deb
+-rw-r--r--   0        0        0    10435 2022-10-22 23:25:02.692255 foursight_core-4.1.0.1b6/foursight_core/react/api/react_app.py-saaave
+-rw-r--r--   0        0        0     8025 2023-03-31 17:00:42.033249 foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0     5576 2022-10-19 22:12:16.865537 foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_utils.py-
+-rw-r--r--   0        0        0     7471 2022-10-22 19:19:42.543417 foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_utils.py.save
+-rw-r--r--   0        0        0    32302 2023-04-20 18:33:16.326327 foursight_core-4.1.0.1b6/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0    12876 2022-10-22 19:00:58.268720 foursight_core-4.1.0.1b6/foursight_core/react/api/react_routes.py.save
+-rw-r--r--   0        0        0     4861 2023-03-31 17:00:42.034179 foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0     5027 2022-10-17 22:40:41.733498 foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py-bak
+-rw-r--r--   0        0        0     4206 2022-10-17 22:47:29.529384 foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py-debug
+-rw-r--r--   0        0        0    56415 2022-12-15 17:41:55.903970 foursight_core-4.1.0.1b6/foursight_core/react/api/sa
+-rw-r--r--   0        0        0    42517 2022-11-15 20:10:51.305457 foursight_core-4.1.0.1b6/foursight_core/react/api/sav
+-rw-r--r--   0        0        0    16885 2022-10-19 15:44:40.693752 foursight_core-4.1.0.1b6/foursight_core/react/api/save
+-rw-r--r--   0        0        0     1977 2023-04-20 20:15:19.741349 foursight_core-4.1.0.1b6/foursight_core/react/api/x
+-rw-r--r--   0        0        0    31785 2022-10-21 15:29:37.208969 foursight_core-4.1.0.1b6/foursight_core/react/api/xx
+-rw-r--r--   0        0        0     5648 2023-04-19 14:58:25.494220 foursight_core-4.1.0.1b6/foursight_core/react/api/xxx
+-rw-r--r--   0        0        0    56739 2022-12-15 20:17:56.533252 foursight_core-4.1.0.1b6/foursight_core/react/api/xxy
+-rw-r--r--   0        0        0     5921 2022-10-21 16:32:06.326758 foursight_core-4.1.0.1b6/foursight_core/react/api/xyz
+-rw-r--r--   0        0        0      806 2023-03-31 17:00:42.034293 foursight_core-4.1.0.1b6/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-21 20:16:13.428641 foursight_core-4.1.0.1b6/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-21 20:16:13.426058 foursight_core-4.1.0.1b6/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-21 20:16:03.853748 foursight_core-4.1.0.1b6/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-21 20:16:13.330113 foursight_core-4.1.0.1b6/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1925016 2023-04-21 20:16:13.330346 foursight_core-4.1.0.1b6/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-03-31 17:00:42.046642 foursight_core-4.1.0.1b6/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-03-31 17:00:42.047578 foursight_core-4.1.0.1b6/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-03-31 17:00:42.047831 foursight_core-4.1.0.1b6/foursight_core/run_result.py
+-rw-r--r--   0        0        0    22924 2022-11-21 20:22:40.475142 foursight_core-4.1.0.1b6/foursight_core/run_result.py-deb
+-rw-r--r--   0        0        0     6330 2023-03-31 17:00:42.048014 foursight_core-4.1.0.1b6/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0    95791 2022-11-15 19:33:17.290307 foursight_core-4.1.0.1b6/foursight_core/sav
+-rw-r--r--   0        0        0     5282 2023-03-31 17:00:42.048163 foursight_core-4.1.0.1b6/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     6458 2022-11-04 14:38:30.182413 foursight_core-4.1.0.1b6/foursight_core/schedule_decorator.py-
+-rw-r--r--   0        0        0     1402 2023-03-31 17:00:42.048268 foursight_core-4.1.0.1b6/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-03-31 17:00:42.048339 foursight_core-4.1.0.1b6/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0       65 2022-11-14 16:31:57.489442 foursight_core-4.1.0.1b6/foursight_core/scripts/p
+-rw-r--r--   0        0        0      797 2022-11-17 17:02:52.436871 foursight_core-4.1.0.1b6/foursight_core/scripts/save/decrypt_accounts_file.py
+-rw-r--r--   0        0        0      801 2022-11-17 17:02:55.810728 foursight_core-4.1.0.1b6/foursight_core/scripts/save/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-03-31 17:00:42.048769 foursight_core-4.1.0.1b6/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-03-30 11:23:29.553404 foursight_core-4.1.0.1b6/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-03-30 11:26:56.704948 foursight_core-4.1.0.1b6/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-10 14:14:30.716241 foursight_core-4.1.0.1b6/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2022-09-07 10:08:59.763471 foursight_core-4.1.0.1b6/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-03-30 11:28:21.582264 foursight_core-4.1.0.1b6/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2022-09-07 10:08:59.763671 foursight_core-4.1.0.1b6/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-03-30 11:26:56.705625 foursight_core-4.1.0.1b6/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-03-30 11:26:56.705764 foursight_core-4.1.0.1b6/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-03-30 11:26:56.706033 foursight_core-4.1.0.1b6/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-03-30 11:26:56.706216 foursight_core-4.1.0.1b6/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1489 2023-03-29 22:45:57.789020 foursight_core-4.1.0.1b6/foursight_core/x
+-rw-r--r--   0        0        0      231 2023-02-23 19:48:15.449939 foursight_core-4.1.0.1b6/foursight_core/x.py]
+-rw-r--r--   0        0        0     1531 2023-04-21 18:54:34.138109 foursight_core-4.1.0.1b6/pyproject.toml
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b6/setup.py
+-rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b6/PKG-INFO
```

### Comparing `foursight_core-4.1.0.1b5/LICENSE.txt` & `foursight_core-4.1.0.1b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/'` & `foursight_core-4.1.0.1b6/foursight_core/'`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.1b6/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/adfasdfad` & `foursight_core-4.1.0.1b6/foursight_core/adfasdfad`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/app_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/app_utils.py---` & `foursight_core-4.1.0.1b6/foursight_core/app_utils.py---`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/app_utils.py-deb` & `foursight_core-4.1.0.1b6/foursight_core/app_utils.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/app_utils.py-debug` & `foursight_core-4.1.0.1b6/foursight_core/app_utils.py-debug`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/app_utils.py-debugg` & `foursight_core-4.1.0.1b6/foursight_core/app_utils.py-debugg`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/asdf` & `foursight_core-4.1.0.1b6/foursight_core/asdf`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/buckets.py` & `foursight_core-4.1.0.1b6/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/check_schema.py` & `foursight_core-4.1.0.1b6/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/check_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.1b6/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/d` & `foursight_core-4.1.0.1b6/foursight_core/d`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/decorators.py` & `foursight_core-4.1.0.1b6/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/decorators.py-new` & `foursight_core-4.1.0.1b6/foursight_core/decorators.py-new`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/deploy.py` & `foursight_core-4.1.0.1b6/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/environment.py` & `foursight_core-4.1.0.1b6/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/es_connection.py` & `foursight_core-4.1.0.1b6/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/exceptions.py` & `foursight_core-4.1.0.1b6/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/fs_connection.py` & `foursight_core-4.1.0.1b6/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/identity.py` & `foursight_core-4.1.0.1b6/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/mapping.json` & `foursight_core-4.1.0.1b6/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/okk` & `foursight_core-4.1.0.1b6/foursight_core/okk`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/package.py` & `foursight_core-4.1.0.1b6/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/'` & `foursight_core-4.1.0.1b6/foursight_core/react/api/'`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/:w` & `foursight_core-4.1.0.1b6/foursight_core/react/api/:w`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/]:w` & `foursight_core-4.1.0.1b6/foursight_core/react/api/]:w`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/adsfa` & `foursight_core-4.1.0.1b6/foursight_core/react/api/adsfa`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/alkd` & `foursight_core-4.1.0.1b6/foursight_core/react/api/alkd`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/asav` & `foursight_core-4.1.0.1b6/foursight_core/react/api/asav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/asdf` & `foursight_core-4.1.0.1b6/foursight_core/react/api/asdf`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/asdff` & `foursight_core-4.1.0.1b6/foursight_core/react/api/asdff`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/auth.py-deb`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import time
 import redis
 from typing import Optional
 from dcicutils.redis_utils import create_redis_client
 from dcicutils.redis_tools import RedisBase, RedisSessionToken, SESSION_TOKEN_COOKIE
 from dcicutils.env_utils import full_env_name
-from dcicutils.misc_utils import ignored, PRINT
+from dcicutils.misc_utils import PRINT
 from ...app import app
 from .cookie_utils import read_cookie
 from .envs import Envs
 from .jwt_utils import JWT_AUDIENCE_PROPERTY_NAME, JWT_SUBJECT_PROPERTY_NAME, jwt_decode, jwt_encode
 from .misc_utils import get_request_domain
 
 logging.basicConfig()
@@ -27,58 +27,66 @@
 
     def __init__(self, auth0_client: str, auth0_secret: str, envs: Envs):
         self._auth0_client = auth0_client
         self._auth0_secret = auth0_secret
         self._envs = envs
         # acquired from identity or env variable locally
         try:
+            print('xyzzy/Auth/enter')
             self._redis = RedisBase(create_redis_client(
                 url=os.environ['REDIS_HOST'])
             ) if 'REDIS_HOST' in os.environ else None
+            print('xyzzy/Auth/redis-info')
+            print(self._redis)
+            print(os.environ['REDIS_HOST'])
         except redis.exceptions.ConnectionError:
             PRINT('Cannot connect to Redis')
             PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
             self._redis = None
 
     _cached_aws_credentials = {}
 
     def get_redis_handler(self):
         """
         Returns a handler to Redis or None if not in use
         """
         return self._redis
 
-    @classmethod
-    def get_redis_namespace(cls, env: str) -> str:
-        ignored(env)
-        # As of April 2023 simply use a static non-per-environment namespace for the Redis
-        # auth token; this is so we can switch among different environments in Foursight
-        # with the same login session, as it was working before the Redis auth work;
-        return "foursight"
-
     def authorize(self, request: dict, env: Optional[str] = None) -> dict:
         """
         Verifies that the given request is authenticated AND authorized, based on the authtoken
         cookie (a JWT-signed-encoded value) in the given request. If so, returns the verified and
         decoded authtoken as a dictionary. If not, returns a dictionary indicating not authorized
         and/or not authenticated, and containing the basic info from the authtoken.
         """
+        print('xyzzy/authorize/enter')
+        print(request)
+        print(env)
+        print(full_env_name(env))
         try:
             # Read the c4_st token (new Redis session token if Redis is in use)
             if self._redis:
+                print('xyzzy/authorize/redis')
                 c4_st = read_cookie(request, SESSION_TOKEN_COOKIE)
+                print('xyzzy/authorize/redis/c4_st')
+                print(c4_st)
                 redis_session_token = RedisSessionToken.from_redis(
                     redis_handler=self._redis,
-                    namespace=self.get_redis_namespace(env),
+                    namespace=full_env_name(env),
                     token=c4_st
                 )
+                print('xyzzy/authorize/redis/session_token')
+                print(redis_session_token)
+                print(redis_session_token.validate_session_token(redis_handler=self._redis))
                 # if this session token is not valid, nothing else is to be trusted, so bail here
                 if (not redis_session_token or
                         not redis_session_token.validate_session_token(redis_handler=self._redis)):
+                    print('xyzzy/authorize/redis/not-validated')
                     return self._create_unauthenticated_response(request, "missing-or-invalid-session-token")
+            print('xyzzy/authorize/redis/a')
 
             # Read the authtoken cookie (will always be present).
 
             authtoken = read_cookie(request, AUTH_TOKEN_COOKIE)
             if not authtoken:
                 return self._create_unauthenticated_response(request, "no-authtoken")
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/aws_logs.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/aws_logs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py---` & `foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py---`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/checks.py-new` & `foursight_core-4.1.0.1b6/foursight_core/react/api/checks.py-new`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 return True
         return False
 
     @memoize
     def is_same_env(self, env_a: str, env_b: str) -> bool:
         return foursight_env_name(env_a) == foursight_env_name(env_b)
 
-    def get_user_auth_info(self, email: str) -> Tuple[list, str, str]:
+    def get_user_auth_info(self, email: str, raise_exception: bool = False) -> Tuple[list, str, str]:
         """
         Returns a tuple containing (in left-right order): the list of known environments,
         i.e the list of annotated environment name objects; the list of allowed environment
         names for the given user/email, via the users store in ElasticSearch; and since we're
         getting the user record anyways, the first/last name of the user, for display only.
         """
         allowed_envs = []
@@ -87,14 +87,16 @@
                     # Since this is in a loop, for each env, this setup here will end up getting first/last name
                     # from the last env in the loop; doesn't really matter, just pick one set; this is just for
                     # informational/display purposes in the UI.
                     first_name = user.get("first_name")
                     last_name = user.get("last_name")
                     allowed_envs.append(known_env["full_name"])
             except Exception as e:
+                if raise_exception:
+                    raise e
                 logger.warning(f"Exception getting allowed envs for {email}: {e}")
         return allowed_envs, first_name, last_name
 
     @staticmethod
     def _is_user_allowed_access(user: Optional[dict]) -> bool:
         return user and Envs._is_user_in_one_or_more_groups(user, ["admin", "foursight"])
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/foo` & `foursight_core-4.1.0.1b6/foursight_core/react/api/foo`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/hama` & `foursight_core-4.1.0.1b6/foursight_core/react/api/hama`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/hmm` & `foursight_core-4.1.0.1b6/foursight_core/react/api/hmm`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/ok` & `foursight_core-4.1.0.1b6/foursight_core/react/api/ok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/oklk` & `foursight_core-4.1.0.1b6/foursight_core/react/api/oklk`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/okok` & `foursight_core-4.1.0.1b6/foursight_core/react/api/okok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/okokok` & `foursight_core-4.1.0.1b6/foursight_core/react/api/okokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/okokokok` & `foursight_core-4.1.0.1b6/foursight_core/react/api/okokokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/okokokokok` & `foursight_core-4.1.0.1b6/foursight_core/react/api/okokokokok`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/ot` & `foursight_core-4.1.0.1b6/foursight_core/react/api/ot`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .gac import Gac
 from .misc_utils import (
     get_base_url,
     is_running_locally,
     memoize,
     sort_dictionary_by_case_insensitive_keys
 )
+from .portal_access_key_utils import get_portal_access_key_info
 from .react_routes import ReactRoutes
 from .react_api_base import ReactApiBase
 from .react_ui import ReactUi
 
 
 # Implementation functions corresponding directly to the routes in react_routes.
 class ReactApi(ReactApiBase, ReactRoutes):
@@ -277,15 +278,17 @@
         data["auth"] = auth
         # 2022-10-18
         # No longer sharing known-envs widely; send only if authenticated;
         # if not authenticated then act as-if the default-env is the only known-env;
         # in this case also include (as an FYI for the UI) the real number of known-envs.
         if auth["authenticated"]:
             data["auth"]["known_envs"] = self._envs.get_known_envs_with_gac_names()
+            is_logged_in = True
         else:
+            is_logged_in = False
             known_envs_default = self._envs.find_known_env(self._envs.get_default_env())
             known_envs_actual_count = self._envs.get_known_envs_count()
             data["auth"]["known_envs"] = [known_envs_default]
             data["auth"]["known_envs_actual_count"] = known_envs_actual_count
         data["auth"]["default_env"] = self._envs.get_default_env()
         test_mode_certificate_simulate_error = read_cookie_bool(request, "test_mode_certificate_simulate_error")
         if test_mode_certificate_simulate_error:
@@ -305,15 +308,32 @@
                 e = str(e)
                 data["portal"]["exception"] = e
                 if "certifi" in e.lower():
                     data["portal"]["ssl_certificate_error"] = True
                 portal_url = env_utils_get_portal_url(env)
                 data["portal"]["url"] = portal_url
                 data["portal"]["ssl_certificate"] = get_ssl_certificate_info(portal_url)
+                data["portal"]["ssl_certificate"]["name"] = "Portal"
+                data["portal"]["ssl_certificate"]["exception"] = e
         data["timestamp"] = convert_utc_datetime_to_useastern_datetime_string(datetime.datetime.utcnow())
+        test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
+        if auth.get("user_exception"): # or test_mode_access_key_simulate_error:
+            # Since this call to get the Portal access key info can be relatively expensive, we don't want to
+            # do it on every /header API call; so we only call it if, according to the user's authtoken cookie,
+            # an exception was experienced when trying to authorize the user (via envs.get_user_auth_info) on
+            # login, which if so, would indicate that the is likely a problem with the Portal access key.
+            test_mode_access_key_expiration_warning_days = \
+                read_cookie_int(request, "test_mode_access_key_expiration_warning_days")
+            data["portal_access_key"] = get_portal_access_key_info(
+                env,
+                obfuscate=not is_logged_in,
+                test_mode_access_key_simulate_error=test_mode_access_key_simulate_error,
+                test_mode_access_key_expiration_warning_days=test_mode_access_key_expiration_warning_days)
+            if not data["portal_access_key"].get("valid"):
+                data["portal_access_key_error"] = True
         return self.create_success_response(data)
 
     def _reactapi_header_nocache(self, request: dict, env: str) -> dict:
         """
         No-cache version of above reactapi_header function.
         """
         domain, context = app.core.get_domain_and_context(request)
@@ -331,14 +351,15 @@
                 "domain": domain,
                 "context": context,
                 "stack": self._get_stack_name(),
                 "local": is_running_locally(request),
                 "credentials": {
                     "aws_account_number": aws_credentials.get("aws_account_number"),
                     "aws_account_name": aws_credentials.get("aws_account_name"),
+                    "aws_access_key_id": aws_credentials.get("aws_access_key_id"),
                     "re_captcha_key": os.environ.get("reCaptchaKey", None)
                 },
                 "launched": app.core.init_load_time,
                 "deployed": app.core.get_lambda_last_modified(),
                 "accounts_file": self._get_accounts_file(),
                 "accounts_file_from_s3": self._get_accounts_file_from_s3()
             },
@@ -377,14 +398,28 @@
             portal_ssl_certificate_info = get_ssl_certificate_info(
                 portal_url, test_mode_certificate_expiration_warning_days=test_mode_certificate_expiration_warning_days)
             if portal_ssl_certificate_info:
                 portal_ssl_certificate_info["name"] = "Portal"
                 response.append(portal_ssl_certificate_info)
         return self.create_success_response(response)
 
+    def reactapi_portal_access_key(self, request: dict, args: Optional[dict] = None) -> Response:
+        env = self._envs.get_default_env()
+        auth = self._auth.authorize(request, env)
+        is_logged_in = auth.get("authenticated")
+        test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
+        test_mode_access_key_expiration_warning_days = read_cookie_int(
+                request, "test_mode_access_key_expiration_warning_days")
+        response = get_portal_access_key_info(
+            env,
+            obfuscate=not is_logged_in,
+            test_mode_access_key_simulate_error=test_mode_access_key_simulate_error,
+            test_mode_access_key_expiration_warning_days=test_mode_access_key_expiration_warning_days)
+        return self.create_success_response(response)
+
     @memoize
     def _get_env_and_bucket_info(self, env: str, stage_name: str) -> dict:
         return sort_dictionary_by_case_insensitive_keys(
             obfuscate_dict(app.core.environment.get_environment_and_bucket_info(env, stage_name)))
 
     @memoize
     def _get_check_result_bucket_name(self, env: str) -> Optional[str]:
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py--` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py--`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py----` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py----`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-deb` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api.py-saaave` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api.py-saaave`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         if not jwt:
             return self.create_forbidden_response()
 
         jwt_expires_in = auth0_response_json.get("expires_in")
         jwt_expires_at = convert_datetime_to_time_t(datetime.datetime.utcnow() +
                                                     datetime.timedelta(seconds=jwt_expires_in))
         domain, context = app.core.get_domain_and_context(request)
-        authtoken = self._auth.create_authtoken(jwt, jwt_expires_at, domain)
+        authtoken = self._auth.create_authtoken(jwt, jwt_expires_at, domain, request=request)
         authtoken_cookie = create_set_cookie_string(request, name=AUTH_TOKEN_COOKIE,
                                                     value=authtoken,
                                                     domain=domain,
                                                     expires=jwt_expires_at, http_only=False)
 
         # if Redis is in use, create and return session token as well
         redis_handler = self._auth.get_redis_handler()
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_api_base.py-deb` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_api_base.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_app.py-saaave` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_app.py-saaave`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_utils.py-` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_utils.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_route_utils.py.save` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_route_utils.py.save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,28 +79,45 @@
     @route("/{env}/certificates", authorize=False)
     def reactapi_route_certificates(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
         Note that this in an UNPROTECTED route.
         Returns SSL certificate info about this Foursight instance and its associated Portal instance.
         """
         ignored(env)
-        #args = get_request_args(request_dict)
-        #return app.core.reactapi_certificates(app.current_request.to_dict(), args)
         return ReactRoutes.reactapi_route_certificates_noenv()
 
     @route("/certificates", authorize=False)
     def reactapi_route_certificates_noenv() -> Response:  # noqa: implicit @staticmethod via @route
         """
         Note that this in an UNPROTECTED route.
         Returns SSL certificate info about this Foursight instance and its associated Portal instance.
         """
         request_dict = app.current_request.to_dict()
         args = get_request_args(request_dict)
         return app.core.reactapi_certificates(request_dict, args)
 
+    @route("/{env}/portal_access_key", authorize=False)
+    def reactapi_route_portal_access_key(env: str) -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Returns Portal access key info about this Foursight instance.
+        """
+        ignored(env)
+        return ReactRoutes.reactapi_route_portal_access_key_noenv()
+
+    @route("/portal_access_key", authorize=False)
+    def reactapi_route_portal_access_key_noenv() -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Returns Portal access key info about this Foursight instance.
+        """
+        request_dict = app.current_request.to_dict()
+        args = get_request_args(request_dict)
+        return app.core.reactapi_portal_access_key(request_dict, args)
+
     # ----------------------------------------------------------------------------------------------
     # Foursight React API routes PROTECTED by authorization/authentication.
     # ----------------------------------------------------------------------------------------------
 
     @route("/{env}/info", authorize=True)
     def reactapi_route_info(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_routes.py.save` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_routes.py.save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py-bak` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py-bak`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/react_ui.py-debug` & `foursight_core-4.1.0.1b6/foursight_core/react/api/react_ui.py-debug`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/sa` & `foursight_core-4.1.0.1b6/foursight_core/react/api/sa`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/sav` & `foursight_core-4.1.0.1b6/foursight_core/react/api/sav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/save` & `foursight_core-4.1.0.1b6/foursight_core/react/api/save`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/xx` & `foursight_core-4.1.0.1b6/foursight_core/react/api/xx`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/xxy` & `foursight_core-4.1.0.1b6/foursight_core/react/api/xxy`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/xyz` & `foursight_core-4.1.0.1b6/foursight_core/react/api/xyz`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.1b6/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.1b6/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.1b6/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.86d9a011.js.LICENSE.txt */
+/*! For license information please see main.ebf666e0.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -49228,14 +49228,196 @@
                     }), e.tooltip && (0, Kr.jsx)(Mi, {
                         id: e.href,
                         text: e.tooltip
                     })]
                 })
             },
             Ii = function(e) {
+                var n = e.accessKey,
+                    r = e.error ? "darkred" : "inhert",
+                    o = {
+                        fontSize: "11pt",
+                        color: r,
+                        verticalAlign: "top",
+                        paddingBottom: "2pt",
+                        paddingRight: "10pt",
+                        whiteSpace: "nowrap"
+                    },
+                    i = Ye(Ye({}, o), {}, {
+                        width: "1%"
+                    }),
+                    s = a((0, t.useState)(!1), 2),
+                    u = s[0],
+                    l = s[1];
+                return n ? (0, Kr.jsx)(Kr.Fragment, {
+                    children: (0, Kr.jsx)("table", {
+                        width: "100%",
+                        children: (0, Kr.jsxs)("tbody", {
+                            children: [(0, Kr.jsxs)("tr", {
+                                children: [(0, Kr.jsx)("td", {
+                                    style: i,
+                                    children: "Access Key:"
+                                }), (0, Kr.jsxs)("td", {
+                                    style: o,
+                                    children: [n.key, (0, Kr.jsx)("small", {
+                                        style: {
+                                            float: "right",
+                                            marginRight: "-10pt"
+                                        },
+                                        children: (0, Kr.jsx)("b", {
+                                            children: u ? (0, Kr.jsx)(Kr.Fragment, {
+                                                children: (0, Kr.jsxs)("span", {
+                                                    onClick: function() {
+                                                        return l(!1)
+                                                    },
+                                                    style: {
+                                                        cursor: "pointer"
+                                                    },
+                                                    children: ["JSON\xa0", Fr.DownArrow]
+                                                })
+                                            }) : (0, Kr.jsx)(Kr.Fragment, {
+                                                children: (0, Kr.jsxs)("span", {
+                                                    onClick: function() {
+                                                        return l(!0)
+                                                    },
+                                                    style: {
+                                                        cursor: "pointer"
+                                                    },
+                                                    children: ["JSON\xa0", Fr.UpArrow]
+                                                })
+                                            })
+                                        })
+                                    })]
+                                })]
+                            }), (0, Kr.jsxs)("tr", {
+                                children: [(0, Kr.jsx)("td", {
+                                    style: i,
+                                    children: "Access Key Secret:"
+                                }), (0, Kr.jsx)("td", {
+                                    style: o,
+                                    children: n.secret
+                                })]
+                            }), (0, Kr.jsxs)("tr", {
+                                children: [(0, Kr.jsx)("td", {
+                                    style: i,
+                                    children: "Expiration Date:"
+                                }), (0, Kr.jsxs)("td", {
+                                    style: o,
+                                    children: [n.expires_at, n.expired ? (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0\xa0", Fr.RightArrow, "\xa0\xa0", (0, Kr.jsx)("b", {
+                                            children: (0, Kr.jsx)("u", {
+                                                children: "Expired"
+                                            })
+                                        }), "\xa0\xa0", Fr.LeftArrow, "\xa0\xa0", (0, Kr.jsx)("small", {
+                                            children: Pr.Ago(n.expires_at, !0, !1)
+                                        })]
+                                    }) : (0, Kr.jsxs)(Kr.Fragment, {
+                                        children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)("small", {
+                                            children: Pr.FromNow(n.expires_at, !0, !1)
+                                        })]
+                                    })]
+                                })]
+                            }), n.exception && (0, Kr.jsxs)("tr", {
+                                children: [(0, Kr.jsx)("td", {
+                                    style: i,
+                                    children: "Error:"
+                                }), (0, Kr.jsx)("td", {
+                                    style: o,
+                                    children: n.exception
+                                })]
+                            }), u && (0, Kr.jsxs)(Kr.Fragment, {
+                                children: [(0, Kr.jsx)("tr", {
+                                    children: (0, Kr.jsx)("td", {
+                                        style: {
+                                            height: "2pt"
+                                        }
+                                    })
+                                }), (0, Kr.jsx)("tr", {
+                                    children: (0, Kr.jsx)("td", {
+                                        colSpan: "2",
+                                        children: (0, Kr.jsx)("pre", {
+                                            style: {
+                                                background: "inherit",
+                                                color: r,
+                                                marginTop: "2pt",
+                                                whiteSpace: "pre-wrap"
+                                            },
+                                            children: JSON.stringify(n, null, 2)
+                                        })
+                                    })
+                                })]
+                            })]
+                        })
+                    })
+                }) : (0, Kr.jsx)(Kr.Fragment, {})
+            },
+            Di = function(e) {
+                var t, n, r = e.header;
+                return (0, Kr.jsx)(Kr.Fragment, {
+                    children: (0, Kr.jsx)("div", {
+                        className: "container",
+                        style: {
+                            width: "800pt"
+                        },
+                        children: (0, Kr.jsxs)("div", {
+                            className: "box error thickborder",
+                            children: [(0, Kr.jsx)("img", {
+                                src: "https://cdn.pixabay.com/photo/2015/06/09/16/12/no-access-803719_1280.png",
+                                height: "30",
+                                style: {
+                                    paddingBottom: "3pt"
+                                }
+                            }), (0, Kr.jsx)("b", {
+                                style: {
+                                    fontSize: "16pt",
+                                    marginLeft: "10pt"
+                                },
+                                children: "Access Key Error"
+                            }), (0, Kr.jsx)("br", {}), (0, Kr.jsx)(wi, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), "There is a problem with the access key for the ", (0, Kr.jsx)("b", {
+                                children: "Portal"
+                            }), " associated with this Foursight instance: \xa0", (0, Kr.jsx)("b", {
+                                children: (0, Kr.jsx)("small", {
+                                    children: (0, Kr.jsx)("a", {
+                                        href: null === r || void 0 === r || null === (t = r.portal) || void 0 === t ? void 0 : t.url,
+                                        style: {
+                                            color: "darkred"
+                                        },
+                                        target: "_blank",
+                                        children: null === r || void 0 === r || null === (n = r.portal) || void 0 === n ? void 0 : n.url
+                                    })
+                                })
+                            }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)(wi, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), (0, Kr.jsxs)("b", {
+                                children: [Fr.RightArrow, " ", (0, Kr.jsxs)("small", {
+                                    children: [(0, Kr.jsxs)("i", {
+                                        children: ["You ", (0, Kr.jsx)("u", {
+                                            children: "must"
+                                        }), " contact your system adminstrator to resolve this issue"]
+                                    }), "\xa0\xa0:-("]
+                                })]
+                            }), (0, Kr.jsx)(wi, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), (0, Kr.jsx)(Ii, {
+                                accessKey: null === r || void 0 === r ? void 0 : r.portal_access_key,
+                                error: !0
+                            })]
+                        })
+                    })
+                })
+            },
+            Si = function(e) {
                 var n = e.certificate,
                     r = e.error ? "darkred" : "inhert",
                     o = {
                         fontSize: "11pt",
                         color: r,
                         verticalAlign: "top",
                         paddingBottom: "2pt",
@@ -49478,16 +49660,16 @@
                                     })
                                 })]
                             })]
                         })
                     })
                 }) : (0, Kr.jsx)(Kr.Fragment, {})
             },
-            Di = function(e) {
-                var t = e.header;
+            Li = function(e) {
+                var t, n, r, o = e.header;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
                         children: (0, Kr.jsxs)("div", {
@@ -49506,20 +49688,20 @@
                                 bottom: "6pt",
                                 color: "darkred"
                             }), "There is a problem with the SSL certificate for the ", (0, Kr.jsx)("b", {
                                 children: "Portal"
                             }), " associated with this Foursight instance: \xa0", (0, Kr.jsx)("b", {
                                 children: (0, Kr.jsx)("small", {
                                     children: (0, Kr.jsx)("a", {
-                                        href: t.portal.url,
+                                        href: null === o || void 0 === o || null === (t = o.portal) || void 0 === t ? void 0 : t.url,
                                         style: {
                                             color: "darkred"
                                         },
                                         target: "_blank",
-                                        children: t.portal.url
+                                        children: null === o || void 0 === o || null === (n = o.portal) || void 0 === n ? void 0 : n.url
                                     })
                                 })
                             }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)(wi, {
                                 top: "6pt",
                                 bottom: "6pt",
                                 color: "darkred"
                             }), (0, Kr.jsxs)("b", {
@@ -49530,123 +49712,134 @@
                                         }), " contact your system adminstrator to resolve this issue"]
                                     }), "\xa0\xa0:-("]
                                 })]
                             }), (0, Kr.jsx)(wi, {
                                 top: "6pt",
                                 bottom: "6pt",
                                 color: "darkred"
-                            }), (0, Kr.jsx)(Ii, {
-                                certificate: t.portal.ssl_certificate,
+                            }), (0, Kr.jsx)(Si, {
+                                certificate: null === o || void 0 === o || null === (r = o.portal) || void 0 === r ? void 0 : r.ssl_certificate,
                                 error: !0
                             })]
                         })
                     })
                 })
             },
-            Si = function(e) {
+            ki = function(e) {
+                return null === e || void 0 === e ? void 0 : e.portal_access_key_error
+            },
+            Ci = function(e) {
                 var t;
                 return null === e || void 0 === e || null === (t = e.portal) || void 0 === t ? void 0 : t.ssl_certificate_error
             },
-            Li = function(e) {
-                var t = Xi();
-                return Si(t) ? (0, Kr.jsx)(Kr.Fragment, {
-                    children: (0, Kr.jsx)(Di, {
+            Ei = function(e) {
+                var t = ta();
+                return (0, Kr.jsxs)(Kr.Fragment, {
+                    children: [ki(t) && (0, Kr.jsx)(Di, {
                         header: t
-                    })
-                }) : (0, Kr.jsx)(Kr.Fragment, {})
+                    }), Ci(t) && (0, Kr.jsx)(Li, {
+                        header: t
+                    })]
+                })
             };
-        Li.IsFatalError = Si;
-        var ki = Li;
+        Ei.IsFatalError = function(e) {
+            return Ci(e) || ki(e)
+        };
+        var _i = Ei;
 
-        function Ci(e) {
+        function Ti(e) {
             var t = At.PreferredName(At.Default(e), e);
             if (At.IsKnown(t, e)) {
                 var n = kr.Path(kr.CurrentLogicalPath(), t);
                 n !== window.location.href && (window.location.href = n)
             }
         }
 
-        function Ei() {
+        function Ai() {
             var e = window.location.pathname.substring(1).split("/");
             return e.length >= 2 && ("api" !== e[0] || "react" !== e[1]) && ("react" === e[0] ? (window.location.pathname = "/api/".concat(e.join("/")), !0) : ("api" === e[0] && e.shift(), window.location.pathname = "/api/react/".concat(e.join("/")), !0))
         }
 
-        function _i(e) {
+        function Oi(e) {
             At.IsKnown(At.Current(), e) && bt.SetLastUrl(window.location.href)
         }
 
-        function Ti() {
+        function zi() {
             return bt.LastUrl() || kr.HomeUrl()
         }
-        var Ai = {
+        var Ui = {
             AuthorizationRequired: function(e) {
                 var t = e.children,
-                    n = Xi();
-                return ki.IsFatalError(n) ? (0, Kr.jsx)(xe, {
+                    n = ta();
+                return _i.IsFatalError(n) ? (0, Kr.jsx)(xe, {
                     to: kr.Path("/error"),
                     replace: !0
-                }) : Ei() ? void 0 : Br.IsLoggedIn(n) ? At.IsKnown(At.Current(), n) ? At.IsAllowed(At.Current(), n) ? (_i(), t) : (0, Kr.jsx)(xe, {
+                }) : Ai() ? void 0 : Br.IsLoggedIn(n) ? At.IsKnown(At.Current(), n) ? At.IsAllowed(At.Current(), n) ? (Oi(), t) : (0, Kr.jsx)(xe, {
                     to: kr.Path("/env"),
                     replace: !0
-                }) : Ci(n) : (0, Kr.jsx)(xe, {
+                }) : Ti(n) : (0, Kr.jsx)(xe, {
                     to: kr.Path("/login"),
                     replace: !0
                 })
             },
             KnownEnvRequired: function(e) {
                 var t = e.children,
-                    n = Xi();
-                return ki.IsFatalError(n) ? (0, Kr.jsx)(xe, {
-                    to: kr.Path("/error"),
-                    replace: !0
-                }) : Ei() ? void 0 : n.loading ? t : At.IsKnown(At.Current(), n) ? (_i(), t) : Ci(n)
+                    n = ta();
+                if (_i.IsFatalError(n)) {
+                    var r = At.PreferredName(At.Default(n), n);
+                    return (0, Kr.jsx)(xe, {
+                        to: kr.Path("/error", r),
+                        replace: !0
+                    })
+                }
+                if (!Ai()) return n.loading ? t : At.IsKnown(At.Current(), n) ? (Oi(), t) : Ti(n)
             },
             LastPath: function() {
-                var e = Ti(),
+                var e = zi(),
                     t = kr.BaseUrl();
                 return e.startsWith(t) ? kr.Path(e.substring(t.length), !1) : e
             },
-            LastUrl: Ti,
-            NoteLastUrl: _i,
+            LastUrl: zi,
+            NoteLastUrl: Oi,
             Unprotected: function(e) {
                 return e.children
             }
         };
-        var Oi = function() {
-                bt.DeleteAuth(), bt.SetRedirect(Ai.LastUrl()), window.location.replace(zt.Url("/logout"))
+        var Pi = function() {
+                bt.DeleteAuth(), bt.SetRedirect(Ui.LastUrl()), window.location.replace(zt.Url("/logout"))
             },
-            zi = __webpack_require__(599),
-            Ui = {
+            Ri = __webpack_require__(599),
+            Bi = {
                 Format: function(e) {
                     var t;
-                    return null === (t = zi.stringify(e)) || void 0 === t ? void 0 : t.trimLeft()
+                    return null === (t = Ri.stringify(e)) || void 0 === t ? void 0 : t.trimLeft()
                 }
             },
-            Pi = function() {
+            Fi = function() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null;
                 return "function" === typeof e && (e = e()), {
                     value: e,
                     __listeners: new Set
                 }
             },
-            Ri = function(e) {
+            Yi = function(e) {
                 var n = a((0, t.useState)(), 2)[1];
                 return (0, t.useEffect)((function() {
                     return e.__listeners.add(n),
                         function() {
                             return e.__listeners.delete(n)
                         }
                 }), [e.value, e.__listeners]), [e.value, function(t) {
                     e.value = t, e.__listeners.forEach((function(e) {
                         return e({})
                     }))
                 }]
             },
-            Bi = bt.TestMode.FetchSleep(),
-            Fi = function(e, n) {
+            Qi = bt.TestMode.FetchSleep(),
+            Gi = function(e, n) {
                 var r = st.IsObject(e) ? e.initial : st.IsObject(n) ? n.initial : null,
                     o = a((0, t.useState)(r), 2),
                     i = o[0],
                     l = o[1],
                     c = a((0, t.useState)(!1), 2),
                     d = c[0],
                     f = c[1],
@@ -49655,48 +49848,48 @@
                     g = p[1],
                     y = a((0, t.useState)(!1), 2),
                     m = y[0],
                     v = y[1],
                     M = a((0, t.useState)(null), 2),
                     b = M[0],
                     w = M[1],
-                    j = Gi(),
-                    x = Wi();
+                    j = Zi(),
+                    x = Vi();
 
                 function N() {
                     var t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                         r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                         o = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
-                    return Vi(e, n, t, r, l, f, g, v, w, j, x, o)
+                    return Ki(e, n, t, r, l, f, g, v, w, j, x, o)
                 }
                 var I = N(),
                     D = {
                         loading: d,
                         data: i,
                         status: h,
                         error: b,
                         timeout: m,
                         set: l,
                         __usefetch_response: !0
                     };
                 return D.fetch = function(e, t) {
-                        Zi(N(e, t, !0), this && !0 === this.__usefetch_response ? this.data : void 0, this)
+                        Ji(N(e, t, !0), this && !0 === this.__usefetch_response ? this.data : void 0, this)
                     }.bind(D), D.refresh = function(e, t) {
-                        Zi(Ye(Ye({}, N(e, t, !0)), {}, {
+                        Ji(Ye(Ye({}, N(e, t, !0)), {}, {
                             nocache: !0
                         }), this && !0 === this.__usefetch_response ? this.data : void 0, this)
                     }.bind(D), D.update = function(e) {
                         var t;
                         void 0 === e && (e = this), !0 === (null === (t = e) || void 0 === t ? void 0 : t.__usefetch_response) && (e = e.data),
                             function(e, t) {
                                 var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : void 0;
                                 Object.is(t, n) ? st.IsObject(t) ? e(Ye({}, t)) : st.IsArray(t) ? e(st.CopyArrayProperties(t, u(t))) : st.IsFunction(t) ? e(t()) : e(t) : e(t)
                             }(l, e, this && this.__usefetch_response ? this.data : void 0)
                     }.bind(D), D.uncache = function(e, t) {
-                        I.cache && Hi[e] && delete Hi[e]
+                        I.cache && qi[e] && delete qi[e]
                     }.bind(D),
                     function(e) {
                         e.__response = !0, Object.defineProperty(e, "length", {
                             get: function() {
                                 if (this && this.__response) return st.IsArray(this.data) ? this.data.length : void 0
                             }.bind(e)
                         }), Object.defineProperty(e, "null", {
@@ -49779,24 +49972,24 @@
                                 var r = this.get(n);
                                 st.IsArray(r) && r.forEach(e)
                             }
                         }.bind(e), e.json = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                             if (this && this.__response) return st.IsBoolean(e) && e ? Tr.Format(this.data) : Tr.Str(this.data)
                         }.bind(e), e.yaml = function() {
-                            if (this && this.__response) return Ui.Format(this.data)
+                            if (this && this.__response) return Bi.Format(this.data)
                         }.bind(e)
                     }(D), (0, t.useEffect)((function() {
-                        Zi(I, void 0, D)
+                        Ji(I, void 0, D)
                     }), [I.url]), D
             },
-            Yi = Pi(new Map),
-            Qi = Pi([]),
-            Gi = function() {
-                var e = a(Ri(Yi), 2),
+            Wi = Fi(new Map),
+            Hi = Fi([]),
+            Zi = function() {
+                var e = a(Yi(Wi), 2),
                     t = e[0],
                     n = e[1];
                 return {
                     value: t,
                     add: function(e) {
                         var r = Dr()();
                         return e.id = r, e.timestamp = new Date, t.set(r, e), n(t), r
@@ -49806,36 +49999,36 @@
                         return t.delete(e), n(t), r
                     },
                     clear: function() {
                         t.clear(), n(t)
                     }
                 }
             },
-            Wi = function() {
-                var e = a(Ri(Qi), 2),
+            Vi = function() {
+                var e = a(Yi(Hi), 2),
                     t = e[0],
                     n = e[1];
                 return {
                     value: t,
                     add: function(e, r) {
                         e.data = r, e.duration = new Date - e.timestamp, t.length >= 25 && t.shift(), t.push(e), n(t)
                     },
                     clear: function() {
                         t.length = 0, n(t)
                     }
                 }
             },
-            Hi = {};
+            qi = {};
 
-        function Zi(e) {
+        function Ji(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                 n = arguments.length > 2 ? arguments[2] : void 0;
             if (!e.nofetch && it.HasValue(e.url)) {
                 if (e.cache && !e.nocache) {
-                    var r = Hi[e.url];
+                    var r = qi[e.url];
                     if (r) return _r.Info("FETCH FOUND CACHED RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(r.status)), e.onData(r.data, r.data), e.setData(r.data), e.setStatus(r.status), e.setLoading(!1), e.setTimeout(!1), e.setError(null), n || (n = {
                         data: r.data,
                         loading: !1,
                         status: r.status,
                         timeout: !1,
                         error: null
                     }), e.onSuccess(n), void e.onDone(n)
@@ -49859,15 +50052,15 @@
                 }))
             }
 
             function a(r, o) {
                 var i = r.status;
                 _r.Info("FETCH RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i), r.data);
                 var a = e.onData(r.data, t);
-                void 0 === a && (a = r.data), n && (n.status = i, n.data = a, n.loading = !1), e.setStatus(i), e.setData(a), e.setLoading(!1), l(o, a), e.onSuccess(n), e.onDone(n), e.cache && (_r.Info("FETCH CACHING RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i)), Hi[e.url] = {
+                void 0 === a && (a = r.data), n && (n.status = i, n.data = a, n.loading = !1), e.setStatus(i), e.setData(a), e.setLoading(!1), l(o, a), e.onSuccess(n), e.onDone(n), e.cache && (_r.Info("FETCH CACHING RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i)), qi[e.url] = {
                     data: a,
                     status: i
                 })
             }
 
             function s(t, r) {
                 var o, i, a, s, u, c = (null === (o = t.response) || void 0 === o ? void 0 : o.status) || 0,
@@ -49886,43 +50079,43 @@
                         loading: !1,
                         data: d,
                         status: c,
                         error: t,
                         timeout: f
                     }
                 }
-                401 === c ? (_r.Info("FETCH UNAUTHENTICATED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.nologout || (p(), Oi())) : 403 === c ? (_r.Info("FETCH UNAUTHORIZED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.noredirect || "/env" !== kr.CurrentLogicalPath() && (p(), window.location.pathname = kr.Path("/env"))) : "ECONNABORTED" === t.code ? (_r.Info("FETCH TIMEOUT ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), f = !0, c || (c = 504)) : "ERR_NETWORK" === t.code ? (_r.Info("FETCH NETWORK ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), c || (c = 404)) : _r.Info("FETCH ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c));
+                401 === c ? (_r.Info("FETCH UNAUTHENTICATED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.nologout || (p(), Pi())) : 403 === c ? (_r.Info("FETCH UNAUTHORIZED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.noredirect || "/env" !== kr.CurrentLogicalPath() && (p(), window.location.pathname = kr.Path("/env"))) : "ECONNABORTED" === t.code ? (_r.Info("FETCH TIMEOUT ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), f = !0, c || (c = 504)) : "ERR_NETWORK" === t.code ? (_r.Info("FETCH NETWORK ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), c || (c = 404)) : _r.Info("FETCH ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c));
                 var h = p();
                 l(r), void 0 !== (d = e.onError(h)) && (n && (n.data = d), e.setData(d)), e.onDone(h)
             }
 
             function u(t) {
                 return e.fetching.add(t)
             }
 
             function l(t) {
                 var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                 e.fetched.add(e.fetching.remove(t), n)
             }
         }
 
-        function Vi(e, t, n, r, o, i, a, s, u, l, c, d) {
+        function Ki(e, t, n, r, o, i, a, s, u, l, c, d) {
             var f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R, B, F;
             return st.IsObject(e) && (t = e, e = null), st.IsObject(n) && (r = n, n = null), t = {
                 url: st.First([n, null === (f = r) || void 0 === f ? void 0 : f.url, e, null === (p = t) || void 0 === p ? void 0 : p.url, ""], it.HasValue),
                 method: st.First([null === (h = r) || void 0 === h ? void 0 : h.method, null === (g = t) || void 0 === g ? void 0 : g.method, "GET"], it.HasValue),
                 payload: st.First([null === (y = r) || void 0 === y ? void 0 : y.payload, null === (m = t) || void 0 === m ? void 0 : m.payload, null], st.IsObject),
                 timeout: st.First([null === (v = r) || void 0 === v ? void 0 : v.timeout, null === (M = t) || void 0 === M ? void 0 : M.timeout, 3e4], st.IsInteger),
                 initial: st.First([null === (b = r) || void 0 === b ? void 0 : b.initial, null === (w = t) || void 0 === w ? void 0 : w.initial, null], (function(e) {
                     return !st.IsNull(e)
                 })),
                 nofetch: st.First([null === (j = r) || void 0 === j ? void 0 : j.nofetch, null === (x = t) || void 0 === x ? void 0 : x.nofetch, !1], st.IsBoolean),
                 nologout: st.First([null === (N = r) || void 0 === N ? void 0 : N.nologout, null === (I = t) || void 0 === I ? void 0 : I.nologout, !1], st.IsBoolean),
                 noredirect: st.First([null === (D = r) || void 0 === D ? void 0 : D.noredirect, null === (S = t) || void 0 === S ? void 0 : S.noredirect, !1], st.IsBoolean),
-                delay: st.First([null === (L = r) || void 0 === L ? void 0 : L.delay, null === (k = t) || void 0 === k ? void 0 : k.delay, Bi > 0 ? Bi : 0], st.IsInteger),
+                delay: st.First([null === (L = r) || void 0 === L ? void 0 : L.delay, null === (k = t) || void 0 === k ? void 0 : k.delay, Qi > 0 ? Qi : 0], st.IsInteger),
                 cache: st.First([null === (C = r) || void 0 === C ? void 0 : C.cache, null === (E = t) || void 0 === E ? void 0 : E.cache, null], st.IsBoolean),
                 nocache: st.First([null === (_ = r) || void 0 === _ ? void 0 : _.nocache, null === (T = t) || void 0 === T ? void 0 : T.nocache, null], st.IsBoolean),
                 onData: st.First([null === (A = r) || void 0 === A ? void 0 : A.onData, null === (O = t) || void 0 === O ? void 0 : O.onData, function() {}], st.IsFunction),
                 onSuccess: st.First([null === (z = r) || void 0 === z ? void 0 : z.onSuccess, null === (U = t) || void 0 === U ? void 0 : U.onSuccess, function() {}], st.IsFunction),
                 onError: st.First([null === (P = r) || void 0 === P ? void 0 : P.onError, null === (R = t) || void 0 === R ? void 0 : R.onError, function() {}], st.IsFunction),
                 onDone: st.First([null === (B = r) || void 0 === B ? void 0 : B.onDone, null === (F = t) || void 0 === F ? void 0 : F.onDone, function() {}], st.IsFunction),
                 setData: o,
@@ -49930,29 +50123,29 @@
                 setStatus: a,
                 setTimeout: s,
                 setError: u,
                 fetching: l,
                 fetched: c
             }, d && delete t.nofetch, !it.HasValue(t.url) || t.url.startsWith("https://") || t.url.startsWith("http://") || (t.url = zt.Url(t.url)), t
         }
-        var qi = Fi,
-            Ji = function(e, t) {
-                return Fi(e, Ye(Ye({}, t), {}, {
+        var Xi = Gi,
+            $i = function(e, t) {
+                return Gi(e, Ye(Ye({}, t), {}, {
                     nofetch: !0
                 }))
             },
-            Ki = t.createContext({}),
-            Xi = function() {
-                var e = (0, t.useContext)(Ki);
+            ea = t.createContext({}),
+            ta = function() {
+                var e = (0, t.useContext)(ea);
                 return e ? e[0] : {}
             },
-            $i = function() {
-                return [Array.from(Ri(Yi)[0].values())]
+            na = function() {
+                return [Array.from(Yi(Wi)[0].values())]
             },
-            ea = function(e) {
+            ra = function(e) {
                 var t, n, r, o, i, a, s, u, l = e.info,
                     c = e.foursightUrl;
                 return (0, Kr.jsx)("table", {
                     style: {
                         width: "100%"
                     },
                     children: (0, Kr.jsxs)("tbody", {
@@ -50359,15 +50552,15 @@
                                     children: Fr.EmptySet
                                 })
                             })]
                         })]
                     })
                 })
             },
-            ta = function(e) {
+            oa = function(e) {
                 var t = e.info;
                 return (0, Kr.jsx)("table", {
                     style: {
                         width: "100%",
                         margin: "0",
                         padding: "0"
                     },
@@ -50659,22 +50852,22 @@
                                     children: Fr.EmptySet
                                 })
                             })]
                         })]
                     })
                 })
             },
-            na = function(e) {
+            ia = function(e) {
                 var n, r, o, i, a, s, u = e.account,
                     l = e.header,
                     c = e.foursightUrl,
                     d = e.all,
                     f = e.decrementAccountCount,
                     p = e.brighten,
-                    h = qi("/accounts_from_s3/".concat(u.id), {
+                    h = Xi("/accounts_from_s3/".concat(u.id), {
                         onDone: function() {
                             return f()
                         },
                         cache: !0,
                         nofetch: !0
                     });
 
@@ -50800,15 +50993,15 @@
                                     style: {
                                         verticalAlign: "top"
                                     },
                                     children: [(0, Kr.jsx)("td", {
                                         style: {
                                             width: "70%"
                                         },
-                                        children: (0, Kr.jsx)(ea, {
+                                        children: (0, Kr.jsx)(ra, {
                                             info: h,
                                             header: l,
                                             foursightUrl: c
                                         })
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             paddingLeft: "10pt",
@@ -50822,15 +51015,15 @@
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             width: "30%",
                                             paddingLeft: "12pt",
                                             textAlign: "top",
                                             verticalAlign: "top"
                                         },
-                                        children: (0, Kr.jsx)(ta, {
+                                        children: (0, Kr.jsx)(oa, {
                                             info: h,
                                             header: l
                                         })
                                     })]
                                 })
                             })
                         }), (null === (s = h.data) || void 0 === s ? void 0 : s.__showraw) && (0, Kr.jsxs)(Kr.Fragment, {
@@ -50841,39 +51034,39 @@
                                     border: "1px",
                                     borderTop: "solid"
                                 }
                             }), (0, Kr.jsx)("pre", {
                                 style: {
                                     background: "inherit"
                                 },
-                                children: Ui.Format(h.data)
+                                children: Bi.Format(h.data)
                             })]
                         })]
                     })
                 }) : null
             },
-            ra = function(e) {
+            aa = function(e) {
                 var n, r, o, i, s, u, l, c, d, f = e.header,
                     p = a(Re(), 2),
                     h = p[0],
                     g = p[1],
                     y = h.get("all"),
                     m = a((0, t.useState)("true" === (null === y || void 0 === y ? void 0 : y.toLowerCase()) || "1" === y), 2),
                     v = m[0],
                     M = m[1],
-                    b = qi("/accounts_from_s3", {
+                    b = Xi("/accounts_from_s3", {
                         cache: !0
                     }),
                     w = a((0, t.useState)(0), 2),
                     j = w[0],
                     x = w[1],
                     N = a((0, t.useState)(!0), 2),
                     I = N[0],
                     D = N[1],
-                    S = a($i(), 1)[0];
+                    S = a(na(), 1)[0];
 
                 function L() {
                     x((function(e) {
                         return e - 1
                     })), D(!1)
                 }
 
@@ -50965,15 +51158,15 @@
                                     })]
                                 })
                             })]
                         })
                     }), b.length > 0 ? (0, Kr.jsxs)(Kr.Fragment, {
                         children: [null === b || void 0 === b ? void 0 : b.map((function(e, n) {
                             return (0, Kr.jsx)(t.Fragment, {
-                                children: (0, Kr.jsx)(na, {
+                                children: (0, Kr.jsx)(ia, {
                                     account: e,
                                     header: f,
                                     all: v,
                                     decrementAccountCount: L,
                                     foursightUrl: e.foursight_url
                                 })
                             }, e.id)
@@ -51004,24 +51197,24 @@
                             }) : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "No accounts info found."
                             })
                         })
                     })]
                 })
             },
-            oa = function(e) {
-                var t = Xi();
+            sa = function(e) {
+                var t = ta();
                 return (0, Kr.jsx)("div", {
                     className: "container",
-                    children: (0, Kr.jsx)(ra, {
+                    children: (0, Kr.jsx)(aa, {
                         header: t
                     })
                 })
             },
-            ia = function(e) {
+            ua = function(e) {
                 var t = e.columns,
                     n = e.list,
                     r = e.update,
                     o = e.refresh,
                     i = e.sort,
                     a = void 0 === i ? null : i,
                     s = e.state,
@@ -51219,23 +51412,23 @@
                                 },
                                 colSpan: "6"
                             })
                         })]
                     }), M]
                 })
             },
-            aa = function(e) {
+            la = function(e) {
                 var n = pe().environ,
-                    r = qi(zt.Url("/aws/s3/buckets", n), {
+                    r = Xi(zt.Url("/aws/s3/buckets", n), {
                         initial: []
                     }),
-                    o = qi({
+                    o = Xi({
                         initial: []
                     }),
-                    i = qi({
+                    i = Xi({
                         initial: []
                     }),
                     s = a((0, t.useState)(""), 2),
                     u = s[0],
                     l = s[1];
 
                 function c() {
@@ -51435,15 +51628,15 @@
                                         style: {
                                             height: "1px",
                                             background: Ft.GetForegroundColor(),
                                             marginBottom: "1pt"
                                         }
                                     }), (0, Kr.jsxs)("table", {
                                         width: "100%",
-                                        children: [(0, Kr.jsxs)(ia, {
+                                        children: [(0, Kr.jsxs)(ua, {
                                             columns: [{
                                                 label: "Key",
                                                 key: "key"
                                             }, {
                                                 label: "Size",
                                                 key: "size",
                                                 align: "right"
@@ -51629,15 +51822,15 @@
                                         style: {
                                             cursor: "copy",
                                             float: "right",
                                             fontFamily: "monospace"
                                         },
                                         src: Ut.Clipboard(),
                                         height: "19"
-                                    }), Ui.Format(t.content)]
+                                    }), Bi.Format(t.content)]
                                 })]
                             })
                         })
                     },
                     S = function(e) {
                         var t = e.condition,
                             n = e.color,
@@ -51707,39 +51900,39 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            sa = Pi((function() {
+            ca = Fi((function() {
                 return bt.IsReadOnlyMode()
             })),
-            ua = function() {
-                var e = a(Ri(sa), 2),
+            da = function() {
+                var e = a(Yi(ca), 2),
                     t = e[0],
                     n = e[1];
                 return [t, function(e) {
                     n(e), bt.SetReadOnlyMode(e)
                 }]
             },
-            la = function() {
+            fa = function() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                     t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
-                    n = Gi(),
-                    r = Wi();
+                    n = Zi(),
+                    r = Vi();
 
                 function o(o, i) {
-                    return Vi(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
+                    return Ki(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
                 }
                 return function(e, t) {
-                    return Zi(o(e, t))
+                    return Ji(o(e, t))
                 }
             },
-            ca = {
+            pa = {
                 FormatDateTime: function(e) {
                     var n = e.verbose,
                         r = void 0 !== n && n,
                         o = e.timezone,
                         i = void 0 === o || o,
                         s = a((0, t.useState)(new Date), 2),
                         u = s[0],
@@ -51789,143 +51982,143 @@
                                 id: "tooltip-timestamp-".concat(r || i),
                                 text: Pr.FormatDateTime(r || i)
                             })]
                         })
                     })
                 }
             },
-            da = ca;
+            ha = pa;
 
-        function fa(e) {
+        function ga(e) {
             e.update()
         }
 
-        function pa(e) {
+        function ya(e) {
             e.update()
         }
 
-        function ha(e) {
+        function ma(e) {
             e.update()
         }
 
-        function ga(e, t) {
-            e.__showingResults = !1, fa(t)
+        function va(e, t) {
+            e.__showingResults = !1, ga(t)
         }
 
-        function ya(e, t, n) {
-            e.__showingResults = !0, fa(n)
+        function Ma(e, t, n) {
+            e.__showingResults = !0, ga(n)
         }
 
-        function ma(e, t, n) {
-            Ma(e, n) || (n.prepend(e), fa(n))
+        function ba(e, t, n) {
+            ja(e, n) || (n.prepend(e), ga(n))
         }
 
-        function va(e, t, n) {
+        function wa(e, t, n) {
             e.checks.map((function(e) {
-                return ja(e, n)
+                return Ia(e, n)
             }));
             var r = function(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     if (t.get(n).group === e.group) return n
                 }
                 return -1
             }(e, t);
             t.remove(r)
         }
 
-        function Ma(e, t) {
+        function ja(e, t) {
             for (var n = 0; n < t.length; n++) {
                 if (t.get(n).group === e.group) return !0
             }
             return !1
         }
 
-        function ba(e) {
+        function xa(e) {
             return null === e || void 0 === e ? void 0 : e.__showingResults
         }
 
-        function wa(e) {
+        function Na(e) {
             Object.keys(e.kwargs).forEach((function(t) {
                 if (!st.IsBoolean(e.kwargs[t]) && !st.IsNonEmptyArray(e.kwargs[t])) {
                     var n = "".concat(e.name, ".").concat(t),
                         r = document.getElementById(n),
                         o = null === r || void 0 === r ? void 0 : r.value;
                     e.kwargs[t] = o
                 }
             }))
         }
 
-        function ja(e, t) {
+        function Ia(e, t) {
             if (e.__showingHistory) {
                 e.__showingHistory = !1;
                 var n = function(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         if (t.get(n).name === e.name) return n
                     }
                     return -1
                 }(e, t);
                 t.remove(n)
             }
         }
 
-        function xa(e, t, n) {
+        function Da(e, t, n) {
             ! function(e, t, n) {
-                e.__showingHistory ? ja(e, n) : Na(e, t, n)
+                e.__showingHistory ? Ia(e, n) : Sa(e, t, n)
             }(e, t, n)
         }
 
-        function Na(e, t, n) {
+        function Sa(e, t, n) {
             e.__showingHistory || (e.__showingHistory = !0, n.prepend(e))
         }
 
-        function Ia(e, t, n, r, o) {
+        function La(e, t, n, r, o) {
             var i = e.kwargs,
                 a = Tr.Str(i),
                 s = btoa(a);
-            Sa(e, n), ha(n), e.__queueingCheckRun = !0, o({
+            Ca(e, n), ma(n), e.__queueingCheckRun = !0, o({
                     url: zt.Url("/checks/".concat(e.name, "/run?args=").concat(s), t),
                     onData: function(t) {
                         return e.__queueingCheckRun = !1, e.__queuedCheckRun = t.uuid, setTimeout((function() {
                             ! function(e) {
                                 e.__resultHistory && e.__resultHistory.refresh()
-                            }(e), ha(n)
+                            }(e), ma(n)
                         }), 4e3), t.uuid
                     }
                 }), e.__queuedCheckRun = null,
                 function(e, t) {
-                    e.showingCheckRunningBox = !0, ha(t)
-                }(e, n), Na(e, 0, r)
+                    e.showingCheckRunningBox = !0, ma(t)
+                }(e, n), Sa(e, 0, r)
         }
 
-        function Da(e, t, n, r, o) {
+        function ka(e, t, n, r, o) {
             var i, a = {
                     check_name: e.name,
                     called_by: null === (i = e.__result) || void 0 === i ? void 0 : i.get("uuid")
                 },
                 s = Tr.Str(a),
                 u = btoa(s);
-            La(e, r), ha(r), e.__queueingActionRun = !0, o({
+            Ea(e, r), ma(r), e.__queueingActionRun = !0, o({
                     url: zt.Url("/action/".concat(t, "/run?args=").concat(u), n),
                     onData: function(t) {
                         return e.__queueingActionRun = !1, e.__queuedActionRun = t.uuid, t.uuid
                     }
                 }), e.__queuedActionRun = null,
                 function(e, t) {
-                    e.__showingActionRunningBox = !0, ha(t)
+                    e.__showingActionRunningBox = !0, ma(t)
                 }(e, r)
         }
 
-        function Sa(e, t) {
-            e.showingCheckRunningBox = !1, ha(t)
+        function Ca(e, t) {
+            e.showingCheckRunningBox = !1, ma(t)
         }
 
-        function La(e, t) {
-            e.__showingActionRunningBox = !1, ha(t)
+        function Ea(e, t) {
+            e.__showingActionRunningBox = !1, ma(t)
         }
-        var ka = function(e) {
+        var _a = function(e) {
                 var t = e.groupList,
                     n = e.env,
                     r = e.historyList,
                     o = e.info,
                     i = e.toggleShowingChecksSearch;
                 return t.error ? (0, Kr.jsx)(xi, {
                     error: t.error,
@@ -51951,45 +52144,45 @@
                                 id: "tooltip-search",
                                 position: "right",
                                 shape: "squared",
                                 size: "small",
                                 text: "Click to search for checks."
                             })]
                         }), t.map((function(e, i) {
-                            return (0, Kr.jsx)(Ca, {
+                            return (0, Kr.jsx)(Ta, {
                                 group: e,
                                 env: n,
                                 groupList: t,
                                 historyList: r,
                                 info: o,
                                 style: {
                                     paddingBottom: "6pt"
                                 }
                             }, e.group)
                         }))]
                     }) : (0, Kr.jsx)(Kr.Fragment, {})
                 })
             },
-            Ca = function(e) {
+            Ta = function(e) {
                 var t, n = e.group,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.env,
                     a = e.info,
                     s = e.style,
                     u = void 0 === s ? {} : s;
 
                 function l(e, t) {
                     c(e) ? function(e, t) {
                         e.map((function(e) {
-                            return e.__showingResults && ga(e, t)
+                            return e.__showingResults && va(e, t)
                         }))
                     }(e, t) : function(e, t, n) {
                         e.map((function(e) {
-                            return !e.__showingResults && ya(e, 0, n)
+                            return !e.__showingResults && Ma(e, 0, n)
                         }))
                     }(e, 0, t)
                 }
 
                 function c(e) {
                     for (var t = 0; t < (null === e || void 0 === e ? void 0 : e.length); t++)
                         if (e[t].__showingResults) return !0;
@@ -52023,15 +52216,15 @@
                                 })]
                             }), (0, Kr.jsx)("span", {
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
                                 },
                                 onClick: function() {
-                                    va(n, r, o)
+                                    wa(n, r, o)
                                 },
                                 children: (0, Kr.jsx)("b", {
                                     children: Fr.X
                                 })
                             })]
                         }), (0, Kr.jsx)("div", {
                             style: {
@@ -52041,27 +52234,27 @@
                             return e.title > t.title ? 1 : e.title < t.title ? -1 : 0
                         })).map((function(e, t) {
                             return (0, Kr.jsxs)("div", {
                                 children: [t > 0 && (0, Kr.jsx)("div", {
                                     style: {
                                         marginBottom: "12px"
                                     }
-                                }), (0, Kr.jsx)(Ea, {
+                                }), (0, Kr.jsx)(Aa, {
                                     check: e,
                                     env: i,
                                     groupList: r,
                                     historyList: o,
                                     info: a
                                 })]
                             }, t)
                         }))]
                     })
                 })
             },
-            Ea = function(e) {
+            Aa = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.historyList,
                     u = e.info,
                     l = (0, t.useState)(!1);
 
@@ -52094,19 +52287,19 @@
                 function f(e, t, n) {
                     var r, o = arguments.length > 3 && void 0 !== arguments[3] && arguments[3];
                     (t = (null === (r = e.__result) || void 0 === r ? void 0 : r.get("action")) || t) && e.__resultByAction.fetch({
                         url: zt.Url("/checks/".concat(t, "/history/latest")),
                         nocache: o
                     })
                 }
-                r.__result = qi({
+                r.__result = Xi({
                     cache: !0
-                }), r.__resultByUuid = qi({
+                }), r.__resultByUuid = Xi({
                     cache: !0
-                }), r.__resultByAction = qi({
+                }), r.__resultByAction = Xi({
                     cache: !0
                 }), (0, t.useEffect)((function() {
                     c(r, o, i)
                 }), []), (0, t.useEffect)((function() {
                     r.__showingResults = !0, c(r, o, i)
                 }), []);
                 var p = a((0, t.useState)(!0), 2),
@@ -52134,19 +52327,19 @@
                                         style: {
                                             verticalAlign: "top",
                                             width: "1%",
                                             cursor: "pointer"
                                         },
                                         onClick: function() {
                                             ! function(e, t, n) {
-                                                e.__showingResults ? ga(e, n) : (ya(e, 0, n), g(!0))
+                                                e.__showingResults ? va(e, n) : (Ma(e, 0, n), g(!0))
                                             }(r, 0, i)
                                         },
                                         children: (0, Kr.jsxs)("b", {
-                                            children: [ba(r) ? (0, Kr.jsx)("small", {
+                                            children: [xa(r) ? (0, Kr.jsx)("small", {
                                                 children: Fr.DownArrowHollow
                                             }) : (0, Kr.jsx)("small", {
                                                 children: Fr.RightArrowHollow
                                             }), "\xa0"]
                                         })
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
@@ -52161,15 +52354,15 @@
                                                     id: "tooltip-configure ".concat(r.name),
                                                     className: r.__configuringCheckRun ? "check-config-button" : "check-run-button",
                                                     style: {
                                                         marginTop: "-2pt",
                                                         float: "right"
                                                     },
                                                     onClick: function() {
-                                                        r.__configuringCheckRun ? (wa(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, ha(i), g(!0)
+                                                        r.__configuringCheckRun ? (Na(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, ma(i), g(!0)
                                                     },
                                                     children: [(0, Kr.jsx)("span", {
                                                         style: {
                                                             fontSize: "small"
                                                         },
                                                         children: Fr.DownArrowFat
                                                     }), "\xa0Configure"]
@@ -52181,15 +52374,15 @@
                                             })
                                         }) : (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginLeft: "10pt",
                                                     float: "right"
                                                 },
-                                                children: (0, Kr.jsx)(Oa, {
+                                                children: (0, Kr.jsx)(Pa, {
                                                     check: r,
                                                     env: o,
                                                     groupList: i,
                                                     historyList: s,
                                                     style: {
                                                         marginTop: "-1pt"
                                                     }
@@ -52199,19 +52392,19 @@
                                             style: {
                                                 whiteSpace: "nowrap"
                                             },
                                             children: [(0, Kr.jsx)("u", {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 style: {
                                                     cursor: "pointer",
-                                                    fontWeight: ba(r) ? "bold" : "normal",
+                                                    fontWeight: xa(r) ? "bold" : "normal",
                                                     whiteSpace: "break-spaces"
                                                 },
                                                 onClick: function() {
-                                                    xa(r, o, s)
+                                                    Da(r, o, s)
                                                 },
                                                 children: (null === (n = r.title) || void 0 === n ? void 0 : n.length) > 70 ? r.title.substring(0, 69) + " ..." : r.title
                                             }), (0, Kr.jsx)(Mi, {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 text: "Check: ".concat(r.name, ". Module: ").concat(r.module, ".")
                                             }), r.__result.get("action") && (0, Kr.jsx)("u", {
                                                 children: l[0] ? (0, Kr.jsxs)(Kr.Fragment, {
@@ -52269,15 +52462,15 @@
                                                         height: "18"
                                                     })
                                                 }), (0, Kr.jsx)(Mi, {
                                                     id: "tooltip-view-source ".concat(r.name),
                                                     text: "Click to view source code for this check (in new tab)."
                                                 })]
                                             })]
-                                        }), (0, Kr.jsx)(_a, {
+                                        }), (0, Kr.jsx)(Oa, {
                                             check: r,
                                             env: o,
                                             historyList: s
                                         }), Object.keys(null === r || void 0 === r ? void 0 : r.schedule).map((function(e, t) {
                                             var n, o;
                                             return (0, Kr.jsx)("div", {
                                                 children: it.HasValue(null === (n = r.schedule[e]) || void 0 === n ? void 0 : n.cron_description) ? (0, Kr.jsxs)("div", {
@@ -52299,42 +52492,42 @@
                                                     })]
                                                 }, t) : (0, Kr.jsx)("small", {
                                                     children: (0, Kr.jsx)("i", {
                                                         children: "Not scheduled."
                                                     })
                                                 })
                                             }, e)
-                                        })), (0, Kr.jsx)(za, {
+                                        })), (0, Kr.jsx)(Ra, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             historyList: s,
                                             update: function() {
-                                                return ha(i)
+                                                return ma(i)
                                             },
                                             showDependenciesBox: h,
                                             setShowDependenciesBox: g
-                                        }), (0, Kr.jsx)(Ua, {
+                                        }), (0, Kr.jsx)(Ba, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Qa, {
+                                        }), (0, Kr.jsx)(Ha, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             update: function() {
                                                 return i.update()
                                             },
                                             fetchResult: c,
                                             runActionAllowedState: l
-                                        }), (0, Kr.jsx)(Pa, {
+                                        }), (0, Kr.jsx)(Fa, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Ta, {
+                                        }), (0, Kr.jsx)(za, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             fetchResult: c,
                                             runActionAllowedState: l
                                         })]
                                     })]
@@ -52345,25 +52538,25 @@
                                     children: (0, Kr.jsx)("td", {})
                                 })]
                             })
                         })
                     })
                 })
             },
-            _a = function(e) {
+            Oa = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.historyList,
                     o = e.style;
                 return (0, Kr.jsxs)("span", {
                     style: Ye(Ye({}, o), {}, {
                         cursor: "pointer"
                     }),
                     onClick: function() {
-                        return xa(t, n, r)
+                        return Da(t, n, r)
                     },
                     children: [(0, Kr.jsx)("span", {
                         id: "tooltip-recent-history ".concat(t.name),
                         children: (0, Kr.jsx)("img", {
                             alt: "history",
                             onClick: function(e) {},
                             src: Ut.History(),
@@ -52377,15 +52570,15 @@
                         id: "tooltip-recent-history ".concat(t.name),
                         text: "Click to " + (t.__showingHistory ? "hide" : "show") + " recent history of check runs."
                     }), t.__showingHistory ? (0, Kr.jsx)("span", {
                         children: Fr.RightArrow
                     }) : (0, Kr.jsx)(Kr.Fragment, {})]
                 })
             },
-            Ta = function(e) {
+            za = function(e) {
                 var n, r, o, i = e.check,
                     s = e.env,
                     u = e.groupList,
                     l = e.fetchResult,
                     c = (e.runActionAllowedState, a((0, t.useState)(!1), 2)),
                     d = c[0],
                     f = c[1],
@@ -52402,15 +52595,15 @@
                 }
 
                 function v(e, t) {
                     f(!1), g(!0)
                 }
 
                 function M(e, t) {
-                    e.__showingResultDetails = !e.__showingResultDetails, pa(t)
+                    e.__showingResultDetails = !e.__showingResultDetails, ya(t)
                 }
                 var b = function(e) {
                     var t, n = e.check,
                         r = e.env,
                         o = (e.checkUuid, e.groupList);
                     return t = d ? n.__resultByUuid.loading ? "Fetching latest result: ".concat(n.__result.get("uuid")) : "Click to fetch latest result: ".concat(n.__result.get("uuid")) : n.__result.loading ? "Fetching latest result." : "Click to fetch latest result.", (0, Kr.jsxs)("span", {
                         style: {
@@ -52717,24 +52910,24 @@
                             })]
                         })
                     }), i.__showingResultDetails && (!i.__result.empty || !i.__resultByUuid.empty || !i.__resultByAction.empty) && (0, Kr.jsxs)(Kr.Fragment, {
                         children: [(0, Kr.jsx)("div", {
                             style: {
                                 height: "2pt"
                             }
-                        }), (0, Kr.jsx)(Aa, {
+                        }), (0, Kr.jsx)(Ua, {
                             check: i,
                             groupList: u,
                             showResultByUuid: d,
                             showResultByAction: h
                         })]
                     })]
                 })
             },
-            Aa = function(e) {
+            Ua = function(e) {
                 var t, n = e.check,
                     r = e.groupList,
                     o = e.showResultByUuid,
                     i = e.showResultByAction;
                 e.style;
                 return n.__showingResults ? o ? (0, Kr.jsxs)("pre", {
                     className: "box lighten",
@@ -52775,26 +52968,26 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, pa(r)
+                                n.__showingResultDetails = !1, ya(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
                             label: "Loading latest result "
                         })
                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                        children: Ui.Format(n.__resultByUuid.get())
+                        children: Bi.Format(n.__resultByUuid.get())
                     })]
                 }) : i ? (0, Kr.jsxs)("pre", {
                     className: "box lighten",
                     style: {
                         wordWrap: "break-word",
                         paddingBottom: "4pt",
                         marginBottom: "3px",
@@ -52831,26 +53024,26 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, pa(r)
+                                n.__showingResultDetails = !1, ya(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
                             label: "Loading latest result "
                         })
                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                        children: Ui.Format(n.__resultByAction.get())
+                        children: Bi.Format(n.__resultByAction.get())
                     })]
                 }) : (0, Kr.jsxs)("pre", {
                     className: "box lighten",
                     style: {
                         color: "PASS" === (null === (t = n.__result.get("status")) || void 0 === t ? void 0 : t.toUpperCase()) ? "inherit" : "darkred",
                         wordWrap: "break-word",
                         paddingBottom: "4pt",
@@ -52888,53 +53081,53 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "x-large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.showingResultDetailsFull = !n.showingResultDetailsFull, pa(r)
+                                n.showingResultDetailsFull = !n.showingResultDetailsFull, ya(r)
                             },
                             children: n.showingResultDetailsFull ? (0, Kr.jsx)("span", {
                                 title: "Show full result output.",
                                 children: Fr.UpArrow
                             }) : (0, Kr.jsx)("span", {
                                 children: Fr.DownArrow
                             })
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, pa(r)
+                                n.__showingResultDetails = !1, ya(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(no, {
                         condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                         color: Ft.GetForegroundColor(),
                         label: "Loading latest result "
                     }) : n.__result.empty ? (0, Kr.jsx)("div", {
                         style: {
                             marginTop: "1pt"
                         },
                         children: "No result."
-                    }) : Ui.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
+                    }) : Bi.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
                 }) : (0, Kr.jsx)(Kr.Fragment, {})
             },
-            Oa = function(e) {
+            Pa = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.style,
-                    s = a(ua(), 1)[0],
-                    u = la();
+                    s = a(da(), 1)[0],
+                    u = fa();
                 if (t.__queueingCheckRun) return t.__queueingCheckRun && (0, Kr.jsxs)("div", {
                     className: "check-run-wait-button",
                     style: i,
                     children: [(0, Kr.jsx)("span", {
                         id: "tooltip-queueing",
                         children: (0, Kr.jsx)("i", {
                             children: "Queueing"
@@ -52955,15 +53148,15 @@
                         className: "check-run-button" + (t.__configuringCheckRun, ""),
                         style: Ye(Ye({}, i), {}, {
                             cursor: s && t.__configuringCheckRun ? "not-allowed" : "",
                             background: s && t.__configuringCheckRun ? "#888888" : "",
                             color: t.__configuringCheckRun ? "yellow" : ""
                         }),
                         onClick: function(e) {
-                            t.__configuringCheckRun ? s || (wa(t), Ia(t, n, r, o, u)) : (t.__configuringCheckRun = !0, ha(r))
+                            t.__configuringCheckRun ? s || (Na(t), La(t, n, r, o, u)) : (t.__configuringCheckRun = !0, ma(r))
                         },
                         children: (0, Kr.jsx)("span", {
                             children: s ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: t.__configuringCheckRun ? (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsxs)("span", {
                                         style: {
                                             fontSize: "",
@@ -53000,15 +53193,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            za = function(e) {
+            Ra = function(e) {
                 var n = e.check,
                     r = e.env,
                     o = e.groupList,
                     i = e.historyList,
                     a = (e.update, e.showDependenciesBox),
                     s = e.setShowDependenciesBox;
 
@@ -53105,15 +53298,15 @@
                         },
                         children: st.IsNonEmptyObject(n.kwargs) ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-2pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Oa, {
+                                children: (0, Kr.jsx)(Pa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
@@ -53144,15 +53337,15 @@
                                                     defaultValue: n.kwargs[e] ? "true" : "false",
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray",
                                                         borderRadius: "4pt"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e] = "true" === t.target.value, ha(o)
+                                                        n.kwargs[e] = "true" === t.target.value, ma(o)
                                                     },
                                                     children: (n.kwargs[e], (0, Kr.jsxs)(Kr.Fragment, {
                                                         children: [(0, Kr.jsx)("option", {
                                                             children: "true"
                                                         }), (0, Kr.jsx)("option", {
                                                             children: "false"
                                                         })]
@@ -53160,28 +53353,28 @@
                                                 }), st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)("select", {
                                                     defaultValue: null === (t = n.kwargs[e]) || void 0 === t ? void 0 : t.__selected,
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e].__selected = t.target.value, ha(o)
+                                                        n.kwargs[e].__selected = t.target.value, ma(o)
                                                     },
                                                     children: n.kwargs[e].map((function(e) {
                                                         return (0, Kr.jsx)("option", {
                                                             children: e
                                                         }, Dr()())
                                                     }))
                                                 }, Dr()()), !st.IsBoolean(n.kwargs[e]) && !st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)(Kr.Fragment, {
                                                     children: (0, Kr.jsx)("input", {
                                                         id: "".concat(n.name, ".").concat(e),
                                                         defaultValue: n.kwargs[e],
                                                         placeholder: "Empty",
                                                         onBlur: function() {
-                                                            wa(n)
+                                                            Na(n)
                                                         },
                                                         style: {
                                                             marginLeft: "0pt",
                                                             height: "14pt",
                                                             background: "lightyellow",
                                                             border: "1px solid lightgray",
                                                             borderRadius: "2pt"
@@ -53195,29 +53388,29 @@
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-3pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Oa, {
+                                children: (0, Kr.jsx)(Pa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
                                 })
                             }), "No arguments."]
                         })
                     })]
                 })
             },
-            Ua = function(e) {
+            Ba = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.showingCheckRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53295,15 +53488,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        Sa(n, r)
+                                        Ca(n, r)
                                     },
                                     children: ["\xa0", (0, Kr.jsx)("b", {
                                         children: Fr.X
                                     }), "\xa0"]
                                 })]
                             })
                         }), !n.__queuedCheckRun && (0, Kr.jsx)("div", {
@@ -53315,15 +53508,15 @@
                                 label: " Queueing check run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Pa = function(e) {
+            Fa = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.__showingActionRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53402,15 +53595,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        La(n, r)
+                                        Ea(n, r)
                                     },
                                     children: ["\xa0", Fr.X]
                                 })]
                             })
                         }), !n.__queuedActionRun && (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "-2pt"
@@ -53420,15 +53613,15 @@
                                 label: " Queueing action run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Ra = function(e) {
+            Ya = function(e) {
                 var t = e.env,
                     n = e.historyList;
                 if (n.error) return (0, Kr.jsx)(xi, {
                     error: n.error,
                     message: "Error loading check history from Foursight API"
                 });
                 var r = n.filter((function(e) {
@@ -53441,24 +53634,24 @@
                         },
                         children: "Recent Results"
                     }), null === r || void 0 === r ? void 0 : r.map((function(e, r) {
                         return (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "3pt"
                             },
-                            children: (0, Kr.jsx)(Ba, {
+                            children: (0, Kr.jsx)(Qa, {
                                 check: e,
                                 env: t,
                                 historyList: n
                             })
                         }, e.name)
                     }))]
                 })
             },
-            Ba = function(e) {
+            Qa = function(e) {
                 var n, r, o, i = e.check,
                     a = (e.env, e.historyList);
 
                 function s(e, t) {
                     e.__resultShowing = !1, e.__result = null, e.__resultLoading = !1, t.update()
                 }
 
@@ -53519,15 +53712,15 @@
                     })
                 }
 
                 function y() {
                     g(!0)
                 }
                 return i.__resultHistory = function() {
-                    return qi({
+                    return Xi({
                         url: zt.Url("/checks/".concat(i.name, "/history")),
                         nofetch: !0,
                         cache: !0
                     })
                 }(), (0, t.useEffect)((function() {
                     g()
                 }), []), (0, Kr.jsxs)("div", {
@@ -53594,15 +53787,15 @@
                             })]
                         }), (0, Kr.jsxs)("span", {
                             style: {
                                 float: "right",
                                 cursor: "pointer"
                             },
                             onClick: function() {
-                                ja(i, a)
+                                Ia(i, a)
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("b", {
                                 children: Fr.X
                             })]
                         })]
                     }), (0, Kr.jsx)("div", {
                         style: {
@@ -53610,15 +53803,15 @@
                         }
                     }), i.__showingHistory && (0, Kr.jsx)(Kr.Fragment, {
                         children: (null === (n = i.__resultHistory) || void 0 === n || null === (r = n.data) || void 0 === r || null === (o = r.list) || void 0 === o ? void 0 : o.length) > 0 ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsxs)("table", {
                                 style: {
                                     width: "100%"
                                 },
-                                children: [(0, Kr.jsx)(ia, {
+                                children: [(0, Kr.jsx)(ua, {
                                     loading: i.__resultHistory.loading,
                                     columns: h,
                                     list: i.__resultHistory.data.list,
                                     refresh: y,
                                     update: function(e) {
                                         return a.update()
                                     },
@@ -53786,15 +53979,15 @@
                                                                         marginRight: "2pt",
                                                                         fontSize: "large",
                                                                         fontWeight: "bold",
                                                                         cursor: "pointer"
                                                                     },
                                                                     children: "X"
                                                                 })]
-                                                            }), Ui.Format(e.__result)]
+                                                            }), Bi.Format(e.__result)]
                                                         })
                                                     })
                                                 })
                                             })]
                                         }, n)
                                     }))
                                 })]
@@ -53839,15 +54032,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            Fa = function(e) {
+            Ga = function(e) {
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: ["\xa0", (0, Kr.jsxs)("span", {
                         style: {
                             fontWeight: e.showingChecksSearch ? "bold" : "normal"
                         },
                         onClick: e.toggleShowingChecksSearch,
                         children: [(0, Kr.jsx)("span", {
@@ -53865,15 +54058,15 @@
                             },
                             src: Ut.NewIcon(),
                             height: "42"
                         })]
                     }), " ", (0, Kr.jsx)("br", {})]
                 })
             },
-            Ya = function(e) {
+            Wa = function(e) {
                 var n = a((0, t.useState)(""), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)([]), 2),
                     s = i[0],
                     l = i[1];
                 (0, t.useEffect)((function() {
@@ -54060,32 +54253,32 @@
                                     children: "No results."
                                 })
                             })]
                         })
                     })]
                 })
             },
-            Qa = function(e) {
+            Ha = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.fetchResult,
                     u = e.runActionAllowedState,
                     l = a((0, t.useState)(!1), 2),
                     c = l[0],
                     d = l[1],
-                    f = a(ua(), 1)[0],
-                    p = la();
+                    f = a(da(), 1)[0],
+                    p = fa();
 
                 function h() {
                     if (c) {
                         var e;
                         d(!1);
                         var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
-                        t && (Da(r, t, o, i, p), u[1](!1))
+                        t && (ka(r, t, o, i, p), u[1](!1))
                     } else d(!0)
                 }
                 return (0, t.useEffect)((function() {
                     d(!1)
                 }), []), (0, Kr.jsx)(Kr.Fragment, {
                     children: r.__configuringCheckRun && (null === (n = r.__result) || void 0 === n ? void 0 : n.get("action")) && (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsxs)("div", {
@@ -54237,62 +54430,62 @@
                                     })]
                                 })]
                             })]
                         })
                     })
                 })
             },
-            Ga = function(e) {
+            Za = function(e) {
                 var n = pe().environ,
-                    r = qi({
+                    r = Xi({
                         initial: []
                     }),
-                    o = qi({
+                    o = Xi({
                         initial: []
                     }),
-                    i = qi(zt.Url("/info")),
+                    i = Xi(zt.Url("/info")),
                     s = a((0, t.useState)(!1), 2),
                     u = s[0],
                     l = s[1];
-                var c = qi({
+                var c = Xi({
                         url: zt.Url("/checks/grouped/schedule", n),
                         nofetch: !0,
                         cache: !0,
                         onData: function(e) {
                             return e.sort((function(e, t) {
                                 return e.group > t.group ? 1 : e.group < t.group ? -1 : 0
-                            })), e.length > 0 && ma(function(e) {
+                            })), e.length > 0 && ba(function(e) {
                                 for (var t = null, n = 0; n < (null === e || void 0 === e ? void 0 : e.length); n++) {
                                     var r, o;
                                     (!t || (null === (r = e[n]) || void 0 === r || null === (o = r.checks) || void 0 === o ? void 0 : o.length) < t.checks.length) && (t = e[n])
                                 }
                                 return t
                             }(e), 0, o), e
                         }
                     }),
-                    d = qi({
+                    d = Xi({
                         url: zt.Url("/lambdas", n),
                         cache: !0,
                         onData: function(e) {
                             return e.sort((function(e, t) {
                                 return e.lambda_name > t.lambda_name ? 1 : e.lambda_name < t.lambda_name ? -1 : 0
                             })), e
                         }
                     });
                 (0, t.useEffect)((function() {
                     p(), c.fetch(u ? zt.Url("/checks/grouped/schedule") : zt.Url("/checks/grouped"))
                 }), [u]);
-                var f = qi();
+                var f = Xi();
 
                 function p() {
                     f.refresh(zt.Url("/checks_status", n))
                 }
 
                 function h(e, t, n, r) {
-                    Ma(e, n) ? va(e, n, r) : ma(e, 0, n)
+                    ja(e, n) ? wa(e, n, r) : ba(e, 0, n)
                 }
 
                 function g() {
                     l(!u), o.update([])
                 }
                 var y = function(e) {
                         e.props;
@@ -54409,15 +54602,15 @@
                                 },
                                 children: c.map((function(e, t) {
                                     var n;
                                     return (0, Kr.jsxs)("div", {
                                         children: [(0, Kr.jsxs)("span", {
                                             id: "tooltip-group-count-".concat(t),
                                             style: {
-                                                fontWeight: Ma(e, o) ? "bold" : "normal",
+                                                fontWeight: ja(e, o) ? "bold" : "normal",
                                                 cursor: "pointer"
                                             },
                                             onClick: function() {
                                                 return h(e, 0, o, r)
                                             },
                                             children: [e.group.replace(/ checks$/i, ""), " \xa0", (0, Kr.jsxs)("small", {
                                                 children: ["(", e.checks.length, ")"]
@@ -54436,15 +54629,15 @@
                                             }
                                         })]
                                     }, e.group)
                                 }))
                             })]
                         })
                     },
-                    m = qi(null),
+                    m = Xi(null),
                     v = a((0, t.useState)(!1), 2),
                     M = v[0],
                     b = v[1];
 
                 function w() {
                     return !m.empty
                 }
@@ -54545,15 +54738,15 @@
                                             })]
                                         }), m.yaml()]
                                     })
                                 })
                             })]
                         })
                     },
-                    C = qi(zt.Url("/checks/history/recent?limit=20", n), {
+                    C = Xi(zt.Url("/checks/history/recent?limit=20", n), {
                         nofetch: !0,
                         cache: !0
                     }),
                     E = a((0, t.useState)(!1), 2),
                     _ = E[0],
                     T = E[1];
 
@@ -54647,15 +54840,15 @@
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Most Recent"
                                             }), ":\xa0"]
                                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Top"
                                             }), ":\xa0"]
-                                        }), (0, Kr.jsx)(da.FormatDuration, {
+                                        }), (0, Kr.jsx)(ha.FormatDuration, {
                                             start: null === C || void 0 === C || null === (u = C.data[0]) || void 0 === u ? void 0 : u.timestamp,
                                             verbose: !0,
                                             fallback: "just now",
                                             suffix: "ago",
                                             tooltip: !0
                                         })]
                                     }), (0, Kr.jsx)("b", {
@@ -54667,15 +54860,15 @@
                                         onClick: O,
                                         children: Fr.X
                                     }), (0, Kr.jsxs)("table", {
                                         style: {
                                             width: "100%"
                                         },
                                         border: "0",
-                                        children: [(0, Kr.jsx)(ia, {
+                                        children: [(0, Kr.jsx)(ua, {
                                             columns: [{
                                                 label: "__refresh"
                                             }, {
                                                 label: "Timestamp",
                                                 key: "timestamp"
                                             }, {
                                                 label: "Check",
@@ -54767,15 +54960,15 @@
                                                                 width: "45%"
                                                             },
                                                             children: [(0, Kr.jsx)("b", {
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
                                                                 onClick: function() {
-                                                                    return xa(P(e.check, e.group), n, r)
+                                                                    return Da(P(e.check, e.group), n, r)
                                                                 },
                                                                 children: e.title
                                                             }), "\xa0\xa0", (0, Kr.jsxs)(Oe, {
                                                                 to: kr.Path("/checks/".concat(e.check, "/history")),
                                                                 rel: "noreferrer",
                                                                 target: "_blank",
                                                                 children: [(0, Kr.jsx)("small", {
@@ -55241,15 +55434,15 @@
                                                                             children: [(0, Kr.jsx)("b", {
                                                                                 id: "tooltip-lambda-check-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
                                                                                 },
                                                                                 onClick: function() {
-                                                                                    return xa(P(e.check_name, e.check_group), n, r)
+                                                                                    return Da(P(e.check_name, e.check_group), n, r)
                                                                                 },
                                                                                 children: e.check_title
                                                                             }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("i", {
                                                                                 id: "tooltip-lambda-check-group-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
@@ -55332,60 +55525,60 @@
                                             }), (0, Kr.jsx)(N, {}), (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginTop: "3pt",
                                                     marginBottom: "3pt",
                                                     height: "1px",
                                                     backgroundColor: "var(--box-fg)"
                                                 }
-                                            }), (0, Kr.jsx)(Fa, {
+                                            }), (0, Kr.jsx)(Ga, {
                                                 showingChecksSearch: D,
                                                 toggleShowingChecksSearch: L
                                             })]
                                         }), (0, Kr.jsx)(F, {}), (0, Kr.jsx)(H, {})]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: "8pt",
                                             verticalAlign: "top"
                                         },
                                         children: [(0, Kr.jsx)(k, {
                                             info: i
-                                        }), (0, Kr.jsx)(ka, {
+                                        }), (0, Kr.jsx)(_a, {
                                             env: n,
                                             groupList: o,
                                             historyList: r,
                                             info: i,
                                             toggleShowingChecksSearch: L
                                         })]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: (null === o || void 0 === o ? void 0 : o.length) > 0 || o.error || w() ? "8pt" : "0",
                                             verticalAlign: "top"
                                         },
-                                        children: [(0, Kr.jsx)(Ya, {
+                                        children: [(0, Kr.jsx)(Wa, {
                                             checks: c,
                                             groupList: o,
                                             environ: n,
                                             findGroup: U,
                                             toggleShowGroup: h,
                                             showingChecksSearch: D,
                                             toggleShowingChecksSearch: L
-                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(Ra, {
+                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(Ya, {
                                             env: n,
                                             historyList: r
                                         })]
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            Wa = __webpack_require__(8145),
-            Ha = __webpack_require__.n(Wa),
-            Za = function(e) {
+            Va = __webpack_require__(8145),
+            qa = __webpack_require__.n(Va),
+            Ja = function(e) {
                 var t = e.pages,
                     n = e.page,
                     r = e.onChange,
                     o = e.refresh,
                     i = e.loading,
                     a = e.spinner;
                 return (0, Kr.jsx)("table", {
@@ -55400,15 +55593,15 @@
                                         style: {
                                             pointerEvents: i ? "none" : "",
                                             opacity: i ? "0.4" : "",
                                             fontSize: "8pt",
                                             fontWeight: "bold"
                                         },
                                         className: "pagination-control",
-                                        children: (0, Kr.jsx)(Ha(), {
+                                        children: (0, Kr.jsx)(qa(), {
                                             nextLabel: "NEXT",
                                             onPageChange: r,
                                             pageRangeDisplayed: 2,
                                             initialPage: n,
                                             disableInitialCallback: !0,
                                             marginPagesDisplayed: 2,
                                             pageCount: t,
@@ -55463,23 +55656,23 @@
                                 })
                             })]
                         })
                     })
                 })
             };
 
-        function Va(e) {
+        function Ka(e) {
             var t;
             return null === e || void 0 === e || null === (t = e.split("/")) || void 0 === t ? void 0 : t.reverse()[0]
         }
 
-        function qa(e) {
+        function Xa(e) {
             return null === e || void 0 === e ? void 0 : e.substring(0, null === e || void 0 === e ? void 0 : e.lastIndexOf("/"))
         }
-        var Ja = function(e) {
+        var $a = function(e) {
                 var t = e.check,
                     n = e.checkInfo;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box",
                         children: (0, Kr.jsx)("table", {
                             children: (0, Kr.jsxs)("tbody", {
@@ -55594,16 +55787,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [Va(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: qa(n.get("file"))
+                                        children: [Ka(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: Xa(n.get("file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "2px"
                                         }
@@ -55696,15 +55889,15 @@
                                     })]
                                 })]
                             })
                         })
                     })
                 })
             },
-            Ka = function(e) {
+            es = function(e) {
                 var n, r = e.check,
                     o = e.checkInfo;
 
                 function i(e) {
                     var t = e.get("schedule");
                     if (t) {
                         var n = Object.values(t);
@@ -55968,16 +56161,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [Va(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: qa(o.get("registered_file"))
+                                        children: [Ka(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: Xa(o.get("registered_file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "3px"
                                         }
@@ -56184,16 +56377,16 @@
                                             style: {
                                                 paddingRight: "8pt"
                                             },
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Code"
                                             }), ":"]
                                         }), (0, Kr.jsxs)("td", {
-                                            children: [Va(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                                children: qa(o.get("registered_action.file"))
+                                            children: [Ka(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                                children: Xa(o.get("registered_action.file"))
                                             })]
                                         })]
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "3px"
                                             }
@@ -56293,15 +56486,15 @@
                                     })]
                                 })
                             })
                         })]
                     })]
                 })
             },
-            Xa = function(e) {
+            ts = function(e) {
                 var n, r = pe(),
                     o = r.environ,
                     i = r.check,
                     s = a(Re(), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(parseInt(u.get("limit")) || 25), 2),
@@ -56315,16 +56508,16 @@
                     v = y[1],
                     M = a((0, t.useState)(Math.floor(h / d)), 2),
                     b = M[0],
                     w = M[1],
                     j = a((0, t.useState)(Math.max(1, b + 1)), 2),
                     x = j[0],
                     N = j[1],
-                    I = qi(),
-                    D = qi();
+                    I = Xi(),
+                    D = Xi();
 
                 function S(e, t, n) {
                     f(e), g(t), v(n)
                 }
 
                 function L(e, t, n) {
                     it.HasValue(n) || (n = "timestamp.desc"), l(Ye(Ye({}, u), {}, {
@@ -56458,15 +56651,15 @@
                             }
                         }), (null === (r = o.get("list")) || void 0 === r ? void 0 : r.length) > 0 ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsxs)("table", {
                                 style: {
                                     width: "100%"
                                 },
                                 className: "fg",
-                                children: [(0, Kr.jsx)(ia, {
+                                children: [(0, Kr.jsx)(ua, {
                                     columns: f,
                                     list: o.get("list"),
                                     state: {
                                         key: u,
                                         order: m.endsWith(".desc") ? -1 : 1
                                     },
                                     update: function(e, t) {
@@ -56659,15 +56852,15 @@
                                                                         marginRight: "2pt",
                                                                         fontSize: "large",
                                                                         fontWeight: "bold",
                                                                         cursor: "pointer"
                                                                     },
                                                                     children: "X"
                                                                 })]
-                                                            }), Ui.Format(e.__result)]
+                                                            }), Bi.Format(e.__result)]
                                                         })
                                                     })
                                                 })
                                             })]
                                         }, a(e))
                                     }))
                                 })]
@@ -56714,15 +56907,15 @@
                                         },
                                         children: (0, Kr.jsx)("tbody", {
                                             children: (0, Kr.jsxs)("tr", {
                                                 children: [(0, Kr.jsx)("td", {
                                                     style: {
                                                         width: "90%"
                                                     },
-                                                    children: (0, Kr.jsx)(Za, {
+                                                    children: (0, Kr.jsx)(Ja, {
                                                         pages: x,
                                                         onChange: function(e) {
                                                             var t = e.selected * d % I.get("paging.total");
                                                             S(d, t, m)
                                                         },
                                                         refresh: function() {
                                                             return L(d, h, m)
@@ -56838,45 +57031,45 @@
                                     children: (0, Kr.jsx)(_, {
                                         history: I
                                     })
                                 }), (0, Kr.jsx)("td", {
                                     style: {
                                         verticalAlign: "top"
                                     },
-                                    children: "action" === D.get("type") ? (0, Kr.jsx)(Ja, {
+                                    children: "action" === D.get("type") ? (0, Kr.jsx)($a, {
                                         check: i,
                                         checkInfo: D
-                                    }) : (0, Kr.jsx)(Ka, {
+                                    }) : (0, Kr.jsx)(es, {
                                         check: i,
                                         checkInfo: D
                                     })
                                 })]
                             })]
                         })
                     })
                 })
             },
-            $a = function() {
-                var e = a((0, t.useContext)(Ki), 2),
+            ns = function() {
+                var e = a((0, t.useContext)(ea), 2),
                     n = (e[0], e[1]),
-                    r = Ji();
+                    r = $i();
                 return function(e) {
                     return r.refresh(zt.Url("/header", e), {
                         onData: function(e) {
                             return n(e)
                         },
                         cache: !0
                     })
                 }
             },
-            es = function(e) {
-                var t, n, r = Xi(),
-                    o = $a(),
-                    i = qi(Br.IsLoggedIn() ? zt.Url("/info") : null);
-                Ai.NoteLastUrl(r);
+            rs = function(e) {
+                var t, n, r = ta(),
+                    o = ns(),
+                    i = Xi(Br.IsLoggedIn() ? zt.Url("/info") : null);
+                Ui.NoteLastUrl(r);
                 var a = fe();
 
                 function s() {
                     return At.IsKnown(At.Current(), r)
                 }
 
                 function u(e) {
@@ -57209,16 +57402,16 @@
                             style: {
                                 marginTop: "8pt"
                             }
                         })]
                     })
                 })
             },
-            ts = function(e) {
-                var t = Xi();
+            os = function(e) {
+                var t = ta();
                 return t.loading ? null : (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("br", {}), (0, Kr.jsx)("table", {
                         width: "100%",
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
                                 style: {
                                     backgroundColor: "darkred",
@@ -57250,31 +57443,31 @@
                                 },
                                 children: (0, Kr.jsx)("td", {})
                             })]
                         })
                     })]
                 })
             },
-            ns = function(e) {
-                var t = Xi();
+            is = function(e) {
+                var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-error",
                             style: {
                                 margin: "20pt",
                                 padding: "10pt"
                             },
                             children: [(0, Kr.jsx)("b", {
                                 children: "Forbidden response from server."
                             }), ".  ", (0, Kr.jsx)("br", {}), "You seem to be logged in but the server does not seem to think so. ", (0, Kr.jsx)("br", {}), "Try ", (0, Kr.jsx)("span", {
                                 onClick: function() {
-                                    return Oi()
+                                    return Pi()
                                 },
                                 style: {
                                     cursor: "pointer"
                                 },
                                 children: (0, Kr.jsx)("u", {
                                     children: "logging out"
                                 })
@@ -57297,16 +57490,16 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            rs = function() {
-                var e = a(ua(), 2),
+            as = function() {
+                var e = a(da(), 2),
                     t = e[0],
                     n = e[1];
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("img", {
                         id: "tooltip-readonly",
                         alt: "lock",
                         src: t ? Ut.Lock() : Ut.Unlock(),
@@ -57320,63 +57513,106 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-readonly",
                         position: "bottom",
                         text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
                     })]
                 })
             },
-            os = function(e) {
-                var t = e.header,
-                    n = (a(Re(), 1)[0], qi("/certificates"));
-                if (n.loading) return (0, Kr.jsx)(Kr.Fragment, {});
-                var r = n.find((function(e) {
+            ss = function(e) {
+                var t = e.header;
+                return (0, Kr.jsxs)(Kr.Fragment, {
+                    children: [(0, Kr.jsx)(us, {
+                        header: t
+                    }), (0, Kr.jsx)(ls, {
+                        header: t
+                    })]
+                })
+            },
+            us = function() {
+                a(Re(), 1)[0];
+                var e = Xi("/certificates");
+                if (e.loading) return (0, Kr.jsx)(Kr.Fragment, {});
+                var t = e.find((function(e) {
                     return "Portal" === e.name
                 }));
-                return r && r.expires_soon ? (0, Kr.jsxs)(Kr.Fragment, {
+                return t && t.expires_soon ? (0, Kr.jsxs)(cs, {
+                    children: [(0, Kr.jsx)("b", {
+                        children: "Warning: SSL certificate for associated Portal will expire soon"
+                    }), "\xa0", Fr.RightArrow, "\xa0 ", t.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(t.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
+                        to: kr.Path("/certificates"),
+                        style: {
+                            color: "inherit"
+                        },
+                        children: "View"
+                    })]
+                }) : void 0
+            },
+            ls = function() {
+                var e = Xi("/portal_access_key");
+                if (e.loading) return (0, Kr.jsx)(Kr.Fragment, {});
+                if (e) {
+                    var t, n;
+                    if (null !== e && void 0 !== e && null !== (t = e.data) && void 0 !== t && t.expires_soon) return (0, Kr.jsxs)(cs, {
+                        children: [(0, Kr.jsx)("b", {
+                            children: "Warning: Access key for associated Portal will expire soon"
+                        }), "\xa0", Fr.RightArrow, "\xa0 ", e.data.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(e.data.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
+                            to: kr.Path("/portal_access_key"),
+                            style: {
+                                color: "inherit"
+                            },
+                            children: "View"
+                        })]
+                    });
+                    if (null === e || void 0 === e || null === (n = e.data) || void 0 === n || !n.valid) return (0, Kr.jsxs)(cs, {
+                        children: [(0, Kr.jsx)("b", {
+                            children: "Warning: Access key for associated Portal is invalid"
+                        }), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
+                            to: kr.Path("/portal_access_key"),
+                            style: {
+                                color: "inherit"
+                            },
+                            children: "View"
+                        })]
+                    })
+                }
+            },
+            cs = function(e) {
+                var t = e.children;
+                return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("tr", {
                         children: (0, Kr.jsx)("td", {
                             style: {
                                 background: "black",
                                 height: "2px"
                             },
                             colSpan: "3"
                         })
                     }), (0, Kr.jsx)("tr", {
-                        children: (0, Kr.jsxs)("td", {
+                        children: (0, Kr.jsx)("td", {
                             style: {
                                 background: "darkred",
                                 color: "#FFF4F3",
                                 padding: "3pt",
                                 fontSize: "9pt"
                             },
                             colSpan: "3",
-                            children: [(0, Kr.jsx)("b", {
-                                children: "Warning: SSL certificate for associated Portal will expire soon"
-                            }), "\xa0", Fr.RightArrow, "\xa0", r.expires_at, "\xa0", Fr.RightArrow, "\xa0", Pr.FromNow(r.expires_at, !0, !1), "/certificate" !== kr.CurrentLogicalPath(t) && (0, Kr.jsxs)(Kr.Fragment, {
-                                children: ["\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
-                                    to: kr.Path("/certificate"),
-                                    style: {
-                                        color: "inherit"
-                                    },
-                                    children: "View"
-                                })]
-                            })]
+                            children: t
                         })
                     }), (0, Kr.jsx)("tr", {
                         children: (0, Kr.jsx)("td", {
                             style: {
                                 background: "black",
                                 height: "1px"
                             },
                             colSpan: "3"
                         })
                     })]
-                }) : (0, Kr.jsx)(Kr.Fragment, {})
+                })
             },
-            is = function(e) {
+            ds = function(e) {
                 var t = e.header,
                     n = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10),
                     r = function(e) {
                         var t = e.path,
                             n = e.label;
                         return (0, Kr.jsx)(Kr.Fragment, {
                             children: kr.CurrentLogicalPath() === t ? (0, Kr.jsxs)("span", {
@@ -57450,15 +57686,15 @@
                                 path: "/login",
                                 label: Br.IsLoggedIn(t) ? "Session" : "Login"
                             })]
                         })]
                     })
                 })
             },
-            as = function(e) {
+            fs = function(e) {
                 var t, n, r, o, i = e.header;
 
                 function a(e) {
                     return e ? {
                         textDecoration: "none",
                         color: "black",
                         fontWeight: "bold"
@@ -57534,31 +57770,31 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-header-aws",
                         position: "bottom",
                         text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
                     })]
                 })
             },
-            ss = function(e) {
+            ps = function(e) {
                 var t = e.header;
                 return (0, Kr.jsxs)("span", {
-                    children: [(0, Kr.jsx)(is, {
+                    children: [(0, Kr.jsx)(ds, {
                         header: t
                     }), (0, Kr.jsx)(Kr.Fragment, {
                         children: "\xa0|\xa0"
-                    }), (0, Kr.jsx)(as, {
+                    }), (0, Kr.jsx)(fs, {
                         header: t
                     })]
                 })
             },
-            us = function(e) {
-                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k = Xi(),
-                    C = $a(),
+            hs = function(e) {
+                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k = ta(),
+                    C = ns(),
                     E = fe(),
-                    _ = a($i(), 1)[0],
+                    _ = a(na(), 1)[0],
                     T = At.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                     A = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10);
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: k.loading ? (0, Kr.jsxs)("div", {
                         style: {
                             width: "100%"
                         },
@@ -57837,15 +58073,15 @@
                                             style: {
                                                 paddingRight: "10pt",
                                                 whiteSpace: "nowrap",
                                                 color: "#D6EAF8"
                                             },
                                             align: "right",
                                             children: [(0, Kr.jsx)("small", {
-                                                children: (0, Kr.jsx)(da.FormatDateTime, {
+                                                children: (0, Kr.jsx)(ha.FormatDateTime, {
                                                     verbose: !0,
                                                     timezone: !1
                                                 })
                                             }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, Kr.jsxs)(Kr.Fragment, {
                                                 children: ["\xa0|\xa0", (0, Kr.jsx)(Oe, {
                                                     id: "tooltip-header-account",
                                                     to: kr.Path("/login"),
@@ -57864,15 +58100,15 @@
                                             }), Br.IsLoggedIn(k) ? (0, Kr.jsxs)("span", {
                                                 children: ["\xa0|\xa0", (0, Kr.jsx)("span", {
                                                     style: {
                                                         cursor: "pointer",
                                                         color: "#D6EAF8"
                                                     },
                                                     onClick: function() {
-                                                        return Oi()
+                                                        return Pi()
                                                     },
                                                     children: "LOGOUT"
                                                 })]
                                             }) : (0, Kr.jsxs)("span", {
                                                 children: ["\xa0|\xa0", (0, Kr.jsx)(Oe, {
                                                     to: kr.Path("/login?auth", At.Current(k)),
                                                     style: {
@@ -57903,15 +58139,15 @@
                                             width: "49%",
                                             style: {
                                                 paddingLeft: "10pt",
                                                 paddingTop: "3pt",
                                                 paddingBottom: "3pt",
                                                 whiteSpace: "nowrap"
                                             },
-                                            children: (0, Kr.jsx)(ss, {
+                                            children: (0, Kr.jsx)(ps, {
                                                 header: k
                                             })
                                         }), (0, Kr.jsx)("td", {
                                             width: "2%",
                                             align: "center",
                                             style: {
                                                 whiteSpace: "nowrap",
@@ -58233,15 +58469,15 @@
                                                                 })]
                                                             })
                                                         })]
                                                     })
                                                 })
                                             })
                                         })]
-                                    }), (0, Kr.jsx)(os, {
+                                    }), (0, Kr.jsx)(ss, {
                                         header: k
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 height: "1px",
                                                 background: "darkblue"
                                             }
@@ -58259,50 +58495,50 @@
                                 children: (0, Kr.jsx)("table", {
                                     children: (0, Kr.jsx)("tbody", {
                                         children: (0, Kr.jsx)("tr", {
                                             children: (0, Kr.jsx)("td", {
                                                 style: {
                                                     paddingLeft: "10pt"
                                                 },
-                                                children: (0, Kr.jsx)(rs, {})
+                                                children: (0, Kr.jsx)(as, {})
                                             })
                                         })
                                     })
                                 })
                             })]
                         })]
                     })
                 })
             },
-            ls = function(e) {
+            gs = function(e) {
                 var n = e.children,
                     r = a((0, t.useState)({
                         loading: !0
                     }), 2),
                     o = r[0],
                     i = r[1];
-                return qi("/header", {
+                return Xi("/header", {
                     onData: function(e) {
                         e.loading = !1, i(e), At.IsFoursightFourfront(e) ? Ft.SetFoursightFourfront() : Ft.SetFoursightCgap()
                     },
                     onError: function(e) {
                         i((function(e) {
                             return Ye(Ye({}, e), {
                                 error: !0
                             })
                         }))
                     },
                     cache: !0
-                }), (0, Kr.jsx)(Ki.Provider, {
+                }), (0, Kr.jsx)(ea.Provider, {
                     value: [o, i],
                     children: n
                 })
             },
-            cs = function(e) {
-                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j = Xi(),
+            ys = function(e) {
+                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j = ta(),
                     x = (At.IsFoursightFourfront(j) ? "foursight" : "foursight-cgap") + ": " + (null === j || void 0 === j || null === (n = j.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === j || void 0 === j || null === (r = j.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === j || void 0 === j || null === (o = j.versions) || void 0 === o ? void 0 : o.dcicutils),
                     N = {
                         id: "".concat(null === (i = j.app) || void 0 === i || null === (s = i.credentials) || void 0 === s ? void 0 : s.aws_account_name, ":").concat(null === j || void 0 === j || null === (u = j.app) || void 0 === u ? void 0 : u.stage),
                         name: null === (l = j.app) || void 0 === l || null === (c = l.credentials) || void 0 === c ? void 0 : c.aws_account_name,
                         stage: null === (d = j.app) || void 0 === d ? void 0 : d.stage
                     },
                     I = a((0, t.useState)(!1), 2),
@@ -58408,15 +58644,15 @@
                                 top: "4pt",
                                 bottom: "10pt"
                             }), D && (0, Kr.jsx)(Kr.Fragment, {
                                 children: (0, Kr.jsx)("div", {
                                     style: {
                                         marginBottom: "12pt"
                                     },
-                                    children: (0, Kr.jsx)(na, {
+                                    children: (0, Kr.jsx)(ia, {
                                         account: N,
                                         header: j,
                                         decrementAccountCount: function() {},
                                         all: !0,
                                         brighten: !0
                                     })
                                 })
@@ -58523,20 +58759,20 @@
                                 children: (0, Kr.jsx)(bi, {
                                     to: "/login",
                                     children: (0, Kr.jsx)("u", {
                                         children: "here"
                                     })
                                 })
                             }), ". ", (0, Kr.jsx)("br", {}), "To ", (0, Kr.jsx)("b", {
-                                onClick: Oi,
+                                onClick: Pi,
                                 children: (0, Kr.jsx)(bi, {
                                     children: "logout"
                                 })
                             }), " click ", (0, Kr.jsx)("b", {
-                                onClick: Oi,
+                                onClick: Pi,
                                 children: (0, Kr.jsx)(bi, {
                                     children: (0, Kr.jsx)("u", {
                                         children: "here"
                                     })
                                 })
                             }), "."]
                         }), (0, Kr.jsx)(Kr.Fragment, {
@@ -58576,15 +58812,15 @@
                                     }
                                 })]
                             })
                         })]
                     })
                 })
             },
-            ds = function(e) {
+            ms = function(e) {
                 var n = e.title,
                     r = e.show,
                     o = void 0 === r || r,
                     i = e.info,
                     s = e.children,
                     u = a((0, t.useState)(o), 2),
                     l = u[0],
@@ -58673,15 +58909,15 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })
                 })
             },
-            fs = function(e) {
+            vs = function(e) {
                 var t = e.name,
                     n = e.value,
                     r = e.monospace,
                     o = void 0 !== r && r,
                     i = e.copy,
                     a = void 0 === i || i,
                     s = e.size,
@@ -58817,334 +59053,334 @@
                                     })
                                 }), I]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
-            ps = function() {
-                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = Xi(),
-                    B = qi("/info"),
+            Ms = function() {
+                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = ta(),
+                    B = Xi("/info"),
                     F = a((0, t.useState)(!1), 2),
                     Y = F[0],
                     Q = F[1],
                     G = a((0, t.useState)(!1), 2),
                     W = G[0],
                     H = G[1],
                     Z = a((0, t.useState)(!1), 2),
                     V = Z[0],
                     q = Z[1],
-                    J = la();
+                    J = fa();
                 return B.error ? (0, Kr.jsx)(xi, {
                     error: B.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
-                    children: [(0, Kr.jsxs)(ds, {
+                    children: [(0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Versions",
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
                             value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "foursight-core",
                             value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "dcicutils",
                             value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "tibanna",
                             value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "tibanna-ff",
                             value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "chalice",
                             value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
                             monospace: !0,
                             copy: !0,
                             chalice: !0,
                             size: "2",
                             pypi: !0,
                             github: "aws"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "python",
                             value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
                             monospace: !0,
                             copy: !0,
                             python: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "elasticsearch-server",
                             value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             elasticsearch: !0
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "elasticsearch",
                             value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "elasticsearch-dsl",
                             value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         })]
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Credentials Info",
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "AWS Account Number",
                             value: B.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "AWS User ARN",
                             value: B.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "AWS Access Key ID",
                             value: B.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "AWS Region Name",
                             value: B.get("app.credentials.aws_region"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Auth0 Client ID",
                             value: B.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Resources",
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "Foursight Server",
                             value: B.get("server.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Portal Server",
                             value: B.get("server.portal"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "ElasticSearch Server",
                             value: B.get("server.es"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "RDS Server",
                             value: B.get("server.rds"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "SQS Server",
                             value: B.get("server.sqs"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Environment Names",
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "Environment Name",
                             value: At.RegularName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment Name (Full)",
                             value: At.FullName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment Name (Short)",
                             value: At.ShortName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment Name (Public)",
                             value: At.PublicName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment Name (Foursight)",
                             value: At.FoursightName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment Name (Preferred)",
                             value: At.PreferredName(At.Current(R), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Bucket Names",
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "Global Environment Bucket",
                             value: B.get("buckets.env"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Foursight Bucket Name",
                             value: B.get("buckets.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Foursight Bucket Prefix",
                             value: B.get("buckets.foursight_prefix"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsx)(ds, {
+                    }), (0, Kr.jsx)(ms, {
                         info: B,
                         title: "Environment & Bucket Names",
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 padding: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
                             children: (0, Kr.jsxs)("span", {
-                                children: [Ui.Format(B.get("buckets.info")), (null === (g = B.get("buckets.info")) || void 0 === g ? void 0 : g.length) > 1 ? (0, Kr.jsx)("div", {
+                                children: [Bi.Format(B.get("buckets.info")), (null === (g = B.get("buckets.info")) || void 0 === g ? void 0 : g.length) > 1 ? (0, Kr.jsx)("div", {
                                     style: {
                                         height: "1px",
                                         marginTop: "6px",
                                         marginBottom: "6px",
                                         background: "black"
                                     }
                                 }) : (0, Kr.jsx)("span", {})]
                             }, Dr()())
                         })
-                    }), (0, Kr.jsx)(ds, {
+                    }), (0, Kr.jsx)(ms, {
                         info: B,
                         title: "Ecosystem",
                         show: !1,
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 paddingTop: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
-                            children: Ui.Format(B.get("buckets.ecosystem"))
+                            children: Bi.Format(B.get("buckets.ecosystem"))
                         })
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Authentication/Authorization Info",
                         show: !1,
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "Email",
                             value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
                             monospace: !0,
                             copy: !0,
                             check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
                             link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "First Name",
                             value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Last Name",
                             value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environments",
                             value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Audience",
                             value: null === (w = Br.Token()) || void 0 === w ? void 0 : w.aud,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Issued At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(da.FormatDuration, {
+                            value: (0, Kr.jsx)(ha.FormatDuration, {
                                 start: null === (j = Br.Token()) || void 0 === j ? void 0 : j.authenticated_at,
                                 verbose: !0,
                                 fallback: "just now",
                                 suffix: "ago",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Expires At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(da.FormatDuration, {
+                            value: (0, Kr.jsx)(ha.FormatDuration, {
                                 end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
                                 verbose: !0,
                                 fallback: "now",
                                 suffix: "from now",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
@@ -59190,15 +59426,15 @@
                                         return Yr.Copy("authtoken")
                                     },
                                     style: {
                                         float: "right",
                                         height: "20px",
                                         cursor: "copy"
                                     }
-                                }), Ui.Format(Br.Token())]
+                                }), Bi.Format(Br.Token())]
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("small", {
                                 onClick: function() {
                                     return Q(!0)
                                 },
                                 style: {
@@ -59209,70 +59445,70 @@
                                     children: [(0, Kr.jsx)("u", {
                                         children: "AuthToken"
                                     }), "\xa0", Fr.UpArrow]
                                 })
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
-                        children: (0, Kr.jsxs)(ds, {
+                        children: (0, Kr.jsxs)(ms, {
                             info: B,
                             title: "Logs",
-                            children: [(0, Kr.jsx)(fs, {
+                            children: [(0, Kr.jsx)(vs, {
                                 name: "Log Group",
                                 value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, Kr.jsx)(fs, {
+                            }), (0, Kr.jsx)(vs, {
                                 name: "Log Stream",
                                 value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                 monospace: !0,
                                 size: "2"
                             })]
                         })
-                    }), B.get("app.lambda") && (0, Kr.jsxs)(ds, {
+                    }), B.get("app.lambda") && (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Lambda",
                         show: !1,
-                        children: [(0, Kr.jsx)(fs, {
+                        children: [(0, Kr.jsx)(vs, {
                             name: "Name",
                             value: B.get("app.lambda.lambda_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Function",
                             value: B.get("app.lambda.lambda_function_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "ARN",
                             value: B.get("app.lambda.lambda_function_arn"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "S3 Location",
                             value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Size",
                             value: B.get("app.lambda.lambda_code_size"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Modified",
                             value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Role",
                             value: B.get("app.lambda.lambda_role"),
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ds, {
+                    }), (0, Kr.jsxs)(ms, {
                         info: B,
                         title: "Miscellany",
                         children: [V ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 id: "tooltip-info-reloading",
                                 style: {
                                     float: "right"
@@ -59326,127 +59562,127 @@
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "App Deployed At",
                             value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             copy: !0,
                             optional: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "App Launched At",
                             value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Page Loaded At",
                             value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Package",
                             value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Stage",
                             value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Environment",
                             value: At.Current(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Domain",
                             value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Context",
                             value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Path",
                             value: B.get("page.path"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Endpoint",
                             value: B.get("page.endpoint"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Client (React UI)",
                             value: kr.BaseUrl(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Server (React API)",
                             value: zt.BaseUrl(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(fs, {
+                        }), (0, Kr.jsx)(vs, {
                             name: "Checks File",
                             value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(fs, {
+                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(vs, {
                             name: "Accounts File",
                             value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(fs, {
+                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(vs, {
                             name: "Accounts File (S3)",
                             value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsx)(ds, {
+                    }), (0, Kr.jsx)(ms, {
                         info: B,
                         title: "GAC: ".concat(B.get("gac.name")),
                         show: !1,
                         children: B.get("gac.values") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("gac.values")).map((function(e) {
-                                return (0, Kr.jsx)(fs, {
+                                return (0, Kr.jsx)(vs, {
                                     name: e,
                                     value: B.get("gac.values")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
-                    }), (0, Kr.jsx)(ds, {
+                    }), (0, Kr.jsx)(ms, {
                         info: B,
                         title: "Environment Variables",
                         show: !1,
                         children: B.get("environ") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("environ")).map((function(e) {
-                                return (0, Kr.jsx)(fs, {
+                                return (0, Kr.jsx)(vs, {
                                     name: e,
                                     value: B.get("environ")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
                     }), (null === (P = R.app) || void 0 === P ? void 0 : P.accounts) && (0, Kr.jsx)("div", {
                         className: "container",
                         style: {
                             marginTop: "4pt"
                         },
                         children: W ? (0, Kr.jsx)(Kr.Fragment, {
-                            children: (0, Kr.jsx)(ra, {})
+                            children: (0, Kr.jsx)(aa, {})
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("b", {
                                 onClick: function() {
                                     return H(!0)
                                 },
                                 style: {
                                     cursor: "pointer"
@@ -59472,40 +59708,40 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })]
                 })
             },
-            hs = function(e, t) {
-                return hs = Object.setPrototypeOf || {
+            bs = function(e, t) {
+                return bs = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, hs(e, t)
+                }, bs(e, t)
             };
 
-        function gs(e, t) {
+        function ws(e, t) {
             function n() {
                 this.constructor = e
             }
-            hs(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            bs(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var ys, ms, vs, Ms = function() {
-            return Ms = Object.assign || function(e) {
+        var js, xs, Ns, Is = function() {
+            return Is = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Ms.apply(this, arguments)
+            }, Is.apply(this, arguments)
         };
 
-        function bs(e, t, n, r) {
+        function Ds(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -59525,15 +59761,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function ws(e, t) {
+        function Ss(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -59601,15 +59837,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function js(e, t) {
+        function Ls(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59623,50 +59859,50 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function xs(e) {
+        function ks(e) {
             return e && !!["provider"].find((function(t) {
                 return e.hasOwnProperty(t)
             }))
         }
 
-        function Ns(e) {
+        function Cs(e) {
             return void 0 !== e.redirectSignIn
         }! function(e) {
             e.Cognito = "COGNITO", e.Google = "Google", e.Facebook = "Facebook", e.Amazon = "LoginWithAmazon", e.Apple = "SignInWithApple"
-        }(ys || (ys = {})),
+        }(js || (js = {})),
         function(e) {
             e.NoConfig = "noConfig", e.MissingAuthConfig = "missingAuthConfig", e.EmptyUsername = "emptyUsername", e.InvalidUsername = "invalidUsername", e.EmptyPassword = "emptyPassword", e.EmptyCode = "emptyCode", e.SignUpError = "signUpError", e.NoMFA = "noMFA", e.InvalidMFA = "invalidMFA", e.EmptyChallengeResponse = "emptyChallengeResponse", e.NoUserSession = "noUserSession", e.Default = "default", e.DeviceConfig = "deviceConfig", e.NetworkError = "networkError", e.AutoSignInError = "autoSignInError"
-        }(ms || (ms = {})),
+        }(xs || (xs = {})),
         function(e) {
             e.API_KEY = "API_KEY", e.AWS_IAM = "AWS_IAM", e.OPENID_CONNECT = "OPENID_CONNECT", e.AMAZON_COGNITO_USER_POOLS = "AMAZON_COGNITO_USER_POOLS", e.AWS_LAMBDA = "AWS_LAMBDA"
-        }(vs || (vs = {}));
-        var Is = function(e, t) {
-            return Is = Object.setPrototypeOf || {
+        }(Ns || (Ns = {}));
+        var Es = function(e, t) {
+            return Es = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-            }, Is(e, t)
+            }, Es(e, t)
         };
-        var Ds = function() {
-            return Ds = Object.assign || function(e) {
+        var _s = function() {
+            return _s = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Ds.apply(this, arguments)
+            }, _s.apply(this, arguments)
         };
 
-        function Ss(e, t, n, r) {
+        function Ts(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -59686,15 +59922,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Ls(e, t) {
+        function As(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -59762,15 +59998,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function ks(e) {
+        function Os(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -59778,15 +60014,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Cs(e, t) {
+        function zs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59800,58 +60036,58 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Es() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Cs(arguments[t]));
+        function Us() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(zs(arguments[t]));
             return e
         }
-        var _s, Ts = {
+        var Ps, Rs = {
             VERBOSE: 1,
             DEBUG: 2,
             INFO: 3,
             WARN: 4,
             ERROR: 5
         };
         ! function(e) {
             e.DEBUG = "DEBUG", e.ERROR = "ERROR", e.INFO = "INFO", e.WARN = "WARN", e.VERBOSE = "VERBOSE"
-        }(_s || (_s = {}));
-        var As = function() {
+        }(Ps || (Ps = {}));
+        var Bs = function() {
                 function e(e, t) {
-                    void 0 === t && (t = _s.WARN), this.name = e, this.level = t, this._pluggables = []
+                    void 0 === t && (t = Ps.WARN), this.name = e, this.level = t, this._pluggables = []
                 }
                 return e.prototype._padding = function(e) {
                     return e < 10 ? "0" + e : "" + e
                 }, e.prototype._ts = function() {
                     var e = new Date;
                     return [this._padding(e.getMinutes()), this._padding(e.getSeconds())].join(":") + "." + e.getMilliseconds()
                 }, e.prototype.configure = function(e) {
                     return e ? (this._config = e, this._config) : this._config
                 }, e.prototype._log = function(t) {
                     for (var n, r, o = [], i = 1; i < arguments.length; i++) o[i - 1] = arguments[i];
                     var a = this.level;
                     e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL);
-                    var s = Ts[a],
-                        u = Ts[t];
+                    var s = Rs[a],
+                        u = Rs[t];
                     if (u >= s) {
                         var l = console.log.bind(console);
-                        t === _s.ERROR && console.error && (l = console.error.bind(console)), t === _s.WARN && console.warn && (l = console.warn.bind(console));
+                        t === Ps.ERROR && console.error && (l = console.error.bind(console)), t === Ps.WARN && console.warn && (l = console.warn.bind(console));
                         var c = "[" + t + "] " + this._ts() + " " + this.name,
                             d = "";
                         if (1 === o.length && "string" === typeof o[0]) l(d = c + " - " + o[0]);
                         else if (1 === o.length) d = c + " " + o[0], l(c, o[0]);
                         else if ("string" === typeof o[0]) {
                             var f = o.slice(1);
                             1 === f.length && (f = f[0]), d = c + " - " + o[0] + " " + f, l(c + " - " + o[0], f)
                         } else d = c + " " + o, l(c, o);
                         try {
-                            for (var p = ks(this._pluggables), h = p.next(); !h.done; h = p.next()) {
+                            for (var p = Os(this._pluggables), h = p.next(); !h.done; h = p.next()) {
                                 var g = h.value,
                                     y = {
                                         message: d,
                                         timestamp: Date.now()
                                     };
                                 g.pushLogs([y])
                             }
@@ -59865,78 +60101,78 @@
                             } finally {
                                 if (n) throw n.error
                             }
                         }
                     }
                 }, e.prototype.log = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.INFO], e))
+                    this._log.apply(this, Us([Ps.INFO], e))
                 }, e.prototype.info = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.INFO], e))
+                    this._log.apply(this, Us([Ps.INFO], e))
                 }, e.prototype.warn = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.WARN], e))
+                    this._log.apply(this, Us([Ps.WARN], e))
                 }, e.prototype.error = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.ERROR], e))
+                    this._log.apply(this, Us([Ps.ERROR], e))
                 }, e.prototype.debug = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.DEBUG], e))
+                    this._log.apply(this, Us([Ps.DEBUG], e))
                 }, e.prototype.verbose = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Es([_s.VERBOSE], e))
+                    this._log.apply(this, Us([Ps.VERBOSE], e))
                 }, e.prototype.addPluggable = function(e) {
                     e && "Logging" === e.getCategoryName() && (this._pluggables.push(e), e.configure(this._config))
                 }, e.prototype.listPluggables = function() {
                     return this._pluggables
                 }, e.LOG_LEVEL = null, e
             }(),
-            Os = new As("Hub"),
-            zs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
-        var Us = function() {
+            Fs = new Bs("Hub"),
+            Ys = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
+        var Qs = function() {
                 function e(e) {
                     this.listeners = [], this.patterns = [], this.protectedChannels = ["core", "auth", "api", "analytics", "interactions", "pubsub", "storage", "ui", "xr"], this.name = e
                 }
                 return e.prototype._remove = function(e, t) {
                     if (e instanceof RegExp) {
                         var n = this.patterns.find((function(t) {
                             return t.pattern.source === e.source
                         }));
-                        if (!n) return void Os.warn("No listeners for " + e);
-                        this.patterns = Es(this.patterns.filter((function(e) {
+                        if (!n) return void Fs.warn("No listeners for " + e);
+                        this.patterns = Us(this.patterns.filter((function(e) {
                             return e !== n
                         })))
                     } else {
                         var r = this.listeners[e];
-                        if (!r) return void Os.warn("No listeners for " + e);
-                        this.listeners[e] = Es(r.filter((function(e) {
+                        if (!r) return void Fs.warn("No listeners for " + e);
+                        this.listeners[e] = Us(r.filter((function(e) {
                             return e.callback !== t
                         })))
                     }
                 }, e.prototype.remove = function(e, t) {
                     this._remove(e, t)
                 }, e.prototype.dispatch = function(e, t, n, r) {
-                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === zs || Os.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
+                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === Ys || Fs.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
                     var o = {
                         channel: e,
-                        payload: Ds({}, t),
+                        payload: _s({}, t),
                         source: n,
                         patternInfo: []
                     };
                     try {
                         this._toListeners(o)
                     } catch (i) {
-                        Os.error(i)
+                        Fs.error(i)
                     }
                 }, e.prototype.listen = function(e, t, n) {
                     var r, o = this;
                     if (void 0 === n && (n = "noname"), function(e) {
                             return void 0 !== e.onHubCapsule
-                        }(t)) Os.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
+                        }(t)) Fs.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
                     else {
                         if ("function" !== typeof t) throw new Error("No callback supplied to Hub");
                         r = t
                     }
                     if (e instanceof RegExp) this.patterns.push({
                         pattern: e,
                         callback: r
@@ -59952,115 +60188,115 @@
                         o._remove(e, r)
                     }
                 }, e.prototype._toListeners = function(e) {
                     var t = e.channel,
                         n = e.payload,
                         r = this.listeners[t];
                     if (r && r.forEach((function(r) {
-                            Os.debug("Dispatching to " + t + " with ", n);
+                            Fs.debug("Dispatching to " + t + " with ", n);
                             try {
                                 r.callback(e)
                             } catch (o) {
-                                Os.error(o)
+                                Fs.error(o)
                             }
                         })), this.patterns.length > 0) {
-                        if (!n.message) return void Os.warn("Cannot perform pattern matching without a message key");
+                        if (!n.message) return void Fs.warn("Cannot perform pattern matching without a message key");
                         var o = n.message;
                         this.patterns.forEach((function(t) {
                             var n = o.match(t.pattern);
                             if (n) {
-                                var r = Cs(n).slice(1),
-                                    i = Ds(Ds({}, e), {
+                                var r = zs(n).slice(1),
+                                    i = _s(_s({}, e), {
                                         patternInfo: r
                                     });
                                 try {
                                     t.callback(i)
                                 } catch (a) {
-                                    Os.error(a)
+                                    Fs.error(a)
                                 }
                             }
                         }))
                     }
                 }, e
             }(),
-            Ps = new Us("__default__"),
-            Rs = {},
-            Bs = function() {
+            Gs = new Qs("__default__"),
+            Ws = {},
+            Hs = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Rs[e] = t, Rs[e]
+                    return Ws[e] = t, Ws[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Rs, e) ? Rs[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Ws, e) ? Ws[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Rs[e]
+                    return delete Ws[e]
                 }, e.clear = function() {
-                    return Rs = {}
+                    return Ws = {}
                 }, e
             }(),
-            Fs = function() {
+            Zs = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.amplify.test-ls", 1), this.storageWindow.removeItem("aws.amplify.test-ls")
                     } catch (e) {
-                        this.storageWindow = Bs
+                        this.storageWindow = Hs
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            Ys = function() {
+            Vs = function() {
                 return {
                     isBrowser: "undefined" !== typeof window && "undefined" !== typeof window.document,
                     isNode: "undefined" !== typeof process && null != process.versions && null != process.versions.node
                 }
             },
-            Qs = new As("Util"),
-            Gs = function(e) {
+            qs = new Bs("Util"),
+            Js = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     return n.nonRetryable = !0, n
                 }
                 return function(e, t) {
                     function n() {
                         this.constructor = e
                     }
-                    Is(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                    Es(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
                 }(t, e), t
             }(Error);
-        var Ws = 3e5;
-        var Hs = function(e, t, n, r) {
-                return void 0 === n && (n = Ws),
+        var Ks = 3e5;
+        var Xs = function(e, t, n, r) {
+                return void 0 === n && (n = Ks),
                     function(e, t, n, r) {
-                        return Ss(this, void 0, void 0, (function() {
+                        return Ts(this, void 0, void 0, (function() {
                             var o = this;
-                            return Ls(this, (function(i) {
+                            return As(this, (function(i) {
                                 if ("function" !== typeof e) throw Error("functionToRetry must be a function");
                                 return [2, new Promise((function(i, a) {
-                                    return Ss(o, void 0, void 0, (function() {
+                                    return Ts(o, void 0, void 0, (function() {
                                         var o, s, u, l, c, d, f;
-                                        return Ls(this, (function(p) {
+                                        return As(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
                                                     o = 0, s = !1, l = function() {}, r && r.then((function() {
                                                         s = !0, clearTimeout(u), l()
                                                     })), d = function() {
                                                         var r, d, f, p;
-                                                        return Ls(this, (function(h) {
+                                                        return As(this, (function(h) {
                                                             switch (h.label) {
                                                                 case 0:
-                                                                    o++, Qs.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
+                                                                    o++, qs.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
                                                                 case 1:
-                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Es(t))];
+                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Us(t))];
                                                                 case 2:
                                                                     return [2, (r.value = d.apply(void 0, [h.sent()]), r)];
                                                                 case 3:
-                                                                    return f = h.sent(), c = f, Qs.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (Qs.debug(e.name + " non retryable error", f), [2, {
+                                                                    return f = h.sent(), c = f, qs.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (qs.debug(e.name + " non retryable error", f), [2, {
                                                                         value: a(f)
-                                                                    }]) : (p = n(o, t, f), Qs.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
+                                                                    }]) : (p = n(o, t, f), qs.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
                                                                         value: a(f)
                                                                     }] : [3, 4]);
                                                                 case 4:
                                                                     return [4, new Promise((function(e) {
                                                                         l = e, u = setTimeout(l, p)
                                                                     }))];
                                                                 case 5:
@@ -60082,147 +60318,147 @@
                                             }
                                         }))
                                     }))
                                 }))]
                             }))
                         }))
                     }(e, t, function(e) {
-                        return void 0 === e && (e = Ws),
+                        return void 0 === e && (e = Ks),
                             function(t) {
                                 var n = 100 * Math.pow(2, t) + 100 * Math.random();
                                 return !(n > e) && n
                             }
                     }(n), r)
             },
-            Zs = new As("CognitoCredentials"),
-            Vs = new Promise((function(e, t) {
-                return Ys().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (Zs.debug("google api already loaded"), e()) : void setTimeout((function() {
+            $s = new Bs("CognitoCredentials"),
+            eu = new Promise((function(e, t) {
+                return Vs().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? ($s.debug("google api already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (Zs.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : ($s.debug("not in the browser, directly resolved"), e())
             })),
-            qs = function() {
+            tu = function() {
                 function e() {
                     this.initialized = !1, this.refreshGoogleToken = this.refreshGoogleToken.bind(this), this._refreshGoogleTokenImpl = this._refreshGoogleTokenImpl.bind(this)
                 }
                 return e.prototype.refreshGoogleToken = function() {
-                    return Ss(this, void 0, void 0, (function() {
-                        return Ls(this, (function(e) {
+                    return Ts(this, void 0, void 0, (function() {
+                        return As(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (Zs.debug("need to wait for the Google SDK loaded"), [4, Vs]);
+                                    return this.initialized ? [3, 2] : ($s.debug("need to wait for the Google SDK loaded"), [4, eu]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, Zs.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, $s.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshGoogleTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshGoogleTokenImpl = function() {
                     var e = null;
-                    return Ys().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
+                    return Vs().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
                         e.getAuthInstance().then((function(e) {
-                            e || (Zs.debug("google Auth undefined"), n(new Gs("google Auth undefined")));
+                            e || ($s.debug("google Auth undefined"), n(new Js("google Auth undefined")));
                             var r = e.currentUser.get();
-                            r.isSignedIn() ? (Zs.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
+                            r.isSignedIn() ? ($s.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
                                 var n = e.id_token,
                                     r = e.expires_at;
                                 t({
                                     token: n,
                                     expires_at: r
                                 })
                             })).catch((function(e) {
-                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new Gs("Failed to reload google auth response"))
-                            }))) : n(new Gs("User is not signed in with Google"))
+                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new Js("Failed to reload google auth response"))
+                            }))) : n(new Js("User is not signed in with Google"))
                         })).catch((function(e) {
-                            Zs.debug("Failed to refresh google token", e), n(new Gs("Failed to refresh google token"))
+                            $s.debug("Failed to refresh google token", e), n(new Js("Failed to refresh google token"))
                         }))
-                    })) : (Zs.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
+                    })) : ($s.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
                 }, e
             }(),
-            Js = new As("CognitoCredentials"),
-            Ks = new Promise((function(e, t) {
-                return Ys().isBrowser ? window.FB ? (Js.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
+            nu = new Bs("CognitoCredentials"),
+            ru = new Promise((function(e, t) {
+                return Vs().isBrowser ? window.FB ? (nu.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (Js.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (nu.debug("not in the browser, directly resolved"), e())
             })),
-            Xs = function() {
+            ou = function() {
                 function e() {
                     this.initialized = !1, this.refreshFacebookToken = this.refreshFacebookToken.bind(this), this._refreshFacebookTokenImpl = this._refreshFacebookTokenImpl.bind(this)
                 }
                 return e.prototype.refreshFacebookToken = function() {
-                    return Ss(this, void 0, void 0, (function() {
-                        return Ls(this, (function(e) {
+                    return Ts(this, void 0, void 0, (function() {
+                        return As(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (Js.debug("need to wait for the Facebook SDK loaded"), [4, Ks]);
+                                    return this.initialized ? [3, 2] : (nu.debug("need to wait for the Facebook SDK loaded"), [4, ru]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, Js.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, nu.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshFacebookTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshFacebookTokenImpl = function() {
                     var e = null;
-                    if (Ys().isBrowser && (e = window.FB), !e) {
+                    if (Vs().isBrowser && (e = window.FB), !e) {
                         var t = "no fb sdk available";
-                        return Js.debug(t), Promise.reject(new Gs(t))
+                        return nu.debug(t), Promise.reject(new Js(t))
                     }
                     return new Promise((function(t, n) {
                         e.getLoginStatus((function(e) {
                             if (e && e.authResponse) {
                                 var r = e.authResponse,
                                     o = r.accessToken,
                                     i = 1e3 * r.expiresIn + (new Date).getTime();
                                 if (!o) {
                                     a = "the jwtToken is undefined";
-                                    Js.debug(a), n(new Gs(a))
+                                    nu.debug(a), n(new Js(a))
                                 }
                                 t({
                                     token: o,
                                     expires_at: i
                                 })
                             } else {
                                 var a = "no response from facebook when refreshing the jwt token";
-                                Js.debug(a), n(new Gs(a))
+                                nu.debug(a), n(new Js(a))
                             }
                         }), {
                             scope: "public_profile,email"
                         })
                     }))
                 }, e
             }(),
-            $s = new qs,
-            eu = new Xs,
-            tu = new As("Amplify"),
-            nu = new(function() {
+            iu = new tu,
+            au = new ou,
+            su = new Bs("Amplify"),
+            uu = new(function() {
                 function e() {
-                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = As, this.ServiceWorker = null
+                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Bs, this.ServiceWorker = null
                 }
                 return e.prototype.register = function(e) {
-                    tu.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : tu.debug("no getModuleName method for component", e), e.configure(this._config)
+                    su.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : su.debug("no getModuleName method for component", e), e.configure(this._config)
                 }, e.prototype.configure = function(e) {
                     var t = this;
-                    return e ? (this._config = Object.assign(this._config, e), tu.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
-                        var n = Cs(e, 2),
+                    return e ? (this._config = Object.assign(this._config, e), su.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
+                        var n = zs(e, 2),
                             r = (n[0], n[1]);
                         Object.keys(r).forEach((function(e) {
                             t._modules[e] && (r[e] = t._modules[e])
                         }))
                     })), this._components.map((function(e) {
                         e.configure(t._config)
                     })), this._config) : this._config
                 }, e.prototype.addPluggable = function(e) {
                     e && e.getCategory && "function" === typeof e.getCategory && this._components.map((function(t) {
                         t.addPluggable && "function" === typeof t.addPluggable && t.addPluggable(e)
                     }))
                 }, e
             }());
 
-        function ru(e, t, n, r) {
+        function lu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60242,15 +60478,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function ou(e, t) {
+        function cu(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60318,15 +60554,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function iu(e, t) {
+        function du(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60339,42 +60575,42 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var au = function(e, t) {
-            return au = Object.setPrototypeOf || {
+        var fu = function(e, t) {
+            return fu = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-            }, au(e, t)
+            }, fu(e, t)
         };
 
-        function su(e, t) {
+        function pu(e, t) {
             if ("function" !== typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
             function n() {
                 this.constructor = e
             }
-            au(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            fu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var uu = function() {
-            return uu = Object.assign || function(e) {
+        var hu = function() {
+            return hu = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, uu.apply(this, arguments)
+            }, hu.apply(this, arguments)
         };
 
-        function lu(e, t, n, r) {
+        function gu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60394,15 +60630,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function cu(e, t) {
+        function yu(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60471,15 +60707,15 @@
                         }
                     }([i, s])
                 }
             }
         }
         Object.create;
 
-        function du(e, t) {
+        function mu(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60492,312 +60728,312 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var fu, pu, hu, gu, yu, mu, vu, Mu, bu, wu, ju, xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl;
+        var vu, Mu, bu, wu, ju, xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl, gl, yl, ml, vl, Ml, bl;
         Object.create;
         ! function(e) {
             e.AUTHENTICATED_ROLE = "AuthenticatedRole", e.DENY = "Deny"
-        }(fu || (fu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
-        }(pu || (pu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
-        }(hu || (hu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
-        }(gu || (gu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
-        }(yu || (yu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
-        }(mu || (mu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
         }(vu || (vu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Mu || (Mu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(bu || (bu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(wu || (wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(ju || (ju = {})),
         function(e) {
-            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
         }(xu || (xu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Nu || (Nu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Iu || (Iu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Du || (Du = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Su || (Su = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Lu || (Lu = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
+            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
         }(ku || (ku = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Cu || (Cu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Eu || (Eu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(_u || (_u = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Tu || (Tu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Au || (Au = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Ou || (Ou = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(zu || (zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Uu || (Uu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Pu || (Pu = {})),
         function(e) {
-            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
         }(Ru || (Ru = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Bu || (Bu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Fu || (Fu = {})),
         function(e) {
-            e.RULES = "Rules", e.TOKEN = "Token"
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
         }(Yu || (Yu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Qu || (Qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Gu || (Gu = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
+            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
         }(Wu || (Wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Hu || (Hu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Zu || (Zu = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return uu({}, e)
-            }
+            e.RULES = "Rules", e.TOKEN = "Token"
         }(Vu || (Vu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(qu || (qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Ju || (Ju = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Ku || (Ku = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(Xu || (Xu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }($u || ($u = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(el || (el = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(tl || (tl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(nl || (nl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(rl || (rl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(ol || (ol = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(il || (il = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(al || (al = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(sl || (sl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(ul || (ul = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(ll || (ll = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(cl || (cl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(dl || (dl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(fl || (fl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
             }
         }(pl || (pl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return uu({}, e)
+                return hu({}, e)
+            }
+        }(hl || (hl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
+        }(gl || (gl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
+        }(yl || (yl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
             }
-        }(hl || (hl = {}));
-        var gl = function() {
+        }(ml || (ml = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
+        }(vl || (vl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
+        }(Ml || (Ml = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return hu({}, e)
+            }
+        }(bl || (bl = {}));
+        var wl = function() {
             function e(e) {
                 this.statusCode = e.statusCode, this.headers = e.headers || {}, this.body = e.body
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "number" === typeof t.statusCode && "object" === typeof t.headers
             }, e
         }();
-        var yl = function() {
-            return yl = Object.assign || function(e) {
+        var jl = function() {
+            return jl = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, yl.apply(this, arguments)
+            }, jl.apply(this, arguments)
         };
 
-        function ml(e, t) {
+        function xl(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60810,44 +61046,44 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var vl = function() {
+        var Nl = function() {
             function e(e) {
                 this.method = e.method || "GET", this.hostname = e.hostname || "localhost", this.port = e.port, this.query = e.query || {}, this.headers = e.headers || {}, this.body = e.body, this.protocol = e.protocol ? ":" !== e.protocol.substr(-1) ? e.protocol + ":" : e.protocol : "https:", this.path = e.path ? "/" !== e.path.charAt(0) ? "/" + e.path : e.path : "/"
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "method" in t && "protocol" in t && "hostname" in t && "path" in t && "object" === typeof t.query && "object" === typeof t.headers
             }, e.prototype.clone = function() {
-                var t, n = new e(yl(yl({}, this), {
-                    headers: yl({}, this.headers)
+                var t, n = new e(jl(jl({}, this), {
+                    headers: jl({}, this.headers)
                 }));
                 return n.query && (n.query = (t = n.query, Object.keys(t).reduce((function(e, n) {
                     var r, o = t[n];
-                    return yl(yl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
-                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(ml(arguments[t]));
+                    return jl(jl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
+                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(xl(arguments[t]));
                         return e
                     }(o) : o, r))
                 }), {}))), n
             }, e
         }();
-        var Ml = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+        var Il = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return cu(this, (function(m) {
+                    return yu(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [uu({}, e)], y = {}, [4, Vl(e.body, t)];
+                                return r = [hu({}, e)], y = {}, [4, ec(e.body, t)];
                             case 1:
-                                switch (n = uu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ql(e, n.body), i) {
+                                switch (n = hu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = tc(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidIdentityPoolConfigurationException":
@@ -60867,91 +61103,91 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, wl(n, t)];
+                                return a = [{}], [4, Sl(n, t)];
                             case 3:
-                                return o = uu.apply(void 0, [uu.apply(void 0, a.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, jl(n, t)];
+                                return s = [{}], [4, Ll(n, t)];
                             case 5:
-                                return o = uu.apply(void 0, [uu.apply(void 0, s.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, xl(n, t)];
+                                return u = [{}], [4, kl(n, t)];
                             case 7:
-                                return o = uu.apply(void 0, [uu.apply(void 0, u.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Nl(n, t)];
+                                return l = [{}], [4, Cl(n, t)];
                             case 9:
-                                return o = uu.apply(void 0, [uu.apply(void 0, l.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, Dl(n, t)];
+                                return c = [{}], [4, _l(n, t)];
                             case 11:
-                                return o = uu.apply(void 0, [uu.apply(void 0, c.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Sl(n, t)];
+                                return d = [{}], [4, Tl(n, t)];
                             case 13:
-                                return o = uu.apply(void 0, [uu.apply(void 0, d.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Ll(n, t)];
+                                return f = [{}], [4, Al(n, t)];
                             case 15:
-                                return o = uu.apply(void 0, [uu.apply(void 0, f.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, kl(n, t)];
+                                return p = [{}], [4, Ol(n, t)];
                             case 17:
-                                return o = uu.apply(void 0, [uu.apply(void 0, p.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = uu(uu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = hu(hu({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            bl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Dl = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return cu(this, (function(m) {
+                    return yu(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [uu({}, e)], y = {}, [4, Vl(e.body, t)];
+                                return r = [hu({}, e)], y = {}, [4, ec(e.body, t)];
                             case 1:
-                                switch (n = uu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ql(e, n.body), i) {
+                                switch (n = hu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = tc(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidParameterException":
@@ -60971,340 +61207,340 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, wl(n, t)];
+                                return a = [{}], [4, Sl(n, t)];
                             case 3:
-                                return o = uu.apply(void 0, [uu.apply(void 0, a.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, jl(n, t)];
+                                return s = [{}], [4, Ll(n, t)];
                             case 5:
-                                return o = uu.apply(void 0, [uu.apply(void 0, s.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, Nl(n, t)];
+                                return u = [{}], [4, Cl(n, t)];
                             case 7:
-                                return o = uu.apply(void 0, [uu.apply(void 0, u.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Il(n, t)];
+                                return l = [{}], [4, El(n, t)];
                             case 9:
-                                return o = uu.apply(void 0, [uu.apply(void 0, l.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, Dl(n, t)];
+                                return c = [{}], [4, _l(n, t)];
                             case 11:
-                                return o = uu.apply(void 0, [uu.apply(void 0, c.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Sl(n, t)];
+                                return d = [{}], [4, Tl(n, t)];
                             case 13:
-                                return o = uu.apply(void 0, [uu.apply(void 0, d.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Ll(n, t)];
+                                return f = [{}], [4, Al(n, t)];
                             case 15:
-                                return o = uu.apply(void 0, [uu.apply(void 0, f.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, kl(n, t)];
+                                return p = [{}], [4, Ol(n, t)];
                             case 17:
-                                return o = uu.apply(void 0, [uu.apply(void 0, p.concat([m.sent()])), {
+                                return o = hu.apply(void 0, [hu.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = uu(uu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = hu(hu({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: Wl(e)
+                                    $metadata: Kl(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            wl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Sl = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Al(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Bl(n, t), [2, hu({
                             name: "ExternalServiceException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            jl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Ll = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Ul(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Ql(n, t), [2, hu({
                             name: "InternalErrorException",
                             $fault: "server",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            xl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            kl = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Pl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Gl(n, t), [2, hu({
                             name: "InvalidIdentityPoolConfigurationException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Nl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Cl = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Rl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Wl(n, t), [2, hu({
                             name: "InvalidParameterException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Il = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            El = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Bl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Hl(n, t), [2, hu({
                             name: "LimitExceededException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Dl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            _l = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Fl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Zl(n, t), [2, hu({
                             name: "NotAuthorizedException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Sl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Tl = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Yl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Vl(n, t), [2, hu({
                             name: "ResourceConflictException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Ll = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Al = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Ql(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = ql(n, t), [2, hu({
                             name: "ResourceNotFoundException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            kl = function(e, t) {
-                return lu(void 0, void 0, void 0, (function() {
+            Ol = function(e, t) {
+                return gu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return cu(this, (function(o) {
-                        return n = e.body, r = Gl(n, t), [2, uu({
+                    return yu(this, (function(o) {
+                        return n = e.body, r = Jl(n, t), [2, hu({
                             name: "TooManyRequestsException",
                             $fault: "client",
-                            $metadata: Wl(e)
+                            $metadata: Kl(e)
                         }, r)]
                     }))
                 }))
             },
-            Cl = function(e, t) {
-                return uu(uu(uu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
+            zl = function(e, t) {
+                return hu(hu(hu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
                     CustomRoleArn: e.CustomRoleArn
                 }), void 0 !== e.IdentityId && null !== e.IdentityId && {
                     IdentityId: e.IdentityId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: _l(e.Logins, t)
+                    Logins: Pl(e.Logins, t)
                 })
             },
-            El = function(e, t) {
-                return uu(uu(uu({}, void 0 !== e.AccountId && null !== e.AccountId && {
+            Ul = function(e, t) {
+                return hu(hu(hu({}, void 0 !== e.AccountId && null !== e.AccountId && {
                     AccountId: e.AccountId
                 }), void 0 !== e.IdentityPoolId && null !== e.IdentityPoolId && {
                     IdentityPoolId: e.IdentityPoolId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: _l(e.Logins, t)
+                    Logins: Pl(e.Logins, t)
                 })
             },
-            _l = function(e, t) {
+            Pl = function(e, t) {
                 return Object.entries(e).reduce((function(e, t) {
-                    var n, r = du(t, 2),
+                    var n, r = mu(t, 2),
                         o = r[0],
                         i = r[1];
-                    return null === i ? e : uu(uu({}, e), ((n = {})[o] = i, n))
+                    return null === i ? e : hu(hu({}, e), ((n = {})[o] = i, n))
                 }), {})
             },
-            Tl = function(e, t) {
+            Rl = function(e, t) {
                 return {
                     AccessKeyId: void 0 !== e.AccessKeyId && null !== e.AccessKeyId ? e.AccessKeyId : void 0,
                     Expiration: void 0 !== e.Expiration && null !== e.Expiration ? new Date(Math.round(1e3 * e.Expiration)) : void 0,
                     SecretKey: void 0 !== e.SecretKey && null !== e.SecretKey ? e.SecretKey : void 0,
                     SessionToken: void 0 !== e.SessionToken && null !== e.SessionToken ? e.SessionToken : void 0
                 }
             },
-            Al = function(e, t) {
+            Bl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Ol = function(e, t) {
+            Fl = function(e, t) {
                 return {
-                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Tl(e.Credentials) : void 0,
+                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Rl(e.Credentials) : void 0,
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            zl = function(e, t) {
+            Yl = function(e, t) {
                 return {
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            Ul = function(e, t) {
+            Ql = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Pl = function(e, t) {
+            Gl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Rl = function(e, t) {
+            Wl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Bl = function(e, t) {
+            Hl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Fl = function(e, t) {
+            Zl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Yl = function(e, t) {
+            Vl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Ql = function(e, t) {
+            ql = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Gl = function(e, t) {
+            Jl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Wl = function(e) {
+            Kl = function(e) {
                 var t;
                 return {
                     httpStatusCode: e.statusCode,
                     requestId: null !== (t = e.headers["x-amzn-requestid"]) && void 0 !== t ? t : e.headers["x-amzn-request-id"],
                     extendedRequestId: e.headers["x-amz-id-2"],
                     cfId: e.headers["x-amz-cf-id"]
                 }
             },
-            Hl = function(e, t) {
+            Xl = function(e, t) {
                 return void 0 === e && (e = new Uint8Array), e instanceof Uint8Array ? Promise.resolve(e) : t.streamCollector(e) || Promise.resolve(new Uint8Array)
             },
-            Zl = function(e, t, n, r, o) {
-                return lu(void 0, void 0, void 0, (function() {
+            $l = function(e, t, n, r, o) {
+                return gu(void 0, void 0, void 0, (function() {
                     var i, a, s, u, l, c;
-                    return cu(this, (function(d) {
+                    return yu(this, (function(d) {
                         switch (d.label) {
                             case 0:
                                 return [4, e.endpoint()];
                             case 1:
                                 return i = d.sent(), a = i.hostname, s = i.protocol, u = void 0 === s ? "https" : s, l = i.port, c = {
                                     protocol: u,
                                     hostname: a,
                                     port: l,
                                     method: "POST",
                                     path: n,
                                     headers: t
-                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new vl(c)]
+                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new Nl(c)]
                         }
                     }))
                 }))
             },
-            Vl = function(e, t) {
+            ec = function(e, t) {
                 return function(e, t) {
-                    return Hl(e, t).then((function(e) {
+                    return Xl(e, t).then((function(e) {
                         return t.utf8Encoder(e)
                     }))
                 }(e, t).then((function(e) {
                     return e.length ? JSON.parse(e) : {}
                 }))
             },
-            ql = function(e, t) {
+            tc = function(e, t) {
                 var n, r, o = function(e) {
                         var t = e;
                         return t.indexOf(":") >= 0 && (t = t.split(":")[0]), t.indexOf("#") >= 0 && (t = t.split("#")[1]), t
                     },
                     i = (n = e.headers, r = "x-amzn-errortype", Object.keys(n).find((function(e) {
                         return e.toLowerCase() === r.toLowerCase()
                     })));
                 return void 0 !== i ? o(e.headers[i]) : void 0 !== t.code ? o(t.code) : void 0 !== t.__type ? o(t.__type) : ""
             };
-        var Jl = function() {
-            return Jl = Object.assign || function(e) {
+        var nc = function() {
+            return nc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Jl.apply(this, arguments)
+            }, nc.apply(this, arguments)
         };
 
-        function Kl(e, t, n, r) {
+        function rc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -61324,15 +61560,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Xl(e, t) {
+        function oc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61399,36 +61635,36 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var $l = {
+        var ic = {
                 name: "deserializerMiddleware",
                 step: "deserialize",
                 tags: ["DESERIALIZER"],
                 override: !0
             },
-            ec = {
+            ac = {
                 name: "serializerMiddleware",
                 step: "serialize",
                 tags: ["SERIALIZER"],
                 override: !0
             };
 
-        function tc(e, t, n) {
+        function sc(e, t, n) {
             return {
                 applyToStack: function(r) {
                     r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return Kl(void 0, void 0, void 0, (function() {
+                                return rc(void 0, void 0, void 0, (function() {
                                     var o, i;
-                                    return Xl(this, (function(a) {
+                                    return oc(this, (function(a) {
                                         switch (a.label) {
                                             case 0:
                                                 return [4, n(r)];
                                             case 1:
                                                 return o = a.sent().response, [4, t(o, e)];
                                             case 2:
                                                 return i = a.sent(), [2, {
@@ -61436,45 +61672,45 @@
                                                     output: i
                                                 }]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, n), $l), r.add(function(e, t) {
+                    }(e, n), ic), r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return Kl(void 0, void 0, void 0, (function() {
+                                return rc(void 0, void 0, void 0, (function() {
                                     var o;
-                                    return Xl(this, (function(i) {
+                                    return oc(this, (function(i) {
                                         switch (i.label) {
                                             case 0:
                                                 return [4, t(r.input, e)];
                                             case 1:
-                                                return o = i.sent(), [2, n(Jl(Jl({}, r), {
+                                                return o = i.sent(), [2, n(nc(nc({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, t), ec)
+                    }(e, t), ac)
                 }
             }
         }
-        var nc = function() {
-            return nc = Object.assign || function(e) {
+        var uc = function() {
+            return uc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, nc.apply(this, arguments)
+            }, uc.apply(this, arguments)
         };
 
-        function rc(e) {
+        function lc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -61482,15 +61718,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function oc(e, t) {
+        function cc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61504,75 +61740,75 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function ic() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(oc(arguments[t]));
+        function dc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(cc(arguments[t]));
             return e
         }
-        var ac = function e() {
+        var fc = function e() {
                 var t = [],
                     n = [],
                     r = new Set,
                     o = function(e) {
                         return t.forEach((function(t) {
-                            e.add(t.middleware, nc({}, t))
+                            e.add(t.middleware, uc({}, t))
                         })), n.forEach((function(t) {
-                            e.addRelativeTo(t.middleware, nc({}, t))
+                            e.addRelativeTo(t.middleware, uc({}, t))
                         })), e
                     },
                     i = function e(t) {
                         var n = [];
                         return t.before.forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, ic(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, dc(e(t)))
                         })), n.push(t), t.after.reverse().forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, ic(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, dc(e(t)))
                         })), n
                     },
                     a = function() {
                         var e = [],
                             r = [],
                             o = {};
                         t.forEach((function(t) {
-                            var n = nc(nc({}, t), {
+                            var n = uc(uc({}, t), {
                                 before: [],
                                 after: []
                             });
                             n.name && (o[n.name] = n), e.push(n)
                         })), n.forEach((function(e) {
-                            var t = nc(nc({}, e), {
+                            var t = uc(uc({}, e), {
                                 before: [],
                                 after: []
                             });
                             t.name && (o[t.name] = t), r.push(t)
                         })), r.forEach((function(e) {
                             if (e.toMiddleware) {
                                 var t = o[e.toMiddleware];
                                 if (void 0 === t) throw new Error(e.toMiddleware + " is not found when adding " + (e.name || "anonymous") + " middleware " + e.relation + " " + e.toMiddleware);
                                 "after" === e.relation && t.after.push(e), "before" === e.relation && t.before.push(e)
                             }
                         }));
                         var a, s = (a = e, a.sort((function(e, t) {
-                            return sc[t.step] - sc[e.step] || uc[t.priority || "normal"] - uc[e.priority || "normal"]
+                            return pc[t.step] - pc[e.step] || hc[t.priority || "normal"] - hc[e.priority || "normal"]
                         }))).map(i).reduce((function(e, t) {
-                            return e.push.apply(e, ic(t)), e
+                            return e.push.apply(e, dc(t)), e
                         }), []);
                         return s.map((function(e) {
                             return e.middleware
                         }))
                     },
                     s = {
                         add: function(e, n) {
                             void 0 === n && (n = {});
                             var o = n.name,
                                 i = n.override,
-                                a = nc({
+                                a = uc({
                                     step: "initialize",
                                     priority: "normal",
                                     middleware: e
                                 }, n);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
@@ -61586,15 +61822,15 @@
                                 r.add(o)
                             }
                             t.push(a)
                         },
                         addRelativeTo: function(e, t) {
                             var o = t.name,
                                 i = t.override,
-                                a = nc({
+                                a = uc({
                                     middleware: e
                                 }, t);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
                                     var s = n.findIndex((function(e) {
                                             return e.name === o
@@ -61641,15 +61877,15 @@
                             var n = o(e());
                             return n.use(t), n
                         },
                         applyToStack: o,
                         resolve: function(e, t) {
                             var n, r;
                             try {
-                                for (var o = rc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = lc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
                                     e = (0, i.value)(e, t)
                                 }
                             } catch (s) {
                                 n = {
                                     error: s
                                 }
                             } finally {
@@ -61660,29 +61896,29 @@
                                 }
                             }
                             return e
                         }
                     };
                 return s
             },
-            sc = {
+            pc = {
                 initialize: 5,
                 serialize: 4,
                 build: 3,
                 finalizeRequest: 2,
                 deserialize: 1
             },
-            uc = {
+            hc = {
                 high: 3,
                 normal: 2,
                 low: 1
             },
-            lc = function() {
+            gc = function() {
                 function e(e) {
-                    this.middlewareStack = ac(), this.config = e
+                    this.middlewareStack = fc(), this.config = e
                 }
                 return e.prototype.send = function(e, t, n) {
                     var r = "function" !== typeof t ? t : void 0,
                         o = "function" === typeof t ? t : n,
                         i = e.resolveMiddleware(this.middlewareStack, this.config, r);
                     if (!o) return i(e).then((function(e) {
                         return e.output
@@ -61692,29 +61928,29 @@
                     }), (function(e) {
                         return o(e)
                     })).catch((function() {}))
                 }, e.prototype.destroy = function() {
                     this.config.requestHandler.destroy && this.config.requestHandler.destroy()
                 }, e
             }(),
-            cc = function() {
-                this.middlewareStack = ac()
+            yc = function() {
+                this.middlewareStack = fc()
             },
-            dc = function(e, t) {
-                return dc = Object.setPrototypeOf || {
+            mc = function(e, t) {
+                return mc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, dc(e, t)
+                }, mc(e, t)
             };
 
-        function fc(e, t) {
+        function vc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61728,225 +61964,225 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function pc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(fc(arguments[t]));
+        function Mc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(vc(arguments[t]));
             return e
         }
-        var hc = function() {
+        var bc = function() {
             var e = Object.getPrototypeOf(this).constructor,
-                t = Function.bind.apply(String, pc([null], arguments)),
+                t = Function.bind.apply(String, Mc([null], arguments)),
                 n = new t;
             return Object.setPrototypeOf(n, e.prototype), n
         };
-        hc.prototype = Object.create(String.prototype, {
+        bc.prototype = Object.create(String.prototype, {
             constructor: {
-                value: hc,
+                value: bc,
                 enumerable: !1,
                 writable: !0,
                 configurable: !0
             }
-        }), Object.setPrototypeOf(hc, String);
+        }), Object.setPrototypeOf(bc, String);
         ! function(e) {
             function t() {
                 return null !== e && e.apply(this, arguments) || this
             }(function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                dc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                mc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             })(t, e), t.prototype.deserializeJSON = function() {
                 return JSON.parse(e.prototype.toString.call(this))
             }, t.prototype.toJSON = function() {
                 return e.prototype.toString.call(this)
             }, t.fromObject = function(e) {
                 return e instanceof t ? e : new t(e instanceof String || "string" === typeof e ? e : JSON.stringify(e))
             }
-        }(hc);
-        var gc = function(e) {
+        }(bc);
+        var wc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return su(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(tc(t, this.serialize, this.deserialize));
+                return pu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(sc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetCredentialsForIdentityCommand",
-                            inputFilterSensitiveLog: _u.filterSensitiveLog,
-                            outputFilterSensitiveLog: Au.filterSensitiveLog
+                            inputFilterSensitiveLog: Pu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Bu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return lu(void 0, void 0, void 0, (function() {
+                        return gu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return cu(this, (function(o) {
+                            return yu(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetCredentialsForIdentity"
-                                }, r = JSON.stringify(Cl(e, t)), [2, Zl(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(zl(e, t)), [2, $l(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return lu(void 0, void 0, void 0, (function() {
+                        return gu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return cu(this, (function(i) {
+                            return yu(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, Ml(e, t)] : [4, Vl(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, Il(e, t)] : [4, ec(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Ol(n, t), o = uu({
-                                            $metadata: Wl(e)
+                                        return n = i.sent(), r = Fl(n, t), o = hu({
+                                            $metadata: Kl(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(cc),
-            yc = function(e, t) {
-                return yc = Object.setPrototypeOf || {
+            }(yc),
+            jc = function(e, t) {
+                return jc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, yc(e, t)
+                }, jc(e, t)
             };
-        var mc = function(e) {
+        var xc = function(e) {
             function t(t, n) {
                 void 0 === n && (n = !0);
                 var r = e.call(this, t) || this;
                 return r.tryNextLink = n, r
             }
             return function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                yc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                jc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             }(t, e), t
         }(Error);
 
-        function vc(e) {
+        function Nc(e) {
             return Promise.all(Object.keys(e).reduce((function(t, n) {
                 var r = e[n];
                 return "string" === typeof r ? t.push([n, r]) : t.push(r().then((function(e) {
                     return [n, e]
                 }))), t
             }), [])).then((function(e) {
                 return e.reduce((function(e, t) {
-                    var n = iu(t, 2),
+                    var n = du(t, 2),
                         r = n[0],
                         o = n[1];
                     return e[r] = o, e
                 }), {})
             }))
         }
 
-        function Mc(e) {
+        function Ic(e) {
             var t = this;
             return function() {
-                return ru(t, void 0, void 0, (function() {
+                return lu(t, void 0, void 0, (function() {
                     var t, n, r, o, i, a, s, u, l, c, d, f, p;
-                    return ou(this, (function(h) {
+                    return cu(this, (function(h) {
                         switch (h.label) {
                             case 0:
-                                return c = (l = e.client).send, d = gc.bind, p = {
+                                return c = (l = e.client).send, d = wc.bind, p = {
                                     CustomRoleArn: e.customRoleArn,
                                     IdentityId: e.identityId
-                                }, e.logins ? [4, vc(e.logins)] : [3, 2];
+                                }, e.logins ? [4, Nc(e.logins)] : [3, 2];
                             case 1:
                                 return f = h.sent(), [3, 3];
                             case 2:
                                 f = void 0, h.label = 3;
                             case 3:
-                                return [4, c.apply(l, [new(d.apply(gc, [void 0, (p.Logins = f, p)]))])];
+                                return [4, c.apply(l, [new(d.apply(wc, [void 0, (p.Logins = f, p)]))])];
                             case 4:
                                 return t = h.sent().Credentials, n = void 0 === t ? function() {
-                                    throw new mc("Response from Amazon Cognito contained no credentials")
+                                    throw new xc("Response from Amazon Cognito contained no credentials")
                                 }() : t, r = n.AccessKeyId, o = void 0 === r ? function() {
-                                    throw new mc("Response from Amazon Cognito contained no access key ID")
+                                    throw new xc("Response from Amazon Cognito contained no access key ID")
                                 }() : r, i = n.Expiration, a = n.SecretKey, s = void 0 === a ? function() {
-                                    throw new mc("Response from Amazon Cognito contained no secret key")
+                                    throw new xc("Response from Amazon Cognito contained no secret key")
                                 }() : a, u = n.SessionToken, [2, {
                                     identityId: e.identityId,
                                     accessKeyId: o,
                                     secretAccessKey: s,
                                     sessionToken: u,
                                     expiration: i
                                 }]
                         }
                     }))
                 }))
             }
         }
-        var bc = function(e) {
+        var Dc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return su(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(tc(t, this.serialize, this.deserialize));
+                return pu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(sc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetIdCommand",
-                            inputFilterSensitiveLog: zu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Uu.filterSensitiveLog
+                            inputFilterSensitiveLog: Yu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Qu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return lu(void 0, void 0, void 0, (function() {
+                        return gu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return cu(this, (function(o) {
+                            return yu(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetId"
-                                }, r = JSON.stringify(El(e, t)), [2, Zl(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(Ul(e, t)), [2, $l(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return lu(void 0, void 0, void 0, (function() {
+                        return gu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return cu(this, (function(i) {
+                            return yu(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, bl(e, t)] : [4, Vl(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, Dl(e, t)] : [4, ec(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = zl(n, t), o = uu({
-                                            $metadata: Wl(e)
+                                        return n = i.sent(), r = Yl(n, t), o = hu({
+                                            $metadata: Kl(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(cc),
-            wc = "IdentityIds",
-            jc = function() {
+            }(yc),
+            Sc = "IdentityIds",
+            Lc = function() {
                 function e(e) {
                     void 0 === e && (e = "aws:cognito-identity-ids"), this.dbName = e
                 }
                 return e.prototype.getItem = function(e) {
                     return this.withObjectStore("readonly", (function(t) {
                         var n = t.get(e);
                         return new Promise((function(e) {
@@ -61993,106 +62229,106 @@
                             n(e.error)
                         }, e.onblocked = function() {
                             n(new Error("Unable to access DB"))
                         }, e.onupgradeneeded = function() {
                             var t = e.result;
                             t.onerror = function() {
                                 n(new Error("Failed to create object store"))
-                            }, t.createObjectStore(wc, {
+                            }, t.createObjectStore(Sc, {
                                 keyPath: "id"
                             })
                         }
                     }))
                 }, e.prototype.withObjectStore = function(e, t) {
                     return this.getDb().then((function(n) {
-                        var r = n.transaction(wc, e);
+                        var r = n.transaction(Sc, e);
                         return r.oncomplete = function() {
                             return n.close()
                         }, new Promise((function(e, n) {
                             r.onerror = function() {
                                 return n(r.error)
-                            }, e(t(r.objectStore(wc)))
+                            }, e(t(r.objectStore(Sc)))
                         })).catch((function(e) {
                             throw n.close(), e
                         }))
                     }))
                 }, e
             }(),
-            xc = new(function() {
+            kc = new(function() {
                 function e(e) {
                     void 0 === e && (e = {}), this.store = e
                 }
                 return e.prototype.getItem = function(e) {
                     return e in this.store ? this.store[e] : null
                 }, e.prototype.removeItem = function(e) {
                     delete this.store[e]
                 }, e.prototype.setItem = function(e, t) {
                     this.store[e] = t
                 }, e
             }());
 
-        function Nc(e) {
+        function Cc(e) {
             var t = this,
                 n = e.accountId,
                 r = e.cache,
-                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new jc : "object" === typeof window && window.localStorage ? window.localStorage : xc : r,
+                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new Lc : "object" === typeof window && window.localStorage ? window.localStorage : kc : r,
                 i = e.client,
                 a = e.customRoleArn,
                 s = e.identityPoolId,
                 u = e.logins,
                 l = e.userIdentifier,
                 c = void 0 === l ? u && 0 !== Object.keys(u).length ? void 0 : "ANONYMOUS" : l,
                 d = c ? "aws:cognito-identity-credentials:" + s + ":" + c : void 0,
                 f = function() {
-                    return ru(t, void 0, void 0, (function() {
+                    return lu(t, void 0, void 0, (function() {
                         var e, t, r, l, c, p, h, g, y;
-                        return ou(this, (function(m) {
+                        return cu(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return (t = d) ? [4, o.getItem(d)] : [3, 2];
                                 case 1:
                                     t = m.sent(), m.label = 2;
                                 case 2:
-                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = bc.bind, y = {
+                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = Dc.bind, y = {
                                         AccountId: n,
                                         IdentityPoolId: s
-                                    }, u ? [4, vc(u)] : [3, 4]);
+                                    }, u ? [4, Nc(u)] : [3, 4]);
                                 case 3:
                                     return g = m.sent(), [3, 5];
                                 case 4:
                                     g = void 0, m.label = 5;
                                 case 5:
-                                    return [4, p.apply(c, [new(h.apply(bc, [void 0, (y.Logins = g, y)]))])];
+                                    return [4, p.apply(c, [new(h.apply(Dc, [void 0, (y.Logins = g, y)]))])];
                                 case 6:
                                     r = m.sent().IdentityId, l = void 0 === r ? function() {
-                                        throw new mc("Response from Amazon Cognito contained no identity ID")
+                                        throw new xc("Response from Amazon Cognito contained no identity ID")
                                     }() : r, e = l, d && Promise.resolve(o.setItem(d, e)).catch((function() {})), m.label = 7;
                                 case 7:
-                                    return [2, (f = Mc({
+                                    return [2, (f = Ic({
                                         client: i,
                                         customRoleArn: a,
                                         logins: u,
                                         identityId: e
                                     }))()]
                             }
                         }))
                     }))
                 };
             return function() {
                 return f().catch((function(e) {
-                    return ru(t, void 0, void 0, (function() {
-                        return ou(this, (function(t) {
+                    return lu(t, void 0, void 0, (function() {
+                        return cu(this, (function(t) {
                             throw d && Promise.resolve(o.removeItem(d)).catch((function() {})), e
                         }))
                     }))
                 }))
             }
         }
-        var Ic = new As("Parser"),
-            Dc = function(e) {
+        var Ec = new Bs("Parser"),
+            _c = function(e) {
                 var t, n = {};
                 if (e.aws_mobile_analytics_app_id) {
                     var r = {
                         AWSPinpoint: {
                             appId: e.aws_mobile_analytics_app_id,
                             region: e.aws_mobile_analytics_app_region
                         }
@@ -62109,23 +62345,23 @@
                     signUpVerificationMethod: e.aws_cognito_sign_up_verification_method || "code"
                 }), t = e.aws_user_files_s3_bucket ? {
                     AWSS3: {
                         bucket: e.aws_user_files_s3_bucket,
                         region: e.aws_user_files_s3_bucket_region,
                         dangerouslyConnectToHttpEndpointForTesting: e.aws_user_files_s3_dangerously_connect_to_http_endpoint_for_testing
                     }
-                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = Ds(Ds({}, e.Logging), {
+                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = _s(_s({}, e.Logging), {
                     region: e.aws_project_region
                 })), e.geo && (n.Geo = Object.assign({}, e.geo), e.geo.amazon_location_service && (n.Geo = {
                     AmazonLocationService: e.geo.amazon_location_service
-                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), Ic.debug("parse config", e, "to amplifyconfig", n), n
+                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), Ec.debug("parse config", e, "to amplifyconfig", n), n
             },
-            Sc = __webpack_require__(3219);
+            Tc = __webpack_require__(3219);
 
-        function Lc(e, t, n, r) {
+        function Ac(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62145,15 +62381,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function kc(e, t) {
+        function Oc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62221,15 +62457,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Cc(e) {
+        function zc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62237,36 +62473,36 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Ec(e) {
+        function Uc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
                         value: e && e[r++],
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
-        var _c = function(e) {
-                return encodeURIComponent(e).replace(/[!'()*]/g, Tc)
+        var Pc = function(e) {
+                return encodeURIComponent(e).replace(/[!'()*]/g, Rc)
             },
-            Tc = function(e) {
+            Rc = function(e) {
                 return "%" + e.charCodeAt(0).toString(16).toUpperCase()
             };
-        for (var Ac = function() {
+        for (var Bc = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).requestTimeout;
                     this.requestTimeout = t
                 }
                 return e.prototype.destroy = function() {}, e.prototype.handle = function(e, t) {
                     var n = (void 0 === t ? {} : t).abortSignal,
                         r = this.requestTimeout;
@@ -62275,22 +62511,22 @@
                         return o.name = "AbortError", Promise.reject(o)
                     }
                     var i = e.path;
                     if (e.query) {
                         var a = function(e) {
                             var t, n, r = [];
                             try {
-                                for (var o = Ec(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = Uc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
                                     var a = i.value,
                                         s = e[a];
-                                    if (a = _c(a), Array.isArray(s))
-                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + _c(s[u]));
+                                    if (a = Pc(a), Array.isArray(s))
+                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Pc(s[u]));
                                     else {
                                         var c = a;
-                                        (s || "string" === typeof s) && (c += "=" + _c(s)), r.push(c)
+                                        (s || "string" === typeof s) && (c += "=" + Pc(s)), r.push(c)
                                     }
                                 }
                             } catch (d) {
                                 t = {
                                     error: d
                                 }
                             } finally {
@@ -62314,15 +62550,15 @@
                         };
                     "undefined" !== typeof AbortController && (c.signal = n);
                     var d, f = new Request(l, c),
                         p = [fetch(f).then((function(e) {
                             var t, n, r = e.headers,
                                 o = {};
                             try {
-                                for (var i = Cc(r.entries()), a = i.next(); !a.done; a = i.next()) {
+                                for (var i = zc(r.entries()), a = i.next(); !a.done; a = i.next()) {
                                     var s = a.value;
                                     o[s[0]] = s[1]
                                 }
                             } catch (u) {
                                 t = {
                                     error: u
                                 }
@@ -62330,22 +62566,22 @@
                                 try {
                                     a && !a.done && (n = i.return) && n.call(i)
                                 } finally {
                                     if (t) throw t.error
                                 }
                             }
                             return void 0 !== e.body ? {
-                                response: new gl({
+                                response: new wl({
                                     headers: o,
                                     statusCode: e.status,
                                     body: e.body
                                 })
                             } : e.blob().then((function(t) {
                                 return {
-                                    response: new gl({
+                                    response: new wl({
                                         headers: o,
                                         statusCode: e.status,
                                         body: t
                                     })
                                 }
                             }))
                         })), (d = r, void 0 === d && (d = 0), new Promise((function(e, t) {
@@ -62357,46 +62593,46 @@
                     return n && p.push(new Promise((function(e, t) {
                         n.onabort = function() {
                             var e = new Error("Request aborted");
                             e.name = "AbortError", t(e)
                         }
                     }))), Promise.race(p)
                 }, e
-            }(), Oc = {}, zc = new Array(64), Uc = 0, Pc = "A".charCodeAt(0), Rc = "Z".charCodeAt(0); Uc + Pc <= Rc; Uc++) {
-            var Bc = String.fromCharCode(Uc + Pc);
-            Oc[Bc] = Uc, zc[Uc] = Bc
-        }
-        for (Uc = 0, Pc = "a".charCodeAt(0), Rc = "z".charCodeAt(0); Uc + Pc <= Rc; Uc++) {
-            Bc = String.fromCharCode(Uc + Pc);
-            var Fc = Uc + 26;
-            Oc[Bc] = Fc, zc[Fc] = Bc
-        }
-        for (Uc = 0; Uc < 10; Uc++) {
-            Oc[Uc.toString(10)] = Uc + 52;
-            Bc = Uc.toString(10), Fc = Uc + 52;
-            Oc[Bc] = Fc, zc[Fc] = Bc
+            }(), Fc = {}, Yc = new Array(64), Qc = 0, Gc = "A".charCodeAt(0), Wc = "Z".charCodeAt(0); Qc + Gc <= Wc; Qc++) {
+            var Hc = String.fromCharCode(Qc + Gc);
+            Fc[Hc] = Qc, Yc[Qc] = Hc
+        }
+        for (Qc = 0, Gc = "a".charCodeAt(0), Wc = "z".charCodeAt(0); Qc + Gc <= Wc; Qc++) {
+            Hc = String.fromCharCode(Qc + Gc);
+            var Zc = Qc + 26;
+            Fc[Hc] = Zc, Yc[Zc] = Hc
+        }
+        for (Qc = 0; Qc < 10; Qc++) {
+            Fc[Qc.toString(10)] = Qc + 52;
+            Hc = Qc.toString(10), Zc = Qc + 52;
+            Fc[Hc] = Zc, Yc[Zc] = Hc
         }
-        Oc["+"] = 62, zc[62] = "+", Oc["/"] = 63, zc[63] = "/";
+        Fc["+"] = 62, Yc[62] = "+", Fc["/"] = 63, Yc[63] = "/";
 
-        function Yc(e) {
+        function Vc(e) {
             var t = e.length / 4 * 3;
             "==" === e.substr(-2) ? t -= 2 : "=" === e.substr(-1) && t--;
             for (var n = new ArrayBuffer(t), r = new DataView(n), o = 0; o < e.length; o += 4) {
-                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Oc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
+                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Fc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
                 var l = o / 4 * 3;
                 i >>= a % 8;
                 for (var c = Math.floor(a / 8), d = 0; d < c; d++) {
                     var f = 8 * (c - d - 1);
                     r.setUint8(l + d, (i & 255 << f) >> f)
                 }
             }
             return new Uint8Array(n)
         }
 
-        function Qc(e) {
+        function qc(e) {
             return new Promise((function(t, n) {
                 var r = new FileReader;
                 r.onloadend = function() {
                     var e;
                     if (2 !== r.readyState) return n(new Error("Reader aborted too early"));
                     var o = null !== (e = r.result) && void 0 !== e ? e : "",
                         i = o.indexOf(","),
@@ -62405,23 +62641,23 @@
                 }, r.onabort = function() {
                     return n(new Error("Read aborted"))
                 }, r.onerror = function() {
                     return n(r.error)
                 }, r.readAsDataURL(e)
             }))
         }
-        var Gc = function() {
-            return Gc = Object.assign || function(e) {
+        var Jc = function() {
+            return Jc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Gc.apply(this, arguments)
+            }, Jc.apply(this, arguments)
         };
 
-        function Wc(e, t, n, r) {
+        function Kc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62441,15 +62677,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Hc(e, t) {
+        function Xc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62517,15 +62753,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Zc(e, t) {
+        function $c(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62538,65 +62774,65 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Vc = function(e) {
+        var ed = function(e) {
                 return function(t, n) {
                     return function(r) {
-                        return Wc(void 0, void 0, void 0, (function() {
+                        return Kc(void 0, void 0, void 0, (function() {
                             var o;
-                            return Hc(this, (function(i) {
+                            return Xc(this, (function(i) {
                                 return (null === (o = null === e || void 0 === e ? void 0 : e.retryStrategy) || void 0 === o ? void 0 : o.mode) && (n.userAgent = function() {
-                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Zc(arguments[t]));
+                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat($c(arguments[t]));
                                     return e
                                 }(n.userAgent || [], [
                                     ["cfg/retry-mode", e.retryStrategy.mode]
                                 ])), [2, e.retryStrategy.retry(t, r)]
                             }))
                         }))
                     }
                 }
             },
-            qc = {
+            td = {
                 name: "retryMiddleware",
                 tags: ["RETRY"],
                 step: "finalizeRequest",
                 priority: "high",
                 override: !0
             },
-            Jc = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
-            Kc = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
-            Xc = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
-            $c = [500, 502, 503, 504],
-            ed = function(e) {
+            nd = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
+            rd = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
+            od = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
+            id = [500, 502, 503, 504],
+            ad = function(e) {
                 var t, n;
-                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || Kc.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
+                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || rd.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
             },
-            td = __webpack_require__(6231),
-            nd = function(e, t) {
+            sd = __webpack_require__(6231),
+            ud = function(e, t) {
                 return Math.floor(Math.min(2e4, Math.random() * Math.pow(2, t) * e))
             },
-            rd = function(e) {
+            ld = function(e) {
                 return !!e && (function(e) {
                     return void 0 !== e.$retryable
                 }(e) || function(e) {
-                    return Jc.includes(e.name)
-                }(e) || ed(e) || function(e) {
+                    return nd.includes(e.name)
+                }(e) || ad(e) || function(e) {
                     var t;
-                    return Xc.includes(e.name) || $c.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
+                    return od.includes(e.name) || id.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
                 }(e))
             },
-            od = "standard",
-            id = function() {
+            cd = "standard",
+            dd = function() {
                 function e(e, t) {
                     var n, r, o;
-                    this.maxAttemptsProvider = e, this.mode = od, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : rd, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : nd, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
+                    this.maxAttemptsProvider = e, this.mode = cd, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : ld, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : ud, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
                         var t = e,
                             n = e,
                             r = function(e) {
                                 return "TimeoutError" === e.name ? 10 : 5
                             },
                             o = function(e) {
                                 return r(e) <= n
@@ -62613,52 +62849,52 @@
                             }
                         })
                     }(500)
                 }
                 return e.prototype.shouldRetry = function(e, t, n) {
                     return t < n && this.retryDecider(e) && this.retryQuota.hasRetryTokens(e)
                 }, e.prototype.getMaxAttempts = function() {
-                    return Wc(this, void 0, void 0, (function() {
+                    return Kc(this, void 0, void 0, (function() {
                         var e;
-                        return Hc(this, (function(t) {
+                        return Xc(this, (function(t) {
                             switch (t.label) {
                                 case 0:
                                     return t.trys.push([0, 2, , 3]), [4, this.maxAttemptsProvider()];
                                 case 1:
                                     return e = t.sent(), [3, 3];
                                 case 2:
                                     return t.sent(), e = 3, [3, 3];
                                 case 3:
                                     return [2, e]
                             }
                         }))
                     }))
                 }, e.prototype.retry = function(e, t) {
-                    return Wc(this, void 0, void 0, (function() {
+                    return Kc(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l;
-                        return Hc(this, (function(c) {
+                        return Xc(this, (function(c) {
                             switch (c.label) {
                                 case 0:
                                     return r = 0, o = 0, [4, this.getMaxAttempts()];
                                 case 1:
-                                    i = c.sent(), a = t.request, vl.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, td.v4)()), s = function() {
+                                    i = c.sent(), a = t.request, Nl.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, sd.v4)()), s = function() {
                                         var s, l, c, d, f;
-                                        return Hc(this, (function(p) {
+                                        return Xc(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
-                                                    return p.trys.push([0, 2, , 5]), vl.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
+                                                    return p.trys.push([0, 2, , 5]), Nl.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
                                                 case 1:
                                                     return s = p.sent(), l = s.response, c = s.output, u.retryQuota.releaseRetryTokens(n), c.$metadata.attempts = r + 1, c.$metadata.totalRetryDelay = o, [2, {
                                                         value: {
                                                             response: l,
                                                             output: c
                                                         }
                                                     }];
                                                 case 2:
-                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(ed(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
+                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(ad(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
                                                         return setTimeout(e, f)
                                                     }))]) : [3, 4];
                                                 case 3:
                                                     return p.sent(), [2, "continue"];
                                                 case 4:
                                                     throw d.$metadata || (d.$metadata = {}), d.$metadata.attempts = r, d.$metadata.totalRetryDelay = o, d;
                                                 case 5:
@@ -62673,25 +62909,25 @@
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e
             }(),
-            ad = function(e) {
+            fd = function(e) {
                 if (void 0 === e && (e = 3), "number" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function sd(e, t, n, r) {
+        function pd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62711,15 +62947,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function ud(e, t) {
+        function hd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62786,25 +63022,25 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var ld = __webpack_require__(984),
-            cd = __webpack_require__.n(ld),
-            dd = __webpack_require__(5863),
-            fd = "cognito-identity.{region}.amazonaws.com",
-            pd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
-            hd = new Set(["cn-north-1", "cn-northwest-1"]),
-            gd = new Set(["us-iso-east-1"]),
-            yd = new Set(["us-isob-east-1"]),
-            md = new Set(["us-gov-east-1", "us-gov-west-1"]);
+        var gd = __webpack_require__(984),
+            yd = __webpack_require__.n(gd),
+            md = __webpack_require__(5863),
+            vd = "cognito-identity.{region}.amazonaws.com",
+            Md = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
+            bd = new Set(["cn-north-1", "cn-northwest-1"]),
+            wd = new Set(["us-iso-east-1"]),
+            jd = new Set(["us-isob-east-1"]),
+            xd = new Set(["us-gov-east-1", "us-gov-west-1"]);
 
-        function vd(e) {
+        function Nd(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62812,15 +63048,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Md(e, t) {
+        function Id(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62833,15 +63069,15 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var bd, wd = {
+        var Dd, Sd = {
                 apiVersion: "2014-06-30",
                 disableHostPrefix: !1,
                 logger: {},
                 regionInfoProvider: function(e, t) {
                     var n = void 0;
                     switch (e) {
                         case "ap-northeast-1":
@@ -62977,51 +63213,51 @@
                         case "us-west-2":
                             n = {
                                 hostname: "cognito-identity.us-west-2.amazonaws.com",
                                 partition: "aws"
                             };
                             break;
                         default:
-                            pd.has(e) && (n = {
-                                hostname: fd.replace("{region}", e),
+                            Md.has(e) && (n = {
+                                hostname: vd.replace("{region}", e),
                                 partition: "aws"
-                            }), hd.has(e) && (n = {
+                            }), bd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com.cn".replace("{region}", e),
                                 partition: "aws-cn"
-                            }), gd.has(e) && (n = {
+                            }), wd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.c2s.ic.gov".replace("{region}", e),
                                 partition: "aws-iso"
-                            }), yd.has(e) && (n = {
+                            }), jd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.sc2s.sgov.gov".replace("{region}", e),
                                 partition: "aws-iso-b"
-                            }), md.has(e) && (n = {
+                            }), xd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com".replace("{region}", e),
                                 partition: "aws-us-gov"
                             }), void 0 === n && (n = {
-                                hostname: fd.replace("{region}", e),
+                                hostname: vd.replace("{region}", e),
                                 partition: "aws"
                             })
                     }
-                    return Promise.resolve(uu({
+                    return Promise.resolve(hu({
                         signingService: "cognito-identity"
                     }, n))
                 },
                 serviceId: "Cognito Identity",
                 urlParser: function(e) {
                     var t, n = new URL(e),
                         r = n.hostname,
                         o = n.pathname,
                         i = n.port,
                         a = n.protocol,
                         s = n.search;
                     return s && (t = function(e) {
                         var t, n, r = {};
                         if (e = e.replace(/^\?/, "")) try {
-                            for (var o = vd(e.split("&")), i = o.next(); !i.done; i = o.next()) {
-                                var a = Md(i.value.split("="), 2),
+                            for (var o = Nd(e.split("&")), i = o.next(); !i.done; i = o.next()) {
+                                var a = Id(i.value.split("="), 2),
                                     s = a[0],
                                     u = a[1],
                                     l = void 0 === u ? null : u;
                                 s = decodeURIComponent(s), l && (l = decodeURIComponent(l)), s in r ? Array.isArray(r[s]) ? r[s].push(l) : r[s] = [r[s], l] : r[s] = l
                             }
                         } catch (c) {
                             t = {
@@ -63040,25 +63276,25 @@
                         port: i ? parseInt(i) : void 0,
                         protocol: a,
                         path: o,
                         query: t
                     }
                 }
             },
-            jd = uu(uu({}, wd), {
+            Ld = hu(hu({}, Sd), {
                 runtime: "browser",
-                base64Decoder: Yc,
+                base64Decoder: Vc,
                 base64Encoder: function(e) {
                     for (var t = "", n = 0; n < e.length; n += 3) {
                         for (var r = 0, o = 0, i = n, a = Math.min(n + 3, e.length); i < a; i++) r |= e[i] << 8 * (a - i - 1), o += 8;
                         var s = Math.ceil(o / 6);
                         r <<= 6 * s - o;
                         for (var u = 1; u <= s; u++) {
                             var l = 6 * (s - u);
-                            t += zc[(r & 63 << l) >> l]
+                            t += Yc[(r & 63 << l) >> l]
                         }
                         t += "==".slice(0, 4 - s)
                     }
                     return t
                 },
                 bodyLengthChecker: function(e) {
                     if ("string" === typeof e) {
@@ -63075,79 +63311,79 @@
                         return Promise.reject(new Error("Credential is missing"))
                     }
                 },
                 defaultUserAgentProvider: function(e) {
                     var t = e.serviceId,
                         n = e.clientVersion;
                     return function() {
-                        return sd(void 0, void 0, void 0, (function() {
+                        return pd(void 0, void 0, void 0, (function() {
                             var e, r, o, i, a, s, u, l, c;
-                            return ud(this, (function(d) {
-                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? cd().parse(window.navigator.userAgent) : void 0, r = [
+                            return hd(this, (function(d) {
+                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? yd().parse(window.navigator.userAgent) : void 0, r = [
                                     ["aws-sdk-js", n],
                                     ["os/" + ((null === (i = null === e || void 0 === e ? void 0 : e.os) || void 0 === i ? void 0 : i.name) || "other"), null === (a = null === e || void 0 === e ? void 0 : e.os) || void 0 === a ? void 0 : a.version],
                                     ["lang/js"],
                                     ["md/browser", (null !== (u = null === (s = null === e || void 0 === e ? void 0 : e.browser) || void 0 === s ? void 0 : s.name) && void 0 !== u ? u : "unknown") + "_" + (null !== (c = null === (l = null === e || void 0 === e ? void 0 : e.browser) || void 0 === l ? void 0 : l.version) && void 0 !== c ? c : "unknown")]
                                 ], t && r.push(["api/" + t, n]), [2, r]
                             }))
                         }))
                     }
                 }({
-                    serviceId: wd.serviceId,
+                    serviceId: Sd.serviceId,
                     clientVersion: "3.6.1"
                 }),
                 maxAttempts: 3,
-                region: (bd = "Region is missing", function() {
-                    return Promise.reject(bd)
+                region: (Dd = "Region is missing", function() {
+                    return Promise.reject(Dd)
                 }),
-                requestHandler: new Ac,
-                sha256: Sc.Sha256,
+                requestHandler: new Bc,
+                sha256: Tc.Sha256,
                 streamCollector: function(e) {
                     return "function" === typeof Blob && e instanceof Blob ? function(e) {
-                        return Lc(this, void 0, void 0, (function() {
+                        return Ac(this, void 0, void 0, (function() {
                             var t, n;
-                            return kc(this, (function(r) {
+                            return Oc(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
-                                        return [4, Qc(e)];
+                                        return [4, qc(e)];
                                     case 1:
-                                        return t = r.sent(), n = Yc(t), [2, new Uint8Array(n)]
+                                        return t = r.sent(), n = Vc(t), [2, new Uint8Array(n)]
                                 }
                             }))
                         }))
                     }(e) : function(e) {
-                        return Lc(this, void 0, void 0, (function() {
+                        return Ac(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s;
-                            return kc(this, (function(u) {
+                            return Oc(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
                                         t = new Uint8Array(0), n = e.getReader(), r = !1, u.label = 1;
                                     case 1:
                                         return r ? [3, 3] : [4, n.read()];
                                     case 2:
                                         return o = u.sent(), i = o.done, (a = o.value) && (s = t, (t = new Uint8Array(s.length + a.length)).set(s), t.set(a, s.length)), r = i, [3, 1];
                                     case 3:
                                         return [2, t]
                                 }
                             }))
                         }))
                     }(e)
                 },
-                utf8Decoder: dd.fromUtf8,
-                utf8Encoder: dd.toUtf8
+                utf8Decoder: md.fromUtf8,
+                utf8Encoder: md.toUtf8
             });
-        var xd = function() {
-            return xd = Object.assign || function(e) {
+        var kd = function() {
+            return kd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, xd.apply(this, arguments)
+            }, kd.apply(this, arguments)
         };
 
-        function Nd(e, t, n, r) {
+        function Cd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63167,15 +63403,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Id(e, t) {
+        function Ed(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63242,15 +63478,15 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Dd = function(e) {
+        var _d = function(e) {
                 var t = e.endpoint,
                     n = e.urlParser;
                 if ("string" === typeof t) {
                     var r = Promise.resolve(n(t));
                     return function() {
                         return r
                     }
@@ -63259,49 +63495,49 @@
                     var o = Promise.resolve(t);
                     return function() {
                         return o
                     }
                 }
                 return t
             },
-            Sd = function(e) {
-                return Nd(void 0, void 0, void 0, (function() {
+            Td = function(e) {
+                return Cd(void 0, void 0, void 0, (function() {
                     var t, n, r, o, i;
-                    return Id(this, (function(a) {
+                    return Ed(this, (function(a) {
                         switch (a.label) {
                             case 0:
                                 return t = e.tls, n = void 0 === t || t, [4, e.region()];
                             case 1:
                                 if (r = a.sent(), !new RegExp(/^([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]{0,61}[a-zA-Z0-9])$/).test(r)) throw new Error("Invalid region in client config");
                                 return [4, e.regionInfoProvider(r)];
                             case 2:
                                 if (!(o = (null !== (i = a.sent()) && void 0 !== i ? i : {}).hostname)) throw new Error("Cannot resolve hostname from client config");
                                 return [2, e.urlParser((n ? "https:" : "http:") + "//" + o)]
                         }
                     }))
                 }))
             },
-            Ld = function(e) {
+            Ad = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
-        var kd = function() {
-            return kd = Object.assign || function(e) {
+        var Od = function() {
+            return Od = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, kd.apply(this, arguments)
+            }, Od.apply(this, arguments)
         };
 
-        function Cd(e, t, n, r) {
+        function zd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63321,15 +63557,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Ed(e, t) {
+        function Ud(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63396,46 +63632,46 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var _d = "content-length";
-        var Td = {
+        var Pd = "content-length";
+        var Rd = {
                 step: "build",
                 tags: ["SET_CONTENT_LENGTH", "CONTENT_LENGTH"],
                 name: "contentLengthMiddleware",
                 override: !0
             },
-            Ad = function(e) {
+            Bd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             var t = this;
                             return function(n) {
                                 return function(r) {
-                                    return Cd(t, void 0, void 0, (function() {
+                                    return zd(t, void 0, void 0, (function() {
                                         var t, o, i, a, s;
-                                        return Ed(this, (function(u) {
-                                            return t = r.request, vl.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
+                                        return Ud(this, (function(u) {
+                                            return t = r.request, Nl.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
                                                 return e.toLowerCase()
-                                            })).indexOf(_d) && void 0 !== (a = e(o)) && (t.headers = kd(kd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(kd(kd({}, r), {
+                                            })).indexOf(Pd) && void 0 !== (a = e(o)) && (t.headers = Od(Od({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(Od(Od({}, r), {
                                                 request: t
                                             }))]
                                         }))
                                     }))
                                 }
                             }
-                        }(e.bodyLengthChecker), Td)
+                        }(e.bodyLengthChecker), Rd)
                     }
                 }
             };
 
-        function Od(e, t, n, r) {
+        function Fd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63455,15 +63691,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function zd(e, t) {
+        function Yd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63530,41 +63766,41 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Ud = {
+        var Qd = {
                 name: "hostHeaderMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["HOST"],
                 override: !0
             },
-            Pd = function(e) {
+            Gd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             return function(t) {
                                 return function(n) {
-                                    return Od(void 0, void 0, void 0, (function() {
+                                    return Fd(void 0, void 0, void 0, (function() {
                                         var r, o;
-                                        return zd(this, (function(i) {
-                                            return vl.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
+                                        return Yd(this, (function(i) {
+                                            return Nl.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
                                         }))
                                     }))
                                 }
                             }
-                        }(e), Ud)
+                        }(e), Qd)
                     }
                 }
             };
 
-        function Rd(e, t, n, r) {
+        function Wd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63584,15 +63820,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Bd(e, t) {
+        function Hd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63659,20 +63895,20 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Fd = function() {
+        var Zd = function() {
                 return function(e, t) {
                     return function(n) {
-                        return Rd(void 0, void 0, void 0, (function() {
+                        return Wd(void 0, void 0, void 0, (function() {
                             var r, o, i, a, s, u, l, c, d;
-                            return Bd(this, (function(f) {
+                            return Hd(this, (function(f) {
                                 switch (f.label) {
                                     case 0:
                                         return r = t.clientName, o = t.commandName, i = t.inputFilterSensitiveLog, a = t.logger, s = t.outputFilterSensitiveLog, [4, e(n)];
                                     case 1:
                                         return u = f.sent(), a ? ("function" === typeof a.info && (l = u.output, c = l.$metadata, d = function(e, t) {
                                             var n = {};
                                             for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
@@ -63690,29 +63926,29 @@
                                         })), [2, u]) : [2, u]
                                 }
                             }))
                         }))
                     }
                 }
             },
-            Yd = {
+            Vd = {
                 name: "loggerMiddleware",
                 tags: ["LOGGER"],
                 step: "initialize",
                 override: !0
             };
-        var Qd = function() {
-            return Qd = Object.assign || function(e) {
+        var qd = function() {
+            return qd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Qd.apply(this, arguments)
+            }, qd.apply(this, arguments)
         };
 
-        function Gd(e, t, n, r) {
+        function Jd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63732,15 +63968,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Wd(e, t) {
+        function Kd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63808,15 +64044,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Hd(e, t) {
+        function Xd(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63829,23 +64065,23 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Zd = function() {
-            return Zd = Object.assign || function(e) {
+        var $d = function() {
+            return $d = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Zd.apply(this, arguments)
+            }, $d.apply(this, arguments)
         };
 
-        function Vd(e, t, n, r) {
+        function ef(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63865,15 +64101,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function qd(e, t) {
+        function tf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63941,15 +64177,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Jd(e) {
+        function nf(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -63957,15 +64193,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Kd(e, t) {
+        function rf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63978,33 +64214,33 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        for (var Xd = {}, $d = {}, ef = 0; ef < 256; ef++) {
-            var tf = ef.toString(16).toLowerCase();
-            1 === tf.length && (tf = "0" + tf), Xd[ef] = tf, $d[tf] = ef
+        for (var of = {}, af = {}, sf = 0; sf < 256; sf++) {
+            var uf = sf.toString(16).toLowerCase();
+            1 === uf.length && (uf = "0" + uf), of [sf] = uf, af[uf] = sf
         }
 
-        function nf(e) {
-            for (var t = "", n = 0; n < e.byteLength; n++) t += Xd[e[n]];
+        function lf(e) {
+            for (var t = "", n = 0; n < e.byteLength; n++) t += of [e[n]];
             return t
         }
-        var rf = "X-Amz-Date",
-            of = "X-Amz-Signature",
-            af = "X-Amz-Security-Token",
-            sf = "authorization",
-            uf = rf.toLowerCase(),
-            lf = [sf, uf, "date"],
-            cf = of.toLowerCase(),
-            df = "x-amz-content-sha256",
-            ff = af.toLowerCase(),
-            pf = {
+        var cf = "X-Amz-Date",
+            df = "X-Amz-Signature",
+            ff = "X-Amz-Security-Token",
+            pf = "authorization",
+            hf = cf.toLowerCase(),
+            gf = [pf, hf, "date"],
+            yf = df.toLowerCase(),
+            mf = "x-amz-content-sha256",
+            vf = ff.toLowerCase(),
+            Mf = {
                 authorization: !0,
                 "cache-control": !0,
                 connection: !0,
                 expect: !0,
                 from: !0,
                 "keep-alive": !0,
                 "max-forwards": !0,
@@ -64013,39 +64249,39 @@
                 te: !0,
                 trailer: !0,
                 "transfer-encoding": !0,
                 upgrade: !0,
                 "user-agent": !0,
                 "x-amzn-trace-id": !0
             },
-            hf = /^proxy-/,
-            gf = /^sec-/,
-            yf = "AWS4-HMAC-SHA256",
-            mf = "AWS4-HMAC-SHA256-PAYLOAD",
-            vf = "aws4_request",
-            Mf = {},
-            bf = [];
+            bf = /^proxy-/,
+            wf = /^sec-/,
+            jf = "AWS4-HMAC-SHA256",
+            xf = "AWS4-HMAC-SHA256-PAYLOAD",
+            Nf = "aws4_request",
+            If = {},
+            Df = [];
 
-        function wf(e, t, n) {
-            return e + "/" + t + "/" + n + "/" + vf
+        function Sf(e, t, n) {
+            return e + "/" + t + "/" + n + "/" + Nf
         }
 
-        function jf(e, t, n) {
+        function Lf(e, t, n) {
             var r = new e(t);
             return r.update(n), r.digest()
         }
 
-        function xf(e, t, n) {
+        function kf(e, t, n) {
             var r, o, i = e.headers,
                 a = {};
             try {
-                for (var s = Jd(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
+                for (var s = nf(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
                     var l = u.value,
                         c = l.toLowerCase();
-                    (c in pf || (null === t || void 0 === t ? void 0 : t.has(c)) || hf.test(c) || gf.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
+                    (c in Mf || (null === t || void 0 === t ? void 0 : t.has(c)) || bf.test(c) || wf.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
                 }
             } catch (d) {
                 r = {
                     error: d
                 }
             } finally {
                 try {
@@ -64053,84 +64289,84 @@
                 } finally {
                     if (r) throw r.error
                 }
             }
             return a
         }
 
-        function Nf(e, t) {
+        function Cf(e, t) {
             var n = e.headers,
                 r = e.body;
-            return Vd(this, void 0, void 0, (function() {
+            return ef(this, void 0, void 0, (function() {
                 var e, o, i, a, s, u, l;
-                return qd(this, (function(c) {
+                return tf(this, (function(c) {
                     switch (c.label) {
                         case 0:
                             try {
-                                for (e = Jd(Object.keys(n)), o = e.next(); !o.done; o = e.next())
-                                    if ((i = o.value).toLowerCase() === df) return [2, n[i]]
+                                for (e = nf(Object.keys(n)), o = e.next(); !o.done; o = e.next())
+                                    if ((i = o.value).toLowerCase() === mf) return [2, n[i]]
                             } catch (f) {
                                 u = {
                                     error: f
                                 }
                             } finally {
                                 try {
                                     o && !o.done && (l = e.return) && l.call(e)
                                 } finally {
                                     if (u) throw u.error
                                 }
                             }
                             return void 0 != r ? [3, 1] : [2, "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"];
                         case 1:
-                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = nf, [4, a.digest()]) : [3, 3];
+                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = lf, [4, a.digest()]) : [3, 3];
                         case 2:
                             return [2, s.apply(void 0, [c.sent()])];
                         case 3:
                             return [2, "UNSIGNED-PAYLOAD"]
                     }
                     var d
                 }))
             }))
         }
 
-        function If(e) {
+        function Ef(e) {
             var t = e.headers,
                 n = e.query,
                 r = function(e, t) {
                     var n = {};
                     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
                     if (null != e && "function" === typeof Object.getOwnPropertySymbols) {
                         var o = 0;
                         for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                     }
                     return n
                 }(e, ["headers", "query"]);
-            return Zd(Zd({}, r), {
-                headers: Zd({}, t),
-                query: n ? Df(n) : void 0
+            return $d($d({}, r), {
+                headers: $d({}, t),
+                query: n ? _f(n) : void 0
             })
         }
 
-        function Df(e) {
+        function _f(e) {
             return Object.keys(e).reduce((function(t, n) {
                 var r, o = e[n];
-                return Zd(Zd({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
-                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Kd(arguments[t]));
+                return $d($d({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
+                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(rf(arguments[t]));
                     return e
                 }(o) : o, r))
             }), {})
         }
 
-        function Sf(e) {
+        function Tf(e) {
             var t, n;
-            e = "function" === typeof e.clone ? e.clone() : If(e);
+            e = "function" === typeof e.clone ? e.clone() : Ef(e);
             try {
-                for (var r = Jd(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
+                for (var r = nf(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
                     var i = o.value;
-                    lf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
+                    gf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
                 }
             } catch (a) {
                 t = {
                     error: a
                 }
             } finally {
                 try {
@@ -64138,55 +64374,55 @@
                 } finally {
                     if (t) throw t.error
                 }
             }
             return e
         }
 
-        function Lf(e) {
+        function Af(e) {
             return function(e) {
                 if ("number" === typeof e) return new Date(1e3 * e);
                 if ("string" === typeof e) return Number(e) ? new Date(1e3 * Number(e)) : new Date(e);
                 return e
             }(e).toISOString().replace(/\.\d{3}Z$/, "Z")
         }
-        var kf = function() {
+        var Of = function() {
                 function e(e) {
                     var t = e.applyChecksum,
                         n = e.credentials,
                         r = e.region,
                         o = e.service,
                         i = e.sha256,
                         a = e.uriEscapePath,
                         s = void 0 === a || a;
-                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = _f(r), this.credentialProvider = Tf(n)
+                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Pf(r), this.credentialProvider = Rf(n)
                 }
                 return e.prototype.presign = function(e, t) {
-                    return void 0 === t && (t = {}), Vd(this, void 0, void 0, (function() {
+                    return void 0 === t && (t = {}), ef(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I;
-                        return qd(this, (function(D) {
+                        return tf(this, (function(D) {
                             switch (D.label) {
                                 case 0:
                                     return n = t.signingDate, r = void 0 === n ? new Date : n, o = t.expiresIn, i = void 0 === o ? 3600 : o, a = t.unsignableHeaders, s = t.unhoistableHeaders, u = t.signableHeaders, l = t.signingRegion, c = t.signingService, [4, this.credentialProvider()];
                                 case 1:
                                     return d = D.sent(), null === l || void 0 === l ? [3, 2] : (p = l, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     p = D.sent(), D.label = 4;
                                 case 4:
-                                    return f = p, h = Cf(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = wf(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
+                                    return f = p, h = zf(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = Sf(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
                                         var n, r, o;
                                         void 0 === t && (t = {});
-                                        var i = "function" === typeof e.clone ? e.clone() : If(e),
+                                        var i = "function" === typeof e.clone ? e.clone() : Ef(e),
                                             a = i.headers,
                                             s = i.query,
                                             u = void 0 === s ? {} : s;
                                         try {
-                                            for (var l = Jd(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
+                                            for (var l = nf(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
                                                 var d = c.value,
                                                     f = d.toLowerCase();
                                                 "x-amz-" !== f.substr(0, 6) || (null === (o = t.unhoistableHeaders) || void 0 === o ? void 0 : o.has(f)) || (u[d] = a[d], delete a[d])
                                             }
                                         } catch (p) {
                                             n = {
                                                 error: p
@@ -64194,159 +64430,159 @@
                                         } finally {
                                             try {
                                                 c && !c.done && (r = l.return) && r.call(l)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
-                                        return Zd(Zd({}, e), {
+                                        return $d($d({}, e), {
                                             headers: a,
                                             query: u
                                         })
-                                    }(Sf(e), {
+                                    }(Tf(e), {
                                         unhoistableHeaders: s
-                                    }), d.sessionToken && (v.query[af] = d.sessionToken), v.query["X-Amz-Algorithm"] = yf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = xf(v, a, u), v.query["X-Amz-SignedHeaders"] = Ef(M), b = v.query, w = of, j = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Nf(e, this.sha256)]);
+                                    }), d.sessionToken && (v.query[ff] = d.sessionToken), v.query["X-Amz-Algorithm"] = jf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = kf(v, a, u), v.query["X-Amz-SignedHeaders"] = Uf(M), b = v.query, w = df, j = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Cf(e, this.sha256)]);
                                 case 5:
                                     return [4, j.apply(this, x.concat([N.apply(this, I.concat([D.sent()]))]))];
                                 case 6:
                                     return b[w] = D.sent(), [2, v]
                             }
                         }))
                     }))
                 }, e.prototype.sign = function(e, t) {
-                    return Vd(this, void 0, void 0, (function() {
-                        return qd(this, (function(n) {
+                    return ef(this, void 0, void 0, (function() {
+                        return tf(this, (function(n) {
                             return "string" === typeof e ? [2, this.signString(e, t)] : e.headers && e.payload ? [2, this.signEvent(e, t)] : [2, this.signRequest(e, t)]
                         }))
                     }))
                 }, e.prototype.signEvent = function(e, t) {
                     var n = e.headers,
                         r = e.payload,
                         o = t.signingDate,
                         i = void 0 === o ? new Date : o,
                         a = t.priorSignature,
                         s = t.signingRegion,
                         u = t.signingService;
-                    return Vd(this, void 0, void 0, (function() {
+                    return ef(this, void 0, void 0, (function() {
                         var e, t, o, l, c, d, f, p, h, g, y;
-                        return qd(this, (function(m) {
+                        return tf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return null === s || void 0 === s ? [3, 1] : (t = s, [3, 3]);
                                 case 1:
                                     return [4, this.regionProvider()];
                                 case 2:
                                     t = m.sent(), m.label = 3;
                                 case 3:
-                                    return e = t, o = Cf(i), l = o.shortDate, c = o.longDate, d = wf(l, e, null !== u && void 0 !== u ? u : this.service), [4, Nf({
+                                    return e = t, o = zf(i), l = o.shortDate, c = o.longDate, d = Sf(l, e, null !== u && void 0 !== u ? u : this.service), [4, Cf({
                                         headers: {},
                                         body: r
                                     }, this.sha256)];
                                 case 4:
-                                    return f = m.sent(), (p = new this.sha256).update(n), g = nf, [4, p.digest()];
+                                    return f = m.sent(), (p = new this.sha256).update(n), g = lf, [4, p.digest()];
                                 case 5:
-                                    return h = g.apply(void 0, [m.sent()]), y = [mf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
+                                    return h = g.apply(void 0, [m.sent()]), y = [xf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
                                         signingDate: i,
                                         signingRegion: e,
                                         signingService: u
                                     })]
                             }
                         }))
                     }))
                 }, e.prototype.signString = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signingRegion,
                         a = n.signingService;
-                    return Vd(this, void 0, void 0, (function() {
+                    return ef(this, void 0, void 0, (function() {
                         var t, n, r, s, u, l, c, d;
-                        return qd(this, (function(f) {
+                        return tf(this, (function(f) {
                             switch (f.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = f.sent(), null === i || void 0 === i ? [3, 2] : (r = i, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = f.sent(), f.label = 4;
                                 case 4:
-                                    return n = r, s = Cf(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
+                                    return n = r, s = zf(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
                                 case 5:
-                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = nf, [4, u.digest()];
+                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = lf, [4, u.digest()];
                                 case 6:
                                     return [2, d.apply(void 0, [f.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.signRequest = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signableHeaders,
                         a = n.unsignableHeaders,
                         s = n.signingRegion,
                         u = n.signingService;
-                    return Vd(this, void 0, void 0, (function() {
+                    return ef(this, void 0, void 0, (function() {
                         var t, n, r, l, c, d, f, p, h, g, y;
-                        return qd(this, (function(m) {
+                        return tf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = m.sent(), null === s || void 0 === s ? [3, 2] : (r = s, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = m.sent(), m.label = 4;
                                 case 4:
-                                    return n = r, l = Sf(e), c = Cf(o), d = c.longDate, f = c.shortDate, p = wf(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[uf] = d, t.sessionToken && (l.headers[ff] = t.sessionToken), [4, Nf(l, this.sha256)];
+                                    return n = r, l = Tf(e), c = zf(o), d = c.longDate, f = c.shortDate, p = Sf(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[hf] = d, t.sessionToken && (l.headers[vf] = t.sessionToken), [4, Cf(l, this.sha256)];
                                 case 5:
                                     return h = m.sent(), ! function(e, t) {
                                         var n, r;
                                         e = e.toLowerCase();
                                         try {
-                                            for (var o = Jd(Object.keys(t)), i = o.next(); !i.done; i = o.next())
+                                            for (var o = nf(Object.keys(t)), i = o.next(); !i.done; i = o.next())
                                                 if (e === i.value.toLowerCase()) return !0
                                         } catch (a) {
                                             n = {
                                                 error: a
                                             }
                                         } finally {
                                             try {
                                                 i && !i.done && (r = o.return) && r.call(o)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
                                         return !1
-                                    }(df, l.headers) && this.applyChecksum && (l.headers[df] = h), g = xf(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
+                                    }(mf, l.headers) && this.applyChecksum && (l.headers[mf] = h), g = kf(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
                                 case 6:
-                                    return y = m.sent(), l.headers[sf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Ef(g) + ", Signature=" + y, [2, l]
+                                    return y = m.sent(), l.headers[pf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Uf(g) + ", Signature=" + y, [2, l]
                             }
                         }))
                     }))
                 }, e.prototype.createCanonicalRequest = function(e, t, n) {
                     var r = Object.keys(t).sort();
                     return e.method + "\n" + this.getCanonicalPath(e) + "\n" + function(e) {
                         var t, n, r = e.query,
                             o = void 0 === r ? {} : r,
                             i = [],
                             a = {},
                             s = function(e) {
-                                if (e.toLowerCase() === cf) return "continue";
+                                if (e.toLowerCase() === yf) return "continue";
                                 i.push(e);
                                 var t = o[e];
-                                "string" === typeof t ? a[e] = _c(e) + "=" + _c(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
-                                    return t.concat([_c(e) + "=" + _c(n)])
+                                "string" === typeof t ? a[e] = Pc(e) + "=" + Pc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
+                                    return t.concat([Pc(e) + "=" + Pc(n)])
                                 }), []).join("&"))
                             };
                         try {
-                            for (var u = Jd(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
+                            for (var u = nf(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
                         } catch (c) {
                             t = {
                                 error: c
                             }
                         } finally {
                             try {
                                 l && !l.done && (n = u.return) && n.call(u)
@@ -64359,60 +64595,60 @@
                         })).filter((function(e) {
                             return e
                         })).join("&")
                     }(e) + "\n" + r.map((function(e) {
                         return e + ":" + t[e]
                     })).join("\n") + "\n\n" + r.join(";") + "\n" + n
                 }, e.prototype.createStringToSign = function(e, t, n) {
-                    return Vd(this, void 0, void 0, (function() {
+                    return ef(this, void 0, void 0, (function() {
                         var r, o;
-                        return qd(this, (function(i) {
+                        return tf(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return (r = new this.sha256).update(n), [4, r.digest()];
                                 case 1:
-                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + nf(o)]
+                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + lf(o)]
                             }
                         }))
                     }))
                 }, e.prototype.getCanonicalPath = function(e) {
                     var t = e.path;
                     return this.uriEscapePath ? "/" + encodeURIComponent(t.replace(/^\//, "")).replace(/%2F/g, "/") : t
                 }, e.prototype.getSignature = function(e, t, n, r) {
-                    return Vd(this, void 0, void 0, (function() {
+                    return ef(this, void 0, void 0, (function() {
                         var o, i, a, s, u;
-                        return qd(this, (function(l) {
+                        return tf(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return [4, this.createStringToSign(e, t, r)];
                                 case 1:
                                     return o = l.sent(), s = (a = this.sha256).bind, [4, n];
                                 case 2:
-                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = nf, [4, i.digest()];
+                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = lf, [4, i.digest()];
                                 case 3:
                                     return [2, u.apply(void 0, [l.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.getSigningKey = function(e, t, n, r) {
                     return function(e, t, n, r, o) {
-                        return Vd(void 0, void 0, void 0, (function() {
+                        return ef(void 0, void 0, void 0, (function() {
                             var i, a, s, u, l, c, d, f, p;
-                            return qd(this, (function(h) {
+                            return tf(this, (function(h) {
                                 switch (h.label) {
                                     case 0:
-                                        return [4, jf(e, t.secretAccessKey, t.accessKeyId)];
+                                        return [4, Lf(e, t.secretAccessKey, t.accessKeyId)];
                                     case 1:
-                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + nf(i) + ":" + t.sessionToken) in Mf) return [2, Mf[a]];
-                                        for (bf.push(a); bf.length > 50;) delete Mf[bf.shift()];
+                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + lf(i) + ":" + t.sessionToken) in If) return [2, If[a]];
+                                        for (Df.push(a); Df.length > 50;) delete If[Df.shift()];
                                         s = "AWS4" + t.secretAccessKey, h.label = 2;
                                     case 2:
-                                        h.trys.push([2, 7, 8, 9]), u = Jd([n, r, o, vf]), l = u.next(), h.label = 3;
+                                        h.trys.push([2, 7, 8, 9]), u = nf([n, r, o, Nf]), l = u.next(), h.label = 3;
                                     case 3:
-                                        return l.done ? [3, 6] : (c = l.value, [4, jf(e, s, c)]);
+                                        return l.done ? [3, 6] : (c = l.value, [4, Lf(e, s, c)]);
                                     case 4:
                                         s = h.sent(), h.label = 5;
                                     case 5:
                                         return l = u.next(), [3, 3];
                                     case 6:
                                         return [3, 9];
                                     case 7:
@@ -64423,68 +64659,68 @@
                                         try {
                                             l && !l.done && (p = u.return) && p.call(u)
                                         } finally {
                                             if (f) throw f.error
                                         }
                                         return [7];
                                     case 9:
-                                        return [2, Mf[a] = s]
+                                        return [2, If[a] = s]
                                 }
                             }))
                         }))
                     }(this.sha256, e, n, t, r || this.service)
                 }, e
             }(),
-            Cf = function(e) {
-                var t = Lf(e).replace(/[\-:]/g, "");
+            zf = function(e) {
+                var t = Af(e).replace(/[\-:]/g, "");
                 return {
                     longDate: t,
                     shortDate: t.substr(0, 8)
                 }
             },
-            Ef = function(e) {
+            Uf = function(e) {
                 return Object.keys(e).sort().join(";")
             },
-            _f = function(e) {
+            Pf = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             },
-            Tf = function(e) {
+            Rf = function(e) {
                 if ("object" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function Af(e) {
+        function Bf(e) {
             if ("object" === typeof e) {
                 var t = Promise.resolve(e);
                 return function() {
                     return t
                 }
             }
             return e
         }
-        var Of = function() {
-            return Of = Object.assign || function(e) {
+        var Ff = function() {
+            return Ff = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Of.apply(this, arguments)
+            }, Ff.apply(this, arguments)
         };
 
-        function zf(e, t, n, r) {
+        function Yf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64504,15 +64740,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Uf(e, t) {
+        function Qf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64580,15 +64816,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Pf(e, t) {
+        function Gf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64602,213 +64838,213 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Rf() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Pf(arguments[t]));
+        function Wf() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Gf(arguments[t]));
             return e
         }
-        var Bf = "user-agent",
-            Ff = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
-            Yf = function(e) {
-                var t = Pf(e, 2),
+        var Hf = "user-agent",
+            Zf = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
+            Vf = function(e) {
+                var t = Gf(e, 2),
                     n = t[0],
                     r = t[1],
                     o = n.indexOf("/"),
                     i = n.substring(0, o),
                     a = n.substring(o + 1);
                 return "api" === i && (a = a.toLowerCase()), [i, a, r].filter((function(e) {
                     return e && e.length > 0
                 })).map((function(e) {
-                    return null === e || void 0 === e ? void 0 : e.replace(Ff, "_")
+                    return null === e || void 0 === e ? void 0 : e.replace(Zf, "_")
                 })).join("/")
             },
-            Qf = {
+            qf = {
                 name: "getUserAgentMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["SET_USER_AGENT", "USER_AGENT"],
                 override: !0
             },
-            Gf = function(e) {
+            Jf = function(e) {
                 return {
                     applyToStack: function(t) {
                         var n;
                         t.add((n = e, function(e, t) {
                             return function(r) {
-                                return zf(void 0, void 0, void 0, (function() {
+                                return Yf(void 0, void 0, void 0, (function() {
                                     var o, i, a, s, u, l, c, d;
-                                    return Uf(this, (function(f) {
+                                    return Qf(this, (function(f) {
                                         switch (f.label) {
                                             case 0:
-                                                return o = r.request, vl.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(Yf)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
+                                                return o = r.request, Nl.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(Vf)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
                                             case 1:
-                                                return s = f.sent().map(Yf), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(Yf)) || [], i["x-amz-user-agent"] = Rf(s, a, u).join(" "), l = Rf(s.filter((function(e) {
+                                                return s = f.sent().map(Vf), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(Vf)) || [], i["x-amz-user-agent"] = Wf(s, a, u).join(" "), l = Wf(s.filter((function(e) {
                                                     return e.startsWith("aws-sdk-")
-                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Bf] = i[Bf] ? i[Bf] + " " + l : l), [2, e(Of(Of({}, r), {
+                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Hf] = i[Hf] ? i[Hf] + " " + l : l), [2, e(Ff(Ff({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
-                        }), Qf)
+                        }), qf)
                     }
                 }
             },
-            Wf = function(e) {
+            Kf = function(e) {
                 function t(t) {
                     var n, r, o = this,
                         i = function(e) {
                             if (!e.region) throw new Error("Region is missing");
-                            return xd(xd({}, e), {
-                                region: Ld(e.region)
+                            return kd(kd({}, e), {
+                                region: Ad(e.region)
                             })
-                        }(uu(uu({}, jd), t)),
+                        }(hu(hu({}, Ld), t)),
                         a = function(e) {
                             var t;
-                            return xd(xd({}, e), {
+                            return kd(kd({}, e), {
                                 tls: null === (t = e.tls) || void 0 === t || t,
-                                endpoint: e.endpoint ? Dd(e) : function() {
-                                    return Sd(e)
+                                endpoint: e.endpoint ? _d(e) : function() {
+                                    return Td(e)
                                 },
                                 isCustomEndpoint: !!e.endpoint
                             })
                         }(i),
                         s = function(e) {
                             var t, n = this,
-                                r = Af(e.credentials || e.credentialDefaultProvider(e)),
+                                r = Bf(e.credentials || e.credentialDefaultProvider(e)),
                                 o = e.signingEscapePath,
                                 i = void 0 === o || o,
                                 a = e.systemClockOffset,
                                 s = void 0 === a ? e.systemClockOffset || 0 : a,
                                 u = e.sha256;
-                            return t = e.signer ? Af(e.signer) : function() {
-                                return Af(e.region)().then((function(t) {
-                                    return Gd(n, void 0, void 0, (function() {
-                                        return Wd(this, (function(n) {
+                            return t = e.signer ? Bf(e.signer) : function() {
+                                return Bf(e.region)().then((function(t) {
+                                    return Jd(n, void 0, void 0, (function() {
+                                        return Kd(this, (function(n) {
                                             switch (n.label) {
                                                 case 0:
                                                     return [4, e.regionInfoProvider(t)];
                                                 case 1:
                                                     return [2, [n.sent() || {}, t]]
                                             }
                                         }))
                                     }))
                                 })).then((function(t) {
-                                    var n = Hd(t, 2),
+                                    var n = Xd(t, 2),
                                         o = n[0],
                                         a = n[1],
                                         s = o.signingRegion,
                                         l = o.signingService;
-                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new kf({
+                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new Of({
                                         credentials: r,
                                         region: e.signingRegion,
                                         service: e.signingName,
                                         sha256: u,
                                         uriEscapePath: i
                                     })
                                 }))
-                            }, Qd(Qd({}, e), {
+                            }, qd(qd({}, e), {
                                 systemClockOffset: s,
                                 signingEscapePath: i,
                                 credentials: r,
                                 signer: t
                             })
                         }(a),
                         u = function(e) {
-                            var t = ad(e.maxAttempts);
-                            return Gc(Gc({}, e), {
+                            var t = fd(e.maxAttempts);
+                            return Jc(Jc({}, e), {
                                 maxAttempts: t,
-                                retryStrategy: e.retryStrategy || new id(t)
+                                retryStrategy: e.retryStrategy || new dd(t)
                             })
                         }(s),
-                        l = Of(Of({}, n = u), {
+                        l = Ff(Ff({}, n = u), {
                             customUserAgent: "string" === typeof n.customUserAgent ? [
                                 [n.customUserAgent]
                             ] : n.customUserAgent
                         });
                     return (o = e.call(this, l) || this).config = l, o.middlewareStack.use((r = o.config, {
                         applyToStack: function(e) {
-                            e.add(Vc(r), qc)
+                            e.add(ed(r), td)
                         }
-                    })), o.middlewareStack.use(Ad(o.config)), o.middlewareStack.use(Pd(o.config)), o.middlewareStack.use((o.config, {
+                    })), o.middlewareStack.use(Bd(o.config)), o.middlewareStack.use(Gd(o.config)), o.middlewareStack.use((o.config, {
                         applyToStack: function(e) {
-                            e.add(Fd(), Yd)
+                            e.add(Zd(), Vd)
                         }
-                    })), o.middlewareStack.use(Gf(o.config)), o
+                    })), o.middlewareStack.use(Jf(o.config)), o
                 }
-                return su(t, e), t.prototype.destroy = function() {
+                return pu(t, e), t.prototype.destroy = function() {
                     e.prototype.destroy.call(this)
                 }, t
-            }(lc),
-            Hf = "aws-amplify/5.0.10",
-            Zf = {
-                userAgent: Hf + " js",
+            }(gc),
+            Xf = "aws-amplify/5.0.10",
+            $f = {
+                userAgent: Xf + " js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (Zf.product = navigator.product || "", Zf.navigator = navigator || null, "ReactNative" === navigator.product) Zf.userAgent = Hf + " react-native", Zf.isReactNative = !0;
-            else Zf.userAgent = Hf + " js", Zf.isReactNative = !1;
+            if ($f.product = navigator.product || "", $f.navigator = navigator || null, "ReactNative" === navigator.product) $f.userAgent = Xf + " react-native", $f.isReactNative = !0;
+            else $f.userAgent = Xf + " js", $f.isReactNative = !1;
 
-        function Vf(e) {
-            var t, n = new Wf({
+        function ep(e) {
+            var t, n = new Kf({
                 region: e.region,
-                customUserAgent: "" + Zf.userAgent + (t || "")
+                customUserAgent: "" + $f.userAgent + (t || "")
             });
             return n.middlewareStack.add((function(e, t) {
                 return function(t) {
                     return e(function(e) {
-                        return Ds(Ds({}, e), {
-                            request: Ds(Ds({}, e.request), {
-                                headers: Ds(Ds({}, e.request.headers), {
+                        return _s(_s({}, e), {
+                            request: _s(_s({}, e.request), {
+                                headers: _s(_s({}, e.request.headers), {
                                     "cache-control": "no-store"
                                 })
                             })
                         })
                     }(t))
                 }
             }), {
                 step: "build",
                 name: "cacheControlMiddleWare"
             }), n
         }
-        var qf = new As("Credentials"),
-            Jf = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            Kf = function() {
+        var tp = new Bs("Credentials"),
+            np = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            rp = function() {
                 function e(e) {
-                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = $s.refreshGoogleToken, this._refreshHandlers.facebook = eu.refreshFacebookToken
+                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = iu.refreshGoogleToken, this._refreshHandlers.facebook = au.refreshFacebookToken
                 }
                 return e.prototype.getModuleName = function() {
                     return "Credentials"
                 }, e.prototype.getCredSource = function() {
                     return this._credentials_source
                 }, e.prototype.configure = function(e) {
                     if (!e) return this._config || {};
                     this._config = Object.assign({}, this._config, e);
                     var t = this._config.refreshHandlers;
-                    return t && (this._refreshHandlers = Ds(Ds({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Fs).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
+                    return t && (this._refreshHandlers = _s(_s({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Zs).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
                         function(e, t, n) {
-                            Ps.dispatch("core", {
+                            Gs.dispatch("core", {
                                 event: e,
                                 data: t,
                                 message: n
-                            }, "Credentials", Jf)
+                            }, "Credentials", np)
                         }("credentials_configured", null, "Credentials has been configured successfully"), this._config
                 }, e.prototype.get = function() {
-                    return qf.debug("getting credentials"), this._pickupCredentials()
+                    return tp.debug("getting credentials"), this._pickupCredentials()
                 }, e.prototype._getCognitoIdentityIdStorageKey = function(e) {
                     return "CognitoIdentityId-" + e
                 }, e.prototype._pickupCredentials = function() {
-                    return qf.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? qf.debug("getting old cred promise") : (qf.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
+                    return tp.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? tp.debug("getting old cred promise") : (tp.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
                         if (e.isResolved) return e;
                         var t = !0,
                             n = !1,
                             r = !1,
                             o = e.then((function(e) {
                                 return r = !0, t = !1, e
                             }), (function(e) {
@@ -64819,152 +65055,152 @@
                         }, o.isPending = function() {
                             return t
                         }, o.isRejected = function() {
                             return n
                         }, o
                     }(this._keepAlive())), this._gettingCredPromise
                 }, e.prototype._keepAlive = function() {
-                    return Ss(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return Ls(this, (function(s) {
+                        return As(this, (function(s) {
                             switch (s.label) {
                                 case 0:
-                                    if (qf.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return qf.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
-                                    if (qf.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? nu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
+                                    if (tp.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return tp.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
+                                    if (tp.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? uu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
                                     if (this._isExpired(e) || !this._isPastTTL()) return [3, 6];
-                                    qf.debug("ttl has passed but token is not yet expired"), s.label = 1;
+                                    tp.debug("ttl has passed but token is not yet expired"), s.label = 1;
                                 case 1:
                                     return s.trys.push([1, 5, , 6]), [4, n.currentUserPoolUser()];
                                 case 2:
                                     return r = s.sent(), [4, n.currentSession()];
                                 case 3:
                                     return o = s.sent(), i = o.refreshToken, [4, new Promise((function(e, t) {
                                         r.refreshSession(i, (function(n, r) {
                                             return n ? t(n) : e(r)
                                         }))
                                     }))];
                                 case 4:
                                     return s.sent(), [3, 6];
                                 case 5:
-                                    return a = s.sent(), qf.debug("Error attempting to refreshing the session", a), [3, 6];
+                                    return a = s.sent(), tp.debug("Error attempting to refreshing the session", a), [3, 6];
                                 case 6:
                                     return [2, n.currentUserCredentials()]
                             }
                         }))
                     }))
                 }, e.prototype.refreshFederatedToken = function(e) {
-                    qf.debug("Getting federated credentials");
+                    tp.debug("Getting federated credentials");
                     var t = e.provider,
                         n = e.user,
                         r = e.token,
                         o = e.identity_id,
                         i = e.expires_at;
                     i = 1970 === new Date(i).getFullYear() ? 1e3 * i : i;
                     var a = this;
-                    return qf.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (qf.debug("token not expired"), this._setCredentialsFromFederation({
+                    return tp.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (tp.debug("token not expired"), this._setCredentialsFromFederation({
                         provider: t,
                         token: r,
                         user: n,
                         identity_id: o,
                         expires_at: i
-                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (qf.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
+                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (tp.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
                         refreshHandler: a._refreshHandlers[t],
                         provider: t,
                         user: n
-                    })) : (qf.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
+                    })) : (tp.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
                 }, e.prototype._providerRefreshWithRetry = function(e) {
                     var t = this,
                         n = e.refreshHandler,
                         r = e.provider,
                         o = e.user;
-                    return Hs(n, [], 1e4).then((function(e) {
-                        return qf.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
+                    return Xs(n, [], 1e4).then((function(e) {
+                        return tp.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
                             provider: r,
                             token: e.token,
                             user: o,
                             identity_id: e.identity_id,
                             expires_at: e.expires_at
                         })
                     })).catch((function(e) {
-                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), qf.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
+                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), tp.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
                     }))
                 }, e.prototype._isExpired = function(e) {
-                    if (!e) return qf.debug("no credentials for expiration check"), !0;
-                    qf.debug("are these credentials expired?", e);
+                    if (!e) return tp.debug("no credentials for expiration check"), !0;
+                    tp.debug("are these credentials expired?", e);
                     var t = Date.now();
                     return e.expiration.getTime() <= t
                 }, e.prototype._isPastTTL = function() {
                     return this._nextCredentialsRefresh <= Date.now()
                 }, e.prototype._setCredentialsForGuest = function() {
                     var e;
-                    return Ss(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d = this;
-                        return Ls(this, (function(f) {
+                        return As(this, (function(f) {
                             switch (f.label) {
                                 case 0:
-                                    return qf.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, Dc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (qf.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (qf.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
+                                    return tp.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, _c(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (tp.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (tp.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
                                 case 1:
-                                    return a = s._identityId = f.sent(), u = Vf({
+                                    return a = s._identityId = f.sent(), u = ep({
                                         region: i || r
-                                    }), l = void 0, a ? l = Mc({
+                                    }), l = void 0, a ? l = Ic({
                                         identityId: a,
                                         client: u
                                     })() : (c = function() {
-                                        return Ss(d, void 0, void 0, (function() {
+                                        return Ts(d, void 0, void 0, (function() {
                                             var e;
-                                            return Ls(this, (function(t) {
+                                            return As(this, (function(t) {
                                                 switch (t.label) {
                                                     case 0:
-                                                        return [4, u.send(new bc({
+                                                        return [4, u.send(new Dc({
                                                             IdentityPoolId: n
                                                         }))];
                                                     case 1:
-                                                        return e = t.sent().IdentityId, this._identityId = e, [2, Mc({
+                                                        return e = t.sent().IdentityId, this._identityId = e, [2, Ic({
                                                             client: u,
                                                             identityId: e
                                                         })()]
                                                 }
                                             }))
                                         }))
                                     }, l = c().catch((function(e) {
-                                        return Ss(d, void 0, void 0, (function() {
-                                            return Ls(this, (function(t) {
+                                        return Ts(d, void 0, void 0, (function() {
+                                            return As(this, (function(t) {
                                                 throw e
                                             }))
                                         }))
                                     }))), [2, this._loadCredentials(l, "guest", !1, null).then((function(e) {
                                         return e
                                     })).catch((function(e) {
-                                        return Ss(d, void 0, void 0, (function() {
+                                        return Ts(d, void 0, void 0, (function() {
                                             var t, r = this;
-                                            return Ls(this, (function(o) {
+                                            return As(this, (function(o) {
                                                 switch (o.label) {
                                                     case 0:
-                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (qf.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
+                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (tp.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
                                                     case 1:
                                                         return o.sent(), t = function() {
-                                                            return Ss(r, void 0, void 0, (function() {
+                                                            return Ts(r, void 0, void 0, (function() {
                                                                 var e;
-                                                                return Ls(this, (function(t) {
+                                                                return As(this, (function(t) {
                                                                     switch (t.label) {
                                                                         case 0:
-                                                                            return [4, u.send(new bc({
+                                                                            return [4, u.send(new Dc({
                                                                                 IdentityPoolId: n
                                                                             }))];
                                                                         case 1:
-                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, Mc({
+                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, Ic({
                                                                                 client: u,
                                                                                 identityId: e
                                                                             })()]
                                                                     }
                                                                 }))
                                                             }))
                                                         }, l = t().catch((function(e) {
-                                                            return Ss(r, void 0, void 0, (function() {
-                                                                return Ls(this, (function(t) {
+                                                            return Ts(r, void 0, void 0, (function() {
+                                                                return As(this, (function(t) {
                                                                     throw e
                                                                 }))
                                                             }))
                                                         })), [2, this._loadCredentials(l, "guest", !1, null)];
                                                     case 2:
                                                         return [2, e]
                                                 }
@@ -64987,191 +65223,191 @@
                     if (!o) return Promise.reject("You must specify a federated provider");
                     var i = {};
                     i[o] = n;
                     var a = this._config,
                         s = a.identityPoolId,
                         u = a.region,
                         l = a.identityPoolRegion;
-                    if (!s) return qf.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!l && !u) return qf.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
-                    var c = Vf({
+                    if (!s) return tp.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!l && !u) return tp.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    var c = ep({
                             region: l || u
                         }),
                         d = void 0;
-                    r ? d = Mc({
+                    r ? d = Ic({
                         identityId: r,
                         logins: i,
                         client: c
-                    })() : d = Nc({
+                    })() : d = Cc({
                         logins: i,
                         identityPoolId: s,
                         client: c
                     })();
                     return this._loadCredentials(d, "federated", !0, e)
                 }, e.prototype._setCredentialsFromSession = function(e) {
                     var t = this;
-                    qf.debug("set credentials from session");
+                    tp.debug("set credentials from session");
                     var n = e.getIdToken().getJwtToken(),
                         r = this._config,
                         o = r.region,
                         i = r.userPoolId,
                         a = r.identityPoolId,
                         s = r.identityPoolRegion;
-                    if (!a) return qf.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!s && !o) return qf.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    if (!a) return tp.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!s && !o) return tp.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                     var u = {};
                     u["cognito-idp." + o + ".amazonaws.com/" + i] = n;
-                    var l = Vf({
+                    var l = ep({
                             region: s || o
                         }),
-                        c = Ss(t, void 0, void 0, (function() {
+                        c = Ts(t, void 0, void 0, (function() {
                             var e, t, n, r, o, i, s, c, d, f;
-                            return Ls(this, (function(p) {
+                            return As(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
                                         return [4, this._getGuestIdentityId()];
                                     case 1:
-                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new bc({
+                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new Dc({
                                             IdentityPoolId: a,
                                             Logins: u
                                         }))];
                                     case 2:
                                         n = p.sent().IdentityId, t = n, p.label = 3;
                                     case 3:
-                                        return [4, l.send(new gc({
+                                        return [4, l.send(new wc({
                                             IdentityId: e || t,
                                             Logins: u
                                         }))];
                                     case 4:
-                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (qf.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && qf.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
+                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (tp.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && tp.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
                                     case 5:
                                         p.sent(), p.label = 6;
                                     case 6:
                                         return [2, {
                                             accessKeyId: i,
                                             secretAccessKey: c,
                                             sessionToken: d,
                                             expiration: s,
                                             identityId: f
                                         }]
                                 }
                             }))
                         })).catch((function(e) {
-                            return Ss(t, void 0, void 0, (function() {
-                                return Ls(this, (function(t) {
+                            return Ts(t, void 0, void 0, (function() {
+                                return As(this, (function(t) {
                                     throw e
                                 }))
                             }))
                         }));
                     return this._loadCredentials(c, "userPool", !0, null)
                 }, e.prototype._loadCredentials = function(e, t, n, r) {
                     var o = this,
                         i = this;
                     return new Promise((function(a, s) {
                         e.then((function(e) {
-                            return Ss(o, void 0, void 0, (function() {
+                            return Ts(o, void 0, void 0, (function() {
                                 var o, s, u, l, c;
-                                return Ls(this, (function(d) {
+                                return As(this, (function(d) {
                                     switch (d.label) {
                                         case 0:
-                                            if (qf.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
+                                            if (tp.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
                                                 o = Object.assign({
                                                     id: this._credentials.identityId
                                                 }, r.user), s = r.provider, u = r.token, l = r.expires_at, c = r.identity_id;
                                                 try {
                                                     this._storage.setItem("aws-amplify-federatedInfo", JSON.stringify({
                                                         provider: s,
                                                         token: u,
                                                         user: o,
                                                         expires_at: l,
                                                         identity_id: c
                                                     }))
                                                 } catch (f) {
-                                                    qf.debug("Failed to put federated info into auth storage", f)
+                                                    tp.debug("Failed to put federated info into auth storage", f)
                                                 }
                                             }
                                             return "guest" !== t ? [3, 2] : [4, this._setGuestIdentityId(e.identityId)];
                                         case 1:
                                             d.sent(), d.label = 2;
                                         case 2:
                                             return a(i._credentials), [2]
                                     }
                                 }))
                             }))
                         })).catch((function(t) {
-                            if (t) return qf.debug("Failed to load credentials", e), qf.debug("Error loading credentials", t), void s(t)
+                            if (t) return tp.debug("Failed to load credentials", e), tp.debug("Error loading credentials", t), void s(t)
                         }))
                     }))
                 }, e.prototype.set = function(e, t) {
-                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (qf.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
+                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (tp.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
                 }, e.prototype.clear = function() {
-                    return Ss(this, void 0, void 0, (function() {
-                        return Ls(this, (function(e) {
-                            return this._credentials = null, this._credentials_source = null, qf.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
+                    return Ts(this, void 0, void 0, (function() {
+                        return As(this, (function(e) {
+                            return this._credentials = null, this._credentials_source = null, tp.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
                         }))
                     }))
                 }, e.prototype._getGuestIdentityId = function() {
-                    return Ss(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t;
-                        return Ls(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e = this._config.identityPoolId, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return n.sent(), [2, this._storage.getItem(this._getCognitoIdentityIdStorageKey(e))];
                                 case 3:
-                                    return t = n.sent(), qf.debug("Failed to get the cached guest identityId", t), [3, 4];
+                                    return t = n.sent(), tp.debug("Failed to get the cached guest identityId", t), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._setGuestIdentityId = function(e) {
-                    return Ss(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n;
-                        return Ls(this, (function(r) {
+                        return As(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     t = this._config.identityPoolId, r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), this._storage.setItem(this._getCognitoIdentityIdStorageKey(t), e), [3, 4];
                                 case 3:
-                                    return n = r.sent(), qf.debug("Failed to cache guest identityId", n), [3, 4];
+                                    return n = r.sent(), tp.debug("Failed to cache guest identityId", n), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._removeGuestIdentityId = function() {
-                    return Ss(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e;
-                        return Ls(this, (function(t) {
-                            return e = this._config.identityPoolId, qf.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
+                        return As(this, (function(t) {
+                            return e = this._config.identityPoolId, tp.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
                         }))
                     }))
                 }, e.prototype.shear = function(e) {
                     return {
                         accessKeyId: e.accessKeyId,
                         sessionToken: e.sessionToken,
                         secretAccessKey: e.secretAccessKey,
                         identityId: e.identityId,
                         authenticated: e.authenticated
                     }
                 }, e
             }(),
-            Xf = new Kf(null);
-        nu.register(Xf);
-        var $f = Ys().isBrowser,
-            ep = function() {
+            op = new rp(null);
+        uu.register(op);
+        var ip = Vs().isBrowser,
+            ap = function() {
                 function e(e) {
-                    void 0 === e && (e = {}), this.cookies = new tt, this.store = $f ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
+                    void 0 === e && (e = {}), this.cookies = new tt, this.store = ip ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
                 }
                 return Object.defineProperty(e.prototype, "length", {
                     get: function() {
                         return Object.entries(this.store).length
                     },
                     enumerable: !0,
                     configurable: !0
@@ -65203,22 +65439,22 @@
                     var n = e.split(".").pop();
                     ["LastAuthUser", "accessToken", "refreshToken", "idToken"].includes(null !== n && void 0 !== n ? n : "") && this.setUniversalItem(e, t, {
                         expires: new Date(Date.now() + 31536e6)
                     })
                 }, e.prototype.setLocalItem = function(e, t) {
                     this.store[e] = t
                 }, e.prototype.setUniversalItem = function(e, t, n) {
-                    void 0 === n && (n = {}), this.cookies.set(e, t, Ds(Ds({}, n), {
+                    void 0 === n && (n = {}), this.cookies.set(e, t, _s(_s({}, n), {
                         path: "/",
                         sameSite: !0,
-                        secure: !$f || "localhost" !== window.location.hostname
+                        secure: !ip || "localhost" !== window.location.hostname
                     }))
                 }, e
             }();
-        var tp, np = function() {
+        var sp, up = function() {
                 function e(e) {
                     var t = e || {},
                         n = t.ValidationData,
                         r = t.Username,
                         o = t.Password,
                         i = t.AuthParameters,
                         a = t.ClientMetadata;
@@ -65233,253 +65469,253 @@
                     return this.validationData
                 }, t.getAuthParameters = function() {
                     return this.authParameters
                 }, t.getClientMetadata = function() {
                     return this.clientMetadata
                 }, e
             }(),
-            rp = __webpack_require__(2890);
+            lp = __webpack_require__(2890);
 
-        function op() {
-            if (tp) {
-                if ("function" === typeof tp.getRandomValues) try {
-                    return tp.getRandomValues(new Uint32Array(1))[0]
+        function cp() {
+            if (sp) {
+                if ("function" === typeof sp.getRandomValues) try {
+                    return sp.getRandomValues(new Uint32Array(1))[0]
                 } catch (e) {}
-                if ("function" === typeof tp.randomBytes) try {
-                    return tp.randomBytes(4).readInt32LE()
+                if ("function" === typeof sp.randomBytes) try {
+                    return sp.randomBytes(4).readInt32LE()
                 } catch (e) {}
             }
             throw new Error("Native crypto module could not be used to get secure random number.")
         }
-        "undefined" !== typeof window && window.crypto && (tp = window.crypto), !tp && "undefined" !== typeof window && window.msCrypto && (tp = window.msCrypto);
-        var ip, ap = function() {
+        "undefined" !== typeof window && window.crypto && (sp = window.crypto), !sp && "undefined" !== typeof window && window.msCrypto && (sp = window.msCrypto);
+        var dp, fp = function() {
                 function e(e, t) {
                     e = this.words = e || [], this.sigBytes = void 0 != t ? t : 4 * e.length
                 }
                 var t = e.prototype;
                 return t.random = function(t) {
-                    for (var n = [], r = 0; r < t; r += 4) n.push(op());
+                    for (var n = [], r = 0; r < t; r += 4) n.push(cp());
                     return new e(n, t)
                 }, t.toString = function() {
                     return function(e) {
                         for (var t = e.words, n = e.sigBytes, r = [], o = 0; o < n; o++) {
                             var i = t[o >>> 2] >>> 24 - o % 4 * 8 & 255;
                             r.push((i >>> 4).toString(16)), r.push((15 & i).toString(16))
                         }
                         return r.join("")
                     }(this)
                 }, e
             }(),
-            sp = __webpack_require__(6915),
-            up = lp;
+            pp = __webpack_require__(6915),
+            hp = gp;
 
-        function lp(e, t) {
+        function gp(e, t) {
             null != e && this.fromString(e, t)
         }
 
-        function cp() {
-            return new lp(null)
+        function yp() {
+            return new gp(null)
         }
-        var dp = "undefined" !== typeof navigator;
-        dp && "Microsoft Internet Explorer" == navigator.appName ? (lp.prototype.am = function(e, t, n, r, o, i) {
+        var mp = "undefined" !== typeof navigator;
+        mp && "Microsoft Internet Explorer" == navigator.appName ? (gp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 32767 & t, s = t >> 15; --i >= 0;) {
                 var u = 32767 & this[e],
                     l = this[e++] >> 15,
                     c = s * u + l * a;
                 o = ((u = a * u + ((32767 & c) << 15) + n[r] + (1073741823 & o)) >>> 30) + (c >>> 15) + s * l + (o >>> 30), n[r++] = 1073741823 & u
             }
             return o
-        }, ip = 30) : dp && "Netscape" != navigator.appName ? (lp.prototype.am = function(e, t, n, r, o, i) {
+        }, dp = 30) : mp && "Netscape" != navigator.appName ? (gp.prototype.am = function(e, t, n, r, o, i) {
             for (; --i >= 0;) {
                 var a = t * this[e++] + n[r] + o;
                 o = Math.floor(a / 67108864), n[r++] = 67108863 & a
             }
             return o
-        }, ip = 26) : (lp.prototype.am = function(e, t, n, r, o, i) {
+        }, dp = 26) : (gp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 16383 & t, s = t >> 14; --i >= 0;) {
                 var u = 16383 & this[e],
                     l = this[e++] >> 14,
                     c = s * u + l * a;
                 o = ((u = a * u + ((16383 & c) << 14) + n[r] + o) >> 28) + (c >> 14) + s * l, n[r++] = 268435455 & u
             }
             return o
-        }, ip = 28), lp.prototype.DB = ip, lp.prototype.DM = (1 << ip) - 1, lp.prototype.DV = 1 << ip;
-        lp.prototype.FV = Math.pow(2, 52), lp.prototype.F1 = 52 - ip, lp.prototype.F2 = 2 * ip - 52;
-        var fp, pp, hp = new Array;
-        for (fp = "0".charCodeAt(0), pp = 0; pp <= 9; ++pp) hp[fp++] = pp;
-        for (fp = "a".charCodeAt(0), pp = 10; pp < 36; ++pp) hp[fp++] = pp;
-        for (fp = "A".charCodeAt(0), pp = 10; pp < 36; ++pp) hp[fp++] = pp;
+        }, dp = 28), gp.prototype.DB = dp, gp.prototype.DM = (1 << dp) - 1, gp.prototype.DV = 1 << dp;
+        gp.prototype.FV = Math.pow(2, 52), gp.prototype.F1 = 52 - dp, gp.prototype.F2 = 2 * dp - 52;
+        var vp, Mp, bp = new Array;
+        for (vp = "0".charCodeAt(0), Mp = 0; Mp <= 9; ++Mp) bp[vp++] = Mp;
+        for (vp = "a".charCodeAt(0), Mp = 10; Mp < 36; ++Mp) bp[vp++] = Mp;
+        for (vp = "A".charCodeAt(0), Mp = 10; Mp < 36; ++Mp) bp[vp++] = Mp;
 
-        function gp(e) {
+        function wp(e) {
             return "0123456789abcdefghijklmnopqrstuvwxyz".charAt(e)
         }
 
-        function yp(e, t) {
-            var n = hp[e.charCodeAt(t)];
+        function jp(e, t) {
+            var n = bp[e.charCodeAt(t)];
             return null == n ? -1 : n
         }
 
-        function mp(e) {
-            var t = cp();
+        function xp(e) {
+            var t = yp();
             return t.fromInt(e), t
         }
 
-        function vp(e) {
+        function Np(e) {
             var t, n = 1;
             return 0 != (t = e >>> 16) && (e = t, n += 16), 0 != (t = e >> 8) && (e = t, n += 8), 0 != (t = e >> 4) && (e = t, n += 4), 0 != (t = e >> 2) && (e = t, n += 2), 0 != (t = e >> 1) && (e = t, n += 1), n
         }
 
-        function Mp(e) {
+        function Ip(e) {
             this.m = e, this.mp = e.invDigit(), this.mpl = 32767 & this.mp, this.mph = this.mp >> 15, this.um = (1 << e.DB - 15) - 1, this.mt2 = 2 * e.t
         }
 
-        function bp(e) {
-            return rp.lW.from((new ap).random(e).toString(), "hex")
+        function Dp(e) {
+            return lp.lW.from((new fp).random(e).toString(), "hex")
         }
-        Mp.prototype.convert = function(e) {
-            var t = cp();
-            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(lp.ZERO) > 0 && this.m.subTo(t, t), t
-        }, Mp.prototype.revert = function(e) {
-            var t = cp();
+        Ip.prototype.convert = function(e) {
+            var t = yp();
+            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(gp.ZERO) > 0 && this.m.subTo(t, t), t
+        }, Ip.prototype.revert = function(e) {
+            var t = yp();
             return e.copyTo(t), this.reduce(t), t
-        }, Mp.prototype.reduce = function(e) {
+        }, Ip.prototype.reduce = function(e) {
             for (; e.t <= this.mt2;) e[e.t++] = 0;
             for (var t = 0; t < this.m.t; ++t) {
                 var n = 32767 & e[t],
                     r = n * this.mpl + ((n * this.mph + (e[t] >> 15) * this.mpl & this.um) << 15) & e.DM;
                 for (e[n = t + this.m.t] += this.m.am(0, r, e, t, 0, this.m.t); e[n] >= e.DV;) e[n] -= e.DV, e[++n]++
             }
             e.clamp(), e.drShiftTo(this.m.t, e), e.compareTo(this.m) >= 0 && e.subTo(this.m, e)
-        }, Mp.prototype.mulTo = function(e, t, n) {
+        }, Ip.prototype.mulTo = function(e, t, n) {
             e.multiplyTo(t, n), this.reduce(n)
-        }, Mp.prototype.sqrTo = function(e, t) {
+        }, Ip.prototype.sqrTo = function(e, t) {
             e.squareTo(t), this.reduce(t)
-        }, lp.prototype.copyTo = function(e) {
+        }, gp.prototype.copyTo = function(e) {
             for (var t = this.t - 1; t >= 0; --t) e[t] = this[t];
             e.t = this.t, e.s = this.s
-        }, lp.prototype.fromInt = function(e) {
+        }, gp.prototype.fromInt = function(e) {
             this.t = 1, this.s = e < 0 ? -1 : 0, e > 0 ? this[0] = e : e < -1 ? this[0] = e + this.DV : this.t = 0
-        }, lp.prototype.fromString = function(e, t) {
+        }, gp.prototype.fromString = function(e, t) {
             var n;
             if (16 == t) n = 4;
             else if (8 == t) n = 3;
             else if (2 == t) n = 1;
             else if (32 == t) n = 5;
             else {
                 if (4 != t) throw new Error("Only radix 2, 4, 8, 16, 32 are supported");
                 n = 2
             }
             this.t = 0, this.s = 0;
             for (var r = e.length, o = !1, i = 0; --r >= 0;) {
-                var a = yp(e, r);
+                var a = jp(e, r);
                 a < 0 ? "-" == e.charAt(r) && (o = !0) : (o = !1, 0 == i ? this[this.t++] = a : i + n > this.DB ? (this[this.t - 1] |= (a & (1 << this.DB - i) - 1) << i, this[this.t++] = a >> this.DB - i) : this[this.t - 1] |= a << i, (i += n) >= this.DB && (i -= this.DB))
             }
-            this.clamp(), o && lp.ZERO.subTo(this, this)
-        }, lp.prototype.clamp = function() {
+            this.clamp(), o && gp.ZERO.subTo(this, this)
+        }, gp.prototype.clamp = function() {
             for (var e = this.s & this.DM; this.t > 0 && this[this.t - 1] == e;) --this.t
-        }, lp.prototype.dlShiftTo = function(e, t) {
+        }, gp.prototype.dlShiftTo = function(e, t) {
             var n;
             for (n = this.t - 1; n >= 0; --n) t[n + e] = this[n];
             for (n = e - 1; n >= 0; --n) t[n] = 0;
             t.t = this.t + e, t.s = this.s
-        }, lp.prototype.drShiftTo = function(e, t) {
+        }, gp.prototype.drShiftTo = function(e, t) {
             for (var n = e; n < this.t; ++n) t[n - e] = this[n];
             t.t = Math.max(this.t - e, 0), t.s = this.s
-        }, lp.prototype.lShiftTo = function(e, t) {
+        }, gp.prototype.lShiftTo = function(e, t) {
             var n, r = e % this.DB,
                 o = this.DB - r,
                 i = (1 << o) - 1,
                 a = Math.floor(e / this.DB),
                 s = this.s << r & this.DM;
             for (n = this.t - 1; n >= 0; --n) t[n + a + 1] = this[n] >> o | s, s = (this[n] & i) << r;
             for (n = a - 1; n >= 0; --n) t[n] = 0;
             t[a] = s, t.t = this.t + a + 1, t.s = this.s, t.clamp()
-        }, lp.prototype.rShiftTo = function(e, t) {
+        }, gp.prototype.rShiftTo = function(e, t) {
             t.s = this.s;
             var n = Math.floor(e / this.DB);
             if (n >= this.t) t.t = 0;
             else {
                 var r = e % this.DB,
                     o = this.DB - r,
                     i = (1 << r) - 1;
                 t[0] = this[n] >> r;
                 for (var a = n + 1; a < this.t; ++a) t[a - n - 1] |= (this[a] & i) << o, t[a - n] = this[a] >> r;
                 r > 0 && (t[this.t - n - 1] |= (this.s & i) << o), t.t = this.t - n, t.clamp()
             }
-        }, lp.prototype.subTo = function(e, t) {
+        }, gp.prototype.subTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] - e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r -= e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r -= e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r -= e.s
             }
             t.s = r < 0 ? -1 : 0, r < -1 ? t[n++] = this.DV + r : r > 0 && (t[n++] = r), t.t = n, t.clamp()
-        }, lp.prototype.multiplyTo = function(e, t) {
+        }, gp.prototype.multiplyTo = function(e, t) {
             var n = this.abs(),
                 r = e.abs(),
                 o = n.t;
             for (t.t = o + r.t; --o >= 0;) t[o] = 0;
             for (o = 0; o < r.t; ++o) t[o + n.t] = n.am(0, r[o], t, o, 0, n.t);
-            t.s = 0, t.clamp(), this.s != e.s && lp.ZERO.subTo(t, t)
-        }, lp.prototype.squareTo = function(e) {
+            t.s = 0, t.clamp(), this.s != e.s && gp.ZERO.subTo(t, t)
+        }, gp.prototype.squareTo = function(e) {
             for (var t = this.abs(), n = e.t = 2 * t.t; --n >= 0;) e[n] = 0;
             for (n = 0; n < t.t - 1; ++n) {
                 var r = t.am(n, t[n], e, 2 * n, 0, 1);
                 (e[n + t.t] += t.am(n + 1, 2 * t[n], e, 2 * n + 1, r, t.t - n - 1)) >= t.DV && (e[n + t.t] -= t.DV, e[n + t.t + 1] = 1)
             }
             e.t > 0 && (e[e.t - 1] += t.am(n, t[n], e, 2 * n, 0, 1)), e.s = 0, e.clamp()
-        }, lp.prototype.divRemTo = function(e, t, n) {
+        }, gp.prototype.divRemTo = function(e, t, n) {
             var r = e.abs();
             if (!(r.t <= 0)) {
                 var o = this.abs();
                 if (o.t < r.t) return null != t && t.fromInt(0), void(null != n && this.copyTo(n));
-                null == n && (n = cp());
-                var i = cp(),
+                null == n && (n = yp());
+                var i = yp(),
                     a = this.s,
                     s = e.s,
-                    u = this.DB - vp(r[r.t - 1]);
+                    u = this.DB - Np(r[r.t - 1]);
                 u > 0 ? (r.lShiftTo(u, i), o.lShiftTo(u, n)) : (r.copyTo(i), o.copyTo(n));
                 var l = i.t,
                     c = i[l - 1];
                 if (0 != c) {
                     var d = c * (1 << this.F1) + (l > 1 ? i[l - 2] >> this.F2 : 0),
                         f = this.FV / d,
                         p = (1 << this.F1) / d,
                         h = 1 << this.F2,
                         g = n.t,
                         y = g - l,
-                        m = null == t ? cp() : t;
-                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), lp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
+                        m = null == t ? yp() : t;
+                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), gp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
                     for (; --y >= 0;) {
                         var v = n[--g] == c ? this.DM : Math.floor(n[g] * f + (n[g - 1] + h) * p);
                         if ((n[g] += i.am(0, v, n, y, 0, l)) < v)
                             for (i.dlShiftTo(y, m), n.subTo(m, n); n[g] < --v;) n.subTo(m, n)
                     }
-                    null != t && (n.drShiftTo(l, t), a != s && lp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && lp.ZERO.subTo(n, n)
+                    null != t && (n.drShiftTo(l, t), a != s && gp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && gp.ZERO.subTo(n, n)
                 }
             }
-        }, lp.prototype.invDigit = function() {
+        }, gp.prototype.invDigit = function() {
             if (this.t < 1) return 0;
             var e = this[0];
             if (0 == (1 & e)) return 0;
             var t = 3 & e;
             return (t = (t = (t = (t = t * (2 - (15 & e) * t) & 15) * (2 - (255 & e) * t) & 255) * (2 - ((65535 & e) * t & 65535)) & 65535) * (2 - e * t % this.DV) % this.DV) > 0 ? this.DV - t : -t
-        }, lp.prototype.addTo = function(e, t) {
+        }, gp.prototype.addTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] + e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r += e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r += e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += e.s
             }
             t.s = r < 0 ? -1 : 0, r > 0 ? t[n++] = r : r < -1 && (t[n++] = this.DV + r), t.t = n, t.clamp()
-        }, lp.prototype.toString = function(e) {
+        }, gp.prototype.toString = function(e) {
             if (this.s < 0) return "-" + this.negate().toString(e);
             var t;
             if (16 == e) t = 4;
             else if (8 == e) t = 3;
             else if (2 == e) t = 1;
             else if (32 == e) t = 5;
             else {
@@ -65488,236 +65724,236 @@
             }
             var n, r = (1 << t) - 1,
                 o = !1,
                 i = "",
                 a = this.t,
                 s = this.DB - a * this.DB % t;
             if (a-- > 0)
-                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = gp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += gp(n));
+                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = wp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += wp(n));
             return o ? i : "0"
-        }, lp.prototype.negate = function() {
-            var e = cp();
-            return lp.ZERO.subTo(this, e), e
-        }, lp.prototype.abs = function() {
+        }, gp.prototype.negate = function() {
+            var e = yp();
+            return gp.ZERO.subTo(this, e), e
+        }, gp.prototype.abs = function() {
             return this.s < 0 ? this.negate() : this
-        }, lp.prototype.compareTo = function(e) {
+        }, gp.prototype.compareTo = function(e) {
             var t = this.s - e.s;
             if (0 != t) return t;
             var n = this.t;
             if (0 != (t = n - e.t)) return this.s < 0 ? -t : t;
             for (; --n >= 0;)
                 if (0 != (t = this[n] - e[n])) return t;
             return 0
-        }, lp.prototype.bitLength = function() {
-            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + vp(this[this.t - 1] ^ this.s & this.DM)
-        }, lp.prototype.mod = function(e) {
-            var t = cp();
-            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(lp.ZERO) > 0 && e.subTo(t, t), t
-        }, lp.prototype.equals = function(e) {
+        }, gp.prototype.bitLength = function() {
+            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + Np(this[this.t - 1] ^ this.s & this.DM)
+        }, gp.prototype.mod = function(e) {
+            var t = yp();
+            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(gp.ZERO) > 0 && e.subTo(t, t), t
+        }, gp.prototype.equals = function(e) {
             return 0 == this.compareTo(e)
-        }, lp.prototype.add = function(e) {
-            var t = cp();
+        }, gp.prototype.add = function(e) {
+            var t = yp();
             return this.addTo(e, t), t
-        }, lp.prototype.subtract = function(e) {
-            var t = cp();
+        }, gp.prototype.subtract = function(e) {
+            var t = yp();
             return this.subTo(e, t), t
-        }, lp.prototype.multiply = function(e) {
-            var t = cp();
+        }, gp.prototype.multiply = function(e) {
+            var t = yp();
             return this.multiplyTo(e, t), t
-        }, lp.prototype.divide = function(e) {
-            var t = cp();
+        }, gp.prototype.divide = function(e) {
+            var t = yp();
             return this.divRemTo(e, t, null), t
-        }, lp.prototype.modPow = function(e, t, n) {
+        }, gp.prototype.modPow = function(e, t, n) {
             var r, o = e.bitLength(),
-                i = mp(1),
-                a = new Mp(t);
+                i = xp(1),
+                a = new Ip(t);
             if (o <= 0) return i;
             r = o < 18 ? 1 : o < 48 ? 3 : o < 144 ? 4 : o < 768 ? 5 : 6;
             var s = new Array,
                 u = 3,
                 l = r - 1,
                 c = (1 << r) - 1;
             if (s[1] = a.convert(this), r > 1) {
-                var d = cp();
-                for (a.sqrTo(s[1], d); u <= c;) s[u] = cp(), a.mulTo(d, s[u - 2], s[u]), u += 2
+                var d = yp();
+                for (a.sqrTo(s[1], d); u <= c;) s[u] = yp(), a.mulTo(d, s[u - 2], s[u]), u += 2
             }
             var f, p, h = e.t - 1,
                 g = !0,
-                y = cp();
-            for (o = vp(e[h]) - 1; h >= 0;) {
+                y = yp();
+            for (o = Np(e[h]) - 1; h >= 0;) {
                 for (o >= l ? f = e[h] >> o - l & c : (f = (e[h] & (1 << o + 1) - 1) << l - o, h > 0 && (f |= e[h - 1] >> this.DB + o - l)), u = r; 0 == (1 & f);) f >>= 1, --u;
                 if ((o -= u) < 0 && (o += this.DB, --h), g) s[f].copyTo(i), g = !1;
                 else {
                     for (; u > 1;) a.sqrTo(i, y), a.sqrTo(y, i), u -= 2;
                     u > 0 ? a.sqrTo(i, y) : (p = i, i = y, y = p), a.mulTo(y, s[f], i)
                 }
                 for (; h >= 0 && 0 == (e[h] & 1 << o);) a.sqrTo(i, y), p = i, i = y, y = p, --o < 0 && (o = this.DB - 1, --h)
             }
             var m = a.revert(i);
             return n(null, m), m
-        }, lp.ZERO = mp(0), lp.ONE = mp(1);
-        var wp = /^[89a-f]/i,
-            jp = function() {
+        }, gp.ZERO = xp(0), gp.ONE = xp(1);
+        var Sp = /^[89a-f]/i,
+            Lp = function() {
                 function e(e) {
-                    this.N = new up("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new up("2", 16), this.k = new up(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = rp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
+                    this.N = new hp("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new hp("2", 16), this.k = new hp(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = lp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
                 }
                 var t = e.prototype;
                 return t.getSmallAValue = function() {
                     return this.smallAValue
                 }, t.getLargeAValue = function(e) {
                     var t = this;
                     this.largeAValue ? e(null, this.largeAValue) : this.calculateA(this.smallAValue, (function(n, r) {
                         n && e(n, null), t.largeAValue = r, e(null, t.largeAValue)
                     }))
                 }, t.generateRandomSmallA = function() {
-                    var e = bp(128).toString("hex");
-                    return new up(e, 16)
+                    var e = Dp(128).toString("hex");
+                    return new hp(e, 16)
                 }, t.generateRandomString = function() {
-                    return bp(40).toString("base64")
+                    return Dp(40).toString("base64")
                 }, t.getRandomPassword = function() {
                     return this.randomPassword
                 }, t.getSaltDevices = function() {
                     return this.SaltToHashDevices
                 }, t.getVerifierDevices = function() {
                     return this.verifierDevices
                 }, t.generateHashDevice = function(e, t, n) {
                     var r = this;
                     this.randomPassword = this.generateRandomString();
                     var o = "" + e + t + ":" + this.randomPassword,
                         i = this.hash(o),
-                        a = bp(16).toString("hex");
-                    this.SaltToHashDevices = this.padHex(new up(a, 16)), this.g.modPow(new up(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
+                        a = Dp(16).toString("hex");
+                    this.SaltToHashDevices = this.padHex(new hp(a, 16)), this.g.modPow(new hp(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
                         e && n(e, null), r.verifierDevices = r.padHex(t), n(null, null)
                     }))
                 }, t.calculateA = function(e, t) {
                     var n = this;
                     this.g.modPow(e, this.N, (function(e, r) {
-                        e && t(e, null), r.mod(n.N).equals(up.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
+                        e && t(e, null), r.mod(n.N).equals(hp.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
                     }))
                 }, t.calculateU = function(e, t) {
-                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new up(this.UHexHash, 16)
+                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new hp(this.UHexHash, 16)
                 }, t.hash = function(e) {
-                    var t = new sp.Sha256;
+                    var t = new pp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
-                        r = rp.lW.from(n).toString("hex");
+                        r = lp.lW.from(n).toString("hex");
                     return new Array(64 - r.length).join("0") + r
                 }, t.hexHash = function(e) {
-                    return this.hash(rp.lW.from(e, "hex"))
+                    return this.hash(lp.lW.from(e, "hex"))
                 }, t.computehkdf = function(e, t) {
-                    var n = rp.lW.concat([this.infoBits, rp.lW.from(String.fromCharCode(1), "utf8")]),
-                        r = new sp.Sha256(t);
+                    var n = lp.lW.concat([this.infoBits, lp.lW.from(String.fromCharCode(1), "utf8")]),
+                        r = new pp.Sha256(t);
                     r.update(e);
                     var o = r.digestSync(),
-                        i = new sp.Sha256(o);
+                        i = new pp.Sha256(o);
                     return i.update(n), i.digestSync().slice(0, 16)
                 }, t.getPasswordAuthenticationKey = function(e, t, n, r, o) {
                     var i = this;
-                    if (n.mod(this.N).equals(up.ZERO)) throw new Error("B cannot be zero.");
-                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(up.ZERO)) throw new Error("U cannot be zero.");
+                    if (n.mod(this.N).equals(hp.ZERO)) throw new Error("B cannot be zero.");
+                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(hp.ZERO)) throw new Error("U cannot be zero.");
                     var a = "" + this.poolName + e + ":" + t,
                         s = this.hash(a),
-                        u = new up(this.hexHash(this.padHex(r) + s), 16);
+                        u = new hp(this.hexHash(this.padHex(r) + s), 16);
                     this.calculateS(u, n, (function(e, t) {
                         e && o(e, null);
-                        var n = i.computehkdf(rp.lW.from(i.padHex(t), "hex"), rp.lW.from(i.padHex(i.UValue), "hex"));
+                        var n = i.computehkdf(lp.lW.from(i.padHex(t), "hex"), lp.lW.from(i.padHex(i.UValue), "hex"));
                         o(null, n)
                     }))
                 }, t.calculateS = function(e, t, n) {
                     var r = this;
                     this.g.modPow(e, this.N, (function(o, i) {
                         o && n(o, null), t.subtract(r.k.multiply(i)).modPow(r.smallAValue.add(r.UValue.multiply(e)), r.N, (function(e, t) {
                             e && n(e, null), n(null, t.mod(r.N))
                         }))
                     }))
                 }, t.getNewPasswordRequiredChallengeUserAttributePrefix = function() {
                     return "userAttributes."
                 }, t.padHex = function(e) {
-                    if (!(e instanceof up)) throw new Error("Not a BigInteger");
-                    var t = e.compareTo(up.ZERO) < 0,
+                    if (!(e instanceof hp)) throw new Error("Not a BigInteger");
+                    var t = e.compareTo(hp.ZERO) < 0,
                         n = e.abs().toString(16);
-                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = wp.test(n) ? "00" + n : n, t) {
+                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = Sp.test(n) ? "00" + n : n, t) {
                         var r = n.split("").map((function(e) {
                             var t = 15 & ~parseInt(e, 16);
                             return "0123456789ABCDEF".charAt(t)
                         })).join("");
-                        (n = new up(r, 16).add(up.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
+                        (n = new hp(r, 16).add(hp.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
                     }
                     return n
                 }, e
             }(),
-            xp = function() {
+            kp = function() {
                 function e(e) {
                     this.jwtToken = e || "", this.payload = this.decodePayload()
                 }
                 var t = e.prototype;
                 return t.getJwtToken = function() {
                     return this.jwtToken
                 }, t.getExpiration = function() {
                     return this.payload.exp
                 }, t.getIssuedAt = function() {
                     return this.payload.iat
                 }, t.decodePayload = function() {
                     var e = this.jwtToken.split(".")[1];
                     try {
-                        return JSON.parse(rp.lW.from(e, "base64").toString("utf8"))
+                        return JSON.parse(lp.lW.from(e, "base64").toString("utf8"))
                     } catch (t) {
                         return {}
                     }
                 }, e
             }();
 
-        function Np(e, t) {
-            return Np = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Cp(e, t) {
+            return Cp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Np(e, t)
+            }, Cp(e, t)
         }
-        var Ip = function(e) {
+        var Ep = function(e) {
             var t, n;
 
             function r(t) {
                 var n = (void 0 === t ? {} : t).AccessToken;
                 return e.call(this, n || "") || this
             }
-            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Np(t, n), r
-        }(xp);
+            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Cp(t, n), r
+        }(kp);
 
-        function Dp(e, t) {
-            return Dp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function _p(e, t) {
+            return _p = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Dp(e, t)
+            }, _p(e, t)
         }
-        var Sp = function(e) {
+        var Tp = function(e) {
                 var t, n;
 
                 function r(t) {
                     var n = (void 0 === t ? {} : t).IdToken;
                     return e.call(this, n || "") || this
                 }
-                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Dp(t, n), r
-            }(xp),
-            Lp = function() {
+                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, _p(t, n), r
+            }(kp),
+            Ap = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).RefreshToken;
                     this.token = t || ""
                 }
                 return e.prototype.getToken = function() {
                     return this.token
                 }, e
             }(),
-            kp = {
+            Op = {
                 userAgent: "aws-amplify/5.0.4 js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (kp.product = navigator.product || "", kp.navigator = navigator || null, "ReactNative" === navigator.product) kp.userAgent = "aws-amplify/5.0.4 react-native", kp.isReactNative = !0;
-            else kp.userAgent = "aws-amplify/5.0.4 js", kp.isReactNative = !1;
-        var Cp = function() {
+            if (Op.product = navigator.product || "", Op.navigator = navigator || null, "ReactNative" === navigator.product) Op.userAgent = "aws-amplify/5.0.4 react-native", Op.isReactNative = !0;
+            else Op.userAgent = "aws-amplify/5.0.4 js", Op.isReactNative = !1;
+        var zp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.IdToken,
                         r = t.RefreshToken,
                         o = t.AccessToken,
                         i = t.ClockDrift;
                     if (null == o || null == n) throw new Error("Id token and Access Token must be present.");
@@ -65735,32 +65971,32 @@
                 }, t.calculateClockDrift = function() {
                     return Math.floor(new Date / 1e3) - Math.min(this.accessToken.getIssuedAt(), this.idToken.getIssuedAt())
                 }, t.isValid = function() {
                     var e = Math.floor(new Date / 1e3) - this.clockDrift;
                     return e < this.accessToken.getExpiration() && e < this.idToken.getExpiration()
                 }, e
             }(),
-            Ep = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-            _p = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-            Tp = function() {
+            Up = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+            Pp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+            Rp = function() {
                 function e() {}
                 return e.prototype.getNowString = function() {
                     var e = new Date,
-                        t = _p[e.getUTCDay()],
-                        n = Ep[e.getUTCMonth()],
+                        t = Pp[e.getUTCDay()],
+                        n = Up[e.getUTCMonth()],
                         r = e.getUTCDate(),
                         o = e.getUTCHours();
                     o < 10 && (o = "0" + o);
                     var i = e.getUTCMinutes();
                     i < 10 && (i = "0" + i);
                     var a = e.getUTCSeconds();
                     return a < 10 && (a = "0" + a), t + " " + n + " " + r + " " + o + ":" + i + ":" + a + " UTC " + e.getUTCFullYear()
                 }, e
             }(),
-            Ap = function() {
+            Bp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.Name,
                         r = t.Value;
                     this.Name = n || "", this.Value = r || ""
                 }
                 var t = e.prototype;
@@ -65777,44 +66013,44 @@
                 }, t.toJSON = function() {
                     return {
                         Name: this.Name,
                         Value: this.Value
                     }
                 }, e
             }(),
-            Op = {},
-            zp = function() {
+            Fp = {},
+            Yp = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Op[e] = t, Op[e]
+                    return Fp[e] = t, Fp[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Op, e) ? Op[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Fp, e) ? Fp[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Op[e]
+                    return delete Fp[e]
                 }, e.clear = function() {
-                    return Op = {}
+                    return Fp = {}
                 }, e
             }(),
-            Up = function() {
+            Qp = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.cognito.test-ls", 1), this.storageWindow.removeItem("aws.cognito.test-ls")
                     } catch (e) {
-                        this.storageWindow = zp
+                        this.storageWindow = Yp
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            Pp = "undefined" !== typeof navigator ? kp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
-            Rp = function() {
+            Gp = "undefined" !== typeof navigator ? Op.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
+            Wp = function() {
                 function e(e) {
                     if (null == e || null == e.Username || null == e.Pool) throw new Error("Username and Pool information are required.");
-                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Up).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
+                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Qp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
                 }
                 var t = e.prototype;
                 return t.setSignInUserSession = function(e) {
                     this.clearCachedUserData(), this.signInUserSession = e, this.cacheTokens()
                 }, t.getSignInUserSession = function() {
                     return this.signInUserSession
                 }, t.getUsername = function() {
@@ -65840,37 +66076,37 @@
                             i = r.ChallengeParameters;
                         return "CUSTOM_CHALLENGE" === o ? (n.Session = r.Session, t.customChallenge(i)) : (n.signInUserSession = n.getCognitoUserSession(r.AuthenticationResult), n.cacheTokens(), t.onSuccess(n.signInUserSession))
                     }))
                 }, t.authenticateUser = function(e, t) {
                     return "USER_PASSWORD_AUTH" === this.authenticationFlowType ? this.authenticateUserPlainUsernamePassword(e, t) : "USER_SRP_AUTH" === this.authenticationFlowType || "CUSTOM_AUTH" === this.authenticationFlowType ? this.authenticateUserDefaultAuth(e, t) : t.onFailure(new Error("Authentication flow type is invalid."))
                 }, t.authenticateUserDefaultAuth = function(e, t) {
                     var n, r, o = this,
-                        i = new jp(this.pool.getUserPoolName()),
-                        a = new Tp,
+                        i = new Lp(this.pool.getUserPoolName()),
+                        a = new Rp,
                         s = {};
                     null != this.deviceKey && (s.DEVICE_KEY = this.deviceKey), s.USERNAME = this.username, i.getLargeAValue((function(u, l) {
                         u && t.onFailure(u), s.SRP_A = l.toString(16), "CUSTOM_AUTH" === o.authenticationFlowType && (s.CHALLENGE_NAME = "SRP_A");
                         var c = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             d = {
                                 AuthFlow: o.authenticationFlowType,
                                 ClientId: o.pool.getClientId(),
                                 AuthParameters: s,
                                 ClientMetadata: c
                             };
                         o.getUserContextData(o.username) && (d.UserContextData = o.getUserContextData(o.username)), o.client.request("InitiateAuth", d, (function(s, u) {
                             if (s) return t.onFailure(s);
                             var l = u.ChallengeParameters;
-                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new up(l.SRP_B, 16), r = new up(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
+                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new hp(l.SRP_B, 16), r = new hp(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
                                 e && t.onFailure(e);
                                 var r = a.getNowString(),
-                                    s = rp.lW.concat([rp.lW.from(o.pool.getUserPoolName(), "utf8"), rp.lW.from(o.username, "utf8"), rp.lW.from(l.SECRET_BLOCK, "base64"), rp.lW.from(r, "utf8")]),
-                                    d = new sp.Sha256(n);
+                                    s = lp.lW.concat([lp.lW.from(o.pool.getUserPoolName(), "utf8"), lp.lW.from(o.username, "utf8"), lp.lW.from(l.SECRET_BLOCK, "base64"), lp.lW.from(r, "utf8")]),
+                                    d = new pp.Sha256(n);
                                 d.update(s);
                                 var f = d.digestSync(),
-                                    p = rp.lW.from(f).toString("base64"),
+                                    p = lp.lW.from(f).toString("base64"),
                                     h = {};
                                 h.USERNAME = o.username, h.PASSWORD_CLAIM_SECRET_BLOCK = l.SECRET_BLOCK, h.TIMESTAMP = r, h.PASSWORD_CLAIM_SIGNATURE = p, null != o.deviceKey && (h.DEVICE_KEY = o.deviceKey);
                                 var g = {
                                     ChallengeName: "PASSWORD_VERIFIER",
                                     ClientId: o.pool.getClientId(),
                                     ChallengeResponses: h,
                                     Session: u.Session,
@@ -65887,15 +66123,15 @@
                             }))
                         }))
                     }))
                 }, t.authenticateUserPlainUsernamePassword = function(e, t) {
                     var n = this,
                         r = {};
                     if (r.USERNAME = this.username, r.PASSWORD = e.getPassword(), r.PASSWORD) {
-                        var o = new jp(this.pool.getUserPoolName());
+                        var o = new Lp(this.pool.getUserPoolName());
                         this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (r.DEVICE_KEY = this.deviceKey);
                         var i = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             a = {
                                 AuthFlow: "USER_PASSWORD_AUTH",
                                 ClientId: this.pool.getClientId(),
                                 AuthParameters: r,
                                 ClientMetadata: i
@@ -65926,30 +66162,30 @@
                     if ("DEVICE_SRP_AUTH" === o) return this.Session = e.Session, void this.getDeviceResponse(n);
                     this.signInUserSession = this.getCognitoUserSession(e.AuthenticationResult), this.challengeName = o, this.cacheTokens();
                     var d = e.AuthenticationResult.NewDeviceMetadata;
                     if (null == d) return n.onSuccess(this.signInUserSession);
                     t.generateHashDevice(e.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, e.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(o) {
                         if (o) return n.onFailure(o);
                         var i = {
-                            Salt: rp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
-                            PasswordVerifier: rp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
+                            Salt: lp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
+                            PasswordVerifier: lp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
                         };
                         r.verifierDevices = i.PasswordVerifier, r.deviceGroupKey = d.DeviceGroupKey, r.randomPassword = t.getRandomPassword(), r.client.request("ConfirmDevice", {
                             DeviceKey: d.DeviceKey,
                             AccessToken: r.signInUserSession.getAccessToken().getJwtToken(),
                             DeviceSecretVerifierConfig: i,
-                            DeviceName: Pp
+                            DeviceName: Gp
                         }, (function(t, o) {
                             return t ? n.onFailure(t) : (r.deviceKey = e.AuthenticationResult.NewDeviceMetadata.DeviceKey, r.cacheDeviceKeyAndPassword(), !0 === o.UserConfirmationNecessary ? n.onSuccess(r.signInUserSession, o.UserConfirmationNecessary) : n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, t.completeNewPasswordChallenge = function(e, t, n, r) {
                     var o = this;
                     if (!e) return n.onFailure(new Error("New password is required."));
-                    var i = new jp(this.pool.getUserPoolName()),
+                    var i = new Lp(this.pool.getUserPoolName()),
                         a = i.getNewPasswordRequiredChallengeUserAttributePrefix(),
                         s = {};
                     t && Object.keys(t).forEach((function(e) {
                         s[a + e] = t[e]
                     })), s.NEW_PASSWORD = e, s.USERNAME = this.username;
                     var u = {
                         ChallengeName: "NEW_PASSWORD_REQUIRED",
@@ -65959,39 +66195,39 @@
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (u.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", u, (function(e, t) {
                         return e ? n.onFailure(e) : o.authenticateUserInternal(t, i, n)
                     }))
                 }, t.getDeviceResponse = function(e, t) {
                     var n = this,
-                        r = new jp(this.deviceGroupKey),
-                        o = new Tp,
+                        r = new Lp(this.deviceGroupKey),
+                        o = new Rp,
                         i = {};
                     i.USERNAME = this.username, i.DEVICE_KEY = this.deviceKey, r.getLargeAValue((function(a, s) {
                         a && e.onFailure(a), i.SRP_A = s.toString(16);
                         var u = {
                             ChallengeName: "DEVICE_SRP_AUTH",
                             ClientId: n.pool.getClientId(),
                             ChallengeResponses: i,
                             ClientMetadata: t,
                             Session: n.Session
                         };
                         n.getUserContextData() && (u.UserContextData = n.getUserContextData()), n.client.request("RespondToAuthChallenge", u, (function(t, i) {
                             if (t) return e.onFailure(t);
                             var a = i.ChallengeParameters,
-                                s = new up(a.SRP_B, 16),
-                                u = new up(a.SALT, 16);
+                                s = new hp(a.SRP_B, 16),
+                                u = new hp(a.SALT, 16);
                             r.getPasswordAuthenticationKey(n.deviceKey, n.randomPassword, s, u, (function(t, r) {
                                 if (t) return e.onFailure(t);
                                 var s = o.getNowString(),
-                                    u = rp.lW.concat([rp.lW.from(n.deviceGroupKey, "utf8"), rp.lW.from(n.deviceKey, "utf8"), rp.lW.from(a.SECRET_BLOCK, "base64"), rp.lW.from(s, "utf8")]),
-                                    l = new sp.Sha256(r);
+                                    u = lp.lW.concat([lp.lW.from(n.deviceGroupKey, "utf8"), lp.lW.from(n.deviceKey, "utf8"), lp.lW.from(a.SECRET_BLOCK, "base64"), lp.lW.from(s, "utf8")]),
+                                    l = new pp.Sha256(r);
                                 l.update(u);
                                 var c = l.digestSync(),
-                                    d = rp.lW.from(c).toString("base64"),
+                                    d = lp.lW.from(c).toString("base64"),
                                     f = {};
                                 f.USERNAME = n.username, f.PASSWORD_CLAIM_SECRET_BLOCK = a.SECRET_BLOCK, f.TIMESTAMP = s, f.PASSWORD_CLAIM_SIGNATURE = d, f.DEVICE_KEY = n.deviceKey;
                                 var p = {
                                     ChallengeName: "DEVICE_PASSWORD_VERIFIER",
                                     ClientId: n.pool.getClientId(),
                                     ChallengeResponses: f,
                                     Session: i.Session
@@ -66013,15 +66249,15 @@
                     this.getUserContextData() && (o.UserContextData = this.getUserContextData()), this.client.request("ConfirmSignUp", o, (function(e) {
                         return e ? n(e, null) : n(null, "SUCCESS")
                     }))
                 }, t.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this,
                         o = {};
                     o.USERNAME = this.username, o.ANSWER = e;
-                    var i = new jp(this.pool.getUserPoolName());
+                    var i = new Lp(this.pool.getUserPoolName());
                     this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (o.DEVICE_KEY = this.deviceKey);
                     var a = {
                         ChallengeName: "CUSTOM_CHALLENGE",
                         ChallengeResponses: o,
                         ClientId: this.pool.getClientId(),
                         Session: this.Session,
                         ClientMetadata: n
@@ -66042,26 +66278,26 @@
                         Session: this.Session,
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (s.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", s, (function(e, n) {
                         if (e) return t.onFailure(e);
                         if ("DEVICE_SRP_AUTH" !== n.ChallengeName) {
                             if (o.signInUserSession = o.getCognitoUserSession(n.AuthenticationResult), o.cacheTokens(), null == n.AuthenticationResult.NewDeviceMetadata) return t.onSuccess(o.signInUserSession);
-                            var r = new jp(o.pool.getUserPoolName());
+                            var r = new Lp(o.pool.getUserPoolName());
                             r.generateHashDevice(n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, n.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(e) {
                                 if (e) return t.onFailure(e);
                                 var i = {
-                                    Salt: rp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
-                                    PasswordVerifier: rp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
+                                    Salt: lp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
+                                    PasswordVerifier: lp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
                                 };
                                 o.verifierDevices = i.PasswordVerifier, o.deviceGroupKey = n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, o.randomPassword = r.getRandomPassword(), o.client.request("ConfirmDevice", {
                                     DeviceKey: n.AuthenticationResult.NewDeviceMetadata.DeviceKey,
                                     AccessToken: o.signInUserSession.getAccessToken().getJwtToken(),
                                     DeviceSecretVerifierConfig: i,
-                                    DeviceName: Pp
+                                    DeviceName: Gp
                                 }, (function(e, r) {
                                     return e ? t.onFailure(e) : (o.deviceKey = n.AuthenticationResult.NewDeviceMetadata.DeviceKey, o.cacheDeviceKeyAndPassword(), !0 === r.UserConfirmationNecessary ? t.onSuccess(o.signInUserSession, r.UserConfirmationNecessary) : t.onSuccess(o.signInUserSession))
                                 }))
                             }))
                         } else o.getDeviceResponse(t)
                     }))
                 }, t.changePassword = function(e, t, n, r) {
@@ -66133,15 +66369,15 @@
                     }, (function(t, n) {
                         if (t) return e(t, null);
                         for (var r = [], o = 0; o < n.UserAttributes.length; o++) {
                             var i = {
                                     Name: n.UserAttributes[o].Name,
                                     Value: n.UserAttributes[o].Value
                                 },
-                                a = new Ap(i);
+                                a = new Bp(i);
                             r.push(a)
                         }
                         return e(null, r)
                     }))
                 }, t.getMFAOptions = function(e) {
                     if (null == this.signInUserSession || !this.signInUserSession.isValid()) return e(new Error("User is not authenticated"), null);
                     this.client.request("GetUser", {
@@ -66215,25 +66451,25 @@
                     if (null != this.signInUserSession && this.signInUserSession.isValid()) return e(null, this.signInUserSession);
                     var n = "CognitoIdentityServiceProvider." + this.pool.getClientId() + "." + this.username,
                         r = n + ".idToken",
                         o = n + ".accessToken",
                         i = n + ".refreshToken",
                         a = n + ".clockDrift";
                     if (this.storage.getItem(r)) {
-                        var s = new Sp({
+                        var s = new Tp({
                                 IdToken: this.storage.getItem(r)
                             }),
-                            u = new Ip({
+                            u = new Ep({
                                 AccessToken: this.storage.getItem(o)
                             }),
-                            l = new Lp({
+                            l = new Ap({
                                 RefreshToken: this.storage.getItem(i)
                             }),
                             c = parseInt(this.storage.getItem(a), 0) || 0,
-                            d = new Cp({
+                            d = new zp({
                                 IdToken: s,
                                 AccessToken: u,
                                 RefreshToken: l,
                                 ClockDrift: c
                             });
                         if (d.isValid()) return this.signInUserSession = d, e(null, this.signInUserSession);
                         if (!l.getToken()) return e(new Error("Cannot retrieve a new session. Please authenticate."), null);
@@ -66301,18 +66537,18 @@
                         t = e + "." + this.username + ".idToken",
                         n = e + "." + this.username + ".accessToken",
                         r = e + "." + this.username + ".refreshToken",
                         o = e + ".LastAuthUser",
                         i = e + "." + this.username + ".clockDrift";
                     this.storage.removeItem(t), this.storage.removeItem(n), this.storage.removeItem(r), this.storage.removeItem(o), this.storage.removeItem(i)
                 }, t.getCognitoUserSession = function(e) {
-                    var t = new Sp(e),
-                        n = new Ip(e),
-                        r = new Lp(e);
-                    return new Cp({
+                    var t = new Tp(e),
+                        n = new Ep(e),
+                        r = new Ap(e);
+                    return new zp({
                         IdToken: t,
                         AccessToken: n,
                         RefreshToken: r
                     })
                 }, t.forgotPassword = function(e, t) {
                     var n = {
                         ClientId: this.pool.getClientId(),
@@ -66499,106 +66735,106 @@
                             return e ? n.onFailure(e) : (r.signInUserSession = r.getCognitoUserSession(t.AuthenticationResult), r.cacheTokens(), n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, e
             }();
         __webpack_require__(8117);
 
-        function Bp() {}
-        Bp.prototype.userAgent = kp.userAgent;
-        var Fp = Bp;
+        function Hp() {}
+        Hp.prototype.userAgent = Op.userAgent;
+        var Zp = Hp;
 
-        function Yp(e, t) {
-            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, Hp(e, t)
+        function Vp(e, t) {
+            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, Xp(e, t)
         }
 
-        function Qp(e) {
+        function qp(e) {
             var t = "function" === typeof Map ? new Map : void 0;
-            return Qp = function(e) {
+            return qp = function(e) {
                 if (null === e || (n = e, -1 === Function.toString.call(n).indexOf("[native code]"))) return e;
                 var n;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof t) {
                     if (t.has(e)) return t.get(e);
                     t.set(e, r)
                 }
 
                 function r() {
-                    return Gp(e, arguments, Zp(this).constructor)
+                    return Jp(e, arguments, $p(this).constructor)
                 }
                 return r.prototype = Object.create(e.prototype, {
                     constructor: {
                         value: r,
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
-                }), Hp(r, e)
-            }, Qp(e)
+                }), Xp(r, e)
+            }, qp(e)
         }
 
-        function Gp(e, t, n) {
-            return Gp = Wp() ? Reflect.construct.bind() : function(e, t, n) {
+        function Jp(e, t, n) {
+            return Jp = Kp() ? Reflect.construct.bind() : function(e, t, n) {
                 var r = [null];
                 r.push.apply(r, t);
                 var o = new(Function.bind.apply(e, r));
-                return n && Hp(o, n.prototype), o
-            }, Gp.apply(null, arguments)
+                return n && Xp(o, n.prototype), o
+            }, Jp.apply(null, arguments)
         }
 
-        function Wp() {
+        function Kp() {
             if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" === typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }
 
-        function Hp(e, t) {
-            return Hp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Xp(e, t) {
+            return Xp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Hp(e, t)
+            }, Xp(e, t)
         }
 
-        function Zp(e) {
-            return Zp = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+        function $p(e) {
+            return $p = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
-            }, Zp(e)
+            }, $p(e)
         }
-        var Vp = function(e) {
+        var eh = function(e) {
                 function t(t, n, r, o) {
                     var i;
                     return (i = e.call(this, t) || this).code = n, i.name = r, i.statusCode = o, i
                 }
-                return Yp(t, e), t
-            }(Qp(Error)),
-            qp = function() {
+                return Vp(t, e), t
+            }(qp(Error)),
+            th = function() {
                 function e(e, t, n) {
                     this.endpoint = t || "https://cognito-idp." + e + ".amazonaws.com/";
                     var r = (n || {}).credentials;
                     this.fetchOptions = r ? {
                         credentials: r
                     } : {}
                 }
                 var t = e.prototype;
                 return t.promisifyRequest = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.request(e, t, (function(e, t) {
-                            e ? o(new Vp(e.message, e.code, e.name, e.statusCode)) : r(t)
+                            e ? o(new eh(e.message, e.code, e.name, e.statusCode)) : r(t)
                         }))
                     }))
                 }, t.requestWithRetry = function(e, t, n) {
                     var r = this;
                     (function(e, t, n) {
-                        void 0 === n && (n = Xp);
-                        return Kp(e, t, function(e) {
+                        void 0 === n && (n = oh);
+                        return rh(e, t, function(e) {
                             var t = 100,
                                 n = 100;
                             return function(r) {
                                 var o = Math.pow(2, r) * t + n * Math.random();
                                 return !(o > e) && o
                             }
                         }(n))
@@ -66613,15 +66849,15 @@
                     })).catch((function(e) {
                         return n(e)
                     }))
                 }, t.request = function(e, t, n) {
                     var r, o = {
                             "Content-Type": "application/x-amz-json-1.1",
                             "X-Amz-Target": "AWSCognitoIdentityProviderService." + e,
-                            "X-Amz-User-Agent": Fp.prototype.userAgent,
+                            "X-Amz-User-Agent": Zp.prototype.userAgent,
                             "Cache-Control": "no-store"
                         },
                         i = Object.assign({}, this.fetchOptions, {
                             headers: o,
                             method: "POST",
                             mode: "cors",
                             body: JSON.stringify(t)
@@ -66649,43 +66885,43 @@
                         } catch (i) {
                             return n(e)
                         } else e instanceof Error && "Network error" === e.message && (e.code = "NetworkError");
                         return n(e)
                     }))
                 }, e
             }(),
-            Jp = function() {};
+            nh = function() {};
         Error;
 
-        function Kp(e, t, n, r) {
+        function rh(e, t, n, r) {
             if (void 0 === r && (r = 1), "function" !== typeof e) throw Error("functionToRetry must be a function");
-            return Jp(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
-                if (Jp("error on " + e.name, o), (i = o) && i.nonRetryable) throw Jp(e.name + " non retryable error", o), o;
+            return nh(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
+                if (nh("error on " + e.name, o), (i = o) && i.nonRetryable) throw nh(e.name + " non retryable error", o), o;
                 var i, a = n(r, t, o);
-                if (Jp(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
+                if (nh(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
                     return setTimeout(e, a)
                 })).then((function() {
-                    return Kp(e, t, n, r + 1)
+                    return rh(e, t, n, r + 1)
                 }));
                 throw o
             }))
         }
-        var Xp = 3e5;
-        var $p, eh = function() {
+        var oh = 3e5;
+        var ih, ah = function() {
                 function e(e, t) {
                     var n = e || {},
                         r = n.UserPoolId,
                         o = n.ClientId,
                         i = n.endpoint,
                         a = n.fetchOptions,
                         s = n.AdvancedSecurityDataCollectionFlag;
                     if (!r || !o) throw new Error("Both UserPoolId and ClientId are required.");
                     if (r.length > 55 || !/^[\w-]+_[0-9a-zA-Z]+$/.test(r)) throw new Error("Invalid UserPoolId format.");
                     var u = r.split("_")[0];
-                    this.userPoolId = r, this.clientId = o, this.client = new qp(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Up).getStorage(), t && (this.wrapRefreshSessionCallback = t)
+                    this.userPoolId = r, this.clientId = o, this.client = new th(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Qp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
                 }
                 var t = e.prototype;
                 return t.getUserPoolId = function() {
                     return this.userPoolId
                 }, t.getUserPoolName = function() {
                     return this.getUserPoolId().split("_")[1]
                 }, t.getClientId = function() {
@@ -66704,15 +66940,15 @@
                         if (t) return o(t, null);
                         var r = {
                                 Username: e,
                                 Pool: a,
                                 Storage: a.storage
                             },
                             i = {
-                                user: new Rp(r),
+                                user: new Wp(r),
                                 userConfirmed: n.UserConfirmed,
                                 userSub: n.UserSub,
                                 codeDeliveryDetails: n.CodeDeliveryDetails
                             };
                         return o(null, i)
                     }))
                 }, t.getCurrentUser = function() {
@@ -66720,15 +66956,15 @@
                         t = this.storage.getItem(e);
                     if (t) {
                         var n = {
                             Username: t,
                             Pool: this,
                             Storage: this.storage
                         };
-                        return new Rp(n)
+                        return new Wp(n)
                     }
                     return null
                 }, t.getUserContextData = function(e) {
                     if ("undefined" !== typeof AmazonCognitoAdvancedSecurityData) {
                         var t = AmazonCognitoAdvancedSecurityData;
                         if (this.advancedSecurityDataCollectionFlag) {
                             var n = t.getData(e, this.userPoolId, this.clientId);
@@ -66736,16 +66972,16 @@
                                 EncodedData: n
                             }
                         }
                         return {}
                     }
                 }, e
             }(),
-            th = __webpack_require__(5943),
-            nh = function() {
+            sh = __webpack_require__(5943),
+            uh = function() {
                 function e(e) {
                     if (!e.domain) throw new Error("The domain of cookieStorage can not be undefined.");
                     if (this.domain = e.domain, e.path ? this.path = e.path : this.path = "/", Object.prototype.hasOwnProperty.call(e, "expires") ? this.expires = e.expires : this.expires = 365, Object.prototype.hasOwnProperty.call(e, "secure") ? this.secure = e.secure : this.secure = !0, Object.prototype.hasOwnProperty.call(e, "sameSite")) {
                         if (!["strict", "lax", "none"].includes(e.sameSite)) throw new Error('The sameSite value of cookieStorage must be "lax", "strict" or "none".');
                         if ("none" === e.sameSite && !this.secure) throw new Error("sameSite = None requires the Secure attribute in latest browser versions.");
                         this.sameSite = e.sameSite
                     } else this.sameSite = null
@@ -66754,116 +66990,116 @@
                 return t.setItem = function(e, t) {
                     var n = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (n.sameSite = this.sameSite), th.set(e, t, n), th.get(e)
+                    return this.sameSite && (n.sameSite = this.sameSite), sh.set(e, t, n), sh.get(e)
                 }, t.getItem = function(e) {
-                    return th.get(e)
+                    return sh.get(e)
                 }, t.removeItem = function(e) {
                     var t = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (t.sameSite = this.sameSite), th.remove(e, t)
+                    return this.sameSite && (t.sameSite = this.sameSite), sh.remove(e, t)
                 }, t.clear = function() {
-                    for (var e = th.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
+                    for (var e = sh.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
                     return {}
                 }, e
             }(),
-            rh = __webpack_require__(2770),
-            oh = function(e) {
+            lh = __webpack_require__(2770),
+            ch = function(e) {
                 var t = window.open(e, "_self");
                 return t ? Promise.resolve(t) : Promise.reject()
             },
-            ih = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            ah = function(e, t, n) {
-                Ps.dispatch("auth", {
+            dh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            fh = function(e, t, n) {
+                Gs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", ih)
+                }, "Auth", dh)
             },
-            sh = new As("OAuth"),
-            uh = function() {
+            ph = new Bs("OAuth"),
+            hh = function() {
                 function e(e) {
                     var t = e.config,
                         n = e.cognitoClientId,
                         r = e.scopes,
                         o = void 0 === r ? [] : r;
-                    if (this._urlOpener = t.urlOpener || oh, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
+                    if (this._urlOpener = t.urlOpener || ch, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
                     this._scopes = o
                 }
                 return e.prototype.isValidScopes = function(e) {
                     return Array.isArray(e) && e.every((function(e) {
                         return "string" === typeof e
                     }))
                 }, e.prototype.oauthSignIn = function(e, t, n, r, o, i) {
-                    void 0 === e && (e = "code"), void 0 === o && (o = ys.Cognito);
+                    void 0 === e && (e = "code"), void 0 === o && (o = js.Cognito);
                     var a = this._generateState(32),
                         s = i ? a + "-" + i.split("").map((function(e) {
                             return e.charCodeAt(0).toString(16).padStart(2, "0")
                         })).join("") : a;
                     ! function(e) {
                         window.sessionStorage.setItem("oauth_state", e)
                     }(s);
                     var u, l = this._generateRandom(128);
                     u = l, window.sessionStorage.setItem("ouath_pkce_key", u);
                     var c = this._generateChallenge(l),
                         d = this._scopes.join(" "),
-                        f = Object.entries(Ms(Ms({
+                        f = Object.entries(Is(Is({
                             redirect_uri: n,
                             response_type: e,
                             client_id: r,
                             identity_provider: o,
                             scope: d,
                             state: s
                         }, "code" === e ? {
                             code_challenge: c
                         } : {}), "code" === e ? {
                             code_challenge_method: "S256"
                         } : {})).map((function(e) {
-                            var t = js(e, 2),
+                            var t = Ls(e, 2),
                                 n = t[0],
                                 r = t[1];
                             return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                         })).join("&"),
                         p = "https://" + t + "/oauth2/authorize?" + f;
-                    sh.debug("Redirecting to " + p), this._urlOpener(p, n)
+                    ph.debug("Redirecting to " + p), this._urlOpener(p, n)
                 }, e.prototype._handleCodeFlow = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return ws(this, (function(g) {
+                        return Ss(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    return t = ((0, rh.Qc)(e).query || "").split("&").map((function(e) {
+                                    return t = ((0, lh.Qc)(e).query || "").split("&").map((function(e) {
                                         return e.split("=")
                                     })).reduce((function(e, t) {
-                                        var n, r = js(t, 2),
+                                        var n, r = Ls(t, 2),
                                             o = r[0],
                                             i = r[1];
-                                        return Ms(Ms({}, e), ((n = {})[o] = i, n))
+                                        return Is(Is({}, e), ((n = {})[o] = i, n))
                                     }), {
                                         code: void 0
-                                    }).code, n = (0, rh.Qc)(e).pathname || "/", r = (0, rh.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", ah("codeFlow", {}, "Retrieving tokens from " + o), i = Ns(this._config) ? this._cognitoClientId : this._config.clientID, a = Ns(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
+                                    }).code, n = (0, lh.Qc)(e).pathname || "/", r = (0, lh.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", fh("codeFlow", {}, "Retrieving tokens from " + o), i = Cs(this._config) ? this._cognitoClientId : this._config.clientID, a = Cs(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
                                         var e = window.sessionStorage.getItem("ouath_pkce_key");
                                         return window.sessionStorage.removeItem("ouath_pkce_key"), e
-                                    }(), u = Ms({
+                                    }(), u = Is({
                                         grant_type: "authorization_code",
                                         code: t,
                                         client_id: i,
                                         redirect_uri: a
                                     }, s ? {
                                         code_verifier: s
-                                    } : {}), sh.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
-                                        var t = js(e, 2),
+                                    } : {}), ph.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
+                                        var t = Ls(e, 2),
                                             n = t[0],
                                             r = t[1];
                                         return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                                     })).join("&"), [4, fetch(o, {
                                         method: "POST",
                                         headers: {
                                             "Content-Type": "application/x-www-form-urlencoded"
@@ -66879,70 +67115,70 @@
                                         refreshToken: f,
                                         idToken: p
                                     }]
                             }
                         }))
                     }))
                 }, e.prototype._handleImplicitFlow = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r;
-                        return ws(this, (function(o) {
-                            return t = ((0, rh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                        return Ss(this, (function(o) {
+                            return t = ((0, lh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                 return e.split("=")
                             })).reduce((function(e, t) {
-                                var n, r = js(t, 2),
+                                var n, r = Ls(t, 2),
                                     o = r[0],
                                     i = r[1];
-                                return Ms(Ms({}, e), ((n = {})[o] = i, n))
+                                return Is(Is({}, e), ((n = {})[o] = i, n))
                             }), {
                                 id_token: void 0,
                                 access_token: void 0
-                            }), n = t.id_token, r = t.access_token, ah("implicitFlow", {}, "Got tokens from " + e), sh.debug("Retrieving implicit tokens from " + e + " with"), [2, {
+                            }), n = t.id_token, r = t.access_token, fh("implicitFlow", {}, "Got tokens from " + e), ph.debug("Retrieving implicit tokens from " + e + " with"), [2, {
                                 accessToken: r,
                                 idToken: n,
                                 refreshToken: null
                             }]
                         }))
                     }))
                 }, e.prototype.handleAuthResponse = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s;
-                        return ws(this, (function(u) {
+                        return Ss(this, (function(u) {
                             switch (u.label) {
                                 case 0:
-                                    if (u.trys.push([0, 5, , 6]), t = e ? Ms(Ms({}, ((0, rh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                                    if (u.trys.push([0, 5, , 6]), t = e ? Is(Is({}, ((0, lh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = js(t, 2),
+                                            var n = Ls(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
-                                        }), {})), ((0, rh.Qc)(e).query || "").split("&").map((function(e) {
+                                        }), {})), ((0, lh.Qc)(e).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = js(t, 2),
+                                            var n = Ls(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
                                         }), {})) : {}, n = t.error, r = t.error_description, n) throw new Error(r);
-                                    return o = this._validateState(t), sh.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
+                                    return o = this._validateState(t), ph.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
                                 case 1:
-                                    return [2, Ms.apply(void 0, [Ms.apply(void 0, i.concat([u.sent()])), {
+                                    return [2, Is.apply(void 0, [Is.apply(void 0, i.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 2:
                                     return a = [{}], [4, this._handleImplicitFlow(e)];
                                 case 3:
-                                    return [2, Ms.apply(void 0, [Ms.apply(void 0, a.concat([u.sent()])), {
+                                    return [2, Is.apply(void 0, [Is.apply(void 0, a.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 4:
                                     return [3, 6];
                                 case 5:
-                                    throw s = u.sent(), sh.error("Error handling auth response.", s), s;
+                                    throw s = u.sent(), ph.error("Error handling auth response.", s), s;
                                 case 6:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._validateState = function(e) {
                     if (e) {
@@ -66951,33 +67187,33 @@
                                 return window.sessionStorage.removeItem("oauth_state"), e
                             }(),
                             n = e.state;
                         if (t && t !== n) throw new Error("Invalid state in OAuth flow");
                         return n
                     }
                 }, e.prototype.signOut = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t, n;
-                        return ws(this, (function(r) {
-                            return e = "https://" + this._config.domain + "/logout?", t = Ns(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Ns(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
+                        return Ss(this, (function(r) {
+                            return e = "https://" + this._config.domain + "/logout?", t = Cs(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Cs(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
                                 client_id: t,
                                 logout_uri: encodeURIComponent(n)
                             }).map((function(e) {
-                                var t = js(e, 2);
+                                var t = Ls(e, 2);
                                 return t[0] + "=" + t[1]
-                            })).join("&"), ah("oAuthSignOut", {
+                            })).join("&"), fh("oAuthSignOut", {
                                 oAuth: "signOut"
-                            }, "Signing out from " + e), sh.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
+                            }, "Signing out from " + e), ph.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
                         }))
                     }))
                 }, e.prototype._generateState = function(e) {
                     for (var t = "", n = e, r = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"; n > 0; --n) t += r[Math.round(Math.random() * (r.length - 1))];
                     return t
                 }, e.prototype._generateChallenge = function(e) {
-                    var t = new sp.Sha256;
+                    var t = new pp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
                         r = nt.lW.from(n).toString("base64");
                     return this._base64URL(r)
                 }, e.prototype._base64URL = function(e) {
                     return e.replace(/=/g, "").replace(/\+/g, "-").replace(/\//g, "_")
                 }, e.prototype._generateRandom = function(e) {
@@ -66990,104 +67226,104 @@
                     for (var t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", n = [], r = 0; r < e.byteLength; r += 1) {
                         var o = e[r] % t.length;
                         n.push(t[o])
                     }
                     return n.join("")
                 }, e
             }(),
-            lh = uh;
+            gh = hh;
         ! function(e) {
             e.DEFAULT_MSG = "Authentication Error", e.EMPTY_EMAIL = "Email cannot be empty", e.EMPTY_PHONE = "Phone number cannot be empty", e.EMPTY_USERNAME = "Username cannot be empty", e.INVALID_USERNAME = "The username should either be a string or one of the sign in types", e.EMPTY_PASSWORD = "Password cannot be empty", e.EMPTY_CODE = "Confirmation code cannot be empty", e.SIGN_UP_ERROR = "Error creating account", e.NO_MFA = "No valid MFA method provided", e.INVALID_MFA = "Invalid MFA type", e.EMPTY_CHALLENGE = "Challenge response cannot be empty", e.NO_USER_SESSION = "Failed to get the session because the user is empty", e.NETWORK_ERROR = "Network Error", e.DEVICE_CONFIG = "Device tracking has not been configured in this User Pool", e.AUTOSIGNIN_ERROR = "Please use your credentials to sign in"
-        }($p || ($p = {}));
-        var ch = new As("AuthError"),
-            dh = function(e) {
+        }(ih || (ih = {}));
+        var yh = new Bs("AuthError"),
+            mh = function(e) {
                 function t(n) {
                     var r = this,
-                        o = ph[n],
+                        o = Mh[n],
                         i = o.message,
                         a = o.log;
-                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, ch.error(r.log), r
+                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, yh.error(r.log), r
                 }
-                return gs(t, e), t
+                return ws(t, e), t
             }(Error),
-            fh = function(e) {
+            vh = function(e) {
                 function t(n) {
                     var r = e.call(this, n) || this;
                     return r.constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "NoUserPoolError", r
                 }
-                return gs(t, e), t
-            }(dh),
-            ph = {
+                return ws(t, e), t
+            }(mh),
+            Mh = {
                 noConfig: {
-                    message: $p.DEFAULT_MSG,
+                    message: ih.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly.\n            This error is typically caused by one of the following scenarios:\n\n            1. Make sure you're passing the awsconfig object to Amplify.configure() in your app's entry point\n                See https://aws-amplify.github.io/docs/js/authentication#configure-your-app for more information\n            \n            2. There might be multiple conflicting versions of amplify packages in your node_modules.\n\t\t\t\tRefer to our docs site for help upgrading Amplify packages (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js)\n        "
                 },
                 missingAuthConfig: {
-                    message: $p.DEFAULT_MSG,
+                    message: ih.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly. \n            The configuration object is missing required auth properties.\n            This error is typically caused by one of the following scenarios:\n\n            1. Did you run `amplify push` after adding auth via `amplify add auth`?\n                See https://aws-amplify.github.io/docs/js/authentication#amplify-project-setup for more information\n\n            2. This could also be caused by multiple conflicting versions of amplify packages, see (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js) for help upgrading Amplify packages.\n        "
                 },
                 emptyUsername: {
-                    message: $p.EMPTY_USERNAME
+                    message: ih.EMPTY_USERNAME
                 },
                 invalidUsername: {
-                    message: $p.INVALID_USERNAME
+                    message: ih.INVALID_USERNAME
                 },
                 emptyPassword: {
-                    message: $p.EMPTY_PASSWORD
+                    message: ih.EMPTY_PASSWORD
                 },
                 emptyCode: {
-                    message: $p.EMPTY_CODE
+                    message: ih.EMPTY_CODE
                 },
                 signUpError: {
-                    message: $p.SIGN_UP_ERROR,
+                    message: ih.SIGN_UP_ERROR,
                     log: "The first parameter should either be non-null string or object"
                 },
                 noMFA: {
-                    message: $p.NO_MFA
+                    message: ih.NO_MFA
                 },
                 invalidMFA: {
-                    message: $p.INVALID_MFA
+                    message: ih.INVALID_MFA
                 },
                 emptyChallengeResponse: {
-                    message: $p.EMPTY_CHALLENGE
+                    message: ih.EMPTY_CHALLENGE
                 },
                 noUserSession: {
-                    message: $p.NO_USER_SESSION
+                    message: ih.NO_USER_SESSION
                 },
                 deviceConfig: {
-                    message: $p.DEVICE_CONFIG
+                    message: ih.DEVICE_CONFIG
                 },
                 networkError: {
-                    message: $p.NETWORK_ERROR
+                    message: ih.NETWORK_ERROR
                 },
                 autoSignInError: {
-                    message: $p.AUTOSIGNIN_ERROR
+                    message: ih.AUTOSIGNIN_ERROR
                 },
                 default: {
-                    message: $p.DEFAULT_MSG
+                    message: ih.DEFAULT_MSG
                 }
             },
-            hh = new As("AuthClass"),
-            gh = "aws.cognito.signin.user.admin",
-            yh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            mh = function(e, t, n) {
-                Ps.dispatch("auth", {
+            bh = new Bs("AuthClass"),
+            wh = "aws.cognito.signin.user.admin",
+            jh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            xh = function(e, t, n) {
+                Gs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", yh)
+                }, "Auth", jh)
             },
-            vh = function() {
+            Nh = function() {
                 function e(e) {
                     var t = this;
-                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = Xf, this.wrapRefreshSessionCallback = function(e) {
+                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = op, this.wrapRefreshSessionCallback = function(e) {
                         return function(t, n) {
-                            return n ? mh("tokenRefresh", void 0, "New token retrieved") : mh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
+                            return n ? xh("tokenRefresh", void 0, "New token retrieved") : xh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
                         }
-                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), Ps.listen("auth", (function(e) {
+                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), Gs.listen("auth", (function(e) {
                         switch (e.payload.event) {
                             case "verify":
                             case "signIn":
                                 t._storage.setItem("amplify-signin-with-hostedUI", "false");
                                 break;
                             case "signOut":
                                 t._storage.removeItem("amplify-signin-with-hostedUI");
@@ -67098,80 +67334,80 @@
                     }))
                 }
                 return e.prototype.getModuleName = function() {
                     return "Auth"
                 }, e.prototype.configure = function(e) {
                     var t = this;
                     if (!e) return this._config || {};
-                    hh.debug("configure Auth");
-                    var n = Object.assign({}, this._config, Dc(e).Auth, e);
+                    bh.debug("configure Auth");
+                    var n = Object.assign({}, this._config, _c(e).Auth, e);
                     this._config = n;
                     var r = this._config,
                         o = r.userPoolId,
                         i = r.userPoolWebClientId,
                         a = r.cookieStorage,
                         s = r.oauth,
                         u = r.region,
                         l = r.identityPoolId,
                         c = r.mandatorySignIn,
                         d = r.refreshHandlers,
                         f = r.identityPoolRegion,
                         p = r.clientMetadata,
                         h = r.endpoint;
                     if (this._config.storage) {
-                        if (!this._isValidAuthStorage(this._config.storage)) throw hh.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
+                        if (!this._isValidAuthStorage(this._config.storage)) throw bh.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
                         this._storage = this._config.storage
-                    } else this._storage = a ? new nh(a) : e.ssr ? new ep : (new Fs).getStorage();
+                    } else this._storage = a ? new uh(a) : e.ssr ? new ap : (new Zs).getStorage();
                     if (this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), o) {
                         var g = {
                             UserPoolId: o,
                             ClientId: i,
                             endpoint: h
                         };
-                        g.Storage = this._storage, this.userPool = new eh(g, this.wrapRefreshSessionCallback)
+                        g.Storage = this._storage, this.userPool = new ah(g, this.wrapRefreshSessionCallback)
                     }
                     this.Credentials.configure({
                         mandatorySignIn: c,
                         region: u,
                         userPoolId: o,
                         identityPoolId: l,
                         refreshHandlers: d,
                         storage: this._storage,
                         identityPoolRegion: f
                     });
-                    var y = s ? Ns(this._config.oauth) ? s : s.awsCognito : void 0;
+                    var y = s ? Cs(this._config.oauth) ? s : s.awsCognito : void 0;
                     if (y) {
                         var m = Object.assign({
                             cognitoClientId: i,
                             UserPoolId: o,
                             domain: y.domain,
                             scopes: y.scope,
                             redirectSignIn: y.redirectSignIn,
                             redirectSignOut: y.redirectSignOut,
                             responseType: y.responseType,
                             Storage: this._storage,
                             urlOpener: y.urlOpener,
                             clientMetadata: p
                         }, y.options);
-                        this._oAuthHandler = new lh({
+                        this._oAuthHandler = new gh({
                             scopes: m.scopes,
                             config: m,
                             cognitoClientId: m.cognitoClientId
                         });
                         var v = {};
                         ! function(e) {
-                            if (Ys().isBrowser && window.location) e({
+                            if (Vs().isBrowser && window.location) e({
                                 url: window.location.href
                             });
-                            else if (!Ys().isNode) throw new Error("Not supported")
+                            else if (!Vs().isNode) throw new Error("Not supported")
                         }((function(e) {
                             var n = e.url;
                             v[n] || (v[n] = !0, t._handleAuthResponse(n))
                         }))
-                    }(mh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (mh("autoSignIn_failure", null, ms.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
+                    }(xh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (xh("autoSignIn_failure", null, xs.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
                     return this._config
                 }, e.prototype.signUp = function(e) {
                     for (var t, n, r, o = this, i = [], a = 1; a < arguments.length; a++) i[a - 1] = arguments[a];
                     if (!this.userPool) return this.rejectNoUserPool();
                     var s, u = null,
                         l = null,
                         c = [],
@@ -67181,187 +67417,187 @@
                         },
                         p = {},
                         h = {};
                     if (e && "string" === typeof e) {
                         u = e, l = i ? i[0] : null;
                         var g = i ? i[1] : null,
                             y = i ? i[2] : null;
-                        g && c.push(new Ap({
+                        g && c.push(new Bp({
                             Name: "email",
                             Value: g
-                        })), y && c.push(new Ap({
+                        })), y && c.push(new Bp({
                             Name: "phone_number",
                             Value: y
                         }))
                     } else {
-                        if (!e || "object" !== typeof e) return this.rejectAuthError(ms.SignUpError);
+                        if (!e || "object" !== typeof e) return this.rejectAuthError(xs.SignUpError);
                         u = e.username, l = e.password, e && e.clientMetadata ? s = e.clientMetadata : this._config.clientMetadata && (s = this._config.clientMetadata);
                         var m = e.attributes;
                         m && Object.keys(m).map((function(e) {
-                            c.push(new Ap({
+                            c.push(new Bp({
                                 Name: e,
                                 Value: m[e]
                             }))
                         }));
                         var v = e.validationData;
                         v && (d = [], Object.keys(v).map((function(e) {
-                            d.push(new Ap({
+                            d.push(new Bp({
                                 Name: e,
                                 Value: v[e]
                             }))
                         }))), (f = null !== (t = e.autoSignIn) && void 0 !== t ? t : {
                             enabled: !1
                         }).enabled && (this._storage.setItem("amplify-auto-sign-in", "true"), p = null !== (n = f.validationData) && void 0 !== n ? n : {}, h = null !== (r = f.clientMetaData) && void 0 !== r ? r : {})
                     }
-                    return u ? l ? (hh.debug("signUp attrs:", c), hh.debug("signUp validation data:", d), new Promise((function(e, t) {
+                    return u ? l ? (bh.debug("signUp attrs:", c), bh.debug("signUp validation data:", d), new Promise((function(e, t) {
                         o.userPool.signUp(u, l, c, d, (function(n, r) {
-                            n ? (mh("signUp_failure", n, u + " failed to signup"), t(n)) : (mh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
+                            n ? (xh("signUp_failure", n, u + " failed to signup"), t(n)) : (xh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
                         }), s)
-                    }))) : this.rejectAuthError(ms.EmptyPassword) : this.rejectAuthError(ms.EmptyUsername)
+                    }))) : this.rejectAuthError(xs.EmptyPassword) : this.rejectAuthError(xs.EmptyUsername)
                 }, e.prototype.handleAutoSignIn = function(e, t, n, r, o) {
                     this.autoSignInInitiated = !0;
-                    var i = new np({
+                    var i = new up({
                         Username: e,
                         Password: t,
                         ValidationData: n,
                         ClientMetadata: r
                     });
                     o.userConfirmed ? this.signInAfterUserConfirmed(i) : "link" === this._config.signUpVerificationMethod ? this.handleLinkAutoSignIn(i) : this.handleCodeAutoSignIn(i)
                 }, e.prototype.handleCodeAutoSignIn = function(e) {
                     var t = this;
-                    Ps.listen("auth", (function n(r) {
+                    Gs.listen("auth", (function n(r) {
                         "confirmSignUp" === r.payload.event && t.signInAfterUserConfirmed(e, n)
                     }))
                 }, e.prototype.handleLinkAutoSignIn = function(e) {
                     var t = this;
                     this._storage.setItem("amplify-polling-started", "true");
                     var n = Date.now(),
                         r = setInterval((function() {
-                            Date.now() - n > 18e4 ? (clearInterval(r), mh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
+                            Date.now() - n > 18e4 ? (clearInterval(r), xh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
                         }), 5e3)
                 }, e.prototype.signInAfterUserConfirmed = function(e, t, n) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var r, o, i = this;
-                        return ws(this, (function(a) {
+                        return Ss(this, (function(a) {
                             switch (a.label) {
                                 case 0:
                                     r = this.createCognitoUser(e.getUsername()), a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, r.authenticateUser(e, this.authCallbacks(r, (function(r) {
-                                        mh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && Ps.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
+                                        xh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && Gs.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
                                     }), (function(e) {
-                                        hh.error(e), i._storage.removeItem("amplify-auto-sign-in")
+                                        bh.error(e), i._storage.removeItem("amplify-auto-sign-in")
                                     })))];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    return o = a.sent(), hh.error(o), [3, 4];
+                                    return o = a.sent(), bh.error(o), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.confirmSignUp = function(e, t, n) {
                     var r = this;
                     if (!this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ms.EmptyUsername);
-                    if (!t) return this.rejectAuthError(ms.EmptyCode);
+                    if (!e) return this.rejectAuthError(xs.EmptyUsername);
+                    if (!t) return this.rejectAuthError(xs.EmptyCode);
                     var o, i = this.createCognitoUser(e),
                         a = !n || "boolean" !== typeof n.forceAliasCreation || n.forceAliasCreation;
                     return n && n.clientMetadata ? o = n.clientMetadata : this._config.clientMetadata && (o = this._config.clientMetadata), new Promise((function(n, s) {
                         i.confirmRegistration(t, a, (function(t, o) {
-                            t ? s(t) : (mh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (mh("autoSignIn_failure", null, ms.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
+                            t ? s(t) : (xh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (xh("autoSignIn_failure", null, xs.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
                         }), o)
                     }))
                 }, e.prototype.isTrueStorageValue = function(e) {
                     var t = this._storage.getItem(e);
                     return !!t && "true" === t
                 }, e.prototype.resendSignUp = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ms.EmptyUsername);
+                    if (!e) return this.rejectAuthError(xs.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(e, r) {
                         n.resendConfirmationCode((function(t, n) {
                             t ? r(t) : e(n)
                         }), t)
                     }))
                 }, e.prototype.signIn = function(e, t, n) {
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
                     var r = null,
                         o = null,
                         i = {};
                     if ("string" === typeof e) r = e, o = t;
                     else {
-                        if (!e.username) return this.rejectAuthError(ms.InvalidUsername);
-                        "undefined" !== typeof t && hh.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
+                        if (!e.username) return this.rejectAuthError(xs.InvalidUsername);
+                        "undefined" !== typeof t && bh.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
                     }
-                    if (!r) return this.rejectAuthError(ms.EmptyUsername);
-                    var a = new np({
+                    if (!r) return this.rejectAuthError(xs.EmptyUsername);
+                    var a = new up({
                         Username: r,
                         Password: o,
                         ValidationData: i,
                         ClientMetadata: n
                     });
                     return o ? this.signInWithPassword(a) : this.signInWithoutPassword(a)
                 }, e.prototype.authCallbacks = function(e, t, n) {
                     var r = this,
                         o = this;
                     return {
                         onSuccess: function(i) {
-                            return bs(r, void 0, void 0, (function() {
+                            return Ds(r, void 0, void 0, (function() {
                                 var r, a, s, u;
-                                return ws(this, (function(l) {
+                                return Ss(this, (function(l) {
                                     switch (l.label) {
                                         case 0:
-                                            hh.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
+                                            bh.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
                                         case 1:
                                             return l.trys.push([1, 4, 5, 9]), [4, this.Credentials.clear()];
                                         case 2:
                                             return l.sent(), [4, this.Credentials.set(i, "session")];
                                         case 3:
-                                            return r = l.sent(), hh.debug("succeed to get cognito credentials", r), [3, 9];
+                                            return r = l.sent(), bh.debug("succeed to get cognito credentials", r), [3, 9];
                                         case 4:
-                                            return a = l.sent(), hh.debug("cannot get cognito credentials", a), [3, 9];
+                                            return a = l.sent(), bh.debug("cannot get cognito credentials", a), [3, 9];
                                         case 5:
                                             return l.trys.push([5, 7, , 8]), [4, this.currentUserPoolUser()];
                                         case 6:
-                                            return s = l.sent(), o.user = s, mh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
+                                            return s = l.sent(), o.user = s, xh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
                                         case 7:
-                                            return u = l.sent(), hh.error("Failed to get the signed in user", u), n(u), [3, 8];
+                                            return u = l.sent(), bh.error("Failed to get the signed in user", u), n(u), [3, 8];
                                         case 8:
                                             return [7];
                                         case 9:
                                             return [2]
                                     }
                                 }))
                             }))
                         },
                         onFailure: function(t) {
-                            hh.debug("signIn failure", t), mh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
+                            bh.debug("signIn failure", t), xh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
                         },
                         customChallenge: function(n) {
-                            hh.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
+                            bh.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
                         },
                         mfaRequired: function(n, r) {
-                            hh.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
+                            bh.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         mfaSetup: function(n, r) {
-                            hh.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            bh.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         newPasswordRequired: function(n, r) {
-                            hh.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
+                            bh.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
                                 userAttributes: n,
                                 requiredAttributes: r
                             }, t(e)
                         },
                         totpRequired: function(n, r) {
-                            hh.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
+                            bh.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         selectMFAType: function(n, r) {
-                            hh.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            bh.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
                         }
                     }
                 }, e.prototype.signInWithPassword = function(e) {
                     var t = this;
                     if (this.pendingSignIn) throw new Error("Pending sign-in attempt already in progress");
                     var n = this.createCognitoUser(e.getUsername());
                     return this.pendingSignIn = new Promise((function(r, o) {
@@ -67376,32 +67612,32 @@
                         n = this.createCognitoUser(e.getUsername());
                     return n.setAuthenticationFlowType("CUSTOM_AUTH"), new Promise((function(r, o) {
                         n.initiateAuth(e, t.authCallbacks(n, r, o))
                     }))
                 }, e.prototype.getMFAOptions = function(e) {
                     return new Promise((function(t, n) {
                         e.getMFAOptions((function(e, r) {
-                            if (e) return hh.debug("get MFA Options failed", e), void n(e);
-                            hh.debug("get MFA options success", r), t(r)
+                            if (e) return bh.debug("get MFA Options failed", e), void n(e);
+                            bh.debug("get MFA options success", r), t(r)
                         }))
                     }))
                 }, e.prototype.getPreferredMFA = function(e, t) {
                     var n = this,
                         r = this;
                     return new Promise((function(o, i) {
                         var a = n._config.clientMetadata,
                             s = !!t && t.bypassCache;
                         e.getUserData((function(t, a) {
-                            return bs(n, void 0, void 0, (function() {
+                            return Ds(n, void 0, void 0, (function() {
                                 var n, s;
-                                return ws(this, (function(u) {
+                                return Ss(this, (function(u) {
                                     switch (u.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (hh.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (bh.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             u.label = 1;
                                         case 1:
                                             return u.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return u.sent(), [3, 4];
                                         case 3:
                                             return n = u.sent(), i(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -67419,29 +67655,29 @@
                     }))
                 }, e.prototype._getMfaTypeFromUserData = function(e) {
                     var t = null,
                         n = e.PreferredMfaSetting;
                     if (n) t = n;
                     else {
                         var r = e.UserMFASettingList;
-                        if (r) 0 === r.length ? t = "NOMFA" : hh.debug("invalid case for getPreferredMFA", e);
+                        if (r) 0 === r.length ? t = "NOMFA" : bh.debug("invalid case for getPreferredMFA", e);
                         else t = e.MFAOptions ? "SMS_MFA" : "NOMFA"
                     }
                     return t
                 }, e.prototype._getUserData = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         e.getUserData((function(t, i) {
-                            return bs(n, void 0, void 0, (function() {
+                            return Ds(n, void 0, void 0, (function() {
                                 var n;
-                                return ws(this, (function(a) {
+                                return Ss(this, (function(a) {
                                     switch (a.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (hh.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (bh.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             a.label = 1;
                                         case 1:
                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return a.sent(), [3, 4];
                                         case 3:
                                             return n = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -67453,17 +67689,17 @@
                                             return [2]
                                     }
                                 }))
                             }))
                         }), t)
                     }))
                 }, e.prototype.setPreferredMFA = function(e, t) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u = this;
-                        return ws(this, (function(l) {
+                        return Ss(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return n = this._config.clientMetadata, [4, this._getUserData(e, {
                                         bypassCache: !0,
                                         clientMetadata: n
                                     })];
                                 case 1:
@@ -67493,15 +67729,15 @@
                                 case 5:
                                     if ("NOMFA" === (s = l.sent())) return [2, Promise.resolve("No change for mfa type")];
                                     if ("SMS_MFA" === s) o = {
                                         PreferredMfa: !1,
                                         Enabled: !1
                                     };
                                     else {
-                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(ms.InvalidMFA)];
+                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(xs.InvalidMFA)];
                                         i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         }
                                     }
                                     return a && 0 !== a.length && a.forEach((function(e) {
                                         "SMS_MFA" === e ? o = {
@@ -67509,27 +67745,27 @@
                                             Enabled: !1
                                         } : "SOFTWARE_TOKEN_MFA" === e && (i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         })
                                     })), [3, 7];
                                 case 6:
-                                    return hh.debug("no validmfa method provided"), [2, this.rejectAuthError(ms.NoMFA)];
+                                    return bh.debug("no validmfa method provided"), [2, this.rejectAuthError(xs.NoMFA)];
                                 case 7:
                                     return this, [2, new Promise((function(t, r) {
                                         e.setUserMfaPreference(o, i, (function(o, i) {
-                                            if (o) return hh.debug("Set user mfa preference error", o), r(o);
-                                            hh.debug("Set user mfa success", i), hh.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
-                                                return bs(u, void 0, void 0, (function() {
+                                            if (o) return bh.debug("Set user mfa preference error", o), r(o);
+                                            bh.debug("Set user mfa success", i), bh.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
+                                                return Ds(u, void 0, void 0, (function() {
                                                     var o;
-                                                    return ws(this, (function(a) {
+                                                    return Ss(this, (function(a) {
                                                         switch (a.label) {
                                                             case 0:
                                                                 if (!n) return [3, 5];
-                                                                if (hh.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
+                                                                if (bh.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
                                                                 a.label = 1;
                                                             case 1:
                                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                             case 2:
                                                                 return a.sent(), [3, 4];
                                                             case 3:
                                                                 return o = a.sent(), r(new Error("Session is invalid due to: " + n.message + " and failed to clean up invalid session: " + o.message)), [2];
@@ -67548,195 +67784,195 @@
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.disableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.disableMFA((function(e, r) {
-                            if (e) return hh.debug("disable mfa failed", e), void n(e);
-                            hh.debug("disable mfa succeed", r), t(r)
+                            if (e) return bh.debug("disable mfa failed", e), void n(e);
+                            bh.debug("disable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.enableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.enableMFA((function(e, r) {
-                            if (e) return hh.debug("enable mfa failed", e), void n(e);
-                            hh.debug("enable mfa succeed", r), t(r)
+                            if (e) return bh.debug("enable mfa failed", e), void n(e);
+                            bh.debug("enable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.setupTOTP = function(e) {
                     return new Promise((function(t, n) {
                         e.associateSoftwareToken({
                             onFailure: function(e) {
-                                hh.debug("associateSoftwareToken failed", e), n(e)
+                                bh.debug("associateSoftwareToken failed", e), n(e)
                             },
                             associateSecretCode: function(e) {
-                                hh.debug("associateSoftwareToken sucess", e), t(e)
+                                bh.debug("associateSoftwareToken sucess", e), t(e)
                             }
                         })
                     }))
                 }, e.prototype.verifyTotpToken = function(e, t) {
-                    return hh.debug("verification totp token", e, t), new Promise((function(n, r) {
+                    return bh.debug("verification totp token", e, t), new Promise((function(n, r) {
                         e.verifySoftwareToken(t, "My TOTP device", {
                             onFailure: function(e) {
-                                hh.debug("verifyTotpToken failed", e), r(e)
+                                bh.debug("verifyTotpToken failed", e), r(e)
                             },
                             onSuccess: function(t) {
-                                mh("signIn", e, "A user " + e.getUsername() + " has been signed in"), mh("verify", e, "A user " + e.getUsername() + " has been verified"), hh.debug("verifyTotpToken success", t), n(t)
+                                xh("signIn", e, "A user " + e.getUsername() + " has been signed in"), xh("verify", e, "A user " + e.getUsername() + " has been verified"), bh.debug("verifyTotpToken success", t), n(t)
                             }
                         })
                     }))
                 }, e.prototype.confirmSignIn = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(ms.EmptyCode);
+                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(xs.EmptyCode);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.sendMFACode(t, {
                             onSuccess: function(t) {
-                                return bs(o, void 0, void 0, (function() {
+                                return Ds(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return ws(this, (function(o) {
+                                    return Ss(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                hh.debug(t), o.label = 1;
+                                                bh.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), hh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), bh.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), hh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), bh.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, mh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, xh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                hh.debug("confirm signIn failure", e), s(e)
+                                bh.debug("confirm signIn failure", e), s(e)
                             }
                         }, n, r)
                     }))
                 }, e.prototype.completeNewPassword = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(ms.EmptyPassword);
+                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(xs.EmptyPassword);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.completeNewPasswordChallenge(t, n, {
                             onSuccess: function(t) {
-                                return bs(o, void 0, void 0, (function() {
+                                return Ds(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return ws(this, (function(o) {
+                                    return Ss(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                hh.debug(t), o.label = 1;
+                                                bh.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), hh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), bh.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), hh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), bh.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, mh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, xh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                hh.debug("completeNewPassword failure", e), mh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
+                                bh.debug("completeNewPassword failure", e), xh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
                             },
                             mfaRequired: function(t, n) {
-                                hh.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
+                                bh.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             mfaSetup: function(t, n) {
-                                hh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                bh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             totpRequired: function(t, n) {
-                                hh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                bh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             }
                         }, r)
                     }))
                 }, e.prototype.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this;
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!t) return this.rejectAuthError(ms.EmptyChallengeResponse);
+                    if (!t) return this.rejectAuthError(xs.EmptyChallengeResponse);
                     return new Promise((function(o, i) {
                         e.sendCustomChallengeAnswer(t, r.authCallbacks(e, o, i), n)
                     }))
                 }, e.prototype.deleteUserAttributes = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.userSession(e).then((function(n) {
                             e.deleteAttributes(t, (function(e, t) {
                                 return e ? o(e) : r(t)
                             }))
                         }))
                     }))
                 }, e.prototype.deleteUser = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return ws(this, (function(r) {
+                        return Ss(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     return r.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return r.sent(), [3, 3];
                                 case 2:
-                                    throw e = r.sent(), hh.debug("Failed to sync cache info into memory", e), new Error(e);
+                                    throw e = r.sent(), bh.debug("Failed to sync cache info into memory", e), new Error(e);
                                 case 3:
                                     return t = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(e, r) {
-                                        return bs(n, void 0, void 0, (function() {
+                                        return Ds(n, void 0, void 0, (function() {
                                             var n, o = this;
-                                            return ws(this, (function(i) {
+                                            return Ss(this, (function(i) {
                                                 if (this.userPool) {
-                                                    if (!(n = this.userPool.getCurrentUser())) return hh.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
+                                                    if (!(n = this.userPool.getCurrentUser())) return bh.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
                                                     n.getSession((function(i, a) {
-                                                        return bs(o, void 0, void 0, (function() {
+                                                        return Ds(o, void 0, void 0, (function() {
                                                             var o, a = this;
-                                                            return ws(this, (function(s) {
+                                                            return Ss(this, (function(s) {
                                                                 switch (s.label) {
                                                                     case 0:
                                                                         if (!i) return [3, 5];
-                                                                        if (hh.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
+                                                                        if (bh.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
                                                                         s.label = 1;
                                                                     case 1:
                                                                         return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(n)];
                                                                     case 2:
                                                                         return s.sent(), [3, 4];
                                                                     case 3:
                                                                         return o = s.sent(), r(new Error("Session is invalid due to: " + i.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                     case 4:
                                                                         return [2, r(i)];
                                                                     case 5:
                                                                         n.deleteUser((function(o, i) {
                                                                             if (o) r(o);
                                                                             else {
-                                                                                mh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
+                                                                                xh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
                                                                                 try {
                                                                                     a.cleanCachedItems()
                                                                                 } catch (s) {
-                                                                                    hh.debug("failed to clear cached items")
+                                                                                    bh.debug("failed to clear cached items")
                                                                                 }
-                                                                                t ? a.oAuthSignOutRedirect(e, r) : (mh("signOut", a.user, "A user has been signed out"), e(i))
+                                                                                t ? a.oAuthSignOutRedirect(e, r) : (xh("signOut", a.user, "A user has been signed out"), e(i))
                                                                             }
                                                                         })), s.label = 6;
                                                                     case 6:
                                                                         return [2]
                                                                 }
                                                             }))
                                                         }))
                                                     }))
-                                                } else hh.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
+                                                } else bh.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
                                                 return [2]
                                             }))
                                         }))
                                     }))]
                             }
                         }))
                     }))
@@ -67751,17 +67987,17 @@
                                 if ("sub" !== u && u.indexOf("_verified") < 0) {
                                     var l = {
                                         Name: u,
                                         Value: t[u]
                                     };
                                     o.push(l)
                                 } e.updateAttributes(o, (function(e, n, o) {
-                                if (e) return mh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
+                                if (e) return xh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
                                 var i = r.createUpdateAttributesResultList(t, null === o || void 0 === o ? void 0 : o.CodeDeliveryDetailsList);
-                                return mh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
+                                return xh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
                             }), n)
                         }))
                     }))
                 }, e.prototype.createUpdateAttributesResultList = function(e, t) {
                     var n = {};
                     return Object.keys(e).forEach((function(e) {
                         n[e] = {
@@ -67805,73 +68041,73 @@
                 }, e.prototype.isRefreshTokenExpiredError = function(e) {
                     return this.isErrorWithMessage(e) && "Refresh Token has expired" === e.message
                 }, e.prototype.isSignedInHostedUI = function() {
                     return this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI")
                 }, e.prototype.isSessionInvalid = function(e) {
                     return this.isUserDisabledError(e) || this.isUserDoesNotExistError(e) || this.isTokenRevokedError(e) || this.isRefreshTokenRevokedError(e) || this.isRefreshTokenExpiredError(e)
                 }, e.prototype.cleanUpInvalidSession = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t = this;
-                        return ws(this, (function(n) {
+                        return Ss(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e.signOut(), this.user = null, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this.cleanCachedItems()];
                                 case 2:
                                     return n.sent(), [3, 4];
                                 case 3:
-                                    return n.sent(), hh.debug("failed to clear cached items"), [3, 4];
+                                    return n.sent(), bh.debug("failed to clear cached items"), [3, 4];
                                 case 4:
                                     return this.isSignedInHostedUI() ? [2, new Promise((function(e, n) {
                                         t.oAuthSignOutRedirect(e, n)
-                                    }))] : (mh("signOut", this.user, "A user has been signed out"), [2])
+                                    }))] : (xh("signOut", this.user, "A user has been signed out"), [2])
                             }
                         }))
                     }))
                 }, e.prototype.currentUserPoolUser = function(e) {
                     var t = this;
                     return this.userPool ? new Promise((function(n, r) {
                         t._storageSync.then((function() {
-                            return bs(t, void 0, void 0, (function() {
+                            return Ds(t, void 0, void 0, (function() {
                                 var t, o, i, a, s, u, l = this;
-                                return ws(this, (function(c) {
+                                return Ss(this, (function(c) {
                                     switch (c.label) {
                                         case 0:
-                                            return this.isOAuthInProgress() ? (hh.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
+                                            return this.isOAuthInProgress() ? (bh.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
                                                 var t = setTimeout((function() {
-                                                    hh.debug("OAuth signIn in progress timeout"), Ps.remove("auth", n), e()
+                                                    bh.debug("OAuth signIn in progress timeout"), Gs.remove("auth", n), e()
                                                 }), 1e4);
 
                                                 function n(r) {
                                                     var o = r.payload.event;
-                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (hh.debug("OAuth signIn resolved: " + o), clearTimeout(t), Ps.remove("auth", n), e())
+                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (bh.debug("OAuth signIn resolved: " + o), clearTimeout(t), Gs.remove("auth", n), e())
                                                 }
-                                                Ps.listen("auth", n)
+                                                Gs.listen("auth", n)
                                             }))]) : [3, 2];
                                         case 1:
                                             c.sent(), c.label = 2;
                                         case 2:
-                                            if (!(t = this.userPool.getCurrentUser())) return hh.debug("Failed to get user from user pool"), r("No current user"), [2];
+                                            if (!(t = this.userPool.getCurrentUser())) return bh.debug("Failed to get user from user pool"), r("No current user"), [2];
                                             c.label = 3;
                                         case 3:
                                             return c.trys.push([3, 7, , 8]), [4, this._userSession(t)];
                                         case 4:
                                             return o = c.sent(), (i = !!e && e.bypassCache) ? [4, this.Credentials.clear()] : [3, 6];
                                         case 5:
                                             c.sent(), c.label = 6;
                                         case 6:
-                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(gh) ? (t.getUserData((function(e, o) {
-                                                return bs(l, void 0, void 0, (function() {
+                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(wh) ? (t.getUserData((function(e, o) {
+                                                return Ds(l, void 0, void 0, (function() {
                                                     var i, a, s, u, l, c, d;
-                                                    return ws(this, (function(f) {
+                                                    return Ss(this, (function(f) {
                                                         switch (f.label) {
                                                             case 0:
                                                                 if (!e) return [3, 7];
-                                                                if (hh.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
+                                                                if (bh.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
                                                                 f.label = 1;
                                                             case 1:
                                                                 return f.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return f.sent(), [3, 4];
                                                             case 3:
                                                                 return i = f.sent(), r(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + i.message)), [2];
@@ -67881,114 +68117,114 @@
                                                                 n(t), f.label = 6;
                                                             case 6:
                                                                 return [2];
                                                             case 7:
                                                                 for (a = o.PreferredMfaSetting || "NOMFA", s = [], u = 0; u < o.UserAttributes.length; u++) l = {
                                                                     Name: o.UserAttributes[u].Name,
                                                                     Value: o.UserAttributes[u].Value
-                                                                }, c = new Ap(l), s.push(c);
+                                                                }, c = new Bp(l), s.push(c);
                                                                 return d = this.attributesToObject(s), Object.assign(t, {
                                                                     attributes: d,
                                                                     preferredMFA: a
                                                                 }), [2, n(t)]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 bypassCache: i,
                                                 clientMetadata: a
-                                            }), [3, 8]) : (hh.debug("Unable to get the user data because the " + gh + " is not in the scopes of the access token"), [2, n(t)]);
+                                            }), [3, 8]) : (bh.debug("Unable to get the user data because the " + wh + " is not in the scopes of the access token"), [2, n(t)]);
                                         case 7:
                                             return u = c.sent(), r(u), [3, 8];
                                         case 8:
                                             return [2]
                                     }
                                 }))
                             }))
                         })).catch((function(e) {
-                            return hh.debug("Failed to sync cache info into memory", e), r(e)
+                            return bh.debug("Failed to sync cache info into memory", e), r(e)
                         }))
                     })) : this.rejectNoUserPool()
                 }, e.prototype.isOAuthInProgress = function() {
                     return this.oAuthFlowInProgress
                 }, e.prototype.currentAuthenticatedUser = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r, o, i;
-                        return ws(this, (function(a) {
+                        return Ss(this, (function(a) {
                             switch (a.label) {
                                 case 0:
-                                    hh.debug("getting current authenticated user"), t = null, a.label = 1;
+                                    bh.debug("getting current authenticated user"), t = null, a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    throw n = a.sent(), hh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = a.sent(), bh.debug("Failed to sync cache info into memory", n), n;
                                 case 4:
                                     try {
-                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Ms(Ms({}, r.user), {
+                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Is(Is({}, r.user), {
                                             token: r.token
                                         }))
                                     } catch (s) {
-                                        hh.debug("cannot load federated user from auth storage")
+                                        bh.debug("cannot load federated user from auth storage")
                                     }
-                                    return t ? (this.user = t, hh.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
+                                    return t ? (this.user = t, bh.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
                                 case 5:
-                                    hh.debug("get current authenticated userpool user"), o = null, a.label = 6;
+                                    bh.debug("get current authenticated userpool user"), o = null, a.label = 6;
                                 case 6:
                                     return a.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser(e)];
                                 case 7:
                                     return o = a.sent(), [3, 9];
                                 case 8:
-                                    return "No userPool" === (i = a.sent()) && hh.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), hh.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
+                                    return "No userPool" === (i = a.sent()) && bh.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), bh.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
                                 case 9:
                                     return this.user = o, [2, this.user]
                             }
                         }))
                     }))
                 }, e.prototype.currentSession = function() {
                     var e = this;
-                    return hh.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
+                    return bh.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
                         e.currentUserPoolUser().then((function(r) {
                             e.userSession(r).then((function(e) {
                                 t(e)
                             })).catch((function(e) {
-                                hh.debug("Failed to get the current session", e), n(e)
+                                bh.debug("Failed to get the current session", e), n(e)
                             }))
                         })).catch((function(e) {
-                            hh.debug("Failed to get the current user", e), n(e)
+                            bh.debug("Failed to get the current user", e), n(e)
                         }))
                     })) : Promise.reject(new Error("No User Pool in the configuration."))
                 }, e.prototype._userSession = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r = this;
-                        return ws(this, (function(o) {
+                        return Ss(this, (function(o) {
                             switch (o.label) {
                                 case 0:
-                                    if (!e) return hh.debug("the user is null"), [2, this.rejectAuthError(ms.NoUserSession)];
+                                    if (!e) return bh.debug("the user is null"), [2, this.rejectAuthError(xs.NoUserSession)];
                                     t = this._config.clientMetadata, 0 === this.inflightSessionPromiseCounter && (this.inflightSessionPromise = new Promise((function(n, o) {
                                         e.getSession((function(t, i) {
-                                            return bs(r, void 0, void 0, (function() {
+                                            return Ds(r, void 0, void 0, (function() {
                                                 var r;
-                                                return ws(this, (function(a) {
+                                                return Ss(this, (function(a) {
                                                     switch (a.label) {
                                                         case 0:
                                                             if (!t) return [3, 5];
-                                                            if (hh.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
+                                                            if (bh.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
                                                             a.label = 1;
                                                         case 1:
                                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                         case 2:
                                                             return a.sent(), [3, 4];
                                                         case 3:
                                                             return r = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + r.message)), [2];
                                                         case 4:
                                                             return o(t), [2];
                                                         case 5:
-                                                            return hh.debug("Succeed to get the user session", i), n(i), [2]
+                                                            return bh.debug("Succeed to get the user session", i), n(i), [2]
                                                     }
                                                 }))
                                             }))
                                         }), {
                                             clientMetadata: t
                                         })
                                     }))), this.inflightSessionPromiseCounter++, o.label = 1;
@@ -68002,43 +68238,43 @@
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.userSession = function(e) {
                     return this._userSession(e)
                 }, e.prototype.currentUserCredentials = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return ws(this, (function(r) {
+                        return Ss(this, (function(r) {
                             switch (r.label) {
                                 case 0:
-                                    hh.debug("Getting current user credentials"), r.label = 1;
+                                    bh.debug("Getting current user credentials"), r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), [3, 4];
                                 case 3:
-                                    throw e = r.sent(), hh.debug("Failed to sync cache info into memory", e), e;
+                                    throw e = r.sent(), bh.debug("Failed to sync cache info into memory", e), e;
                                 case 4:
                                     t = null;
                                     try {
                                         t = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))
                                     } catch (o) {
-                                        hh.debug("failed to get or parse item aws-amplify-federatedInfo", o)
+                                        bh.debug("failed to get or parse item aws-amplify-federatedInfo", o)
                                     }
                                     return t ? [2, this.Credentials.refreshFederatedToken(t)] : [2, this.currentSession().then((function(e) {
-                                        return hh.debug("getting session success", e), n.Credentials.set(e, "session")
+                                        return bh.debug("getting session success", e), n.Credentials.set(e, "session")
                                     })).catch((function() {
-                                        return hh.debug("getting guest credentials"), n.Credentials.set(null, "guest")
+                                        return bh.debug("getting guest credentials"), n.Credentials.set(null, "guest")
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.currentCredentials = function() {
-                    return hh.debug("getting current credentials"), this.Credentials.get()
+                    return bh.debug("getting current credentials"), this.Credentials.get()
                 }, e.prototype.verifyUserAttribute = function(e, t, n) {
                     return void 0 === n && (n = this._config.clientMetadata), new Promise((function(r, o) {
                         e.getAttributeVerificationCode(t, {
                             onSuccess: function(e) {
                                 return r(e)
                             },
                             onFailure: function(e) {
@@ -68052,289 +68288,289 @@
                             onSuccess: function(e) {
                                 r(e)
                             },
                             onFailure: function(e) {
                                 o(e)
                             }
                         })
-                    })) : this.rejectAuthError(ms.EmptyCode)
+                    })) : this.rejectAuthError(xs.EmptyCode)
                 }, e.prototype.verifyCurrentUserAttribute = function(e) {
                     var t = this;
                     return t.currentUserPoolUser().then((function(n) {
                         return t.verifyUserAttribute(n, e)
                     }))
                 }, e.prototype.verifyCurrentUserAttributeSubmit = function(e, t) {
                     var n = this;
                     return n.currentUserPoolUser().then((function(r) {
                         return n.verifyUserAttributeSubmit(r, e, t)
                     }))
                 }, e.prototype.cognitoIdentitySignOut = function(e, t) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var n, r, o = this;
-                        return ws(this, (function(i) {
+                        return Ss(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return i.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return i.sent(), [3, 3];
                                 case 2:
-                                    throw n = i.sent(), hh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = i.sent(), bh.debug("Failed to sync cache info into memory", n), n;
                                 case 3:
                                     return r = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(n, i) {
                                         if (e && e.global) {
-                                            hh.debug("user global sign out", t);
+                                            bh.debug("user global sign out", t);
                                             var a = o._config.clientMetadata;
                                             t.getSession((function(e, a) {
-                                                return bs(o, void 0, void 0, (function() {
+                                                return Ds(o, void 0, void 0, (function() {
                                                     var o, a = this;
-                                                    return ws(this, (function(s) {
+                                                    return Ss(this, (function(s) {
                                                         switch (s.label) {
                                                             case 0:
                                                                 if (!e) return [3, 5];
-                                                                if (hh.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
+                                                                if (bh.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
                                                                 s.label = 1;
                                                             case 1:
                                                                 return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return s.sent(), [3, 4];
                                                             case 3:
                                                                 return o = s.sent(), i(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                             case 4:
                                                                 return [2, i(e)];
                                                             case 5:
                                                                 return t.globalSignOut({
                                                                     onSuccess: function(e) {
-                                                                        if (hh.debug("global sign out success"), !r) return n();
+                                                                        if (bh.debug("global sign out success"), !r) return n();
                                                                         a.oAuthSignOutRedirect(n, i)
                                                                     },
                                                                     onFailure: function(e) {
-                                                                        return hh.debug("global sign out failed", e), i(e)
+                                                                        return bh.debug("global sign out failed", e), i(e)
                                                                     }
                                                                 }), [2]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 clientMetadata: a
                                             })
-                                        } else hh.debug("user sign out", t), t.signOut((function() {
+                                        } else bh.debug("user sign out", t), t.signOut((function() {
                                             if (!r) return n();
                                             o.oAuthSignOutRedirect(n, i)
                                         }))
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.oAuthSignOutRedirect = function(e, t) {
-                    Ys().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
+                    Vs().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
                 }, e.prototype.oAuthSignOutAndResolve = function(e) {
                     this._oAuthHandler.signOut(), e()
                 }, e.prototype.oAuthSignOutRedirectOrReject = function(e) {
                     this._oAuthHandler.signOut(), setTimeout((function() {
                         return e(Error("Signout timeout fail"))
                     }), 3e3)
                 }, e.prototype.signOut = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t;
-                        return ws(this, (function(n) {
+                        return Ss(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.cleanCachedItems()];
                                 case 1:
                                     return n.sent(), [3, 3];
                                 case 2:
-                                    return n.sent(), hh.debug("failed to clear cached items"), [3, 3];
+                                    return n.sent(), bh.debug("failed to clear cached items"), [3, 3];
                                 case 3:
                                     return this.userPool ? (t = this.userPool.getCurrentUser()) ? [4, this.cognitoIdentitySignOut(e, t)] : [3, 5] : [3, 7];
                                 case 4:
                                     return n.sent(), [3, 6];
                                 case 5:
-                                    hh.debug("no current Cognito user"), n.label = 6;
+                                    bh.debug("no current Cognito user"), n.label = 6;
                                 case 6:
                                     return [3, 8];
                                 case 7:
-                                    hh.debug("no Cognito User pool"), n.label = 8;
+                                    bh.debug("no Cognito User pool"), n.label = 8;
                                 case 8:
-                                    return mh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
+                                    return xh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
                             }
                         }))
                     }))
                 }, e.prototype.cleanCachedItems = function() {
-                    return bs(this, void 0, void 0, (function() {
-                        return ws(this, (function(e) {
+                    return Ds(this, void 0, void 0, (function() {
+                        return Ss(this, (function(e) {
                             switch (e.label) {
                                 case 0:
                                     return [4, this.Credentials.clear()];
                                 case 1:
                                     return e.sent(), [2]
                             }
                         }))
                     }))
                 }, e.prototype.changePassword = function(e, t, n, r) {
                     var o = this;
                     return void 0 === r && (r = this._config.clientMetadata), new Promise((function(i, a) {
                         o.userSession(e).then((function(o) {
                             e.changePassword(t, n, (function(e, t) {
-                                return e ? (hh.debug("change password failure", e), a(e)) : i(t)
+                                return e ? (bh.debug("change password failure", e), a(e)) : i(t)
                             }), r)
                         }))
                     }))
                 }, e.prototype.forgotPassword = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ms.EmptyUsername);
+                    if (!e) return this.rejectAuthError(xs.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(r, o) {
                         n.forgotPassword({
                             onSuccess: function() {
                                 r()
                             },
                             onFailure: function(t) {
-                                hh.debug("forgot password failure", t), mh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
+                                bh.debug("forgot password failure", t), xh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
                             },
                             inputVerificationCode: function(t) {
-                                mh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
+                                xh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
                             }
                         }, t)
                     }))
                 }, e.prototype.forgotPasswordSubmit = function(e, t, n, r) {
                     if (void 0 === r && (r = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ms.EmptyUsername);
-                    if (!t) return this.rejectAuthError(ms.EmptyCode);
-                    if (!n) return this.rejectAuthError(ms.EmptyPassword);
+                    if (!e) return this.rejectAuthError(xs.EmptyUsername);
+                    if (!t) return this.rejectAuthError(xs.EmptyCode);
+                    if (!n) return this.rejectAuthError(xs.EmptyPassword);
                     var o = this.createCognitoUser(e);
                     return new Promise((function(i, a) {
                         o.confirmPassword(t, n, {
                             onSuccess: function(t) {
-                                mh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
+                                xh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
                             },
                             onFailure: function(t) {
-                                mh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
+                                xh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
                             }
                         }, r)
                     }))
                 }, e.prototype.currentUserInfo = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return ws(this, (function(s) {
+                        return Ss(this, (function(s) {
                             switch (s.label) {
                                 case 0:
                                     return (e = this.Credentials.getCredSource()) && "aws" !== e && "userPool" !== e ? [3, 9] : [4, this.currentUserPoolUser().catch((function(e) {
-                                        return hh.error(e)
+                                        return bh.error(e)
                                     }))];
                                 case 1:
                                     if (!(a = s.sent())) return [2, null];
                                     s.label = 2;
                                 case 2:
                                     return s.trys.push([2, 8, , 9]), [4, this.userAttributes(a)];
                                 case 3:
                                     t = s.sent(), n = this.attributesToObject(t), r = null, s.label = 4;
                                 case 4:
                                     return s.trys.push([4, 6, , 7]), [4, this.currentCredentials()];
                                 case 5:
                                     return r = s.sent(), [3, 7];
                                 case 6:
-                                    return o = s.sent(), hh.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
+                                    return o = s.sent(), bh.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
                                 case 7:
                                     return [2, {
                                         id: r ? r.identityId : void 0,
                                         username: a.getUsername(),
                                         attributes: n
                                     }];
                                 case 8:
-                                    return i = s.sent(), hh.error("currentUserInfo error", i), [2, {}];
+                                    return i = s.sent(), bh.error("currentUserInfo error", i), [2, {}];
                                 case 9:
                                     return "federated" === e ? [2, (a = this.user) || {}] : [2]
                             }
                         }))
                     }))
                 }, e.prototype.federatedSignIn = function(e, t, n) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var r, o, i, a, s, u, l, c, d, f, p;
-                        return ws(this, (function(h) {
+                        return Ss(this, (function(h) {
                             switch (h.label) {
                                 case 0:
                                     if (!this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation requires either a User Pool or Identity Pool in config");
                                     if ("undefined" === typeof e && this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation with Identity Pools requires tokens passed as arguments");
-                                    return xs(e) || (g = e) && ["customProvider"].find((function(e) {
+                                    return ks(e) || (g = e) && ["customProvider"].find((function(e) {
                                         return g.hasOwnProperty(e)
                                     })) || function(e) {
                                         return e && !!["customState"].find((function(t) {
                                             return e.hasOwnProperty(t)
                                         }))
                                     }(e) || "undefined" === typeof e ? (r = e || {
-                                        provider: ys.Cognito
-                                    }, s = xs(r) ? r.provider : r.customProvider, xs(r), o = r.customState, this._config.userPoolId && (i = Ns(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Ns(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
+                                        provider: js.Cognito
+                                    }, s = ks(r) ? r.provider : r.customProvider, ks(r), o = r.customState, this._config.userPoolId && (i = Cs(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Cs(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
                                 case 1:
                                     s = e;
                                     try {
-                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && hh.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
+                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && bh.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
                                     } catch (y) {}
                                     return l = t.token, c = t.identity_id, d = t.expires_at, [4, this.Credentials.set({
                                         provider: s,
                                         token: l,
                                         identity_id: c,
                                         user: n,
                                         expires_at: d
                                     }, "federation")];
                                 case 2:
                                     return f = h.sent(), [4, this.currentAuthenticatedUser()];
                                 case 3:
-                                    return p = h.sent(), mh("signIn", p, "A user " + p.username + " has been signed in"), hh.debug("federated sign in credentials", f), [2, f];
+                                    return p = h.sent(), xh("signIn", p, "A user " + p.username + " has been signed in"), bh.debug("federated sign in credentials", f), [2, f];
                                 case 4:
                                     return [2]
                             }
                             var g
                         }))
                     }))
                 }, e.prototype._handleAuthResponse = function(e) {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return ws(this, (function(g) {
+                        return Ss(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    if (this.oAuthFlowInProgress) return hh.debug("Skipping URL " + e + " current flow in progress"), [2];
+                                    if (this.oAuthFlowInProgress) return bh.debug("Skipping URL " + e + " current flow in progress"), [2];
                                     g.label = 1;
                                 case 1:
                                     if (g.trys.push([1, , 8, 9]), this.oAuthFlowInProgress = !0, !this._config.userPoolId) throw new Error("OAuth responses require a User Pool defined in config");
-                                    if (mh("parsingCallbackUrl", {
+                                    if (xh("parsingCallbackUrl", {
                                             url: e
-                                        }, "The callback url is being parsed"), t = e || (Ys().isBrowser ? window.location.href : ""), n = !!((0, rh.Qc)(t).query || "").split("&").map((function(e) {
+                                        }, "The callback url is being parsed"), t = e || (Vs().isBrowser ? window.location.href : ""), n = !!((0, lh.Qc)(t).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = js(e, 1)[0];
+                                            var t = Ls(e, 1)[0];
                                             return "code" === t || "error" === t
-                                        })), r = !!((0, rh.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
+                                        })), r = !!((0, lh.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = js(e, 1)[0];
+                                            var t = Ls(e, 1)[0];
                                             return "access_token" === t || "error" === t
                                         })), !n && !r) return [3, 7];
                                     this._storage.setItem("amplify-redirected-from-hosted-ui", "true"), g.label = 2;
                                 case 2:
                                     return g.trys.push([2, 6, , 7]), [4, this._oAuthHandler.handleAuthResponse(t)];
                                 case 3:
-                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Cp({
-                                        IdToken: new Sp({
+                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new zp({
+                                        IdToken: new Tp({
                                             IdToken: a
                                         }),
-                                        RefreshToken: new Lp({
+                                        RefreshToken: new Ap({
                                             RefreshToken: s
                                         }),
-                                        AccessToken: new Ip({
+                                        AccessToken: new Ep({
                                             AccessToken: i
                                         })
                                     }), c = void 0, this._config.identityPoolId ? [4, this.Credentials.set(l, "session")] : [3, 5];
                                 case 4:
-                                    c = g.sent(), hh.debug("AWS credentials", c), g.label = 5;
+                                    c = g.sent(), bh.debug("AWS credentials", c), g.label = 5;
                                 case 5:
-                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), mh("signIn", f, "A user " + f.getUsername() + " has been signed in"), mh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), mh("customOAuthState", p.match(/.{2}/g).map((function(e) {
+                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), xh("signIn", f, "A user " + f.getUsername() + " has been signed in"), xh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), xh("customOAuthState", p.match(/.{2}/g).map((function(e) {
                                         return String.fromCharCode(parseInt(e, 16))
                                     })).join(""), "State for user " + f.getUsername())), [2, c];
                                 case 6:
-                                    return h = g.sent(), hh.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), mh("signIn_failure", h, "The OAuth response flow failed"), mh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), mh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
+                                    return h = g.sent(), bh.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), xh("signIn_failure", h, "The OAuth response flow failed"), xh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), xh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
                                 case 7:
                                     return [3, 9];
                                 case 8:
                                     return this.oAuthFlowInProgress = !1, [7];
                                 case 9:
                                     return [2]
                             }
@@ -68359,86 +68595,86 @@
                 }, e.prototype.createCognitoUser = function(e) {
                     var t = {
                         Username: e,
                         Pool: this.userPool
                     };
                     t.Storage = this._storage;
                     var n = this._config.authenticationFlowType,
-                        r = new Rp(t);
+                        r = new Wp(t);
                     return n && r.setAuthenticationFlowType(n), r
                 }, e.prototype._isValidAuthStorage = function(e) {
                     return !!e && "function" === typeof e.getItem && "function" === typeof e.setItem && "function" === typeof e.removeItem && "function" === typeof e.clear
                 }, e.prototype.noUserPoolErrorHandler = function(e) {
-                    return !e || e.userPoolId && e.identityPoolId ? ms.NoConfig : ms.MissingAuthConfig
+                    return !e || e.userPoolId && e.identityPoolId ? xs.NoConfig : xs.MissingAuthConfig
                 }, e.prototype.rejectAuthError = function(e) {
-                    return Promise.reject(new dh(e))
+                    return Promise.reject(new mh(e))
                 }, e.prototype.rejectNoUserPool = function() {
                     var e = this.noUserPoolErrorHandler(this._config);
-                    return Promise.reject(new fh(e))
+                    return Promise.reject(new vh(e))
                 }, e.prototype.rememberDevice = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t;
-                        return ws(this, (function(n) {
+                        return Ss(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), hh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), bh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.setDeviceStatusRemembered({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new dh(ms.DeviceConfig)) : "NetworkError" === e.code ? n(new dh(ms.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new mh(xs.DeviceConfig)) : "NetworkError" === e.code ? n(new mh(xs.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.forgetDevice = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t;
-                        return ws(this, (function(n) {
+                        return Ss(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), hh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), bh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.forgetDevice({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new dh(ms.DeviceConfig)) : "NetworkError" === e.code ? n(new dh(ms.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new mh(xs.DeviceConfig)) : "NetworkError" === e.code ? n(new mh(xs.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.fetchDevices = function() {
-                    return bs(this, void 0, void 0, (function() {
+                    return Ds(this, void 0, void 0, (function() {
                         var e, t;
-                        return ws(this, (function(n) {
+                        return Ss(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    throw t = n.sent(), hh.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
+                                    throw t = n.sent(), bh.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         var r = {
                                             onSuccess: function(e) {
                                                 var n = e.Devices.map((function(e) {
                                                     var t = e.DeviceAttributes.find((function(e) {
                                                         return "device_name" === e.Name
@@ -68447,32 +68683,32 @@
                                                         id: e.DeviceKey,
                                                         name: t.Value
                                                     }
                                                 }));
                                                 t(n)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new dh(ms.DeviceConfig)) : "NetworkError" === e.code ? n(new dh(ms.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new mh(xs.DeviceConfig)) : "NetworkError" === e.code ? n(new mh(xs.NetworkError)) : n(e)
                                             }
                                         };
                                         e.listDevices(60, null, r)
                                     }))]
                             }
                         }))
                     }))
                 }, e
             }(),
-            Mh = new vh(null);
-        nu.register(Mh);
-        var bh = "#FEFEFE",
-            wh = function(e) {
+            Ih = new Nh(null);
+        uu.register(Ih);
+        var Dh = "#FEFEFE",
+            Sh = function(e) {
                 var t = e.hide,
                     n = pe().environ,
-                    r = Xi(),
-                    o = qi(zt.Url("/cognito_config", !1), {
+                    r = ta(),
+                    o = Xi(zt.Url("/cognito_config", !1), {
                         cache: !0,
                         onData: function(e) {
                             var t = {
                                 region: e.region,
                                 userPoolId: e.userpool,
                                 userPoolWebClientId: e.client,
                                 mandatorySignIn: !0,
@@ -68480,15 +68716,15 @@
                                     domain: e.domain,
                                     scope: e.scope,
                                     prompt: "select_account",
                                     redirectSignIn: e.callback,
                                     responseType: "code"
                                 }
                             };
-                            Mh.configure(t)
+                            Ih.configure(t)
                         }
                     });
                 var i = (0, Kr.jsx)("div", {
                     children: (0, Kr.jsxs)("div", {
                         className: "title-font",
                         style: {
                             marginTop: "4pt",
@@ -68516,52 +68752,52 @@
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         transform: "scale(1.1)",
                         marginTop: "10pt",
                         marginBottom: "40pt"
                     },
-                    children: (0, Kr.jsx)(jh, {
+                    children: (0, Kr.jsx)(Lh, {
                         links: i,
                         children: o.loading ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsx)(no, {
                                 condition: !0,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: "140px",
                                 label: "Loading configuration "
                             })
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "0pt"
                                 }
-                            }), (0, Kr.jsx)(xh, {
+                            }), (0, Kr.jsx)(kh, {
                                 signin: function() {
-                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), Mh.federatedSignIn({
+                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), Ih.federatedSignIn({
                                         provider: "Google",
                                         prompt: "select_account"
                                     }, {
                                         prompt: "select_account"
                                     })
                                 }
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "6pt"
                                 }
-                            }), (0, Kr.jsx)(Nh, {
+                            }), (0, Kr.jsx)(Ch, {
                                 signin: function() {
                                     window.alert("Sign in with GitHub via Cognito not supported.")
                                 }
                             })]
                         })
                     })
                 })
             },
-            jh = function(e) {
+            Lh = function(e) {
                 var t = e.links,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     className: "container",
                     style: {
                         width: "265pt",
                         marginTop: "30pt"
@@ -68572,15 +68808,15 @@
                                 border: "2px solid var(--box-fg)",
                                 padding: "2px 2px 2px 2px",
                                 borderRadius: "6px",
                                 overflow: "hidden"
                             },
                             children: (0, Kr.jsxs)("div", {
                                 style: {
-                                    background: bh,
+                                    background: Dh,
                                     border: "1px solid var(--box-fg)",
                                     borderRadius: "6px",
                                     overflow: "hidden"
                                 },
                                 children: [(0, Kr.jsx)("div", {
                                     style: {
                                         background: "var(--box-fg)",
@@ -68605,17 +68841,17 @@
                             })
                         }), t && (0, Kr.jsx)(Kr.Fragment, {
                             children: t
                         })]
                     })
                 })
             },
-            xh = function(e) {
+            kh = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(Ih, {
+                return (0, Kr.jsxs)(Eh, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "google",
                         src: Ut.GoogleLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px"
@@ -68627,17 +68863,17 @@
                             fontSize: "12pt",
                             marginLeft: "10pt"
                         },
                         children: "Sign in with Google"
                     })]
                 })
             },
-            Nh = function(e) {
+            Ch = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(Ih, {
+                return (0, Kr.jsxs)(Eh, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "github",
                         src: Ut.GitHubLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px",
@@ -68650,38 +68886,38 @@
                             fontSize: "12pt",
                             marginLeft: "7pt"
                         },
                         children: "Sign in with GitHub"
                     })]
                 })
             },
-            Ih = function(e) {
+            Eh = function(e) {
                 var t = e.signin,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     style: {
-                        background: bh,
+                        background: Dh,
                         padding: "0 10pt 0 10pt"
                     },
                     children: (0, Kr.jsx)("button", {
                         className: "signin-as-button",
                         onClick: t,
                         children: n
                     })
                 })
             },
-            Dh = function(e) {
+            _h = function(e) {
                 var t = a(Re(), 1)[0],
                     n = t.get("code"),
                     r = t.get("state"),
                     o = sessionStorage.getItem("oauth_state"),
                     i = sessionStorage.getItem("ouath_pkce_key"),
                     s = fe(),
                     u = "".concat(zt.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
-                    l = qi(u, {
+                    l = Xi(u, {
                         onDone: function(e) {
                             var t, n, r = null === (t = e.data) || void 0 === t ? void 0 : t.authtoken,
                                 o = null === (n = e.data) || void 0 === n ? void 0 : n.expires;
                             bt.Set("authtoken", r, o);
                             var i = bt.Redirect();
                             if (it.HasValue(i)) i = xt.FromUrl(i);
                             else if (i = bt.LastUrl(), it.HasValue(i)) i = xt.FromUrl(i);
@@ -68696,37 +68932,37 @@
                     var c = bt.Get("signinvia");
                     return (0, Kr.jsx)("div", {
                         style: {
                             transform: "scale(1.1)",
                             marginTop: "10pt",
                             marginBottom: "40pt"
                         },
-                        children: (0, Kr.jsx)(jh, {
+                        children: (0, Kr.jsx)(Lh, {
                             children: (0, Kr.jsx)(no, {
                                 condition: l.loading,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: 140,
                                 label: "Signing in via ".concat(c)
                             })
                         })
                     })
                 }
             },
-            Sh = __webpack_require__(9712),
-            Lh = function(e) {
-                var n, r, o, i, s, u, l, c, d, f, p, h, g = Xi(),
+            Th = __webpack_require__(9712),
+            Ah = function(e) {
+                var n, r, o, i, s, u, l, c, d, f, p, h, g = ta(),
                     y = a((0, t.useState)(!1), 2),
                     m = y[0],
                     v = y[1],
                     M = a((0, t.useState)(!1), 2),
                     b = M[0],
                     w = M[1],
                     j = (null === (n = a(Re(), 1)[0].get("auth")) || void 0 === n ? void 0 : n.length) >= 0,
-                    x = qi(zt.Url("/auth0_config", !1)),
+                    x = Xi(zt.Url("/auth0_config", !1)),
                     N = a((0, t.useState)(!1), 2),
                     I = N[0],
                     D = N[1],
                     S = a((0, t.useState)(kr.IsCognitoEnabled()), 2),
                     L = S[0],
                     k = S[1];
 
@@ -68739,15 +68975,15 @@
                 }
 
                 function _() {
                     k(!1), kr.DisableCognito()
                 }
 
                 function T() {
-                    document.getElementById("login_container").style.display = "none", document.getElementById("login_auth_container").style.display = "block", document.getElementById("login_auth_cancel").style.display = "block", bt.SetRedirect(Ai.LastUrl()),
+                    document.getElementById("login_container").style.display = "none", document.getElementById("login_auth_container").style.display = "block", document.getElementById("login_auth_cancel").style.display = "block", bt.SetRedirect(Ui.LastUrl()),
                         function() {
                             var e, t, n, r, o, i, a, s = {
                                 container: "login_auth_container",
                                 auth: {
                                     redirectUrl: null === x || void 0 === x || null === (e = x.data) || void 0 === e ? void 0 : e.callback,
                                     responseType: "code",
                                     sso: null === x || void 0 === x || null === (t = x.data) || void 0 === t ? void 0 : t.sso,
@@ -68763,15 +68999,15 @@
                                 theme: {
                                     primaryColor: "blue",
                                     backgroundColor: "blue",
                                     logo: ""
                                 },
                                 allowedConnections: null === x || void 0 === x || null === (o = x.data) || void 0 === o ? void 0 : o.connections
                             };
-                            return new Sh.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
+                            return new Th.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
                         }().show(), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && (document.getElementById("login_auth_container").style.height = "200", document.getElementById("login_auth_container").style.background = "white", document.getElementById("login_auth_container").style.borderStyle = "none"), document.getElementById("login_auth_container").firstChild.firstChild.style.paddingLeft = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingRight = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingTop = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingBottom = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", v(!0)
                 }
                 if ((g.loading || x.loading) && !g.error) return (0, Kr.jsx)(Kr.Fragment, {
                     children: "Loading ..."
                 });
                 if (g.error) return (0, Kr.jsx)(xi, {
                     error: g.error,
@@ -68815,15 +69051,15 @@
                                     position: "bottom",
                                     text: "AWS Account Alias: ".concat(null === g || void 0 === g || null === (c = g.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name)
                                 })]
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     })
                 };
-                return I ? (0, Kr.jsx)(wh, {
+                return I ? (0, Kr.jsx)(Sh, {
                     hide: function() {
                         return D(!1)
                     }
                 }) : (0, Kr.jsx)(Kr.Fragment, {
                     children: Br.IsLoggedIn(g) ? (0, Kr.jsx)(t.Fragment, {
                         children: (0, Kr.jsxs)("div", {
                             className: "container",
@@ -68890,42 +69126,42 @@
                                                 }), (0, Kr.jsxs)("div", {
                                                     style: {
                                                         fontSize: "small",
                                                         marginTop: "6pt",
                                                         paddingTop: "5pt",
                                                         borderTop: "1px solid"
                                                     },
-                                                    children: ["Session started: ", (0, Kr.jsx)(da.FormatDuration, {
+                                                    children: ["Session started: ", (0, Kr.jsx)(ha.FormatDuration, {
                                                         start: Br.Token().authenticated_at,
                                                         verbose: !0,
                                                         fallback: "just now",
                                                         suffix: "ago",
                                                         tooltip: !0
-                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(da.FormatDuration, {
+                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(ha.FormatDuration, {
                                                         end: Br.Token().authenticated_until,
                                                         verbose: !0,
                                                         fallback: "now",
                                                         suffix: "from now",
                                                         tooltip: !0
                                                     }), "\xa0", (0, Kr.jsx)("br", {}), "Click ", (0, Kr.jsx)("span", {
                                                         style: {
                                                             textDecoration: "underline",
                                                             fontWeight: "bold",
                                                             cursor: "pointer"
                                                         },
                                                         onClick: function() {
-                                                            return Oi()
+                                                            return Pi()
                                                         },
                                                         children: "here"
                                                     }), " to ", (0, Kr.jsx)("span", {
                                                         style: {
                                                             cursor: "pointer"
                                                         },
                                                         onClick: function() {
-                                                            return Oi()
+                                                            return Pi()
                                                         },
                                                         children: "logout"
                                                     }), "."]
                                                 })]
                                             }), (0, Kr.jsx)("td", {
                                                 style: {
                                                     paddingLeft: "12pt",
@@ -69045,15 +69281,15 @@
                                                 return Yr.Copy("authtoken")
                                             },
                                             style: {
                                                 float: "right",
                                                 height: "20px",
                                                 cursor: "copy"
                                             }
-                                        }), Ui.Format(Br.Token())]
+                                        }), Bi.Format(Br.Token())]
                                     }), (0, Kr.jsxs)("pre", {
                                         className: "box",
                                         style: {
                                             filter: "brightness(1.1)",
                                             background: "inherit",
                                             fontWeight: "bold",
                                             marginTop: "-3pt",
@@ -69103,15 +69339,15 @@
                                         className: "box",
                                         style: {
                                             filter: "brightness(1.1)",
                                             background: "inherit",
                                             fontWeight: "bold",
                                             marginTop: "6pt"
                                         },
-                                        children: Ui.Format(null === g || void 0 === g ? void 0 : g.auth)
+                                        children: Bi.Format(null === g || void 0 === g ? void 0 : g.auth)
                                     })]
                                 })]
                             })]
                         })
                     }) : (0, Kr.jsxs)(t.Fragment, {
                         children: [(0, Kr.jsxs)("div", {
                             className: "container",
@@ -69315,15 +69551,15 @@
                                                 return Yr.Copy("authtoken")
                                             },
                                             style: {
                                                 float: "right",
                                                 height: "20px",
                                                 cursor: "copy"
                                             }
-                                        }), Ui.Format(bt.AuthToken())]
+                                        }), Bi.Format(bt.AuthToken())]
                                     }), (0, Kr.jsxs)("pre", {
                                         className: "box",
                                         style: {
                                             filter: "brightness(1.1)",
                                             background: "inherit",
                                             color: "darkred",
                                             fontWeight: "bold",
@@ -69396,15 +69632,15 @@
                                                 return Yr.Copy("authtoken")
                                             },
                                             style: {
                                                 float: "right",
                                                 height: "20px",
                                                 cursor: "copy"
                                             }
-                                        }), Ui.Format(null === g || void 0 === g ? void 0 : g.auth)]
+                                        }), Bi.Format(null === g || void 0 === g ? void 0 : g.auth)]
                                     })]
                                 })]
                             })]
                         }), x.loading ? (0, Kr.jsx)(Kr.Fragment, {
                             children: "Loading Auth0 configuration ..."
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("br", {}), (0, Kr.jsx)("br", {}), (0, Kr.jsx)("br", {}), (0, Kr.jsxs)("div", {
@@ -69442,24 +69678,24 @@
                                     j && !m && T()
                                 }), 10), "")]
                             })]
                         })]
                     })
                 })
             },
-            kh = function(e) {
-                var n = Xi(),
+            Oh = function(e) {
+                var n = ta(),
                     r = pe().environCompare,
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
                     u = a((0, t.useState)("all"), 2),
                     l = u[0],
                     c = u[1],
-                    d = qi(zt.Url("/gac/".concat(r), At.Current())),
+                    d = Xi(zt.Url("/gac/".concat(r), At.Current())),
                     f = fe();
 
                 function p(e, t) {
                     var n, r;
                     return null === t || void 0 === t || null === (n = t.gac_diffs) || void 0 === n || null === (r = n.same) || void 0 === r ? void 0 : r.includes(e)
                 }
 
@@ -69796,15 +70032,15 @@
                                 display: "none"
                             },
                             children: d.yaml()
                         })]
                     })
                 })
             },
-            Ch = function(e) {
+            zh = function(e) {
                 return {
                     __get: function(t, n, r, o) {
                         var i = e.findIndex((function(e) {
                             return e.type === t
                         }));
                         if (i >= 0) {
                             var a = n ? "".concat(t, ".").concat(n) : t;
@@ -69817,16 +70053,16 @@
                                 }
                             }
                         }
                         return null
                     }
                 }
             },
-            Eh = function(e) {
-                e = Ch(e);
+            Uh = function(e) {
+                e = zh(e);
                 var n = a((0, t.useState)([]), 2),
                     r = n[0],
                     o = n[1];
                 return (0, t.useState)({
                     count: function() {
                         return r.length
                     },
@@ -69871,23 +70107,23 @@
                     __unselect: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                             n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
                         null == n && (n = this.__lookup(e, t)), n >= 0 && (r.splice(n, 1), o(u(r)))
                     }
                 })[0]
             },
-            _h = function(e) {
+            Ph = function(e) {
                 var t;
                 return "function" == typeof e && (e = e()), (null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object ? e : {}
             },
-            Th = function(e, t) {
+            Rh = function(e, t) {
                 return "function" == typeof e && (e = e()), void 0 !== e ? e : {}
             };
 
-        function Ah(e) {
+        function Bh(e) {
             var t, n, r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                 o = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (Object.is(e, r))
                 if ((null === (n = e) || void 0 === n ? void 0 : n.constructor) === Object) e = Ye({}, e);
                 else if (Array.isArray(e)) {
                 var i = function(e) {
                     var t = u(e),
@@ -69902,24 +70138,24 @@
                     return t
                 };
                 e = i(e)
             } else "function" === typeof e && (e = e(r));
             else(null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object && (null === r || void 0 === r ? void 0 : r.constructor) === Object && o && (e = Ye(Ye({}, r), e));
             return e
         }
-        var Oh = function(e, n) {
+        var Fh = function(e, n) {
                 var r = !0 === (null === e || void 0 === e ? void 0 : e.__keyedState) ? !0 === e.__keyedStateUsage ? e : e.keyed("default") : null,
-                    o = r ? r.__state() ? r.__state() : Th(n) : _h(e),
+                    o = r ? r.__state() ? r.__state() : Rh(n) : Ph(e),
                     i = a((0, t.useState)(o), 2),
                     s = i[0],
                     u = i[1];
                 return (0, t.useEffect)((function() {
-                    o && r && !r.__state() && r.__updateState(Ah(o, s, !0))
+                    o && r && !r.__state() && r.__updateState(Bh(o, s, !0))
                 }), []), r ? [s, function(e) {
-                    e = Ah(e, s, !0), u(e), r.__updateState(e)
+                    e = Bh(e, s, !0), u(e), r.__updateState(e)
                 }] : {
                     __keyedState: !0,
                     key: null,
                     keyed: function(e) {
                         var t;
                         if (!0 === this.__keyedState) {
                             (null === (t = e) || void 0 === t ? void 0 : t.constructor) === String && 0 !== e.length || (e = "default");
@@ -69943,27 +70179,27 @@
                                     return s[e]
                                 }
                             }
                         }
                     }
                 }
             },
-            zh = {
+            Yh = {
                 color: "var(--box-fg)",
                 fontWeight: "bold",
                 paddingTop: "1pt",
                 verticalAlign: "top",
                 width: "5%",
                 paddingRight: "8pt",
                 whiteSpace: "nowrap"
             },
-            Uh = {
+            Qh = {
                 verticalAlign: "top"
             },
-            Ph = function(e) {
+            Gh = function(e) {
                 var t = e.showVpcs,
                     n = e.toggleVpcs,
                     r = e.showSecurityGroups,
                     o = e.toggleSecurityGroups,
                     i = e.showSubnetsPublic,
                     a = e.toggleSubnetsPublic,
                     s = e.showSubnetsPrivate,
@@ -70016,15 +70252,15 @@
                             },
                             onClick: o,
                             children: "Security Groups"
                         })]
                     })]
                 })
             },
-            Rh = function(e) {
+            Wh = function(e) {
                 var t = e.showGac,
                     n = e.toggleGac,
                     r = e.showEcosystem,
                     o = e.toggleEcosystem;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "box margin thickborder",
@@ -70049,19 +70285,19 @@
                             },
                             onClick: o,
                             children: "Ecosystem Definition"
                         })]
                     })
                 })
             },
-            Bh = function(e) {
+            Hh = function(e) {
                 var t, n, r = e.keyedState,
                     o = e.hide,
                     i = "true" === (null === (t = Re()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
-                    a = qi("/aws/vpcs".concat(i ? "/all" : ""), {
+                    a = Xi("/aws/vpcs".concat(i ? "/all" : ""), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         marginBottom: "8pt"
                     },
                     children: [(0, Kr.jsxs)("div", {
@@ -70096,27 +70332,27 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading VPCs"
                             })
                         }), a.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(Fh, {
+                                children: (0, Kr.jsx)(Zh, {
                                     vpc: e,
                                     keyedState: null === r || void 0 === r ? void 0 : r.keyed(e.id)
                                 })
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Fh = function(e) {
+            Zh = function(e) {
                 var t = e.vpc,
                     n = e.keyedState,
-                    r = a(Oh(n), 2),
+                    r = a(Fh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -70162,42 +70398,42 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: t.id
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -70220,15 +70456,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return t.id, u("showSubnetsPublic")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Public Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70244,29 +70480,29 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Yh, {
+                                            children: (0, Kr.jsx)(Vh, {
                                                 type: "public",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-public")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSubnetsPrivate")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Private Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70282,29 +70518,29 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Yh, {
+                                            children: (0, Kr.jsx)(Vh, {
                                                 type: "private",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-private")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSecurityGroups")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Security Groups:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70320,28 +70556,28 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Gh, {
+                                            children: (0, Kr.jsx)(Jh, {
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("security-groups")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: f() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70357,34 +70593,34 @@
                                 }), f() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Vh, {
+                                            children: (0, Kr.jsx)(eg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Yh = function(e) {
+            Vh = function(e) {
                 var t, n, r = e.vpcId,
                     o = e.type,
                     i = e.hide,
                     a = e.notitle,
                     s = e.keyedState,
                     u = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     l = r ? "?vpc=".concat(r) : "",
-                    c = qi("/aws/subnets".concat(u ? "/all" : "").concat(l), {
+                    c = Xi("/aws/subnets".concat(u ? "/all" : "").concat(l), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         marginBottom: "8pt"
                     },
                     children: [!a && (0, Kr.jsxs)("div", {
@@ -70415,31 +70651,31 @@
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading Subnets"
                             })
                         }), null === (n = c.filter((function(e) {
                             return !o || e.type === o
                         }))) || void 0 === n ? void 0 : n.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)(Qh, {
+                                children: [(0, Kr.jsx)(qh, {
                                     subnet: e,
                                     keyedState: null === s || void 0 === s ? void 0 : s.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Qh = function(e) {
+            qh = function(e) {
                 var t = e.subnet,
                     n = e.keyedState,
-                    r = a(Oh(n), 2),
+                    r = a(Fh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function() {
                         return o["showTags"]
                     };
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
@@ -70487,60 +70723,60 @@
                                 })
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.subnet_arn
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Zone:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.zone
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -70564,15 +70800,15 @@
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return i(Be({}, e = "showTags", !o[e]));
                                         var e
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: s() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70588,33 +70824,33 @@
                                 }), s() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Vh, {
+                                            children: (0, Kr.jsx)(eg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Gh = function(e) {
+            Jh = function(e) {
                 var t, n = e.vpcId,
                     r = e.notitle,
                     o = e.keyedState,
                     i = e.hide,
                     a = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     s = n ? "?vpc=".concat(n) : "",
-                    u = qi("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
+                    u = Xi("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         marginBottom: "8pt"
                     },
                     children: [!r && (0, Kr.jsxs)("div", {
@@ -70643,31 +70879,31 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading security groups"
                             })
                         }), u.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)(Wh, {
+                                children: [(0, Kr.jsx)(Kh, {
                                     securityGroup: e,
                                     keyedState: null === o || void 0 === o ? void 0 : o.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Wh = function(e) {
+            Kh = function(e) {
                 var t = e.securityGroup,
                     n = e.keyedState,
-                    r = a(Oh(n), 2),
+                    r = a(Fh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -70709,47 +70945,47 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.securityGroup
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -70772,15 +71008,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showInboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Inbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsxs)("small", {
                                                 children: [(0, Kr.jsx)("u", {
                                                     children: "Hide"
                                                 }), "\xa0", Fr.DownArrowHollow]
@@ -70796,27 +71032,27 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Hh, {
+                                            children: (0, Kr.jsx)(Xh, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "inbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showOutboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Outbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70832,27 +71068,27 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Hh, {
+                                            children: (0, Kr.jsx)(Xh, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "outbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70868,55 +71104,55 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(Vh, {
+                                            children: (0, Kr.jsx)(eg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Hh = function(e) {
+            Xh = function(e) {
                 var t = e.securityGroupId,
                     n = e.direction,
                     r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
-                    o = qi("/aws/security_group_rules/".concat(t).concat(r), {
+                    o = Xi("/aws/security_group_rules/".concat(t).concat(r), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [o.loading && (0, Kr.jsx)("div", {
                         className: "box lighten",
                         style: {
                             paddingBottom: "10pt"
                         },
                         children: (0, Kr.jsx)(no, {
                             label: "Loading security group rules"
                         })
                     }), null === o || void 0 === o ? void 0 : o.map((function(e) {
                         return (0, Kr.jsxs)("div", {
-                            children: [(0, Kr.jsx)(Zh, {
+                            children: [(0, Kr.jsx)($h, {
                                 securityGroupRule: e
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     height: "4pt"
                                 }
                             })]
                         }, e.id)
                     }))]
                 })
             },
-            Zh = function(e) {
+            $h = function(e) {
                 var t = e.securityGroupRule;
 
                 function n(e) {
                     var t, n;
                     if ("TCP" === (null === e || void 0 === e || null === (t = e.protocol) || void 0 === t ? void 0 : t.toUpperCase())) {
                         if (22 === (null === e || void 0 === e ? void 0 : e.port_from) && 22 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "SSH";
                         if (443 === (null === e || void 0 === e ? void 0 : e.port_from) && 443 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "HTTPS";
@@ -70971,78 +71207,78 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Direction:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null !== t && void 0 !== t && t.egress ? "Outbound" : "Inbound"
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Protocol:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: r(t)
                                     })]
                                 }), n(t) !== r(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Type:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: n(t)
                                     })]
                                 }), o(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Port:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: o(t)
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.cidr) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.description) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Security Group:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === t || void 0 === t ? void 0 : t.security_group
                                     })]
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Vh = function(e) {
+            eg = function(e) {
                 var t;
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
                         className: "box lighten",
@@ -71077,16 +71313,16 @@
                             children: (0, Kr.jsx)("li", {
                                 children: "No tags."
                             })
                         })
                     })
                 })
             },
-            qh = function(e) {
-                var t = qi("/aws/stacks", {
+            tg = function(e) {
+                var t = Xi("/aws/stacks", {
                         cache: !0
                     }),
                     n = {
                         cursor: "pointer"
                     },
                     r = Ye(Ye({}, n), {}, {
                         borderBottom: "1px solid var(--box-fg)",
@@ -71116,22 +71352,22 @@
                                 },
                                 children: o.name
                             }, o.name)
                         }))]
                     })]
                 })
             },
-            Jh = function(e) {
+            ng = function(e) {
                 var t, n, r, o, i, s, u, l, c, d, f, p, h = e.stackName,
                     g = e.keyedState,
                     y = e.hide,
-                    m = a(Oh(g), 2),
+                    m = a(Fh(g), 2),
                     v = m[0],
                     M = m[1],
-                    b = qi("/aws/stacks/".concat(h), {
+                    b = Xi("/aws/stacks/".concat(h), {
                         cache: !0
                     }),
                     w = function(e) {
                         return v[e]
                     },
                     j = function(e) {
                         return M(Be({}, e, !v[e]))
@@ -71180,56 +71416,56 @@
                         children: b.loading ? (0, Kr.jsx)(no, {
                             label: "Loading stack info"
                         }) : (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Name:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Ye(Ye({}, Uh), {}, {
+                                        style: Ye(Ye({}, Qh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: [(0, Kr.jsx)("b", {
                                             style: {
                                                 float: "right",
                                                 cursor: "pointer",
                                                 marginTop: "-2pt"
                                             },
                                             onClick: y,
                                             children: Fr.X
                                         }), h]
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Ye(Ye({}, Uh), {}, {
+                                        style: Ye(Ye({}, Qh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: (0, Kr.jsx)("small", {
                                             children: null === (n = b.data) || void 0 === n ? void 0 : n.id
                                         })
                                     })]
                                 }), (null === (r = b.data) || void 0 === r ? void 0 : r.role_arn) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Role:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: (null === (o = b.data) || void 0 === o ? void 0 : o.role_arn) || Fr.EmptySet
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === (i = b.data) || void 0 === i ? void 0 : i.description
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71248,34 +71484,34 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === (s = b.data) || void 0 === s ? void 0 : s.status
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Created:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === (u = b.data) || void 0 === u ? void 0 : u.created
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Updated:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: null === (l = b.data) || void 0 === l ? void 0 : l.updated
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71294,18 +71530,18 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Outputs:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [x() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: N,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71330,25 +71566,25 @@
                                 }), x() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(Kh, {
+                                            children: (0, Kr.jsx)(rg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Parameters:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [I() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: D,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71373,25 +71609,25 @@
                                 }), I() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(Xh, {
+                                            children: (0, Kr.jsx)(og, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Resources:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [S() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: L,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71416,25 +71652,25 @@
                                 }), S() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)($h, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: zh,
+                                        style: Yh,
                                         children: "Template:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Uh,
+                                        style: Qh,
                                         children: [k() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: C,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71459,27 +71695,27 @@
                                 }), k() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(eg, {
+                                            children: (0, Kr.jsx)(ag, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 })]
                             })
                         })
                     })]
                 })
             },
-            Kh = function(e) {
-                var t, n = qi("/aws/stacks/".concat(e.stackName, "/outputs"), {
+            rg = function(e) {
+                var t, n = Xi("/aws/stacks/".concat(e.stackName, "/outputs"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
@@ -71521,16 +71757,16 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            Xh = function(e) {
-                var t, n = qi("/aws/stacks/".concat(e.stackName, "/parameters"), {
+            og = function(e) {
+                var t, n = Xi("/aws/stacks/".concat(e.stackName, "/parameters"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
@@ -71572,16 +71808,16 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            $h = function(e) {
-                var t, n = qi("/aws/stacks/".concat(e.stackName, "/resources"), {
+            ig = function(e) {
+                var t, n = Xi("/aws/stacks/".concat(e.stackName, "/resources"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
@@ -71626,16 +71862,16 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            eg = function(e) {
-                var t = qi("/aws/stacks/".concat(e.stackName, "/template"), {
+            ag = function(e) {
+                var t = Xi("/aws/stacks/".concat(e.stackName, "/template"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
@@ -71655,23 +71891,23 @@
                                 style: {
                                     border: "0",
                                     background: "var(--box-bg-lighten)",
                                     marginLeft: "-6pt",
                                     marginTop: "-6pt",
                                     marginBottom: "-6pt"
                                 },
-                                children: st.IsObject(t.data) ? Ui.Format(t.data) : t.data
+                                children: st.IsObject(t.data) ? Bi.Format(t.data) : t.data
                             })
                         })
                     })
                 })
             },
-            tg = function(e) {
+            sg = function(e) {
                 var t, n, r, o, i, a, s = e.hide,
-                    u = qi("/info", {
+                    u = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
                         marginBottom: "8pt"
                     },
@@ -71720,17 +71956,17 @@
                                     }) : u.data.gac.values[e]]
                                 }, e)
                             })))
                         })]
                     })]
                 })
             },
-            ng = function(e) {
+            ug = function(e) {
                 var t, n, r, o, i = e.hide,
-                    a = qi("/info", {
+                    a = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
                         marginBottom: "8pt"
                     },
@@ -71750,85 +71986,85 @@
                             onClick: i,
                             children: Fr.X
                         })]
                     }), (0, Kr.jsxs)("pre", {
                         className: "box margin",
                         children: [a.loading && (0, Kr.jsx)(no, {
                             label: "Loading Ecosystem"
-                        }), !a.loading && Ui.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
+                        }), !a.loading && Bi.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                     })]
                 })
             },
-            rg = function() {
-                var e = Oh(),
+            lg = function() {
+                var e = Fh(),
                     n = [{
                         type: "stack",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Jh, {
+                            return (0, Kr.jsx)(ng, {
                                 stackName: e,
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "vpcs",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Bh, {
+                            return (0, Kr.jsx)(Hh, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-public",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Yh, {
+                            return (0, Kr.jsx)(Vh, {
                                 type: "public",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-private",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Yh, {
+                            return (0, Kr.jsx)(Vh, {
                                 type: "private",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "security-groups",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Gh, {
+                            return (0, Kr.jsx)(Jh, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "gac",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(tg, {
+                            return (0, Kr.jsx)(sg, {
                                 hide: n
                             })
                         }
                     }, {
                         type: "ecosystem",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(ng, {
+                            return (0, Kr.jsx)(ug, {
                                 hide: n
                             })
                         }
                     }],
-                    r = Eh(n),
-                    o = Eh(n);
+                    r = Uh(n),
+                    o = Uh(n);
                 var i = function() {
                         return r.toggle("vpcs")
                     },
                     a = function() {
                         return r.toggle("ecosystem")
                     };
                 return (0, t.useEffect)((function() {
@@ -71837,15 +72073,15 @@
                     children: (0, Kr.jsx)("tbody", {
                         children: (0, Kr.jsxs)("tr", {
                             children: [(0, Kr.jsxs)("td", {
                                 style: {
                                     verticalAlign: "top",
                                     paddingRight: "8pt"
                                 },
-                                children: [(0, Kr.jsx)(Ph, {
+                                children: [(0, Kr.jsx)(Gh, {
                                     keyedState: e,
                                     showVpcs: function() {
                                         return r.selected("vpcs")
                                     },
                                     toggleVpcs: i,
                                     showSubnetsPublic: function() {
                                         return o.selected("subnets-public")
@@ -71861,26 +72097,26 @@
                                     },
                                     showSecurityGroups: function() {
                                         return o.selected("security-groups")
                                     },
                                     toggleSecurityGroups: function() {
                                         return o.toggle("security-groups")
                                     }
-                                }), (0, Kr.jsx)(Rh, {
+                                }), (0, Kr.jsx)(Wh, {
                                     showGac: function() {
                                         return r.selected("gac")
                                     },
                                     toggleGac: function() {
                                         return r.toggle("gac")
                                     },
                                     showEcosystem: function() {
                                         return r.selected("ecosystem")
                                     },
                                     toggleEcosystem: a
-                                }), (0, Kr.jsx)(qh, {
+                                }), (0, Kr.jsx)(tg, {
                                     toggleStack: function(e) {
                                         return r.toggle("stack", e)
                                     },
                                     selectedStack: function(e) {
                                         return r.selected("stack", e)
                                     }
                                 })]
@@ -71909,16 +72145,16 @@
                                     }, t.key)
                                 }))
                             })]
                         })
                     })
                 })
             },
-            og = function(e) {
-                var t = Xi();
+            cg = function(e) {
+                var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-warn",
                             style: {
@@ -71946,66 +72182,88 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            ig = function() {
+            dg = function() {
                 var e = ce().state.url;
                 return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, Kr.jsx)(xe, {
                     to: e,
                     replace: !0
                 })
             },
-            ag = function(e) {
+            fg = function(e) {
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box thickborder",
                         style: {
                             marginBottom: "6pt"
                         },
-                        children: (0, Kr.jsx)(Ii, {
+                        children: (0, Kr.jsx)(Si, {
                             certificate: e.certificate
                         })
                     })
                 })
             },
-            sg = function(e) {
+            pg = function(e) {
                 var t, n = a(Re(), 1)[0].get("hostname"),
-                    r = qi("/certificates?hostname=".concat(n));
+                    r = Xi("/certificates?hostname=".concat(n));
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
                         children: [(0, Kr.jsx)("b", {
                             children: "SSL Certificates"
                         }), null === r || void 0 === r || null === (t = r.data) || void 0 === t ? void 0 : t.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(ag, {
+                                children: (0, Kr.jsx)(fg, {
                                     certificate: e
                                 })
                             }, e.serial_number)
                         }))]
                     })
                 })
             },
-            ug = function() {
-                var e = qi("/users/projects", {
+            hg = function(e) {
+                var t = Xi("/portal_access_key");
+                return (0, Kr.jsx)(Kr.Fragment, {
+                    children: (0, Kr.jsxs)("div", {
+                        className: "container",
+                        style: {
+                            width: "800pt"
+                        },
+                        children: [(0, Kr.jsx)("b", {
+                            children: "Portal Access Key"
+                        }), (0, Kr.jsx)("div", {
+                            className: "box thickborder",
+                            style: {
+                                marginBottom: "6pt"
+                            },
+                            children: (0, Kr.jsx)(Ii, {
+                                accessKey: t.data
+                            })
+                        })]
+                    })
+                })
+            },
+            gg = function() {
+                var e = Xi("/users/projects", {
                         cache: !0
                     }),
-                    t = qi("/users/roles", {
+                    t = Xi("/users/roles", {
                         cache: !0
                     }),
-                    n = qi("/users/institutions", {
+                    n = Xi("/users/institutions", {
                         cache: !0
                     }),
-                    r = qi("/users/statuses", {
+                    r = Xi("/users/statuses", {
                         cache: !0
                     }),
                     o = {
                         projectTitle: function(t) {
                             var n, r;
                             return (null === (n = e.data) || void 0 === n || null === (r = n.find((function(e) {
                                 return e.id === t
@@ -72053,15 +72311,15 @@
                             return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                 return o.title(e)
                             })).join(", ")) || ""
                         }
                     };
                 return o
             },
-            lg = [{
+            yg = [{
                 name: "email",
                 label: "Email Address",
                 type: "email",
                 focus: !0,
                 required: !0
             }, {
                 name: "first_name",
@@ -72106,39 +72364,39 @@
                 label: "Updated",
                 readonly: !0
             }, {
                 name: "uuid",
                 label: "UUID",
                 readonly: !0
             }],
-            cg = {
+            mg = {
                 PrincipalInvestigatorLine: function(e) {
                     var t, n, r = e.institution,
-                        o = ug();
+                        o = gg();
                     return (0, Kr.jsx)("div", {
                         style: e.style,
                         children: o.principleInvestigator(r) && (0, Kr.jsxs)("small", {
                             children: [(0, Kr.jsxs)("b", {
                                 children: ["Principle Investigator ", Fr.RightArrow]
                             }), " ", null === (t = o.principleInvestigator(r)) || void 0 === t ? void 0 : t.name, "\xa0", (0, Kr.jsx)(Ni, {
                                 href: kr.Path("/users/".concat(null === (n = o.principleInvestigator(r)) || void 0 === n ? void 0 : n.uuid))
                             })]
                         })
                     })
                 },
                 useUserInputs: function() {
-                    var e = Xi(),
-                        n = At.IsFoursightFourfront(e) ? lg.filter((function(e) {
+                    var e = ta(),
+                        n = At.IsFoursightFourfront(e) ? yg.filter((function(e) {
                             return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                        })) : lg;
+                        })) : yg;
                     return (0, t.useState)(Tr.Clone(Tr.Clone(n)))
                 }
             },
-            dg = function(e) {
-                var t = qi("/users/".concat(e.email, "?raw=true"));
+            vg = function(e) {
+                var t = Xi("/users/".concat(e.email, "?raw=true"));
                 return (0, Kr.jsxs)("pre", {
                     className: "box",
                     children: [(0, Kr.jsx)("span", {
                         style: {
                             float: "right",
                             marginTop: "-6pt",
                             fontSize: "large",
@@ -72147,19 +72405,19 @@
                         onClick: function() {
                             return t.refresh()
                         },
                         children: Fr.Refresh
                     }), t.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {})
                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                        children: Ui.Format(t.data)
+                        children: Bi.Format(t.data)
                     })]
                 })
             },
-            fg = function(e) {
+            Mg = function(e) {
                 var n = {
                         color: "var(--box-fg)",
                         fontWeight: "bold",
                         fontSize: "small",
                         paddingTop: "1pt",
                         verticalAlign: "top",
                         width: "5%",
@@ -72268,16 +72526,16 @@
                                     })]
                                 }, o.name)
                             }))
                         })
                     })
                 })
             },
-            pg = function(e) {
-                var t = ug(),
+            bg = function(e) {
+                var t = gg(),
                     n = [{
                         label: "Email",
                         name: "email"
                     }, {
                         label: "First Name",
                         name: "first_name"
                     }, {
@@ -72300,26 +72558,26 @@
                         name: "role",
                         map: function(n) {
                             return t.userRoleTitle(e.user, e.user.project)
                         }
                     }, {
                         label: "Roles",
                         name: "roles",
-                        ui: (0, Kr.jsx)(hg, {
+                        ui: (0, Kr.jsx)(wg, {
                             user: e.user
                         }),
                         toggle: !0
                     }, {
                         label: "Institution",
                         name: "institution",
                         map: function(e) {
                             return t.institutionTitle(e)
                         },
                         subComponent: function(e) {
-                            return (0, Kr.jsx)(cg.PrincipalInvestigatorLine, {
+                            return (0, Kr.jsx)(mg.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         }
                     }, {
                         label: "Status",
                         name: "status",
                         map: function(e) {
@@ -72337,24 +72595,24 @@
                         map: function(e) {
                             return Pr.FormatDateTime(e)
                         }
                     }, {
                         label: "UUID",
                         name: "uuid"
                     }];
-                return At.IsFoursightFourfront(Xi()) && (n = n.filter((function(e) {
+                return At.IsFoursightFourfront(ta()) && (n = n.filter((function(e) {
                     return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                }))), (0, Kr.jsx)(fg, {
+                }))), (0, Kr.jsx)(Mg, {
                     keys: n,
                     value: e.user,
                     separators: !0
                 })
             },
-            hg = function(e) {
-                var t = ug();
+            wg = function(e) {
+                var t = gg();
                 return (0, Kr.jsx)("div", {
                     className: "box lighten",
                     style: {
                         marginTop: "2pt",
                         marginBottom: "2pt"
                     },
                     children: (0, Kr.jsx)("table", {
@@ -72417,21 +72675,21 @@
                                     })]
                                 }, e.project)
                             }))]
                         })
                     })
                 })
             },
-            gg = function(e) {
+            jg = function(e) {
                 var n, r, o, i = pe().email,
                     s = a((0, t.useState)(!1), 2),
                     u = s[0],
                     l = s[1],
                     c = fe();
-                var d = qi({
+                var d = Xi({
                     url: "/users/".concat(i),
                     onData: function(e) {
                         return st.IsObject(e) ? [e] : e
                     },
                     nofetch: !0
                 });
                 return (0, t.useEffect)((function() {
@@ -72541,26 +72799,26 @@
                                             float: "right",
                                             fontSize: "small",
                                             marginTop: "-1pt",
                                             marginRight: "2pt"
                                         },
                                         children: "Edit"
                                     })]
-                                }), u ? (0, Kr.jsx)(dg, {
+                                }), u ? (0, Kr.jsx)(vg, {
                                     email: e.email
-                                }) : (0, Kr.jsx)(pg, {
+                                }) : (0, Kr.jsx)(bg, {
                                     user: e
                                 })]
                             }, e.uuid)
                         }))]
                     })
                 })
             },
-            yg = function(e) {
-                var n = qi(e.url, {
+            xg = function(e) {
+                var n = Xi(e.url, {
                         nofetch: !0,
                         cache: !0
                     }),
                     r = a((0, t.useState)(e.selected), 2),
                     o = r[0],
                     i = r[1];
                 return (0, t.useEffect)((function() {
@@ -72592,15 +72850,15 @@
                             }, e.id) : null
                         }))]
                     }), e.subComponent && (0, Kr.jsx)(Kr.Fragment, {
                         children: e.subComponent(o)
                     })]
                 })
             },
-            mg = function(e) {
+            Ng = function(e) {
                 var n = e.inputs,
                     r = (e.setInputs, e.title, e.loading),
                     o = e.onCreate,
                     i = e.onUpdate,
                     u = e.onDelete,
                     l = e.onCancel,
                     c = e.onRefresh,
@@ -72852,15 +73110,15 @@
                                                         }), (0, Kr.jsx)("option", {
                                                             value: !0,
                                                             children: "True"
                                                         })]
                                                     })
                                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                                     children: "select" === e.type ? (0, Kr.jsx)(Kr.Fragment, {
-                                                        children: (0, Kr.jsx)(yg, {
+                                                        children: (0, Kr.jsx)(xg, {
                                                             id: e.name,
                                                             url: e.url,
                                                             required: e.required,
                                                             selected: z(e),
                                                             onChange: T,
                                                             disabled: F() || e.readonly,
                                                             setLoadingCount: S,
@@ -73036,28 +73294,28 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            vg = function() {
-                var e = qi(zt.Url("/users"), {
+            Ig = function() {
+                var e = Xi(zt.Url("/users"), {
                         method: "POST",
                         nofetch: !0
                     }),
-                    n = a(cg.useUserInputs(), 2),
+                    n = a(mg.useUserInputs(), 2),
                     r = n[0],
                     o = (n[1], fe());
                 return (0, t.useEffect)((function() {
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(cg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(mg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), []), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73084,15 +73342,15 @@
                                                 children: "List"
                                             })
                                         })
                                     })]
                                 })
                             }), (0, Kr.jsx)("tr", {
                                 children: (0, Kr.jsx)("td", {
-                                    children: (0, Kr.jsx)(mg, {
+                                    children: (0, Kr.jsx)(Ng, {
                                         title: "Edit User",
                                         inputs: r,
                                         onCreate: function(t) {
                                             t.admin ? (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: ["admin"]
                                             })) : (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: []
@@ -73112,24 +73370,24 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            Mg = function() {
+            Dg = function() {
                 var e = pe().uuid,
-                    n = a(cg.useUserInputs(), 2),
+                    n = a(mg.useUserInputs(), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)(!1), 2),
                     l = i[0],
                     c = i[1],
-                    d = a(ua(), 1)[0],
-                    f = qi({
+                    d = a(da(), 1)[0],
+                    f = Xi({
                         url: "/users/".concat(e),
                         nofetch: !0,
                         onData: function(e) {
                             o((function(t) {
                                 var n, r = s(t);
                                 try {
                                     for (r.s(); !(n = r.n()).done;) {
@@ -73146,27 +73404,27 @@
                                 return u(t)
                             }))
                         },
                         onError: function(e) {
                             404 === e.status && c(!0)
                         }
                     }),
-                    p = ug(),
+                    p = gg(),
                     h = fe();
 
                 function g() {
                     h(kr.Path("/users/".concat(e)))
                 }
                 return (0, t.useEffect)((function() {
                     f.fetch();
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(cg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(mg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), [e]), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73207,15 +73465,15 @@
                                             children: ["The specified user was not found: ", e, " ", (0, Kr.jsx)("p", {}), (0, Kr.jsx)("button", {
                                                 className: "button cancel",
                                                 onClick: g,
                                                 children: "Cancel"
                                             })]
                                         })
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                                        children: (0, Kr.jsx)(mg, {
+                                        children: (0, Kr.jsx)(Ng, {
                                             title: "Edit User",
                                             inputs: r,
                                             setInputs: o,
                                             onUpdate: function(t) {
                                                 var n, r = (null === (n = f.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                     return "admin" !== e
                                                 }))) || [];
@@ -73250,15 +73508,15 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            bg = function(e) {
+            Sg = function(e) {
                 var n, r = e.columns,
                     o = e.data,
                     i = e.update,
                     s = e.initialSort,
                     u = e.children,
                     l = a(Re(), 2),
                     c = l[0],
@@ -73339,15 +73597,15 @@
                         border: "0",
                         children: (0, Kr.jsx)("tbody", {
                             children: (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: {
                                         width: "90%"
                                     },
-                                    children: (0, Kr.jsx)(Za, {
+                                    children: (0, Kr.jsx)(Ja, {
                                         pages: _,
                                         page: k,
                                         onChange: function(e) {
                                             var t = e.selected;
                                             m(t * p)
                                         },
                                         refresh: R,
@@ -73418,15 +73676,15 @@
                             marginTop: "4pt",
                             paddingTop: "8pt"
                         },
                         children: (0, Kr.jsxs)("table", {
                             style: {
                                 width: "100%"
                             },
-                            children: [(0, Kr.jsx)(ia, {
+                            children: [(0, Kr.jsx)(ua, {
                                 columns: r,
                                 sort: M,
                                 list: null === o || void 0 === o || null === (n = o.data) || void 0 === n ? void 0 : n.list,
                                 update: function(e, t) {
                                     b("".concat(e, ".").concat(t))
                                 },
                                 bottomline: !0,
@@ -73438,27 +73696,27 @@
                             }), (0, Kr.jsx)("tbody", {
                                 children: u
                             })]
                         })
                     })]
                 })
             },
-            wg = function() {
+            Lg = function() {
                 var e = pe().environ,
                     n = a(Re(), 2),
                     r = n[0],
                     o = n[1],
-                    i = qi(),
+                    i = Xi(),
                     s = a((0, t.useState)(r.get("search") || ""), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(it.HasValue(u)), 2),
                     d = c[0],
                     f = c[1],
-                    p = ug();
+                    p = gg();
 
                 function h(t) {
                     var n = t.limit,
                         o = t.offset,
                         a = t.sort,
                         s = t.search,
                         u = t.onDone;
@@ -73585,15 +73843,15 @@
                                 style: {
                                     height: "1px",
                                     background: Ft.GetForegroundColor(),
                                     marginTop: "2pt",
                                     marginBottom: "4pt"
                                 }
                             })]
-                        }), (0, Kr.jsx)(bg, {
+                        }), (0, Kr.jsx)(Sg, {
                             columns: [{
                                 label: ""
                             }, {
                                 label: "User",
                                 key: "email"
                             }, {
                                 label: "Groups",
@@ -73722,30 +73980,30 @@
                                     })]
                                 }, e.uuid)
                             }))
                         })]
                     })
                 })
             },
-            jg = function() {
-                var e = Xi();
+            kg = function() {
+                var e = ta();
 
                 function t() {
                     return "/api/react/".concat(At.PreferredName(At.Default(e)), "/login")
                 }
                 return (0, Kr.jsx)(Ae, {
-                    children: (0, Kr.jsxs)(ls, {
-                        children: [(0, Kr.jsx)(us, {}), (0, Kr.jsx)("div", {
+                    children: (0, Kr.jsxs)(gs, {
+                        children: [(0, Kr.jsx)(hs, {}), (0, Kr.jsx)("div", {
                             style: {
                                 margin: "14pt"
                             },
                             children: (0, Kr.jsxs)(De, {
                                 children: [(0, Kr.jsx)(Ne, {
                                     path: "/api/react/cognito/callback",
-                                    element: (0, Kr.jsx)(Dh, {})
+                                    element: (0, Kr.jsx)(_h, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/",
                                     element: (0, Kr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api",
@@ -73760,127 +74018,132 @@
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ",
                                     element: (0, Kr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/accounts",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(oa, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(sa, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/env",
-                                    element: (0, Kr.jsx)(Ai.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(es, {})
+                                    element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
+                                        children: (0, Kr.jsx)(rs, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/env",
-                                    element: (0, Kr.jsx)(Ai.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(es, {})
+                                    element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
+                                        children: (0, Kr.jsx)(rs, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/login",
-                                    element: (0, Kr.jsx)(Ai.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(Lh, {})
+                                    element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
+                                        children: (0, Kr.jsx)(Ah, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Ga, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Za, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks/:check/history",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Xa, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(ts, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/home",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(cs, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(ys, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/info",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(ps, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Ms, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(wg, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Lg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/:email",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(gg, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(jg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/edit/:uuid",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Mg, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Dg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/create",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(vg, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Ig, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/gac/:environCompare",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(kh, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(Oh, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/s3",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(aa, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(la, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/infrastructure",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(rg, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(lg, {})
+                                    })
+                                }), (0, Kr.jsx)(Ne, {
+                                    path: "/api/react/:environ/certificates",
+                                    element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
+                                        children: (0, Kr.jsx)(pg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
-                                    path: "/api/react/:environ/certificate",
-                                    element: (0, Kr.jsx)(Ai.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(sg, {})
+                                    path: "/api/react/:environ/portal_access_key",
+                                    element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
+                                        children: (0, Kr.jsx)(hg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/forbidden",
-                                    element: (0, Kr.jsx)(ns, {})
+                                    element: (0, Kr.jsx)(is, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/error",
-                                    element: (0, Kr.jsx)(ki, {})
+                                    element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/error",
-                                    element: (0, Kr.jsx)(ki, {})
+                                    element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/redirect",
-                                    element: (0, Kr.jsx)(ig, {})
+                                    element: (0, Kr.jsx)(dg, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "*",
-                                    element: (0, Kr.jsx)(Ai.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(og, {})
+                                    element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
+                                        children: (0, Kr.jsx)(cg, {})
                                     })
                                 })]
                             })
-                        }), (0, Kr.jsx)(ts, {})]
+                        }), (0, Kr.jsx)(os, {})]
                     })
                 })
             },
-            xg = r.createRoot(document.getElementById("root"));
-        "1" === bt.Get("test_mode_strict_mode") ? xg.render((0, Kr.jsx)(t.StrictMode, {
-            children: (0, Kr.jsx)(jg, {})
-        })) : xg.render((0, Kr.jsx)("table", {
+            Cg = r.createRoot(document.getElementById("root"));
+        "1" === bt.Get("test_mode_strict_mode") ? Cg.render((0, Kr.jsx)(t.StrictMode, {
+            children: (0, Kr.jsx)(kg, {})
+        })) : Cg.render((0, Kr.jsx)("table", {
             style: {
                 width: "100%"
             },
             cellPadding: "0",
             cellSpacing: "0",
             children: (0, Kr.jsx)("tbody", {
                 children: (0, Kr.jsx)("tr", {
                     children: (0, Kr.jsx)("td", {
-                        children: (0, Kr.jsx)(jg, {})
+                        children: (0, Kr.jsx)(kg, {})
                     })
                 })
             })
         }))
     }()
 })();
```

### Comparing `foursight_core-4.1.0.1b5/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.1b6/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/routes.py` & `foursight_core-4.1.0.1b6/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/run_result.py` & `foursight_core-4.1.0.1b6/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/run_result.py-deb` & `foursight_core-4.1.0.1b6/foursight_core/run_result.py-deb`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/s3_connection.py` & `foursight_core-4.1.0.1b6/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/sav` & `foursight_core-4.1.0.1b6/foursight_core/sav`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.1b6/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/schedule_decorator.py-` & `foursight_core-4.1.0.1b6/foursight_core/schedule_decorator.py-`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.1b6/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.1b6/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/scripts/save/decrypt_accounts_file.py` & `foursight_core-4.1.0.1b6/foursight_core/scripts/save/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/scripts/save/encrypt_accounts_file.py` & `foursight_core-4.1.0.1b6/foursight_core/scripts/save/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.1b6/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/stage.py` & `foursight_core-4.1.0.1b6/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/base.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/header.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/history.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/info.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/unused.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/user.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/users.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.1b6/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/foursight_core/x` & `foursight_core-4.1.0.1b6/foursight_core/x`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.1b5/pyproject.toml` & `foursight_core-4.1.0.1b6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.1b5"
+version = "4.1.0.1b6"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
-cryptography = "39.0.0" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "7.2.0.1b2"
+cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
+dcicutils = "7.2.0.1b3"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
```

### Comparing `foursight_core-4.1.0.1b5/setup.py` & `foursight_core-4.1.0.1b6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
  'cron-descriptor>=1.2.31,<2.0.0',
- 'cryptography==39.0.0',
- 'dcicutils==7.2.0.1b2',
+ 'cryptography==39.0.2',
+ 'dcicutils==7.2.0.1b3',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch==7.13.4',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.12.5,<2.0.0',
  'google-auth-oauthlib>=0.7.0,<0.8.0',
  'google>=3.0.0,<4.0.0',
@@ -45,15 +45,15 @@
 {'console_scripts': ['decrypt-accounts-file = '
                      'foursight_core.scripts.decrypt_accounts_file:main',
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main']}
 
 setup_kwargs = {
     'name': 'foursight-core',
-    'version': '4.1.0.1b5',
+    'version': '4.1.0.1b6',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_core-4.1.0.1b5/PKG-INFO` & `foursight_core-4.1.0.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.1b5
+Version: 4.1.0.1b6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
-Requires-Dist: cryptography (==39.0.0)
-Requires-Dist: dcicutils (==7.2.0.1b2)
+Requires-Dist: cryptography (==39.0.2)
+Requires-Dist: dcicutils (==7.2.0.1b3)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```

