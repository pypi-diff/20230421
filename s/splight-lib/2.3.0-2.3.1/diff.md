# Comparing `tmp/splight-lib-2.3.0.tar.gz` & `tmp/splight-lib-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.3.0.tar", last modified: Wed Apr 19 19:04:25 2023, max compression
+gzip compressed data, was "splight-lib-2.3.1.tar", last modified: Fri Apr 21 15:07:57 2023, max compression
```

## Comparing `splight-lib-2.3.0.tar` & `splight-lib-2.3.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.000000 splight-lib-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-19 19:04:25.831708 splight-lib-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 19:04:25.000000 splight-lib-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.811708 splight-lib-2.3.0/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 19:04:25.000000 splight-lib-2.3.0/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:04:25.831708 splight-lib-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 19:04:25.000000 splight-lib-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.815708 splight-lib-2.3.0/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.819708 splight-lib-2.3.0/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.827708 splight-lib-2.3.0/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.823708 splight-lib-2.3.0/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:25.831708 splight-lib-2.3.0/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 19:04:25.000000 splight-lib-2.3.0/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:56.000000 splight-lib-2.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 15:07:57.054808 splight-lib-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 15:07:56.000000 splight-lib-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 15:07:56.000000 splight-lib-2.3.1/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:07:57.054808 splight-lib-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-21 15:07:56.000000 splight-lib-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.046807 splight-lib-2.3.1/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.050807 splight-lib-2.3.1/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 15:07:57.000000 splight-lib-2.3.1/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:07:57.054808 splight-lib-2.3.1/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-21 15:07:56.000000 splight-lib-2.3.1/splight_models/webhook.py
```

### Comparing `splight-lib-2.3.0/PKG-INFO` & `splight-lib-2.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.0/remote_splight_lib/communication/client.py` & `splight-lib-2.3.1/remote_splight_lib/communication/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+import logging
+from typing import Callable, Dict
+
 import pysher
 import requests
 from furl import furl
+from remote_splight_lib.auth.auth import SplightAuthToken
+from remote_splight_lib.communication.classmap import CLASSMAP
+from remote_splight_lib.settings import settings
 from retry import retry
-from typing import Callable, Dict
-from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_abstract.communication import (
     AbstractCommunicationClient,
     ClientNotReady,
 )
-import logging
-from splight_models.communication import CommunicationClientStatus, CommunicationContext, CommunicationEvent
-
-from remote_splight_lib.auth.auth import SplightAuthToken
-from remote_splight_lib.settings import settings
-from remote_splight_lib.communication.classmap import CLASSMAP
-
+from splight_lib.logging._internal import LogTags, get_splight_logger
+from splight_models.communication import (
+    CommunicationClientStatus,
+    CommunicationContext,
+    CommunicationEvent,
+)
 
 logger = get_splight_logger()
 
 
 class CommunicationFactory:
-
     def __init__(self, model):
         self._model = model
 
     def get_url(self):
         base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         return base_url / CLASSMAP.get(self._model)
 
@@ -32,47 +34,62 @@
         auth_token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         return auth_token.header
 
     def create(self, data: Dict):
-        response = requests.post(self.get_url(), json=data, headers=self.get_headers())
-        assert response.status_code == 201, f"Cant create communication {self._model}."
+        response = requests.post(
+            self.get_url(), json=data, headers=self.get_headers()
+        )
+        assert (
+            response.status_code == 201
+        ), f"Cant create communication {self._model}."
         return self._model.parse_obj(response.json())
 
     def get(self, params=None):
-        response = requests.get(self.get_url(), params=params, headers=self.get_headers())
-        assert response.status_code == 200, f"Cant fetch communication {self._model}."
+        response = requests.get(
+            self.get_url(), params=params, headers=self.get_headers()
+        )
+        assert (
+            response.status_code == 200
+        ), f"Cant fetch communication {self._model}."
         data = response.json()
         return self._model.parse_obj(data)
 
 
 class CommunicationClient(AbstractCommunicationClient):
-
     def __init__(self, daemon: bool = True, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._status = CommunicationClientStatus.STOPPED
         self._channel_bindings = []
         self._client, self._context = None, None
         self._system_bindings = [
-            ("pusher:connection_established", self.__on_connection_established),
+            (
+                "pusher:connection_established",
+                self.__on_connection_established,
+            ),
             ("pusher:connection_failed", self.__on_connection_failed),
             ("pusher:error", self.__on_error),
         ]
         self._daemon = daemon
         try:
             self.__load_context()
             self.__load_client()
             self.__check_readiness()
-            logger.info("Communication client started.", tags=LogTags.COMMUNICATION)
+            logger.info(
+                "Communication client started.", tags=LogTags.COMMUNICATION
+            )
         except Exception as e:
             logger.warning(
                 "Failed to start communication client due to exception %s. Moving forward without remote commands.",
-                e, exc_info=True, tags=LogTags.COMMUNICATION)
+                e,
+                exc_info=True,
+                tags=LogTags.COMMUNICATION,
+            )
             self._status = CommunicationClientStatus.ERROR
 
     @property
     def status(self):
         return self._status
 
     @property
@@ -93,51 +110,62 @@
     def __load_client(self):
         if not self._context:
             raise NotImplementedError
         self._client = pysher.Pusher(
             key=self._context.key,
             auth_endpoint=self._context.auth_endpoint,
             auth_endpoint_headers=self._context.auth_headers,
-            user_data=self._context.channel_data.dict() if self.context.channel_data else None,
+            user_data=self._context.channel_data.dict()
+            if self.context.channel_data
+            else None,
             daemon=self._daemon,
-            log_level=logging.WARNING
+            log_level=logging.WARNING,
         )
         self.__bind_system_events()
         self._client.connect()
 
     def __bind_system_events(self):
         if self._client is None:
             return
         for event, handler in self._system_bindings:
             self._client.connection.bind(event, handler)
 
     def __on_connection_established(self, data):
         self._channel = self._client.subscribe(self._context.channel)
-        self._private_room_channel = self._client.subscribe(self._context.private_room_channel)
+        self._private_room_channel = self._client.subscribe(
+            self._context.private_room_channel
+        )
         for event_name, event_handler in self._channel_bindings:
             self._channel.bind(event_name, event_handler)
             self._private_room_channel.bind(event_name, event_handler)
         self._status = CommunicationClientStatus.READY
 
     def __on_connection_failed(self, data):
         self._status = CommunicationClientStatus.FAILED
 
     def __on_error(self, data):
         logger.error("Error on message %s", data, tags=LogTags.COMMUNICATION)
 
     def bind(self, event_name: str, event_handler: Callable) -> None:
         self._channel_bindings.append((event_name, event_handler))
         if self.status != CommunicationClientStatus.READY:
-            logger.warning("Bind events failed due to comm client is not ready", tags=LogTags.COMMUNICATION)
+            logger.warning(
+                "Bind events failed due to comm client is not ready",
+                tags=LogTags.COMMUNICATION,
+            )
             return
         self._channel.bind(event_name, event_handler)
         self._private_room_channel.bind(event_name, event_handler)
 
     def unbind(self, event_name: str, event_handler: Callable) -> None:
         # TODO implement this
         raise NotImplementedError
 
     def trigger(self, event: CommunicationEvent):
-        return CommunicationFactory(CommunicationEvent).create(data=event.dict())
+        return CommunicationFactory(CommunicationEvent).create(
+            data=event.dict()
+        )
 
-    def authenticate(self, channel_name: str, socket_id: str, custom_data: Dict = None) -> Dict:
+    def authenticate(
+        self, channel_name: str, socket_id: str, custom_data: Dict = None
+    ) -> Dict:
         raise NotImplementedError
```

### Comparing `splight-lib-2.3.0/remote_splight_lib/database/client.py` & `splight-lib-2.3.1/remote_splight_lib/database/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import json
-from .classmap import CLASSMAP
-from retry import retry
-from splight_abstract.remote import AbstractRemoteClient
-from splight_abstract.database import AbstractDatabaseClient
-from splight_models import File
-from remote_splight_lib.settings import settings
-from remote_splight_lib.exceptions import InvalidModel
-from remote_splight_lib.auth import SplightAuthToken
-from splight_lib.logging._internal import get_splight_logger, LogTags
-from splight_lib.encryption import EncryptionClient
+from tempfile import NamedTemporaryFile
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
+from remote_splight_lib.auth import SplightAuthToken
+from remote_splight_lib.exceptions import InvalidModel
+from remote_splight_lib.settings import settings
 from requests import Session
-from requests.exceptions import (
-    ConnectionError,
-    Timeout
-)
-from tempfile import NamedTemporaryFile
+from requests.exceptions import ConnectionError, Timeout
+from retry import retry
+from splight_abstract.database import AbstractDatabaseClient
+from splight_abstract.remote import AbstractRemoteClient
+from splight_lib.encryption import EncryptionClient
+from splight_lib.logging._internal import LogTags, get_splight_logger
+from splight_models import File
 
+from .classmap import CLASSMAP
 
 logger = get_splight_logger()
 
 REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
 
 
 class DatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
@@ -143,19 +140,26 @@
         InvalidModel thrown when the model name is not correct.
         """
 
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         kwargs["page"] = 1  # Always start from the first page
         response = self._list(path, **kwargs)
-        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
+        logger.debug(
+            "Counted %s objects of type: %s.",
+            response["count"],
+            resource_type,
+            tags=LogTags.DATABASE,
+        )
         return response["count"]
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def download(self, instance: BaseModel, decrypt: bool = True, **kwargs) -> NamedTemporaryFile:
+    def download(
+        self, instance: BaseModel, decrypt: bool = True, **kwargs
+    ) -> NamedTemporaryFile:
         """Returns the number of resources in the database for a given model
 
         Parameters
         ----------
         instance : BaseModel
             The instance of the model to be downloaded
 
@@ -209,15 +213,15 @@
             raise InvalidModel(constructor.schema()["title"])
         return model_data
 
     def _create(self, path: str, instance: BaseModel) -> Dict:
         url = self._base_url / f"{path}/"
         data = json.loads(instance.json(exclude_none=True))
         if isinstance(instance, File):
-            with open(instance.file, 'rb') as f:
+            with open(instance.file, "rb") as f:
                 file = {"file": f}
                 response = self._session.post(url, data=data, files=file)
         else:
             response = self._session.post(url, json=data)
 
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.3.0/remote_splight_lib/datalake/client.py` & `splight-lib-2.3.1/remote_splight_lib/datalake/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,53 @@
+import json
 from datetime import timedelta, timezone
 from io import StringIO
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Union
 
 import pandas as pd
-import json
 from furl import furl
 from pydantic import BaseModel
-
 from remote_splight_lib.auth import SplightAuthToken
-from splight_lib.logging._internal import get_splight_logger, LogTags
 from remote_splight_lib.settings import settings
-from splight_abstract import AbstractRemoteClient, QuerySet
-from splight_abstract.datalake import AbstractDatalakeClient, validate_resource_type, validate_instance_type
-from splight_models import Query, DatalakeModel
 from retry import retry
-
+from splight_abstract import AbstractRemoteClient, QuerySet
+from splight_abstract.datalake import (
+    AbstractDatalakeClient,
+    validate_instance_type,
+    validate_resource_type,
+)
+from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import (
-    SplightRestClient,
+    ConnectError,
     HTTPError,
+    SplightRestClient,
     Timeout,
-    ConnectError
 )
+from splight_models import DatalakeModel, Query
 
 logger = get_splight_logger()
 
 REQUEST_EXCEPTIONS = (HTTPError, Timeout, ConnectError)
 
 
 class DatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
-
     _PREFIX = "v2/engine/datalake"
 
     def __init__(self, namespace: str = "default"):
         super(DatalakeClient, self).__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
         logger.info("Datalake client initialized.", tags=LogTags.DATALAKE)
 
-
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def _raw_save(
         self,
         collection: str,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
         url = self._base_url / f"{self._PREFIX}/save/"
@@ -107,61 +107,77 @@
     @validate_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
-        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving object of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(self, *args, **kwargs)
 
-    def get_output(self, resource_type: DatalakeModel, query: Query) -> List[Dict]:
+    def get_output(
+        self, resource_type: DatalakeModel, query: Query
+    ) -> List[Dict]:
         # TODO: Add add_fields, project and renaming
-        logger.debug("Retrieving output of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving output of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
         return self._raw_get(
             resource_type=resource_type,
             collection=query.source,
             limit_=query.limit,
             skip_=query.skip,
             sort=query.sort,
             group_id=query.group_id,
             group_fields=query.group_fields,
             tzinfo=timezone(timedelta(hours=query.timezone_offset)),
-            **query.filters
+            **query.filters,
         )
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     @validate_resource_type
-    def get_dataframe(self, resource_type: DatalakeModel, **kwargs) -> pd.DataFrame:
+    def get_dataframe(
+        self, resource_type: DatalakeModel, **kwargs
+    ) -> pd.DataFrame:
         # GET /datalake/dumpdata/?source=collection
         url = self._base_url / f"{self._PREFIX}/dumpdata/"
         collection = resource_type.Meta.collection_name
         kwargs.update({"source": collection})
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
         response.raise_for_status()
-        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving dataframe from datalake.", tags=LogTags.DATALAKE
+        )
 
         df: pd.DataFrame = pd.DataFrame(pd.read_csv(StringIO(response.text)))
         if df.empty:
             return df
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df.set_index("timestamp", inplace=True)
         return df
 
     def get_dataset(
         self, resource_type: DatalakeModel, queries: List[Dict]
     ) -> pd.DataFrame:
         # TODO this should be
         # def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
-        logger.debug("Retrieving dataset from datalake.", tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving dataset from datalake.", tags=LogTags.DATALAKE
+        )
 
         dfs = [
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
@@ -178,15 +194,17 @@
             return instances
         resource_type = instances[0].__class__
         collection = resource_type.Meta.collection_name
         return self._raw_save(collection=collection, instances=instances)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     @validate_resource_type
-    def save_dataframe(self, resource_type: DatalakeModel, dataframe: pd.DataFrame) -> None:
+    def save_dataframe(
+        self, resource_type: DatalakeModel, dataframe: pd.DataFrame
+    ) -> None:
         # POST /datalake/loaddata/
         logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
 
         url = self._base_url / f"{self._PREFIX}/loaddata/"
 
         tmp_file = NamedTemporaryFile("w")
         with open(tmp_file.name, "wb") as fid:
@@ -197,33 +215,45 @@
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
     @validate_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
-        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Deleting resources of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
 
         collection = resource_type.Meta.collection_name
         return self._raw_delete(collection=collection, **kwargs)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def create_index(self, collection: str, indexes: List[Dict]) -> None:
         # POST /datalake/index/
-        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Creating index for collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
         url = self._base_url / f"{self._PREFIX}/index/"
         data = {"source": collection, "index": indexes}
         response = self._restclient.post(url, json=data)
         response.raise_for_status()
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
-        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Aggregate on datalake collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
         # POST /datalake/aggregate/?source=collection
         url = self._base_url / f"{self._PREFIX}/aggregate/"
         params = {"source": collection}
         data = {"pipeline": pipeline}
         response = self._restclient.post(url, params=params, data=data)
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.3.0/remote_splight_lib/hub/client.py` & `splight-lib-2.3.1/remote_splight_lib/hub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict, List, Optional, Tuple, Type
 
 import requests
 from furl import furl
 from pydantic import BaseModel
-
 from remote_splight_lib.auth import SplightAuthToken
 from remote_splight_lib.settings import settings
 from splight_abstract import (
     AbstractHubClient,
     AbstractHubSubClient,
     validate_resource_type,
 )
@@ -127,15 +126,14 @@
         response = self._session.post(url, headers=self.headers)
         assert (
             response.status_code == 204
         ), f"Failed to rebuild component. {response.content}"
 
 
 class SplightHubClient(AbstractHubClient):
-
     def __init__(
         self, headers: Optional[Dict[str, str]] = {}, *args, **kwargs
     ) -> None:
         super().__init__()
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
```

### Comparing `splight-lib-2.3.0/remote_splight_lib/settings.py` & `splight-lib-2.3.1/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/setup.py` & `splight-lib-2.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="2.3.0",
+    version="2.3.1",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.3.0/splight_abstract/auth/abstract.py` & `splight-lib-2.3.1/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_abstract/auth/exceptions.py` & `splight-lib-2.3.1/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_abstract/cache/abstract.py` & `splight-lib-2.3.1/splight_abstract/cache/abstract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
+from abc import abstractmethod
 from functools import wraps
 from typing import Callable, List
-from abc import abstractmethod
-from splight_abstract.client import AbstractClient
-from splight_lib.logging._internal import get_splight_logger, LogTags
 
+from splight_abstract.client import AbstractClient
+from splight_lib.logging._internal import LogTags, get_splight_logger
 
 logger = get_splight_logger()
 
-class AbstractCacheClient(AbstractClient):
 
+class AbstractCacheClient(AbstractClient):
     @abstractmethod
     def get(self, key):
         pass
 
     @abstractmethod
     def set(self, key, value):
         pass
@@ -22,71 +22,109 @@
     def delete(self, key):
         pass
 
     @abstractmethod
     def clear(self):
         pass
 
+
 # Decorators
-def get_cache(client: AbstractCacheClient, cache_key: str, cache_key_args: str or List[str] = None) -> Callable:
+def get_cache(
+    client: AbstractCacheClient,
+    cache_key: str,
+    cache_key_args: str or List[str] = None,
+) -> Callable:
     def decorator(func: Callable) -> Callable:
         @wraps(func)
         def wrapper(*args, **kwargs) -> Callable:
             final_cache_key = cache_key
             cached_data = None
             full_args = dict(zip(func.__code__.co_varnames, args))
             full_args.update(kwargs)
             if cache_key_args is not None:
                 if isinstance(cache_key_args, str):
-                    final_cache_key = f'{final_cache_key}:{cache_key_args}-{str(full_args.get(cache_key_args))}'
+                    final_cache_key = f"{final_cache_key}:{cache_key_args}-{str(full_args.get(cache_key_args))}"
                 else:
                     for key_arg in cache_key_args:
-                        final_cache_key = f'{final_cache_key}:{key_arg}-{str(full_args.get(key_arg))}'
+                        final_cache_key = f"{final_cache_key}:{key_arg}-{str(full_args.get(key_arg))}"
 
             try:
                 cached_data = client.get(final_cache_key)
             except Exception:
-                logger.error('Error getting cache for %s', final_cache_key, tags=LogTags.CACHE)
+                logger.error(
+                    "Error getting cache for %s",
+                    final_cache_key,
+                    tags=LogTags.CACHE,
+                )
 
             if isinstance(cached_data, bytes):
-                logger.info('Cache hit for %s', final_cache_key, tags=LogTags.CACHE)
+                logger.info(
+                    "Cache hit for %s", final_cache_key, tags=LogTags.CACHE
+                )
 
-                return json.loads(cached_data.decode('utf-8'))
+                return json.loads(cached_data.decode("utf-8"))
             else:
                 cached_data = func(*args, **kwargs)
 
                 try:
-                    client.set(final_cache_key, json.dumps(cached_data), ex=3600)
-                    logger.info('Cache update for %s', final_cache_key, tags=LogTags.CACHE)
+                    client.set(
+                        final_cache_key, json.dumps(cached_data), ex=3600
+                    )
+                    logger.info(
+                        "Cache update for %s",
+                        final_cache_key,
+                        tags=LogTags.CACHE,
+                    )
                 except Exception:
-                    logger.error('Error getting cache for %s', final_cache_key, tags=LogTags.CACHE)
+                    logger.error(
+                        "Error getting cache for %s",
+                        final_cache_key,
+                        tags=LogTags.CACHE,
+                    )
 
                 return cached_data
+
         return wrapper
+
     return decorator
 
 
-def flush_cache(client: AbstractCacheClient, cache_key: str, cache_key_args: str or List[str] = None, prefix_match=False) -> Callable:
+def flush_cache(
+    client: AbstractCacheClient,
+    cache_key: str,
+    cache_key_args: str or List[str] = None,
+    prefix_match=False,
+) -> Callable:
     def decorator(func: Callable) -> Callable:
         @wraps(func)
         def wrapper(*args, **kwargs) -> Callable:
             final_cache_key = cache_key
             full_args = dict(zip(func.__code__.co_varnames, args))
             full_args.update(kwargs)
             if cache_key_args is not None:
                 if isinstance(cache_key_args, str):
-                    final_cache_key = f'{final_cache_key}:{cache_key_args}-{str(full_args.get(cache_key_args))}'
+                    final_cache_key = f"{final_cache_key}:{cache_key_args}-{str(full_args.get(cache_key_args))}"
                 else:
                     for key_arg in cache_key_args:
-                        final_cache_key += f':{key_arg}-{str(full_args.get(key_arg))}'
+                        final_cache_key += (
+                            f":{key_arg}-{str(full_args.get(key_arg))}"
+                        )
 
             try:
                 if prefix_match:
-                    final_cache_key += '*'
+                    final_cache_key += "*"
                 client.delete(final_cache_key)
-                logger.info('Cache flush for %s', final_cache_key, tags=LogTags.CACHE)
+                logger.info(
+                    "Cache flush for %s", final_cache_key, tags=LogTags.CACHE
+                )
             except Exception:
-                logger.error('Error flushing cache for %s', final_cache_key, tags=LogTags.CACHE)
+                logger.error(
+                    "Error flushing cache for %s",
+                    final_cache_key,
+                    tags=LogTags.CACHE,
+                )
 
             return func(*args, **kwargs)
+
         return wrapper
+
     return decorator
```

### Comparing `splight-lib-2.3.0/splight_abstract/client/abstract.py` & `splight-lib-2.3.1/splight_abstract/client/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,81 @@
+from abc import ABC
 from collections import UserList
-from pydantic import BaseModel
-from typing import List, Type, Callable
 from functools import wraps
-from abc import ABC
+from typing import Callable, List, Type
+
+from pydantic import BaseModel
+
 from .filter import FilterMixin
 from .hooks import HooksMixin
 
 
 class empty:
     pass
 
 
 def validate_resource_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, resource_type: Type, *args, **kwargs):
         if resource_type not in self.valid_classes:
-            raise NotImplementedError(f"Not a valid resource_type: {resource_type.__name__}")
+            raise NotImplementedError(
+                f"Not a valid resource_type: {resource_type.__name__}"
+            )
         return func(self, resource_type, *args, **kwargs)
+
     return wrapper
 
 
 def validate_instance_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, instance: BaseModel, *args, **kwargs):
         if type(instance) not in self.valid_classes:
-            raise NotImplementedError(f"Not a valid instance type: {type(instance).__name__}")
+            raise NotImplementedError(
+                f"Not a valid instance type: {type(instance).__name__}"
+            )
         return func(self, instance, *args, **kwargs)
+
     return wrapper
 
 
 class AbstractClient(ABC, HooksMixin, FilterMixin):
     valid_classes: List[Type] = []
 
     def __init__(self, namespace: str = "default", *args, **kwargs):
         self.namespace = namespace.lower().replace("_", "")
 
     def _validated_kwargs(self, resource_type: Type, **kwargs):
-        '''
+        """
         Validate the given kwargs.
-        '''
+        """
         class_fields = list(resource_type.__fields__.keys())
         return super()._validated_kwargs(class_fields, **kwargs)
 
 
 class QuerySet(UserList):
-    def __init__(self,
-                 client: AbstractClient,
-                 *args,
-                 get_func: str = '_get',
-                 count_func: str = 'count',
-                 **kwargs):
+    def __init__(
+        self,
+        client: AbstractClient,
+        *args,
+        get_func: str = "_get",
+        count_func: str = "count",
+        **kwargs,
+    ):
         super().__init__()
         self._client = client
         self._client_func = get_func
         self._count_func = count_func
         self._args = args
         self._kwargs = kwargs
         self._cached_results = empty
 
     def __new__(cls, *args, **kwargs):
         obj = super(QuerySet, cls).__new__(cls)
         obj.__init__(*args, **kwargs)
-        if kwargs.get('first', False):
+        if kwargs.get("first", False):
             return obj.data
         return obj
 
     def filter(self, **kwargs) -> "QuerySet":
         kwargs = {**self._kwargs, **kwargs}
         return QuerySet(self._client, *self._args, **kwargs)
 
@@ -82,31 +92,37 @@
             skip_ = self._kwargs.get("skip_", 0) + i.start
 
             limit_ = i.stop - i.start
             if "limit_" in self._kwargs:
                 old_limit_ = self._kwargs["limit_"]
                 limit_ = min(limit_, old_limit_)
 
-            kwargs = {
-                **self._kwargs
-            }
+            kwargs = {**self._kwargs}
             kwargs["skip_"] = skip_
             kwargs["limit_"] = limit_
             kwargs.pop("get_func", None)
             kwargs.pop("count_func", None)
-            return QuerySet(self._client, get_func=self._client_func, count_func=self._count_func, *self._args, **kwargs)
+            return QuerySet(
+                self._client,
+                get_func=self._client_func,
+                count_func=self._count_func,
+                *self._args,
+                **kwargs,
+            )
 
         return self.data[i]
 
     def __len__(self):
         if self._cached_results is not empty:
             return len(self._cached_results)
 
         if hasattr(self._client, self._count_func):
-            return getattr(self._client, self._count_func)(*self._args, **self._kwargs)
+            return getattr(self._client, self._count_func)(
+                *self._args, **self._kwargs
+            )
 
         return len(self.data)
 
     def count(self):
         return len(self)
 
     @property
```

### Comparing `splight-lib-2.3.0/splight_abstract/client/filter.py` & `splight-lib-2.3.1/splight_abstract/client/filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
-from typing import List, Any
+from typing import Any, List
+
 
 class FilterMixin:
     reserved_filter_keys = ["__in", "__contains", "__lte", "__gte"]
 
     def _get_field_value(self, x: Any, field: str):
         for reserved_key in self.reserved_filter_keys:
             field = field.replace(reserved_key, "")
@@ -17,62 +18,81 @@
             try:
                 return getattr(x, key).get(subkey)
             except:
                 return None
         return getattr(x, field)
 
     def _check_in(self, x: Any, field: str, value: Any):
-        field = self._get_field_value(x,field)
+        field = self._get_field_value(x, field)
         try:
             return field in value
         except:
             return False
 
     def _check_contains(self, x: Any, field: str, value: Any):
         field = self._get_field_value(x, field)
         try:
             return value in field
         except:
             return False
 
     def _filter(self, queryset: list, **kwargs) -> list:
-        '''
+        """
         Filter a queryset by the given kwargs.
-        '''
+        """
         field_filters = [
-            lambda x, field=field, value=value: self._get_field_value(x, field) == value for field, value in kwargs.items() if "__" not in field
+            lambda x, field=field, value=value: self._get_field_value(x, field)
+            == value
+            for field, value in kwargs.items()
+            if "__" not in field
         ]
         in_filters = [
-            lambda x, field=field, values=values: self._check_in(x, field, values) for field, values in kwargs.items() if field.endswith("__in")
+            lambda x, field=field, values=values: self._check_in(
+                x, field, values
+            )
+            for field, values in kwargs.items()
+            if field.endswith("__in")
         ]
         contains_filters = [
-            lambda x, field=field, value=value: self._check_contains(x, field, value) for field, value in kwargs.items() if field.endswith("__contains")
+            lambda x, field=field, value=value: self._check_contains(
+                x, field, value
+            )
+            for field, value in kwargs.items()
+            if field.endswith("__contains")
         ]
         dict_filters = [
-            lambda x, field=field, value=value: self._get_field_value(x, field) == value for field, value in kwargs.items() if "__" in field and not any(field.endswith(reserved_key) for reserved_key in self.reserved_filter_keys)
+            lambda x, field=field, value=value: self._get_field_value(x, field)
+            == value
+            for field, value in kwargs.items()
+            if "__" in field
+            and not any(
+                field.endswith(reserved_key)
+                for reserved_key in self.reserved_filter_keys
+            )
         ]
         filters = field_filters + in_filters + contains_filters + dict_filters
 
         return [obj for obj in queryset if all([f(obj) for f in filters])]
 
     def _validated_kwargs(self, allowed_fields: List[str], **kwargs):
-        '''
+        """
         Validate the given kwargs.
-        '''
-        valid_kwargs = [
-            f"{field}__in" for field in allowed_fields
-        ] + [
-            f"{field}__contains" for field in allowed_fields
-        ] + [
-            f"{field}__lte" for field in allowed_fields
-        ] + [
-            f"{field}__gte" for field in allowed_fields
-        ] + allowed_fields
+        """
+        valid_kwargs = (
+            [f"{field}__in" for field in allowed_fields]
+            + [f"{field}__contains" for field in allowed_fields]
+            + [f"{field}__lte" for field in allowed_fields]
+            + [f"{field}__gte" for field in allowed_fields]
+            + allowed_fields
+        )
 
         invalid_kwargs = []
         for key in kwargs.keys():
-            if key not in valid_kwargs and not any(key.startswith(f"{allowed_field}__") for allowed_field in allowed_fields):
+            if key not in valid_kwargs and not any(
+                key.startswith(f"{allowed_field}__")
+                for allowed_field in allowed_fields
+            ):
                 invalid_kwargs.append(key)
 
         for key in invalid_kwargs:
             kwargs.pop(key)
         return kwargs
```

### Comparing `splight-lib-2.3.0/splight_abstract/client/hooks.py` & `splight-lib-2.3.1/splight_abstract/client/hooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 import inspect
 from enum import Enum
-from typing import Callable, List, Dict
 from functools import wraps
+from typing import Callable, Dict, List
 
 
 class HooksStage(str, Enum):
     BEFORE = "before"
     AFTER = "after"
 
 
 class HooksMixin:
     _original_signature = {}
 
     def add_pre_hook(self, function, hook):
-        setattr(self, function, self._add_hook(getattr(self, function), hook, HooksStage.BEFORE))
+        setattr(
+            self,
+            function,
+            self._add_hook(getattr(self, function), hook, HooksStage.BEFORE),
+        )
 
     def add_post_hook(self, function, hook):
-        setattr(self, function, self._add_hook(getattr(self, function), hook, HooksStage.AFTER))
-
-    def _add_hook(self, func: Callable, hook, stage: HooksStage = HooksStage.BEFORE):
+        setattr(
+            self,
+            function,
+            self._add_hook(getattr(self, function), hook, HooksStage.AFTER),
+        )
+
+    def _add_hook(
+        self, func: Callable, hook, stage: HooksStage = HooksStage.BEFORE
+    ):
         func_name = func.__qualname__
 
         if func_name not in self._original_signature:
             self._original_signature[func_name] = [
                 param
                 for param in inspect.getfullargspec(func).args
-                if param not in ['self', 'cls', 'args', 'kwargs']
+                if param not in ["self", "cls", "args", "kwargs"]
             ]
 
         @wraps(func)
         def pre_hooked_func(*args, **kwargs):
             kwargs = self._args_to_kwargs(func, *args, **kwargs)
             ignore_hook = kwargs.get("ignore_hook", False)
             if ignore_hook:
@@ -41,15 +51,18 @@
         def post_hooked_func(*args, **kwargs):
             kwargs = self._args_to_kwargs(func, *args, **kwargs)
             ignore_hook = kwargs.get("ignore_hook", False)
             if ignore_hook:
                 return func(**kwargs)
             result = func(**kwargs)
             return hook(result)
-        return pre_hooked_func if stage == HooksStage.BEFORE else post_hooked_func
+
+        return (
+            pre_hooked_func if stage == HooksStage.BEFORE else post_hooked_func
+        )
 
     def _args_to_kwargs(self, func: Callable, *args, **kwargs) -> Dict:
         if not args:
             return kwargs
         func_params: List = self._original_signature[func.__qualname__]
         new_kwargs: Dict = dict(zip(func_params, args))
         new_kwargs.update(kwargs)
```

### Comparing `splight-lib-2.3.0/splight_abstract/communication/abstract.py` & `splight-lib-2.3.1/splight_abstract/communication/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+from abc import abstractmethod, abstractproperty
 from enum import Enum
 from typing import Callable, Dict
-from abc import abstractmethod, abstractproperty
+
 from splight_abstract.client import AbstractClient
 from splight_models import CommunicationContext, CommunicationEvent
 
 
 class CommunicationClientStatus(str, Enum):
-    STARTING = 'starting'
-    READY = 'ready'
-    FAILED = 'failed'
-    ERROR =  'error'
+    STARTING = "starting"
+    READY = "ready"
+    FAILED = "failed"
+    ERROR = "error"
 
 
 class AbstractCommunicationClient(AbstractClient):
     def __init__(self, instance_id: str = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.instance_id = instance_id
 
     @abstractproperty
     def context(self) -> CommunicationContext:
         pass
-    
+
     @abstractproperty
     def status(self):
         pass
 
     @abstractmethod
     def bind(self, event_name: str, event_handler: Callable) -> None:
         pass
@@ -34,9 +35,11 @@
         pass
 
     @abstractmethod
     def trigger(self, event: CommunicationEvent):
         pass
 
     @abstractmethod
-    def authenticate(self, channel_name: str, socket_id: str, custom_data: Dict = None) -> dict:
+    def authenticate(
+        self, channel_name: str, socket_id: str, custom_data: Dict = None
+    ) -> dict:
         pass
```

### Comparing `splight-lib-2.3.0/splight_abstract/database/abstract.py` & `splight-lib-2.3.1/splight_abstract/database/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from abc import abstractmethod
+from tempfile import NamedTemporaryFile
+from typing import List, Type
+
 from pydantic import BaseModel
-from typing import Type, List
 from splight_abstract.client import AbstractClient, QuerySet
-from tempfile import NamedTemporaryFile
 
 
 class AbstractDatabaseClient(AbstractClient):
-
     @abstractmethod
     def save(self, instance: BaseModel) -> BaseModel:
         pass
 
     @abstractmethod
-    def _get(self,
-             resource_type: Type,
-             first: bool = False,
-             limit_: int = -1,
-             skip_: int = 0,
-             deleted: bool = False,
-             **kwargs) -> List[BaseModel]:
+    def _get(
+        self,
+        resource_type: Type,
+        first: bool = False,
+        limit_: int = -1,
+        skip_: int = 0,
+        deleted: bool = False,
+        **kwargs
+    ) -> List[BaseModel]:
         pass
 
     def get(self, resource_type: Type, *args, **kwargs) -> QuerySet:
         return QuerySet(self, resource_type, *args, **kwargs)
 
     @abstractmethod
     def delete(self, resource_type: Type, id: str) -> None:
```

### Comparing `splight-lib-2.3.0/splight_abstract/datalake/abstract.py` & `splight-lib-2.3.1/splight_abstract/datalake/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,84 +1,95 @@
 from abc import abstractmethod
-from pydantic import BaseModel
-from typing import Type, List, Dict, Union, Callable
-from datetime import timezone, timedelta
-from splight_models import DatalakeModel, Query
-from splight_abstract.client import AbstractClient, QuerySet
+from datetime import timedelta, timezone
 from functools import wraps
+from typing import Callable, Dict, List, Type, Union
+
 import pandas as pd
+from pydantic import BaseModel
+from splight_abstract.client import AbstractClient, QuerySet
+from splight_models import DatalakeModel, Query
 
 
 def validate_resource_type(func: Callable) -> Callable:
     @wraps(func)
     def inner(self, resource_type, *args, **kwargs):
         if not issubclass(resource_type, DatalakeModel):
-            raise NotImplementedError(f"Not a valid resource_type: {resource_type.__name__}")
+            raise NotImplementedError(
+                f"Not a valid resource_type: {resource_type.__name__}"
+            )
         return func(self, resource_type, *args, **kwargs)
+
     return inner
 
 
 def validate_instance_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, instances: List[BaseModel], *args, **kwargs):
         if instances:
             resource_type = instances[0].__class__
             if not all([isinstance(i, resource_type) for i in instances]):
-                raise TypeError('All instances must be of the same type')
+                raise TypeError("All instances must be of the same type")
             if not issubclass(resource_type, DatalakeModel):
-                raise TypeError('All instances must be of type DatalakeModel')
+                raise TypeError("All instances must be of type DatalakeModel")
         return func(self, instances, *args, **kwargs)
+
     return wrapper
 
 
 class AbstractDatalakeClient(AbstractClient):
-
     valid_filters = ["in", "contains", "gte", "lte"]
 
     def _validated_kwargs(self, resource_type: Type, **kwargs):
         valid_fields: List[str] = list(resource_type.__fields__.keys())
 
         valid_filter: Dict[str, str] = {
-            key: value for key, value in kwargs.items()
-            if key in valid_fields or
-            any(f"{valid_field}__" in key for valid_field in valid_fields)
+            key: value
+            for key, value in kwargs.items()
+            if key in valid_fields
+            or any(f"{valid_field}__" in key for valid_field in valid_fields)
         }
 
         return valid_filter
 
     @abstractmethod
-    def get(self,
-            resource_type: Type,
-            limit_: int = 50,
-            skip_: int = 0,
-            sort: Union[List, str] = ['timestamp__desc'],
-            group_id: Union[List, str] = [],
-            group_fields: Union[List, str] = [],
-            tzinfo: timezone = timezone(timedelta()),
-            **kwargs) -> QuerySet:
+    def get(
+        self,
+        resource_type: Type,
+        limit_: int = 50,
+        skip_: int = 0,
+        sort: Union[List, str] = ["timestamp__desc"],
+        group_id: Union[List, str] = [],
+        group_fields: Union[List, str] = [],
+        tzinfo: timezone = timezone(timedelta()),
+        **kwargs,
+    ) -> QuerySet:
         pass
 
     @abstractmethod
     def get_output(self, query: Query) -> List[Dict]:
         pass
 
     @abstractmethod
-    def get_dataframe(self, resource_type: Type, freq="H", **kwargs) -> pd.DataFrame:
+    def get_dataframe(
+        self, resource_type: Type, freq="H", **kwargs
+    ) -> pd.DataFrame:
         pass
 
     @abstractmethod
     def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
         pass
 
     @abstractmethod
     def save(self, instances: List[BaseModel]) -> List[BaseModel]:
         pass
 
     @abstractmethod
-    def save_dataframe(self, resource_type: Type, dataframe: pd.DataFrame) -> None:
+    def save_dataframe(
+        self, resource_type: Type, dataframe: pd.DataFrame
+    ) -> None:
         pass
 
     @abstractmethod
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
         pass
 
     @abstractmethod
```

### Comparing `splight-lib-2.3.0/splight_abstract/deployment/abstract.py` & `splight-lib-2.3.1/splight_abstract/deployment/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 from abc import abstractmethod
+from typing import List, Optional, Type
+
 from pydantic import BaseModel
-from typing import Type, List, Optional
 from splight_abstract.client import AbstractClient, QuerySet
 
 
 class AbstractDeploymentClient(AbstractClient):
     @abstractmethod
     def save(self, instance: BaseModel) -> BaseModel:
         pass
 
     def get(self, *args, **kwargs) -> QuerySet:
         return QuerySet(self, *args, **kwargs)
 
     @abstractmethod
-    def _get(self, resource_type: Type, id: str = '', first=False, limit_: int = -1, skip_: int = 0, **kwargs) -> List[BaseModel]:
+    def _get(
+        self,
+        resource_type: Type,
+        id: str = "",
+        first=False,
+        limit_: int = -1,
+        skip_: int = 0,
+        **kwargs
+    ) -> List[BaseModel]:
         pass
 
     @abstractmethod
     def delete(self, resource_type: Type, id: str) -> None:
         pass
 
-    def get_deployment_logs(self, id: str, limit: Optional[int] = None, since: Optional[str] = None, previous: bool = False) -> List[str]:
+    def get_deployment_logs(
+        self,
+        id: str,
+        limit: Optional[int] = None,
+        since: Optional[str] = None,
+        previous: bool = False,
+    ) -> List[str]:
         pass
```

### Comparing `splight-lib-2.3.0/splight_abstract/endpoints/__init__.py` & `splight-lib-2.3.1/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_abstract/hub/abstract.py` & `splight-lib-2.3.1/splight_abstract/hub/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from abc import ABC, abstractmethod, abstractproperty
-from typing import Dict, List, Type, Tuple
+from typing import Dict, List, Tuple, Type
 
 from pydantic import BaseModel
-
 from splight_abstract.client import AbstractClient, QuerySet
 
 
 class AbstractHubSubClient(AbstractClient):
     @abstractmethod
     def save(self, instance: BaseModel) -> BaseModel:
         pass
 
     def get(self, *args, **kwargs) -> QuerySet:
         return QuerySet(self, *args, **kwargs)
 
     @abstractmethod
-    def _get(self, resource_type: Type, first=False, limit_: int = -1, skip_: int = 0, **kwargs) -> List[BaseModel]:
+    def _get(
+        self,
+        resource_type: Type,
+        first=False,
+        limit_: int = -1,
+        skip_: int = 0,
+        **kwargs
+    ) -> List[BaseModel]:
         pass
 
     @abstractmethod
     def delete(self, resource_type: Type, id: str) -> None:
         pass
 
     @abstractmethod
```

### Comparing `splight-lib-2.3.0/splight_abstract/storage/abstract.py` & `splight-lib-2.3.1/splight_abstract/storage/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from abc import abstractmethod
+from typing import List, Optional, Type
+
 from pydantic import BaseModel
-from typing import Optional, Type, List
 from splight_abstract.client import AbstractClient, QuerySet
 
 
 class AbstractStorageClient(AbstractClient):
-
     @abstractmethod
     def save(self, instance: BaseModel) -> BaseModel:
         pass
 
     def get(self, *args, **kwargs) -> QuerySet:
         kwargs["get_func"] = "_get"
         kwargs["count_func"] = "None"
         return QuerySet(self, *args, **kwargs)
 
     @abstractmethod
-    def _get(self, resource_type: Type, first=False, prefix: Optional[str] = None, limit_: int = -1, skip_: int = 0, **kwargs) -> List[BaseModel]:
+    def _get(
+        self,
+        resource_type: Type,
+        first=False,
+        prefix: Optional[str] = None,
+        limit_: int = -1,
+        skip_: int = 0,
+        **kwargs
+    ) -> List[BaseModel]:
         pass
 
     @abstractmethod
     def copy(self, old_name: str, new_name: str):
         pass
 
     @abstractmethod
```

### Comparing `splight-lib-2.3.0/splight_lib/auth/mac_auth.py` & `splight-lib-2.3.1/splight_lib/auth/mac_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import six
 import hmac
 import time
 from hashlib import sha256
+
+import six
 from splight_lib.auth.exceptions import SignatureVerificationError
 
 
 def utf8(value):
     if six.PY2 and isinstance(value, six.text_type):
         return value.encode("utf-8")
     else:
@@ -42,15 +43,17 @@
     def _get_timestamp_and_signatures(header, scheme):
         list_items = [i.split("=", 2) for i in header.split(",")]
         timestamp = int([i[1] for i in list_items if i[0] == "t"][0])
         signatures = [i[1] for i in list_items if i[0] == scheme]
         return timestamp, signatures
 
     @classmethod
-    def verify_header(cls, payload, header, secret, tolerance=DEFAULT_TOLERANCE):
+    def verify_header(
+        cls, payload, header, secret, tolerance=DEFAULT_TOLERANCE
+    ):
         if hasattr(payload, "decode"):
             payload = payload.decode("utf-8")
 
         try:
             timestamp, signatures = cls._get_timestamp_and_signatures(
                 header, cls.EXPECTED_SCHEME
             )
@@ -67,15 +70,18 @@
                 "%s" % cls.EXPECTED_SCHEME,
                 header,
                 payload,
             )
 
         signed_payload = "%d.%s" % (timestamp, payload)
         expected_sig = cls._compute_signature(signed_payload, secret)
-        if not any(hmac.compare_digest(utf8(expected_sig), utf8(s)) for s in signatures):
+        if not any(
+            hmac.compare_digest(utf8(expected_sig), utf8(s))
+            for s in signatures
+        ):
             raise SignatureVerificationError(
                 "No signatures found matching the expected signature for "
                 "payload",
                 header,
                 payload,
             )
```

### Comparing `splight-lib-2.3.0/splight_lib/client/database/local_client.py` & `splight-lib-2.3.1/splight_lib/client/database/local_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Type, Union
 from uuid import uuid4
 
 from splight_abstract.database import AbstractDatabaseClient
 from splight_lib.client.exceptions import InstanceNotFound
 from splight_lib.client.filter import value_filter_on_tuple
+from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_models import SplightBaseModel
-from splight_lib.logging._internal import get_splight_logger, LogTags
 
 ResourceType = Type[SplightBaseModel]
 
 logger = get_splight_logger()
 
 
 class LocalDatabaseClient(AbstractDatabaseClient):
@@ -23,15 +23,17 @@
 
     def __init__(self, namespace: str, path: str, *args, **kwargs):
         super().__init__(namespace)
         self._db_file = os.path.join(path, "splight-db.json")
 
         if not os.path.exists(self._db_file):
             self._save_db(self._db_file, {})
-        logger.info("Local database client initialized.", tags=LogTags.DATABASE)
+        logger.info(
+            "Local database client initialized.", tags=LogTags.DATABASE
+        )
 
     def save(self, instance: SplightBaseModel) -> SplightBaseModel:
         """Saves an instance in the local database, if the instance has an id
         will try to update the instance, otherwise it will create a new one.
 
         Parameters
         ----------
@@ -104,15 +106,20 @@
             return parsed[0] if parsed else None
         return parsed
 
     def count(self, resource_type: ResourceType, **kwargs) -> int:
         db = self._load_db_file(self._db_file)
         model_name = resource_type.__name__.lower()
         db_instances = db.get(model_name, {})
-        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
+        logger.debug(
+            "Counted %s objects of type: %s.",
+            response["count"],
+            resource_type,
+            tags=LogTags.DATABASE,
+        )
         return len(db_instances)
 
     def download(
         self, instances: SplightBaseModel, decrtypt: bool = True, **kwargs
     ) -> NamedTemporaryFile:
         raise NotImplementedError()
```

### Comparing `splight-lib-2.3.0/splight_lib/client/database/remote_client.py` & `splight-lib-2.3.1/splight_lib/client/database/remote_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Type
 
 from furl import furl
 from pydantic import BaseModel
-
 from retry import retry
-
 from splight_abstract.database import AbstractDatabaseClient
 from splight_abstract.remote import AbstractRemoteClient
 from splight_lib.auth import SplightAuthToken
-from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_lib.client.database.classmap import CLASSMAP
 from splight_lib.client.exceptions import REQUEST_EXCEPTIONS, InvalidModel
 from splight_lib.client.settings import settings_remote as settings
-from splight_lib.restclient import SplightRestClient
 from splight_lib.encryption import EncryptionClient
+from splight_lib.logging._internal import LogTags, get_splight_logger
+from splight_lib.restclient import SplightRestClient
 from splight_models import File
 
 logger = get_splight_logger()
 
 
 class RemoteDatabaseClient(AbstractDatabaseClient, AbstractRemoteClient):
     """Splight API Database Client.
@@ -32,15 +30,17 @@
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
-        logger.info("Remote database client initialized.", tags=LogTags.DATABASE)
+        logger.info(
+            "Remote database client initialized.", tags=LogTags.DATABASE
+        )
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def save(self, instance: BaseModel) -> BaseModel:
         """Creates or updates a new resource depending on the model if
         it contains the id or not.
 
         Parameters
@@ -129,15 +129,20 @@
         ------
         InvalidModel thrown when the model name is not correct.
         """
         model_data = self._get_model_data(resource_type)
         path = model_data["path"]
         kwargs["page"] = 1  # Always start from the first page
         response = self._list(path, **kwargs)
-        logger.debug("Counted %s objects of type: %s.", response["count"], resource_type, tags=LogTags.DATABASE)
+        logger.debug(
+            "Counted %s objects of type: %s.",
+            response["count"],
+            resource_type,
+            tags=LogTags.DATABASE,
+        )
         return response["count"]
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=1)
     def download(
         self, instance: BaseModel, decrypt: bool = True, **kwargs
     ) -> NamedTemporaryFile:
         """Returns the number of resources in the database for a given model
```

### Comparing `splight-lib-2.3.0/splight_lib/client/datalake/local_client.py` & `splight-lib-2.3.1/splight_lib/client/datalake/local_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import json
 import os
 from datetime import timedelta, timezone
 from functools import partial
 from typing import Dict, List, Type, Union
 
 import pandas as pd
-
 from splight_abstract.client import QuerySet
 from splight_abstract.datalake import AbstractDatalakeClient
 from splight_lib.client.file_handler import FixedLineNumberFileHandler
 from splight_lib.client.filter import value_filter
+from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_models import DatalakeModel, Query
-from splight_lib.logging._internal import get_splight_logger, LogTags
 
 DLResource = Type[DatalakeModel]
 
 logger = get_splight_logger()
 
 
 class LocalDatalakeClient(AbstractDatalakeClient):
@@ -26,15 +25,17 @@
     _DEFAULT = "default"
     _PREFIX = "dl_"
     _TOTAL_DOCS = 10000
 
     def __init__(self, namespace: str, path: str):
         super().__init__(namespace=namespace)
         self._base_path = path
-        logger.info("Local datalake client initialized.", tags=LogTags.DATALAKE)
+        logger.info(
+            "Local datalake client initialized.", tags=LogTags.DATALAKE
+        )
 
     def _raw_get(
         self,
         resource_type: DLResource,
         limit_: int = -1,
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
@@ -73,15 +74,19 @@
         skip_: int = 0,
         sort: Union[List, str] = ["timestamp__desc"],
         group_id: Union[List, str] = [],
         group_fields: Union[List, str] = [],
         tzinfo: timezone = timezone(timedelta()),
         **kwargs,
     ) -> QuerySet:
-        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving object of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
 
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(
             self,
@@ -97,15 +102,17 @@
     def get_output(self, query: Query) -> List[Dict]:
         raise NotImplementedError()
 
     def get_dataframe(
         self, resource_type: Type, freq: str = "H", **kwargs
     ) -> pd.DataFrame:
         """Reads documents and returns a dataframe"""
-        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving dataframe from datalake.", tags=LogTags.DATALAKE
+        )
         documents = self._raw_get(resource_type, **kwargs)
         df = pd.DataFrame([x.dict() for x in documents])
         if not df.empty:
             df.set_index("timestamp", inplace=True, verify_integrity=False)
         return df
 
     def get_dataset(self, queries: List[Query]) -> pd.DataFrame:
@@ -137,25 +144,37 @@
         instances = dataframe.apply(
             lambda x: resource_type.parse_obj(x.to_dict()), axis=1
         )
         instances = instances.to_list()
         _ = self.save(instances)
 
     def delete(self, resource_type: DLResource, **kwargs) -> None:
-        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Deleting resources of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
         raise NotImplementedError()
 
     def create_index(self, collection: str, index: list) -> None:
-        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Creating index for collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
         raise NotImplementedError()
 
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
-        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Aggregate on datalake collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
         raise NotImplementedError()
 
     def _filter(
         self, instances: List[DLResource], filters: Dict
     ) -> List[DLResource]:
         filtered = instances
         for key, value in filters.items():
```

### Comparing `splight-lib-2.3.0/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.3.1/splight_lib/client/datalake/remote_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,46 +3,46 @@
 from io import StringIO
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Union
 
 import pandas as pd
 from furl import furl
 from pydantic import BaseModel
-from retry import retry
-
 from remote_splight_lib.auth import SplightAuthToken
+from retry import retry
 from splight_abstract import AbstractRemoteClient, QuerySet
 from splight_abstract.datalake import (
     AbstractDatalakeClient,
     validate_instance_type,
     validate_resource_type,
 )
 from splight_lib.client.exceptions import SPLIGHT_REQUEST_EXCEPTIONS
 from splight_lib.client.settings import settings_remote as settings
+from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import SplightRestClient
-from splight_lib.logging._internal import get_splight_logger, LogTags
 from splight_models import DatalakeModel, Query
 
 logger = get_splight_logger()
 
 
 class RemoteDatalakeClient(AbstractDatalakeClient, AbstractRemoteClient):
-
     _PREFIX = "v2/engine/datalake"
 
     def __init__(self, namespace: str = "default", *args, **kwargs):
         super().__init__(namespace=namespace)
         self._base_url = furl(settings.SPLIGHT_PLATFORM_API_HOST)
         token = SplightAuthToken(
             access_key=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
-        logger.info("Remote datalake client initialized.", tags=LogTags.DATALAKE)
+        logger.info(
+            "Remote datalake client initialized.", tags=LogTags.DATALAKE
+        )
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def _raw_save(
         self,
         collection: str,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
@@ -103,26 +103,34 @@
     @validate_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
-        logger.debug("Retrieving object of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving object of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
         kwargs["get_func"] = "_raw_get"
         kwargs["count_func"] = "None"
         kwargs["collection"] = resource_type.Meta.collection_name
         kwargs["resource_type"] = resource_type
         return QuerySet(self, *args, **kwargs)
 
     def get_output(
         self, resource_type: DatalakeModel, query: Query
     ) -> List[Dict]:
         # TODO: Add add_fields, project and renaming
-        logger.debug("Retrieving output of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving output of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
         return self._raw_get(
             resource_type=resource_type,
             collection=query.source,
             limit_=query.limit,
             skip_=query.skip,
             sort=query.sort,
             group_id=query.group_id,
@@ -139,27 +147,31 @@
         # GET /datalake/dumpdata/?source=collection
         url = self._base_url / f"{self._PREFIX}/dumpdata/"
         collection = resource_type.Meta.collection_name
         kwargs.update({"source": collection})
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
         response.raise_for_status()
-        logger.debug("Retrieving dataframe from datalake.", tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving dataframe from datalake.", tags=LogTags.DATALAKE
+        )
 
         df: pd.DataFrame = pd.DataFrame(pd.read_csv(StringIO(response.text)))
         if df.empty:
             return df
         df["timestamp"] = pd.to_datetime(df["timestamp"])
         df.set_index("timestamp", inplace=True)
         return df
 
     def get_dataset(
         self, resource_type: DatalakeModel, queries: List[Dict]
     ) -> pd.DataFrame:
-        logger.debug("Retrieving dataset from datalake.", tags=LogTags.DATALAKE)
+        logger.debug(
+            "Retrieving dataset from datalake.", tags=LogTags.DATALAKE
+        )
 
         dfs = [
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
@@ -198,34 +210,46 @@
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
     @validate_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
-        logger.debug("Deleting resources of type %s from datalake.", resource_type, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Deleting resources of type %s from datalake.",
+            resource_type,
+            tags=LogTags.DATALAKE,
+        )
 
         collection = resource_type.Meta.collection_name
         return self._raw_delete(collection=collection, **kwargs)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def create_index(self, collection: str, indexes: List[Dict]) -> None:
         # POST /datalake/index/
-        logger.debug("Creating index for collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Creating index for collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
 
         url = self._base_url / f"{self._PREFIX}/index/"
         data = {"source": collection, "index": indexes}
         response = self._restclient.post(url, json=data)
         response.raise_for_status()
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
     def raw_aggregate(
         self, collection: str, pipeline: List[Dict]
     ) -> List[Dict]:
-        logger.debug("Aggregate on datalake collection: %s.", collection, tags=LogTags.DATALAKE)
+        logger.debug(
+            "Aggregate on datalake collection: %s.",
+            collection,
+            tags=LogTags.DATALAKE,
+        )
         # POST /datalake/aggregate/?source=collection
         url = self._base_url / f"{self._PREFIX}/aggregate/"
         params = {"source": collection}
         data = {"pipeline": pipeline}
         response = self._restclient.post(url, params=params, data=data)
         response.raise_for_status()
         return response.json()
```

### Comparing `splight-lib-2.3.0/splight_lib/client/exceptions.py` & `splight-lib-2.3.1/splight_lib/client/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from requests.exceptions import ConnectionError, Timeout
-from splight_lib.restclient import (
-    ConnectError,
-    HTTPError,
-    Timeout as TimeoutError,
-)
+from splight_lib.restclient import ConnectError, HTTPError
+from splight_lib.restclient import Timeout as TimeoutError
 
 REQUEST_EXCEPTIONS = (ConnectionError, Timeout)
 SPLIGHT_REQUEST_EXCEPTIONS = (HTTPError, TimeoutError, ConnectError)
 
 
 class InvalidModel(Exception):
     def __init__(self, model_name: str):
```

### Comparing `splight-lib-2.3.0/splight_lib/client/file_handler.py` & `splight-lib-2.3.1/splight_lib/client/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._total_lines = total_lines
 
     def write(self, lines: List[str]):
         all_lines = self._read_file()
 
         all_lines.extend(lines)
 
-        lines = all_lines[-self._total_lines:]
+        lines = all_lines[-self._total_lines :]
         lines = [f"{x}\n" for x in lines]
         self._write_file(lines)
 
     def read(self, skip: int = 0, limit: int = -1) -> List[str]:
         all_lines = self._read_file()
         return all_lines[skip:limit]
```

### Comparing `splight-lib-2.3.0/splight_lib/client/filter.py` & `splight-lib-2.3.1/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_lib/client/settings.py` & `splight-lib-2.3.1/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_lib/component/abstract.py` & `splight-lib-2.3.1/splight_lib/component/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,124 @@
+import re
 import sys
 import time
-import splight_models as spmodels
 import uuid
-from functools import partial
 from abc import abstractmethod
-from tempfile import NamedTemporaryFile
-from typing import Optional, Type, List, Dict, Tuple, Set, Any, Callable, Union
-from mergedeep import merge, Strategy as mergeStrategy
 from collections import defaultdict
+from functools import cached_property, partial
+from tempfile import NamedTemporaryFile
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
+
+import splight_models as spmodels
+from mergedeep import Strategy as mergeStrategy
+from mergedeep import merge
 from pydantic import BaseModel, main
-from functools import cached_property
 from splight_lib.execution import ExecutionClient, Thread
-from splight_lib.logging._internal import get_splight_logger, LogTags
+from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.settings import setup as default_setup
 from splight_models import (
-    CustomType,
-    Deployment,
-    DatalakeModel,
-    Component,
-    Command,
     Binding,
-    ComponentObject,
     Boolean,
-    String,
-    Number,
-    Secret
-)
-from splight_models import (
-    EventNames,
-    ComponentCommandUpdateEvent,
+    Command,
+    CommunicationEvent,
+    Component,
     ComponentCommandTriggerEvent,
-    CommunicationEvent
+    ComponentCommandUpdateEvent,
+    ComponentObject,
+    CustomType,
+    DatalakeModel,
+    Deployment,
+    EventNames,
+    Number,
+    Secret,
+    String,
 )
-from splight_models.component import ComponentCommand, ComponentCommandStatus
 from splight_models.component import (
     DATABASE_TYPES,
     NATIVE_TYPES,
-    InputParameter
+    ComponentCommand,
+    ComponentCommandStatus,
+    InputParameter,
 )
 from splight_models.setpoint import (
     SetPoint,
+    SetPointCreateEvent,
     SetPointResponse,
     SetPointResponseStatus,
-    SetPointCreateEvent,
-    SetPointUpdateEvent
+    SetPointUpdateEvent,
 )
-import re
-
 
 logger = get_splight_logger()
 
 
 class SecretValueParser:
-
     def __init__(self, utils, *args, **kwargs):
         self.utils = utils
 
     def get_value(self, name: str) -> Any:
         logger.info("Obtaining secret: %s", name, tags=LogTags.SECRET)
         secret = self.utils.database_client.get(Secret, name=name, first=True)
         return secret.decrypt()
 
 
 class VariableValueMixin:
     _variable_parameter_map_class = {
-        'SECRET': SecretValueParser,
+        "SECRET": SecretValueParser,
     }
 
     def parse_variable_string(self, value: str) -> Any:
         if value is None:
             return ""
         pattern = re.compile(r"^\$\{\{(\w+)\.(\w+)\}\}$")
         match = pattern.search(value)
         if not match:
             return value
         class_key, name = match.groups()
         try:
             parser_class = self._variable_parameter_map_class[class_key]
         except KeyError as e:
-            raise NotImplementedError(f"Variable {class_key} is not supported yet.") from e
+            raise NotImplementedError(
+                f"Variable {class_key} is not supported yet."
+            ) from e
 
         return parser_class(utils=self).get_value(name)
 
 
 class RunnableMixin:
     healthcheck_interval = 5
     _HEALTH_FILE_PREFIX = "healthy_"
     _STARTUP_FILE_PREFIX = "ready_"
 
     def __init__(self):
         self.health_file = NamedTemporaryFile(prefix=self._HEALTH_FILE_PREFIX)
         self.startup_file = NamedTemporaryFile(
             prefix=self._STARTUP_FILE_PREFIX
         )
-        logger.info("Healthcheck file at: %s", self.health_file.name, tags=LogTags.RUNTIME)
-        logger.info("Startup file at: %s", self.startup_file.name, tags=LogTags.RUNTIME)
+        logger.info(
+            "Healthcheck file at: %s",
+            self.health_file.name,
+            tags=LogTags.RUNTIME,
+        )
+        logger.info(
+            "Startup file at: %s", self.startup_file.name, tags=LogTags.RUNTIME
+        )
 
         self.execution_client.start(Thread(self.healthcheck))
 
     def healthcheck(self) -> None:
         self.terminated = False
         while not self.terminated:
             if not self.execution_client.healthcheck():
                 logger.error("Healthcheck task failed.", tags=LogTags.RUNTIME)
                 self.health_file.close()
-                logger.error("Healthcheck file removed: %s", self.health_file, tags=LogTags.RUNTIME)
+                logger.error(
+                    "Healthcheck file removed: %s",
+                    self.health_file,
+                    tags=LogTags.RUNTIME,
+                )
                 sys.exit()
             time.sleep(self.healthcheck_interval)
 
     @abstractmethod
     def start(self):
         pass
 
@@ -117,25 +127,34 @@
 
 
 class IndexMixin:
     def _load_client_indexes(self) -> None:
         indexes: List[Tuple[str, int]] = self.__get_indexes()
         collections: List[str] = self.__get_collections()
         for col in collections:
-            logger.info("Adding indexes: %s for collection %s", indexes , col, tags=LogTags.INDEX)
-            self.datalake_client.create_index(
+            logger.info(
+                "Adding indexes: %s for collection %s",
+                indexes,
                 col,
-                indexes
+                tags=LogTags.INDEX,
             )
+            self.datalake_client.create_index(col, indexes)
 
     def __get_collections(self) -> List[str]:
         native_output_types = [Boolean, String, Number]
         # TODO do this autodiscovery better
-        component_output_types = [v for v in self.output.__dict__.values() if isinstance(v, main.ModelMetaclass)]
-        return [r.Meta.collection_name for r in native_output_types + component_output_types]
+        component_output_types = [
+            v
+            for v in self.output.__dict__.values()
+            if isinstance(v, main.ModelMetaclass)
+        ]
+        return [
+            r.Meta.collection_name
+            for r in native_output_types + component_output_types
+        ]
 
     def __get_indexes(self) -> List[Tuple[str, int]]:
         # order in indexes matters
         indexes: List[Tuple[str, int]] = [
             ("output_format", 1),
             ("instance_id", 1),
             ("instance_type", 1),
@@ -154,27 +173,45 @@
             indexes.append((index, 1))
 
         return indexes
 
 
 class HooksMixin:
     def _load_client_hooks(self):
-
-        logger.info("Adding pre-hooks for database and datalake clients.", tags=LogTags.HOOK)
+        logger.info(
+            "Adding pre-hooks for database and datalake clients.",
+            tags=LogTags.HOOK,
+        )
 
         # Datalake
-        self.datalake_client.add_pre_hook("save", self.__hook_insert_origin_save)
-        self.datalake_client.add_pre_hook("save_dataframe", self.__hook_insert_origin_save_dataframe)
+        self.datalake_client.add_pre_hook(
+            "save", self.__hook_insert_origin_save
+        )
+        self.datalake_client.add_pre_hook(
+            "save_dataframe", self.__hook_insert_origin_save_dataframe
+        )
         # Database
-        self.database_client.add_pre_hook("save", self.__hook_transform_from_custom_instances)
-        self.database_client.add_pre_hook("_get", self.__hook_transform_from_custom_resource_type)
-        self.database_client.add_pre_hook("delete", self.__hook_transform_from_custom_resource_type)
-        self.database_client.add_pre_hook("count", self.__hook_transform_from_custom_resource_type)
-        self.database_client.add_post_hook("_get", self.__hook_transform_to_custom_instances)
-        self.database_client.add_post_hook("save", self.__hook_transform_to_custom_instances)
+        self.database_client.add_pre_hook(
+            "save", self.__hook_transform_from_custom_instances
+        )
+        self.database_client.add_pre_hook(
+            "_get", self.__hook_transform_from_custom_resource_type
+        )
+        self.database_client.add_pre_hook(
+            "delete", self.__hook_transform_from_custom_resource_type
+        )
+        self.database_client.add_pre_hook(
+            "count", self.__hook_transform_from_custom_resource_type
+        )
+        self.database_client.add_post_hook(
+            "_get", self.__hook_transform_to_custom_instances
+        )
+        self.database_client.add_post_hook(
+            "save", self.__hook_transform_to_custom_instances
+        )
 
     def __hook_insert_origin_save(self, *args, **kwargs):
         logger.info("Datalake save pre-hook.", tags=LogTags.HOOK)
         instances = kwargs.get("instances", [])
         for instance in instances:
             if not isinstance(instance, DatalakeModel):
                 continue
@@ -189,164 +226,240 @@
         dataframe["instance_type"] = self.instance_type.__name__
         kwargs["dataframe"] = dataframe
         return args, kwargs
 
     def __hook_transform_from_custom_resource_type(self, *args, **kwargs):
         logger.info("Transform from custom type pre-hook.", tags=LogTags.HOOK)
         resource_type = kwargs["resource_type"]
-        if resource_type and hasattr(self.custom_types, resource_type.__name__):
+        if resource_type and hasattr(
+            self.custom_types, resource_type.__name__
+        ):
             kwargs["resource_type"] = ComponentObject
             kwargs["component_id"] = self.instance_id
             kwargs["type"] = resource_type.__name__
         return args, kwargs
 
     def __hook_transform_from_custom_instances(self, *args, **kwargs):
-        logger.info("Transform from custom instances pre-hook.", tags=LogTags.HOOK)
+        logger.info(
+            "Transform from custom instances pre-hook.", tags=LogTags.HOOK
+        )
         instance = kwargs["instance"]
         if getattr(self.custom_types, type(instance).__name__, None):
             parsed_instance = ComponentObject(
                 component_id=self.instance_id,
                 type=type(instance).__name__,
-                **self.unparse_parameters(instance)
+                **self.unparse_parameters(instance),
             )
             kwargs["instance"] = parsed_instance
         return args, kwargs
 
     def __hook_transform_to_custom_instances(
         self, result: Union[BaseModel, List[BaseModel]]
     ):
-        logger.info("Transform to custom instances pre-hook.", tags=LogTags.HOOK)
+        logger.info(
+            "Transform to custom instances pre-hook.", tags=LogTags.HOOK
+        )
         parsed_result = []
         convert_to_list = not isinstance(result, list)
         result = [result] if convert_to_list else result
         for object in result:
             if isinstance(object, ComponentObject):
                 custom_object_data: List[InputParameter] = object.data
-                custom_object_data.extend([
-                    InputParameter(name=key, value=getattr(object, key))
-                    for key in CustomType._reserved_names
-                ])
+                custom_object_data.extend(
+                    [
+                        InputParameter(name=key, value=getattr(object, key))
+                        for key in CustomType._reserved_names
+                    ]
+                )
                 custom_object_model = getattr(self.custom_types, object.type)
-                parsed_component_object = self.parse_parameters(custom_object_data)
+                parsed_component_object = self.parse_parameters(
+                    custom_object_data
+                )
                 object = custom_object_model(**parsed_component_object)
             parsed_result.append(object)
 
         parsed_result = parsed_result[0] if convert_to_list else parsed_result
         return parsed_result
 
 
 class BindingsMixin:
     def _load_client_bindings(self):
         # Commands
-        self.communication_client.bind(EventNames.COMPONENT_COMMAND_TRIGGER, self.__handle_component_command_trigger)
+        self.communication_client.bind(
+            EventNames.COMPONENT_COMMAND_TRIGGER,
+            self.__handle_component_command_trigger,
+        )
 
         # Bindings
         for binding in self.bindings:
             binding_function = getattr(self, binding.name)
-            binding_model = getattr(spmodels, binding.object_type, ComponentObject)
+            binding_model = getattr(
+                spmodels, binding.object_type, ComponentObject
+            )
             binding_event_name = binding_model.get_event_name(
-                binding.object_type,
-                binding.object_action
+                binding.object_type, binding.object_action
+            )
+            logger.info(
+                "Binding event: %s.", binding_event_name, tags=LogTags.BINDING
             )
-            logger.info("Binding event: %s.", binding_event_name, tags=LogTags.BINDING)
             binding_handler = self.__handle_native_object_trigger
             if binding_model == ComponentObject:
                 binding_handler = self.__handle_component_object_trigger
             if binding_model == SetPoint:
                 binding_handler = self.__handle_setpoint_trigger
 
             self.communication_client.bind(
                 binding_event_name,
                 partial(
-                    binding_handler,
-                    binding_function,
-                    binding.object_type
-                )
+                    binding_handler, binding_function, binding.object_type
+                ),
+            )
+            logger.info(
+                "Binded event: %s", binding_event_name, tags=LogTags.BINDING
             )
-            logger.info("Binded event: %s", binding_event_name, tags=LogTags.BINDING)
 
-    def __handle_setpoint_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
+    def __handle_setpoint_trigger(
+        self, binding_function: Callable, binding_object_type: str, data: str
+    ):
         try:
             logger.debug("Setpoint triggered.", tags=LogTags.SETPOINT)
             object_event = SetPointCreateEvent.parse_raw(data)
             setpoint = object_event.data
-            response_status = SetPointResponseStatus(binding_function(setpoint))
+            response_status = SetPointResponseStatus(
+                binding_function(setpoint)
+            )
             if response_status == SetPointResponseStatus.IGNORE:
                 return
 
             setpoint.responses = [
                 SetPointResponse(
                     component=self.instance_id,
                     status=response_status,
                 )
             ]
             setpoint_callback_event = SetPointUpdateEvent(data=setpoint)
             self.communication_client.trigger(setpoint_callback_event)
         except Exception as e:
-            logger.error("Error while handling setpoint create: %s", e, exc_info=True, tags=LogTags.SETPOINT)
+            logger.error(
+                "Error while handling setpoint create: %s",
+                e,
+                exc_info=True,
+                tags=LogTags.SETPOINT,
+            )
 
-    def __handle_native_object_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
+    def __handle_native_object_trigger(
+        self, binding_function: Callable, binding_object_type: str, data: str
+    ):
         assert self.bindings, "Please define .bindings to start."
         try:
-            logger.info("Binding for native object of type %s triggered.", binding_object_type, tags=LogTags.BINDING)
+            logger.info(
+                "Binding for native object of type %s triggered.",
+                binding_object_type,
+                tags=LogTags.BINDING,
+            )
             object_event = CommunicationEvent.parse_raw(data)
             object_model = getattr(spmodels, binding_object_type)
             binding_kwargs = object_model(**object_event.data)
             binding_function(binding_kwargs)
         except Exception as e:
-            logger.error("Error while handling native object trigger: %s", e, exc_info=True, tags=LogTags.BINDING)
+            logger.error(
+                "Error while handling native object trigger: %s",
+                e,
+                exc_info=True,
+                tags=LogTags.BINDING,
+            )
 
-    def __handle_component_object_trigger(self, binding_function: Callable, binding_object_type: str, data: str):
+    def __handle_component_object_trigger(
+        self, binding_function: Callable, binding_object_type: str, data: str
+    ):
         assert self.bindings, "Please define .bindings to start."
-        logger.info("Binding for component object of type %s triggered.", binding_object_type, tags=LogTags.BINDING)
+        logger.info(
+            "Binding for component object of type %s triggered.",
+            binding_object_type,
+            tags=LogTags.BINDING,
+        )
         component_object_event = CommunicationEvent.parse_raw(data)
-        component_object: ComponentObject = ComponentObject(**component_object_event.data)
+        component_object: ComponentObject = ComponentObject(
+            **component_object_event.data
+        )
         custom_object_data = component_object.data
-        custom_object_data.extend([
-            InputParameter(name=key, value=getattr(component_object, key))
-            for key in CustomType._reserved_names
-        ])
+        custom_object_data.extend(
+            [
+                InputParameter(name=key, value=getattr(component_object, key))
+                for key in CustomType._reserved_names
+            ]
+        )
         custom_object_model = getattr(self.custom_types, binding_object_type)
         parsed_component_object = self.parse_parameters(custom_object_data)
         binding_kwargs = custom_object_model(**parsed_component_object)
         binding_function(binding_kwargs)
 
     def __handle_component_command_trigger(self, data: str):
-        assert self.commands, "Please define .commands to start accepting request."
+        assert (
+            self.commands
+        ), "Please define .commands to start accepting request."
         component_command_event = ComponentCommandTriggerEvent.parse_raw(data)
         component_command: ComponentCommand = component_command_event.data
         command: Command = component_command.command
-        logger.info("Binding for component command '%s' triggered.", command.name, tags=LogTags.COMMAND)
+        logger.info(
+            "Binding for component command '%s' triggered.",
+            command.name,
+            tags=LogTags.COMMAND,
+        )
         try:
             command_function = getattr(self, command.name)
             command_kwargs_model = getattr(self.commands, command.name)
-            parsed_command_kwargs = self.parse_parameters(command.dict()["fields"])
+            parsed_command_kwargs = self.parse_parameters(
+                command.dict()["fields"]
+            )
             command_kwargs = command_kwargs_model(**parsed_command_kwargs)
             # .dict is not keeping the models of subkeys
             command_kwargs = {
-                str(field): getattr(command_kwargs, str(field)) for field in command_kwargs.__fields__
+                str(field): getattr(command_kwargs, str(field))
+                for field in command_kwargs.__fields__
             }
-            component_command.response.return_value = str(command_function(**command_kwargs))
+            component_command.response.return_value = str(
+                command_function(**command_kwargs)
+            )
             component_command.status = ComponentCommandStatus.SUCCESS
         except Exception as e:
-            logger.error("Error while handling component command trigger: %s", e, exc_info=True, tags=LogTags.COMMAND)
+            logger.error(
+                "Error while handling component command trigger: %s",
+                e,
+                exc_info=True,
+                tags=LogTags.COMMAND,
+            )
             component_command.response.error_detail = str(e)
             component_command.status = ComponentCommandStatus.ERROR
-        component_command_callback_event = ComponentCommandUpdateEvent(data=component_command)
+        component_command_callback_event = ComponentCommandUpdateEvent(
+            data=component_command
+        )
         self.communication_client.trigger(component_command_callback_event)
 
 
 class ParametersMixin:
     def unparse_parameters(self, instance: Dict) -> List[Dict]:
-        logger.debug("Unparsing parameters for an instance of %s", type(instance).__name__, tags=LogTags.PARAMETER)
+        logger.debug(
+            "Unparsing parameters for an instance of %s",
+            type(instance).__name__,
+            tags=LogTags.PARAMETER,
+        )
         custom_type = getattr(self.custom_types, type(instance).__name__, None)
         if custom_type is None:
             raise NotImplementedError
-        reserved_parameters = {k: v for k, v in instance.dict().items() if k in CustomType._reserved_names}
-        custom_parameters = {k: v for k, v in instance.dict().items() if k not in CustomType._reserved_names}
+        reserved_parameters = {
+            k: v
+            for k, v in instance.dict().items()
+            if k in CustomType._reserved_names
+        }
+        custom_parameters = {
+            k: v
+            for k, v in instance.dict().items()
+            if k not in CustomType._reserved_names
+        }
         fields = []
         for key, obj in custom_parameters.items():
             field = getattr(custom_type.SpecFields, key)
             if field is None:
                 continue
             value = obj
 
@@ -364,128 +477,195 @@
                     depends_on=field.depends_on,
                     sensitive=field.sensitive,
                 )
             )
         return {"data": fields, **reserved_parameters}
 
     def parse_parameters(self, parameters: List[Dict]) -> Dict:
-        logger.debug("Parsing parameters %s", parameters, tags=LogTags.PARAMETER)
-        parameters = self._fetch_and_reload_component_objects_parameters(parameters)
-        object_ids: Dict[str, Dict[str, List]] = self._get_object_ids(parameters)
+        logger.debug(
+            "Parsing parameters %s", parameters, tags=LogTags.PARAMETER
+        )
+        parameters = self._fetch_and_reload_component_objects_parameters(
+            parameters
+        )
+        object_ids: Dict[str, Dict[str, List]] = self._get_object_ids(
+            parameters
+        )
         objects: Dict[str, BaseModel] = self._fetch_objects(object_ids)
         parameters = self._reload_parameters(parameters, objects=objects)
         transformed_parameters = self._transform_parameters(parameters)
         return transformed_parameters
 
-    def _fetch_and_reload_component_objects_parameters(self, parameters: List[Dict]) -> List[Dict]:
+    def _fetch_and_reload_component_objects_parameters(
+        self, parameters: List[Dict]
+    ) -> List[Dict]:
         reloaded_parameters = []
         for raw_parameter in parameters:
-            raw_parameter = raw_parameter.dict() if not isinstance(raw_parameter, dict) else raw_parameter
+            raw_parameter = (
+                raw_parameter.dict()
+                if not isinstance(raw_parameter, dict)
+                else raw_parameter
+            )
             parameter = raw_parameter.copy()
             type = parameter["type"]
             value = parameter["value"]
             multiple = parameter["multiple"]
-            if type == 'str':
+            if type == "str":
                 parameter["value"] = self.parse_variable_string(value)
             if type in NATIVE_TYPES or type in DATABASE_TYPES:
                 parameter["value"] = value
             else:
                 object_ids = value if multiple else [value]
                 objects = (
                     self.database_client.get(
                         ComponentObject, id__in=object_ids, ignore_hook=True
                     )
-                    if object_ids else []  # TODO: Investigate why the filter is not working properly.
+                    if object_ids
+                    else []  # TODO: Investigate why the filter is not working properly.
                 )
                 for o in objects:
                     component_object_data = [
                         InputParameter(name=key, value=getattr(o, key))
                         for key in CustomType._reserved_names
                     ]
                     o.data.extend(component_object_data)
                 objects = [o.data for o in objects]
-                parameter["value"] = [self._fetch_and_reload_component_objects_parameters(o) for o in objects] if multiple else self._fetch_and_reload_component_objects_parameters(objects[0])
+                parameter["value"] = (
+                    [
+                        self._fetch_and_reload_component_objects_parameters(o)
+                        for o in objects
+                    ]
+                    if multiple
+                    else self._fetch_and_reload_component_objects_parameters(
+                        objects[0]
+                    )
+                )
             reloaded_parameters.append(parameter)
         return reloaded_parameters
 
-    def _get_object_ids(self, parameters: List[Dict]) -> Dict[str, Dict[str, List]]:
-        ids = {
-            "database": defaultdict(list)
-        }
+    def _get_object_ids(
+        self, parameters: List[Dict]
+    ) -> Dict[str, Dict[str, List]]:
+        ids = {"database": defaultdict(list)}
         for parameter in parameters:
-            parameter = parameter.dict() if not isinstance(parameter, dict) else parameter
+            parameter = (
+                parameter.dict()
+                if not isinstance(parameter, dict)
+                else parameter
+            )
             if parameter["value"] is None:
                 continue
-            values = parameter["value"] if parameter["multiple"] else [parameter["value"]]
+            values = (
+                parameter["value"]
+                if parameter["multiple"]
+                else [parameter["value"]]
+            )
             if parameter["type"] in NATIVE_TYPES:
                 continue
             elif parameter["type"] in DATABASE_TYPES:
                 for value in values:
                     ids["database"][parameter["type"]].append(value)
             else:
                 for value in values:
-                    ids = merge(ids, self._get_object_ids(value), strategy=mergeStrategy.ADDITIVE)
+                    ids = merge(
+                        ids,
+                        self._get_object_ids(value),
+                        strategy=mergeStrategy.ADDITIVE,
+                    )
         return ids
 
     def _fetch_objects(self, ids_to_fetch: Dict) -> Dict[str, BaseModel]:
-        res: Dict = {
-            None: None
-        }
+        res: Dict = {None: None}
         for type, ids_ in ids_to_fetch["database"].items():
             objs = self.database_client.get(DATABASE_TYPES[type], id__in=ids_)
             res.update({obj.id: obj for obj in objs})
         return res
 
-    def _reload_parameters(self, parameters: List[Dict], objects: Dict) -> List[Dict]:
+    def _reload_parameters(
+        self, parameters: List[Dict], objects: Dict
+    ) -> List[Dict]:
         reloaded_parameters = []
         for raw_parameter in parameters:
-            raw_parameter = raw_parameter.dict() if not isinstance(raw_parameter, dict) else raw_parameter
+            raw_parameter = (
+                raw_parameter.dict()
+                if not isinstance(raw_parameter, dict)
+                else raw_parameter
+            )
             parameter = raw_parameter.copy()
             type = parameter["type"]
             value = parameter["value"]
             multiple = parameter["multiple"]
-            if type == 'str':
+            if type == "str":
                 parameter["value"] = self.parse_variable_string(value)
             elif type in NATIVE_TYPES or value is None:
                 parameter["value"] = value
             elif type in DATABASE_TYPES:
-                parameter["value"] = [objects[val] for val in value] if multiple else objects[value]
+                parameter["value"] = (
+                    [objects[val] for val in value]
+                    if multiple
+                    else objects[value]
+                )
             else:
-                parameter["value"] = [self._reload_parameters(value, objects) for value in value] if multiple else self._reload_parameters(value, objects)
+                parameter["value"] = (
+                    [
+                        self._reload_parameters(value, objects)
+                        for value in value
+                    ]
+                    if multiple
+                    else self._reload_parameters(value, objects)
+                )
             reloaded_parameters.append(parameter)
         return reloaded_parameters
 
     def _transform_parameters(self, parameters: List[Dict]) -> Dict:
         parameters_dict: Dict = {}
         for parameter in parameters:
             type = parameter["type"]
             name = parameter["name"]
             value = parameter["value"]
             multiple = parameter["multiple"]
 
-            if (value is [] or value == '') and type != "str":
+            if (value is [] or value == "") and type != "str":
                 value = None
 
             if type in NATIVE_TYPES:
                 parameters_dict[name] = value
             elif type in DATABASE_TYPES:
                 parameters_dict[name] = value
             else:
-                parameters_dict[name] = [self._transform_parameters(val) for val in value] if multiple else self._transform_parameters(value)
+                parameters_dict[name] = (
+                    [self._transform_parameters(val) for val in value]
+                    if multiple
+                    else self._transform_parameters(value)
+                )
         return parameters_dict
 
 
-class AbstractComponent(RunnableMixin, HooksMixin, IndexMixin, BindingsMixin, ParametersMixin, VariableValueMixin):
+class AbstractComponent(
+    RunnableMixin,
+    HooksMixin,
+    IndexMixin,
+    BindingsMixin,
+    ParametersMixin,
+    VariableValueMixin,
+):
     database_client_kwargs: Dict[str, Any] = {}
     datalake_client_kwargs: Dict[str, Any] = {}
     deployment_client_kwargs: Dict[str, Any] = {}
     communication_client_kwargs: Dict[str, Any] = {}
     blockchain_client_kwargs: Dict[str, Any] = {}
 
-    def __init__(self, run_spec: dict, initial_setup: Optional[dict] = None, component_id: str = None, *args, **kwargs):
+    def __init__(
+        self,
+        run_spec: dict,
+        initial_setup: Optional[dict] = None,
+        component_id: str = None,
+        *args,
+        **kwargs,
+    ):
         self._setup = default_setup
         if initial_setup:
             self._setup.configure(initial_setup)
 
         self.namespace = self._setup.settings.NAMESPACE
         self.instance_type = Component
         self.instance_id = component_id if component_id else str(uuid.uuid4())
@@ -515,34 +695,33 @@
     @cached_property
     def instance(self):
         return self.database_client.get(
             resource_type=self.instance_type, id=self.instance_id, first=True
         )
 
     def _load_instance_kwargs_for_clients(self):
-        self.communication_client_kwargs['instance_id'] = self.instance_id
+        self.communication_client_kwargs["instance_id"] = self.instance_id
 
     def _load_spec_models(self):
         self.output: Type = self._spec.output_model
         self.custom_types: Type = self._spec.custom_types_model
         self.commands: Type = self._spec.commands_model
         self.bindings: List[Binding] = self._spec.bindings
 
     def _load_input_model(self):
         raw_spec = self.spec.dict()
         parsed_input_parameters = self.parse_parameters(raw_spec["input"])
-        self.input: BaseModel = self._spec.input_model(**parsed_input_parameters)
+        self.input: BaseModel = self._spec.input_model(
+            **parsed_input_parameters
+        )
 
     def _load_clients(self, database_config: Dict, datalake_config: Dict):
         self.database_client = self.setup.DATABASE_CLIENT(
-            namespace=self.namespace,
-            **database_config
+            namespace=self.namespace, **database_config
         )
         self.datalake_client = self.setup.DATALAKE_CLIENT(
-            namespace=self.namespace,
-            **datalake_config
+            namespace=self.namespace, **datalake_config
         )
         self.communication_client = self.setup.COMMUNICATION_CLIENT(
-            namespace=self.namespace,
-            **self.communication_client_kwargs
+            namespace=self.namespace, **self.communication_client_kwargs
         )
         self.execution_client = ExecutionClient(namespace=self.namespace)
```

### Comparing `splight-lib-2.3.0/splight_lib/encryption.py` & `splight-lib-2.3.1/splight_lib/encryption.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import cached_property
-from cryptography.fernet import Fernet as Branca
 from typing import Optional
+
+from cryptography.fernet import Fernet as Branca
 from pydantic import BaseSettings
 
 
 class EncryptionSettings(BaseSettings):
     SPLIGHT_ENCRYPTION_KEY: Optional[str] = None
 
 
@@ -33,23 +34,23 @@
         if not self.key:
             return value
         return self.fernet.decrypt(value.encode()).decode()
 
     def encrypt_file(self, path: str):
         if not self.key:
             return None
-        with open(path, 'rb+') as f:
+        with open(path, "rb+") as f:
             original = f.read()
-        with open(path, 'wb') as f:
+        with open(path, "wb") as f:
             f.seek(0)
             encrypted = self.fernet.encrypt(original)
             f.write(encrypted)
 
     def decrypt_file(self, path: str):
         if not self.key:
             return
-        with open(path, 'rb+') as f:
+        with open(path, "rb+") as f:
             original = f.read()
-        with open(path, 'wb') as f:
+        with open(path, "wb") as f:
             f.seek(0)
             decrypted = self.fernet.decrypt(original)
             f.write(decrypted)
```

### Comparing `splight-lib-2.3.0/splight_lib/execution.py` & `splight-lib-2.3.1/splight_lib/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-
-import time
 import atexit
 import sys
+import time
 import uuid
-from typing import List, Callable, Union, Tuple, Any
-from threading import (
-    Thread as DefaultThread,
-    Event,
-    Lock,
-)
-from subprocess import Popen as DefaultPopen
 from functools import wraps
-from splight_abstract.client.abstract import AbstractClient
-from splight_lib.logging._internal import get_splight_logger, LogTags
+from subprocess import Popen as DefaultPopen
+from threading import Event, Lock
+from threading import Thread as DefaultThread
+from typing import Any, Callable, List, Tuple, Union
 
+from splight_abstract.client.abstract import AbstractClient
+from splight_lib.logging._internal import LogTags, get_splight_logger
 
 logger = get_splight_logger()
 
+
 class Empty(object):
     pass
 
 
 class Task:
     """A periodic task for the scheduler."""
 
-    def __init__(self, handler: Callable[[Any], None], args: Tuple, period: int, hash: str = None) -> None:
+    def __init__(
+        self,
+        handler: Callable[[Any], None],
+        args: Tuple,
+        period: int,
+        hash: str = None,
+    ) -> None:
         if hash is None:
             hash = str(uuid.uuid4())
         self.hash = hash
         self.args = args
         self.period = period
         self.handler = handler
         self._name = self.handler
@@ -49,15 +52,15 @@
 
     def update_event(self) -> None:
         """Set next_event of the TaskSet."""
         if len(self._periods) > 0:
             self.next_event += min(self._periods)
         else:
             # 2**16 is enough to wait and don't overflow.
-            self.next_event = time.time() + 2 ** 16
+            self.next_event = time.time() + 2**16
 
     def in_time(self, now: float) -> bool:
         """
         Check if the TaskSet is in time to execute.
 
         Args:
             now (int): The time now.
@@ -240,28 +243,28 @@
         super().__init__(target=target, args=args, name=target, **kwargs)
 
     def store_result(self, func: Callable) -> Callable:
         @wraps(func)
         def wrapper(*args, **kwargs):
             self.result = func(*args, **kwargs)
             return self.result
+
         return wrapper
 
     def exit_ok(self) -> bool:
         return not isinstance(self.result, Empty)
 
     def kill(self) -> None:
         pass
 
     def terminate(self) -> None:
         pass
 
 
 class Popen(DefaultPopen):
-
     def __init__(self, args: List[str]) -> None:
         self.args: List[str] = args
         super(Popen, self).__init__(args)
 
     def is_alive(self) -> bool:
         return self.poll() is None
 
@@ -322,20 +325,25 @@
         logger.debug("Starting Thread %s", job, tags=LogTags.RUNTIME)
         self.threads.append(job)
         job.start()
         return
 
     def _start_task(self, job: Task) -> None:
         logger.debug("Starting Task %s", job, tags=LogTags.RUNTIME)
-        if not getattr(self, '_scheduler', None):
+        if not getattr(self, "_scheduler", None):
             # Instantiate and start Scheduler thread
             self._scheduler = Scheduler()
             self._start_thread(Thread(target=self._scheduler.start))
 
         return self._scheduler.schedule(job)
 
     def _stop_task(self, job: Task) -> None:
         logger.debug("Stopping Task %s", job, tags=LogTags.RUNTIME)
         return self._scheduler.unschedule(job)
 
     def healthcheck(self):
-        return all([p.is_alive() or p.exit_ok() for p in self.processes + self.threads])
+        return all(
+            [
+                p.is_alive() or p.exit_ok()
+                for p in self.processes + self.threads
+            ]
+        )
```

### Comparing `splight-lib-2.3.0/splight_lib/logging/_internal.py` & `splight-lib-2.3.1/splight_lib/logging/_internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
+from enum import auto
+from logging import INFO, Formatter, Handler
 from typing import Optional
-from logging import Formatter, Handler, INFO
+
+from concurrent_log_handler import ConcurrentRotatingFileHandler
 from splight_lib.logging.logging import (
     SplightFormatter,
     SplightLogger,
     standard_output_handler,
 )
-from concurrent_log_handler import ConcurrentRotatingFileHandler
-from enum import auto
 from strenum import UppercaseStrEnum
 
 
 class LogTags(UppercaseStrEnum):
     RUNTIME = auto()
     BINDING = auto()
     COMMUNICATION = auto()
```

### Comparing `splight-lib-2.3.0/splight_lib/logging/component.py` & `splight-lib-2.3.1/splight_lib/logging/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
+from logging import INFO, Formatter, Handler, basicConfig
 from typing import Optional
-from logging import Formatter, Handler, INFO, basicConfig
+
+from concurrent_log_handler import ConcurrentRotatingFileHandler
 from splight_lib.logging.logging import (
     SplightFormatter,
     SplightLogger,
     standard_output_handler,
 )
-from concurrent_log_handler import ConcurrentRotatingFileHandler
 
 
 def component_file_handler(
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
 ) -> Handler:
     filename = os.getenv("SPLIGHT_COMPONENT_LOG_FILE", "/tmp/components.log")
```

### Comparing `splight-lib-2.3.0/splight_lib/logging/logging.py` & `splight-lib-2.3.1/splight_lib/logging/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import time
 import os
 import sys
-from typing import Dict, Optional
+import time
 from logging import (
-    Formatter,
-    Logger,
-    NOTSET,
+    CRITICAL,
     DEBUG,
+    ERROR,
     INFO,
+    NOTSET,
     WARNING,
-    ERROR,
-    CRITICAL,
+    Formatter,
     Handler,
+    Logger,
     StreamHandler,
-    root as rootLogger,
 )
+from logging import root as rootLogger
+from typing import Dict, Optional
 
 TAGS_KEY = "tags"
 
 
 class SplightFormatter(Formatter):
     DEFAULT_FMT: str = (
         "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
```

### Comparing `splight-lib-2.3.0/splight_lib/restclient/client.py` & `splight-lib-2.3.1/splight_lib/restclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import httpx
-from typing import Optional, Callable, Any, Union, Mapping, List
+from typing import Any, Callable, List, Mapping, Optional, Union
 
+import httpx
 from splight_lib.restclient.types import (
-    AuthTypes,
-    QueryParamTypes,
-    HeaderTypes,
-    CookieTypes,
-    TimeoutTypes,
-    DEFAULT_TIMEOUT_CONFIG,
-    VerifyTypes,
-    CertTypes,
-    ProxiesTypes,
-    Limits,
     DEFAULT_LIMITS,
     DEFAULT_MAX_REDIRECTS,
+    DEFAULT_TIMEOUT_CONFIG,
+    AuthTypes,
     BaseTransport,
+    CertTypes,
+    CookieTypes,
     EventHook,
-    URLTypes,
+    HeaderTypes,
+    Limits,
+    ProxiesTypes,
+    QueryParamTypes,
     RequestData,
-    RequestFiles
+    RequestFiles,
+    TimeoutTypes,
+    URLTypes,
+    VerifyTypes,
 )
 
 
 class DefaultClient(httpx._client.UseClientDefault):
     """
     For some parameters such as `auth=...` and `timeout=...` we need to be able
     to indicate the default "unset" state, in a way that is distinctly different
@@ -36,14 +36,15 @@
     parameter will send a request using whatever default timeout has been
     configured on the client. Including `timeout=None` will ensure no timeout is
     used.
 
     Note that user code shouldn't need to use the `DEFAULT_CLIENT` constant,
     but it is used internally when a parameter is not included.
     """
+
     # Currently, this class is a copy of httpx._client.UseClientDefault.
 
 
 DEFAULT_CLIENT = DefaultClient()
 
 
 class SplightResponse(httpx.Response):
@@ -113,15 +114,15 @@
     requests.
     * timeout (optional) The timeout configuration to use when sending requests.
 
     For POST, PUT and PATCH methods. (Compatible with requests interface)
     * data (optional) Dictionary, list of tuples, bytes, or file-like object to
     send in the body of the request.
     * files (optional) Iterable of files to send into the request.
-    * json (optional) A JSON serializable Python object to send in the request 
+    * json (optional) A JSON serializable Python object to send in the request
     body.
     """
 
     _GET_METHOD = "GET"
     _OPTIONS_METHOD = "OPTIONS"
     _HEAD_METHOD = "HEAD"
     _POST_METHOD = "POST"
@@ -151,15 +152,15 @@
         transport: Optional[BaseTransport] = None,
         app: Optional[Callable[..., Any]] = None,
         trust_env: bool = True,
         default_encoding: Union[str, Callable[[bytes], str]] = "utf-8",
         event_hooks: Optional[Mapping[str, List[EventHook]]] = None,
     ):
         """Initialize the SplightRestClient.
-        
+
         Parameters: See class docstring.
         """
         # Client is the httpx Session impl
         # in httpx.Client allow_redirects is named follow_redirects
         self._client = httpx.Client(
             auth=auth,
             params=params,
@@ -175,15 +176,15 @@
             base_url=base_url,
             limits=limits,
             max_redirects=max_redirects,
             transport=transport,
             app=app,
             trust_env=trust_env,
             default_encoding=default_encoding,
-            event_hooks=event_hooks
+            event_hooks=event_hooks,
         )
 
     def update_headers(self, new_headers: HeaderTypes):
         self._client.headers = self._client._merge_headers(new_headers)
 
     def get(
         self,
```

### Comparing `splight-lib-2.3.0/splight_lib/restclient/exceptions.py` & `splight-lib-2.3.1/splight_lib/restclient/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from typing import Optional
 
 from httpx._models import Request
 
 
 class HTTPError(Exception):
-
     def __init__(self, message: str) -> None:
         super().__init__(message)
         self._request = None
 
     @property
     def request(self) -> Request:
         if self._request is None:
@@ -23,15 +22,14 @@
 
     @request.setter
     def request(self, request: Request) -> None:
         self._request = request
 
 
 class RequestError(HTTPError):
-
     def __init__(
         self, message: str, *, request: Optional[Request] = None
     ) -> None:
         super().__init__(message)
         self._request = request
```

### Comparing `splight-lib-2.3.0/splight_lib/restclient/types.py` & `splight-lib-2.3.1/splight_lib/restclient/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 Type definitions for type checking purposes.
 """
 
 import ssl
-from furl import furl
 from http.cookiejar import CookieJar
 from typing import (
-    Optional,
-    Union,
-    Tuple,
-    Callable,
-    Mapping,
     IO,
-    Sequence,
+    Any,
+    Callable,
     Dict,
     List,
-    Any
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
 )
 
+from furl import furl
 from httpx._auth import Auth
-from httpx._urls import QueryParams
-from httpx._models import Request, Headers, Cookies
-from httpx._config import Timeout, Proxy, Limits
+from httpx._config import Limits, Proxy, Timeout
+from httpx._models import Cookies, Headers, Request
 from httpx._transports.base import BaseTransport  # used in client
+from httpx._urls import QueryParams
 
 # Currently, this types are based on httpx._types.
 
 DEFAULT_TIMEOUT_CONFIG = Timeout(timeout=60.0)
 DEFAULT_LIMITS = Limits(max_connections=100, max_keepalive_connections=20)
 DEFAULT_MAX_REDIRECTS = 20
 
@@ -51,15 +51,17 @@
     "Headers",
     Mapping[str, str],
     Mapping[bytes, bytes],
     Sequence[Tuple[str, str]],
     Sequence[Tuple[bytes, bytes]],
 ]
 
-CookieTypes = Union["Cookies", CookieJar, Dict[str, str], List[Tuple[str, str]]]
+CookieTypes = Union[
+    "Cookies", CookieJar, Dict[str, str], List[Tuple[str, str]]
+]
 
 TimeoutTypes = Union[
     Optional[float],
     Tuple[Optional[float], Optional[float], Optional[float], Optional[float]],
     "Timeout",
 ]
 
@@ -74,17 +76,15 @@
     Tuple[str, Optional[str], Optional[str]],
 ]
 
 # for now is just a string. In the future could be httpx._urls.URL too.
 URLTypes = Union[str, furl]
 
 ProxiesTypes = Union[
-    URLTypes,
-    "Proxy",
-    Dict[URLTypes, Union[None, URLTypes, "Proxy"]]
+    URLTypes, "Proxy", Dict[URLTypes, Union[None, URLTypes, "Proxy"]]
 ]
 
 EventHook = Callable[..., Any]
 
 RequestData = Mapping[str, Any]
 
 FileContent = Union[IO[bytes], bytes, str]
```

### Comparing `splight-lib-2.3.0/splight_lib/settings.py` & `splight-lib-2.3.1/splight_lib/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
             "DATALAKE_CLIENT",
             "NOTIFICATION_CLIENT",
             "HUB_CLIENT",
             "COMMUNICATION_CLIENT",
         ]
 
     class Config:
-
         extra = Extra.ignore
 
         @classmethod
         def customise_sources(
             cls,
             init_settings: SettingsSourceCallable,
             env_settings: SettingsSourceCallable,
```

### Comparing `splight-lib-2.3.0/splight_lib/webhook.py` & `splight-lib-2.3.1/splight_lib/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
-from typing import Tuple
 from functools import cached_property
+from typing import Tuple
+
 from pydantic import BaseSettings
 from splight_lib.auth import HmacSignature
 from splight_models import WebhookEvent
 
 
 class WebhookSettings(BaseSettings):
     SPLIGHTD_WEBHOOK_SECRET: str
@@ -31,12 +32,10 @@
 
     def validate_signature(self, payload: bytes, signature: str) -> bool:
         return HmacSignature.verify_header(
             payload, signature, self._settings.SPLIGHTD_WEBHOOK_SECRET
         )
 
     def get_signature(self, payload: bytes) -> str:
-        hmac = HmacSignature(
-            secret=self._settings.SPLIGHTD_WEBHOOK_SECRET
-        )
+        hmac = HmacSignature(secret=self._settings.SPLIGHTD_WEBHOOK_SECRET)
         signature = hmac.compute_header_signature(payload)
         return signature
```

### Comparing `splight-lib-2.3.0/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.3.1/splight_lib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.0/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.3.1/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_models/__init__.py` & `splight-lib-2.3.1/splight_models/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from splight_models.asset import *
 from splight_models.alert import Alert, AlertCondition
+from splight_models.asset import *
 from splight_models.attribute import *
 from splight_models.blockchain import *
-from splight_models.communication import *
 from splight_models.channel import *
+from splight_models.communication import *
+from splight_models.component import *
 from splight_models.credential import *
 from splight_models.datalake import *
 from splight_models.deployment import *
 from splight_models.file import *
 from splight_models.hub import *
 from splight_models.namespace import *
 from splight_models.notification import *
 from splight_models.query import *
-from splight_models.component import *
+from splight_models.secret import *
+from splight_models.setpoint import *
 from splight_models.user import *
 from splight_models.variable import *
 from splight_models.webhook import *
-from splight_models.secret import *
-from splight_models.setpoint import *
```

### Comparing `splight-lib-2.3.0/splight_models/alert.py` & `splight-lib-2.3.1/splight_models/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import builtins
 import operator
 from typing import List, Optional, Union
 from uuid import UUID
 
 from pydantic import EmailStr, Field, validator
-
 from splight_models.base import SplightBaseModel
 from splight_models.constants import (
     AlertOperator,
     AlertStatus,
     AlertVariableType,
 )
```

### Comparing `splight-lib-2.3.0/splight_models/blockchain.py` & `splight-lib-2.3.1/splight_models/blockchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # TODO remove this models from here.
-import re
 import json
+import re
 from datetime import datetime, timezone
 from typing import Optional, Union
-from pydantic import validator, Json, Field, validator
+
 from hexbytes import HexBytes
+from pydantic import Field, Json, validator
 from splight_models.base import SplightBaseModel
 
 
 class BlockchainContract(SplightBaseModel):
     id: Optional[str]
     name: str
     description: str = ""
     address: str
     abi_json: Json
 
-    @validator('address', pre=True, always=True)
+    @validator("address", pre=True, always=True)
     def set_account_id_now(cls, v):
         regex = r"(\b0x[a-fA-F0-9]{40}\b)"
-        assert re.match(regex, v), 'Account value not allowed it should be a hex str.'
+        assert re.match(
+            regex, v
+        ), "Account value not allowed it should be a hex str."
         return v
 
-    @validator('abi_json', pre=True, always=True)
+    @validator("abi_json", pre=True, always=True)
     def set_abi_json_now(cls, v):
         if isinstance(v, list):
             return json.dumps(v)
         return v
 
 
 class CallResponse(SplightBaseModel):
@@ -39,10 +42,17 @@
     status: Optional[int] = 0
     contract_address: Optional[str] = Field(None, alias="contractAddress")
     block_hash: str = Field(..., alias="blockHash")
     block_number: int = Field(..., alias="blockNumber")
     transaction_hash: str = Field(..., alias="transactionHash")
     transaction_index: int = Field(..., alias="transactionIndex")
 
-    @validator("from_account", "to_account", "block_hash", "transaction_hash", "contract_address", pre=True)
+    @validator(
+        "from_account",
+        "to_account",
+        "block_hash",
+        "transaction_hash",
+        "contract_address",
+        pre=True,
+    )
     def cast_to_str(cls, value):
         return value.hex() if isinstance(value, HexBytes) else value
```

### Comparing `splight-lib-2.3.0/splight_models/communication/events.py` & `splight-lib-2.3.1/splight_models/communication/events.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-
+from datetime import datetime, timezone
 from enum import Enum
 from typing import Dict, Optional
+
 from pydantic import Field
 from splight_models.base import SplightBaseModel
 from splight_models.user import User
-from datetime import datetime, timezone
 
 
 class EventActions(str, Enum):
     CREATE = "CREATE"
     UPDATE = "UPDATE"
     DELETE = "DELETE"
     TRIGGER = "TRIGGER"
     READ = "READ"
 
 
 class EventNames(str, Enum):
     # TODO make this use EventActions.
-    COMPONENT_COMMAND_TRIGGER = 'componentcommand-trigger'
-    COMPONENT_COMMAND_CREATE = 'componentcommand-create'
-    COMPONENT_COMMAND_UPDATE = 'componentcommand-update'
+    COMPONENT_COMMAND_TRIGGER = "componentcommand-trigger"
+    COMPONENT_COMMAND_CREATE = "componentcommand-create"
+    COMPONENT_COMMAND_UPDATE = "componentcommand-update"
     # TODO add Asset Attribute and all shared objects
 
-    SETPOINT_CREATE = 'setpoint-create'
-    SETPOINT_UPDATE = 'setpoint-update'
+    SETPOINT_CREATE = "setpoint-create"
+    SETPOINT_UPDATE = "setpoint-update"
 
 
 class CommunicationEvent(SplightBaseModel):
     event_name: str
     id: Optional[str] = None
     instance_id: Optional[str] = None
     socket_id: Optional[str] = None
-    timestamp: str = Field(default_factory=lambda: datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%S.%fZ"))  # pusher cannot json serialize datetime objects
+    timestamp: str = Field(
+        default_factory=lambda: datetime.now(timezone.utc).strftime(
+            "%Y-%m-%dT%H:%M:%S.%fZ"
+        )
+    )  # pusher cannot json serialize datetime objects
     display_text: Optional[str] = None
     user: Optional[User] = None
     data: Dict
```

### Comparing `splight-lib-2.3.0/splight_models/component.py` & `splight-lib-2.3.1/splight_models/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from splight_models.constants import (
-    ComponentSize,
-    RestartPolicy,
-    LogginLevel,
-    ComponentStatus,
-    ComponentType
+import inspect
+from copy import copy
+from datetime import datetime
+from enum import Enum, auto
+from functools import cached_property
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
+
+from pydantic import (
+    AnyUrl,
+    BaseModel,
+    Field,
+    ValidationError,
+    create_model,
+    validator,
 )
+from splight_models import CommunicationEvent, EventActions, EventNames
 from splight_models.asset import Asset
 from splight_models.attribute import Attribute
 from splight_models.base import SplightBaseModel
-from splight_models.file import File
+from splight_models.constants import (
+    ComponentSize,
+    ComponentStatus,
+    ComponentType,
+    LogginLevel,
+    RestartPolicy,
+)
 from splight_models.datalake import DatalakeModel
+from splight_models.file import File
 from splight_models.query import Query
-from splight_models import EventActions, EventNames, CommunicationEvent
-from datetime import datetime
-from enum import Enum, auto
-from typing import Type, List, Dict, Tuple, Optional, Any, Union
-from pydantic import BaseModel, create_model, Field, AnyUrl, ValidationError, validator
-from copy import copy
-from functools import cached_property
-import inspect
 from strenum import LowercaseStrEnum
 
 
 def choices_validator(cls, value, field):
     parameter = getattr(cls.SpecFields, field.name, None)
     if parameter is None:
         return value
@@ -37,30 +45,30 @@
     READ = auto()
     WRITE = auto()
     READWRITE = auto()
 
 
 class Parameter(SplightBaseModel):
     name: str
-    description: str = ''
+    description: str = ""
     type: str = "str"
     required: bool = False
     multiple: bool = False
     sensitive: bool = False
     choices: Optional[List[Any]] = None
     depends_on: Optional[str] = None
 
 
 class InputParameter(Parameter):
     value: Optional[Any] = None
 
 
 class OutputParameter(SplightBaseModel):
     name: str
-    description: str = ''
+    description: str = ""
     type: str
     choices: Optional[List[Any]] = None
     depends_on: Optional[str] = None
     filterable: bool = False
 
 
 class CommandParameter(InputParameter):
@@ -162,34 +170,36 @@
             component_id=self.id
         ).get_custom_types_model(self.custom_types)
 
     @cached_property
     def input_model(self) -> Type:
         custom_type_model = self.custom_types_model
         custom_types = inspect.getmembers(custom_type_model)
-        custom_types_dict = {a[0]: a[1] for a in custom_types if not a[0].startswith('__')}
+        custom_types_dict = {
+            a[0]: a[1] for a in custom_types if not a[0].startswith("__")
+        }
         return ComponentModelsFactory(
-            type_map=custom_types_dict,
-            component_id=self.id
+            type_map=custom_types_dict, component_id=self.id
         ).get_input_model(self.input)
 
     @cached_property
     def output_model(self) -> Type:
-        return ComponentModelsFactory(
-            component_id=self.id
-        ).get_output_model(self.output)
+        return ComponentModelsFactory(component_id=self.id).get_output_model(
+            self.output
+        )
 
     @cached_property
     def commands_model(self) -> Type:
         custom_type_model = self.custom_types_model
         custom_types = inspect.getmembers(custom_type_model)
-        custom_types_dict = {a[0]: a[1] for a in custom_types if not a[0].startswith('__')}
+        custom_types_dict = {
+            a[0]: a[1] for a in custom_types if not a[0].startswith("__")
+        }
         return ComponentModelsFactory(
-            type_map=custom_types_dict,
-            component_id=self.id
+            type_map=custom_types_dict, component_id=self.id
         ).get_commands_model(self.commands)
 
 
 class Component(BaseComponent):
     id: Optional[str]
     description: Optional[str]
     log_level: LogginLevel = LogginLevel.info
@@ -226,20 +236,21 @@
 }
 
 
 SIMPLE_TYPES = list(NATIVE_TYPES.keys()) + list(DATABASE_TYPES.keys())
 
 
 class ComponentModelsFactory:
-    def __init__(self, type_map: Dict[str, Type] = {}, component_id: Optional[str] = None) -> None:
+    def __init__(
+        self,
+        type_map: Dict[str, Type] = {},
+        component_id: Optional[str] = None,
+    ) -> None:
         self._component_id = component_id
-        self._type_map = {
-            **type_map,
-            **self._load_type_map()
-        }
+        self._type_map = {**type_map, **self._load_type_map()}
 
     @staticmethod
     def _load_type_map() -> Dict[str, Type]:
         type_map: Dict[str, Type] = {}
         type_map.update(NATIVE_TYPES)
         type_map.update({k: Union[str, v] for k, v in DATABASE_TYPES.items()})
         return type_map
@@ -266,34 +277,35 @@
     def get_output_model(self, outputs: List) -> BaseModel:
         output_models: Dict[str, BaseModel] = {}
 
         for output in outputs:
             output_format_field = {
                 "output_format": Field(output.name, const=True),
             }
-            output_models[output.name] = self._create_model(output.name,
-                                                            output.fields,
-                                                            output_format_field,
-                                                            DatalakeModel)
+            output_models[output.name] = self._create_model(
+                output.name, output.fields, output_format_field, DatalakeModel
+            )
 
         return type("Output", (), output_models)
 
     def get_commands_model(self, commands: List) -> BaseModel:
         command_models: Dict[str, BaseModel] = {}
         for command in commands:
-            command_models[command.name] = self._create_model(command.name,
-                                                              command.fields)
+            command_models[command.name] = self._create_model(
+                command.name, command.fields
+            )
         return type("Commands", (), command_models)
 
-    def _create_model(self,
-                      name: str,
-                      fields: List[Parameter],
-                      extra_fields: Dict = {},
-                      base: Type = SplightBaseModel) -> Type:
-
+    def _create_model(
+        self,
+        name: str,
+        fields: List[Parameter],
+        extra_fields: Dict = {},
+        base: Type = SplightBaseModel,
+    ) -> Type:
         # Inline classes for meta attrs
         class SpecFields:
             pass
 
         class Meta:
             collection_name = str(self._component_id)
 
@@ -303,19 +315,21 @@
             setattr(SpecFields, field.name, field)
             type = self._type_map[field.type]
             choices = getattr(field, "choices", None)
             multiple = getattr(field, "multiple", False)
             required = getattr(field, "required", True)
 
             if choices:
-                validators.update({
-                    "choices_validator": validator(
-                        field.name, pre=True, allow_reuse=True
-                    )(choices_validator)
-                })
+                validators.update(
+                    {
+                        "choices_validator": validator(
+                            field.name, pre=True, allow_reuse=True
+                        )(choices_validator)
+                    }
+                )
 
             if multiple:
                 type = List[type]
 
             value = ...
             if not required:
                 type = Optional[type]
```

### Comparing `splight-lib-2.3.0/splight_models/constants.py` & `splight-lib-2.3.1/splight_models/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 class ChoiceMixin(str, Enum):
     @classmethod
     def choices(cls):
         return [(key.value.lower(), key.name.capitalize()) for key in cls]
 
 
 class SeverityType(ChoiceMixin):
-    system = 'system'
-    info = 'info'
-    low = 'low'
-    medium = 'medium'
-    high = 'high'
-    critical = 'critical'
+    system = "system"
+    info = "info"
+    low = "low"
+    medium = "medium"
+    high = "high"
+    critical = "critical"
 
 
 class AlertStatus(ChoiceMixin):
     ALERT = "alert"
     NO_ALERT = "no_alert"
     NO_DATA = "no_data"
 
@@ -75,18 +75,18 @@
     RUNNING = "Running"
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     UNKNOWN = "Unknown"
 
 
 class MinComponentCapacity(ChoiceMixin):
-    SMALL = 'small'
-    MEDIUM = 'medium'
-    LARGE = 'large'
-    VERY_LARGE = 'very_large'
+    SMALL = "small"
+    MEDIUM = "medium"
+    LARGE = "large"
+    VERY_LARGE = "very_large"
 
 
 class ComponentStatus(ChoiceMixin):
     STOPPED = "Stopped"
     PENDING = "Pending"
     RUNNING = "Running"
     SUCCEEDED = "Succeeded"
```

### Comparing `splight-lib-2.3.0/splight_models/datalake.py` & `splight-lib-2.3.1/splight_models/datalake.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from pydantic import Field
-from typing import Optional
 from datetime import datetime, timezone
+from typing import Optional
+
+from pydantic import Field
 from splight_models.base import SplightBaseModel
 
 
 class DatalakeModel(SplightBaseModel):
-    timestamp: datetime = Field(default_factory=lambda: datetime.now(timezone.utc))
+    timestamp: datetime = Field(
+        default_factory=lambda: datetime.now(timezone.utc)
+    )
     instance_id: Optional[str] = None
     instance_type: Optional[str] = None
 
     class Config:
         # pydantic
         validate_assignment = True
 
@@ -19,15 +22,15 @@
     class SpecFields:
         # Fields to reconstruct Spec .fields
         pass
 
     def dict(self, *args, **kwargs):
         d = super().dict(*args, **kwargs)
         return {
-            k: v['id'] if isinstance(v, dict) and 'id' in v.keys() else v
+            k: v["id"] if isinstance(v, dict) and "id" in v.keys() else v
             for k, v in d.items()
         }
 
     def json(self, *args, **kwargs):
         restore = {}
 
         for k in self.__class__.__fields__.keys():
```

### Comparing `splight-lib-2.3.0/splight_models/deployment.py` & `splight-lib-2.3.1/splight_models/deployment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Dict, List, Optional
+
 from splight_models.base import SplightBaseModel
+from splight_models.component import BaseComponent
 from splight_models.constants import (
-    ComponentSize, DeploymentStatus, LogginLevel, RestartPolicy
+    ComponentSize,
+    DeploymentStatus,
+    LogginLevel,
+    RestartPolicy,
 )
-from splight_models.component import BaseComponent
 
 
 class Deployment(BaseComponent):
     # run-spec
     id: Optional[str] = None
     component_id: Optional[str] = None
     status: Optional[DeploymentStatus] = None
```

### Comparing `splight-lib-2.3.0/splight_models/exception.py` & `splight-lib-2.3.1/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.0/splight_models/file.py` & `splight-lib-2.3.1/splight_models/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from .base import SplightBaseModel
-from typing import Optional, Dict
-from pydantic import validator
 import json
 import os
+from typing import Dict, Optional
+
+from pydantic import validator
+
+from .base import SplightBaseModel
 
 
 class File(SplightBaseModel):
     id: Optional[str] = None
     file: str
     description: Optional[str] = None
     metadata: Dict = {}
     content_type: Optional[str] = None
     url: Optional[str] = None
     encrypted: Optional[bool] = False
 
     @validator("file", pre=True)
     def validate_file(cls, v):
-        v = v.replace('/', os.sep)
-        v = v.replace('\\', os.sep)
+        v = v.replace("/", os.sep)
+        v = v.replace("\\", os.sep)
         return v
 
     @property
     def name(self):
         return self.file.split(os.sep)[-1]
 
     def json(self, *args, **kwargs):
```

### Comparing `splight-lib-2.3.0/splight_models/hub.py` & `splight-lib-2.3.1/splight_models/hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional
+from typing import List, Optional
+
 from pydantic import validator
 from splight_models.component import BaseComponent
-from typing import List
 
-VERIFICATION_CHOICES = ['verified', 'unverified', 'official']
+VERIFICATION_CHOICES = ["verified", "unverified", "official"]
 
 
 class HubComponent(BaseComponent):
     id: Optional[str]
     name: str
     splight_cli_version: str
     build_status: Optional[str]
@@ -21,16 +21,16 @@
     verification: Optional[str]
     created_at: Optional[str]
     last_modified: Optional[str]
     tags: List[str] = []
     min_component_capacity: Optional[str]
     usage_count: int = 0
 
-    @validator('verification', pre=True, always=True)
+    @validator("verification", pre=True, always=True)
     def set_verification_now(cls, v):
         if v:
-            assert v in VERIFICATION_CHOICES, 'Verification value not allowed.'
+            assert v in VERIFICATION_CHOICES, "Verification value not allowed."
         return v
 
 
 class HubComponentVersion(HubComponent):
     pass
```

### Comparing `splight-lib-2.3.0/splight_models/notification.py` & `splight-lib-2.3.1/splight_models/notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from pydantic import Field
 from datetime import datetime, timezone
-from typing import Optional
 from enum import Enum
+from typing import Optional
+
+from pydantic import Field
 from splight_models import SplightBaseModel
 
 
 class SourceType(str, Enum):
-    component = 'Component'
-    system = 'System'
-    user = 'User'
+    component = "Component"
+    system = "System"
+    user = "User"
 
 
 class TargetType(str, Enum):
-    component = 'Component'
-    dashboard = 'Dashboard'
-    asset = 'Asset'
-    attribute = 'Attribute'
-    file_ = 'File'
-    query = 'Query'
+    component = "Component"
+    dashboard = "Dashboard"
+    asset = "Asset"
+    attribute = "Attribute"
+    file_ = "File"
+    query = "Query"
 
 
 class Notification(SplightBaseModel):
     id: Optional[str]
     message: str
     seen: bool = False
-    created_at: str = Field(default_factory=lambda: datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%S.%fZ"))
+    created_at: str = Field(
+        default_factory=lambda: datetime.now(timezone.utc).strftime(
+            "%Y-%m-%dT%H:%M:%S.%fZ"
+        )
+    )
     notify_by_email: Optional[bool] = False
     notify_by_web: Optional[bool] = True
     notify_by_sms: Optional[bool] = False
     notify_by_push: Optional[bool] = True
     source_id: Optional[str] = None
     source_type: Optional[SourceType] = None
     target_id: Optional[str] = None
```

### Comparing `splight-lib-2.3.0/splight_models/query.py` & `splight-lib-2.3.1/splight_models/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
-from typing import Dict, Union, List, Optional
+from typing import Dict, List, Optional, Union
+
 from pydantic import validator
 from splight_models.base import SplightBaseModel
 
 
 class QuerySourceType(str, Enum):
     NATIVE = "Native"
     COMPONENT = "Component"
@@ -16,47 +17,67 @@
     source_type: QuerySourceType
     source_component_id: Optional[str] = None
     output_format: str
     target: str
     filters: Dict = {}
     limit: int = 10000
     skip: int = 0
-    sort: Union[List, str] = ['timestamp__desc']
+    sort: Union[List, str] = ["timestamp__desc"]
     add_fields: Union[List, str] = []
     group_id: Union[List, str] = []
     group_fields: Union[List, str] = []
     rename_fields: Union[List, str] = []
     project_fields: Union[List, str] = []
-    timezone_offset: float = 0.0 # UTC
+    timezone_offset: float = 0.0  # UTC
 
     @validator("source_component_id", always=True)
     def source_component_id_validate(cls, source_component_id, values):
         source_type = values.get("source_type")
-        if source_type == QuerySourceType.COMPONENT and not source_component_id:
-            raise ValueError(f"source must be set when source_type is {source_type}")
+        if (
+            source_type == QuerySourceType.COMPONENT
+            and not source_component_id
+        ):
+            raise ValueError(
+                f"source must be set when source_type is {source_type}"
+            )
         return source_component_id
 
     @validator("target", always=True)
     def target_validate(cls, target, values):
         source_type = values.get("source_type")
         if source_type == QuerySourceType.NATIVE and target != "value":
-            raise ValueError(f"target must be 'value' when source_type is {source_type}")
+            raise ValueError(
+                f"target must be 'value' when source_type is {source_type}"
+            )
         if source_type == QuerySourceType.COMPONENT and not target:
-            raise ValueError(f"target must be set when source_type is {source_type}")
+            raise ValueError(
+                f"target must be set when source_type is {source_type}"
+            )
         return target
 
     @property
     def source(self):
-        return "default" if self.source_type == QuerySourceType.NATIVE else self.source_component_id
+        return (
+            "default"
+            if self.source_type == QuerySourceType.NATIVE
+            else self.source_component_id
+        )
 
     @property
     def query_params(self):
         query_params = f"?source={self.source}"
         if self.filters:
-            joined_filters = "&".join([f"{k}={','.join([str(i) for i in v])}" if type(v) == list else f"{k}={v}" for k, v in self.filters.items()])
+            joined_filters = "&".join(
+                [
+                    f"{k}={','.join([str(i) for i in v])}"
+                    if type(v) == list
+                    else f"{k}={v}"
+                    for k, v in self.filters.items()
+                ]
+            )
             query_params += f"&{joined_filters}"
         if self.output_format:
             query_params += f"&output_format={self.output_format}"
         query_params_fields = ["limit", "skip", "sort"]
         underscored_fields = ["limit", "skip"]
         for k in query_params_fields:
             field = k if not k in underscored_fields else k + "_"
```

### Comparing `splight-lib-2.3.0/splight_models/setpoint.py` & `splight-lib-2.3.1/splight_models/setpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from splight_models import EventNames, CommunicationEvent
-from pydantic import Field, validator, ValidationError
-from typing import Union, Optional, List
-from .base import SplightBaseModel
 from datetime import datetime
 from enum import auto
-from strenum import PascalCaseStrEnum, LowercaseStrEnum
+from typing import List, Optional, Union
+
+from pydantic import Field, ValidationError, validator
+from splight_models import CommunicationEvent, EventNames
+from strenum import LowercaseStrEnum, PascalCaseStrEnum
+
+from .base import SplightBaseModel
 
 
 class SetPointType(PascalCaseStrEnum):
     Number = auto()
     String = auto()
     Boolean = auto()
 
@@ -36,15 +38,15 @@
     id: Optional[str]
     asset: str
     attribute: str
     type: SetPointType
     value: Union[str, bool, float]
     responses: List[SetPointResponse] = []
 
-    @validator('value')
+    @validator("value")
     def cast_value(cls, v, values, **kwargs):
         if not "type" in values:
             raise ValueError("type is required")
 
         if values["type"] == SetPointType.Number:
             try:
                 return float(v)
```

### Comparing `splight-lib-2.3.0/splight_models/user.py` & `splight-lib-2.3.1/splight_models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,21 @@
 class Organization(SplightBaseModel):
     id: Optional[str] = None
     connection_id: Optional[str]
     name: str
     display_name: str
     metadata: OrganizationMetadata = OrganizationMetadata()
 
+
 class Connection(SplightBaseModel):
     id: Optional[str] = None
     name: str
     display_name: str
 
+
 class Inviter(SplightBaseModel):
     name: str
 
 
 class Invitee(SplightBaseModel):
     email: str
```

### Comparing `splight-lib-2.3.0/splight_models/variable.py` & `splight-lib-2.3.1/splight_models/variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # TODO rename this file or move it to datalake
-from pydantic import Field
 from typing import Union
+
+from pydantic import Field
+
 from .asset import Asset
 from .attribute import Attribute
 from .datalake import DatalakeModel
 
 
 class NativeOutput(DatalakeModel):
     asset: Union[Asset, str]
```

