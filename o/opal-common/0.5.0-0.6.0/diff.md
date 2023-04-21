# Comparing `tmp/opal-common-0.5.0.tar.gz` & `tmp/opal-common-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.5.0.tar", last modified: Mon Feb 27 17:27:11 2023, max compression
+gzip compressed data, was "opal-common-0.6.0.tar", last modified: Fri Apr 21 07:57:01 2023, max compression
```

## Comparing `opal-common-0.5.0.tar` & `opal-common-0.6.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.761119 opal-common-0.5.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8380 2023-02-27 17:27:11.760919 opal-common-0.5.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.748036 opal-common-0.5.0/opal_common/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      797 2022-10-11 10:23:16.000000 opal-common-0.5.0/opal_common/async_utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.750092 opal-common-0.5.0/opal_common/authentication/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1477 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/authz.py
--rw-r--r--   0 asafc      (501) staff       (20)     3267 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/casting.py
--rw-r--r--   0 asafc      (501) staff       (20)     5016 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/deps.py
--rw-r--r--   0 asafc      (501) staff       (20)     4669 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/signer.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.750316 opal-common-0.5.0/opal_common/authentication/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    17336 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 asafc      (501) staff       (20)      958 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/types.py
--rw-r--r--   0 asafc      (501) staff       (20)     4225 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/authentication/verifier.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.750887 opal-common-0.5.0/opal_common/cli/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/cli/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6657 2022-10-12 14:50:19.000000 opal-common-0.5.0/opal_common/cli/commands.py
--rw-r--r--   0 asafc      (501) staff       (20)      703 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/cli/docs.py
--rw-r--r--   0 asafc      (501) staff       (20)      167 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/cli/typer_app.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.751466 opal-common-0.5.0/opal_common/confi/
--rw-r--r--   0 asafc      (501) staff       (20)       21 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/confi/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2278 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/confi/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    13779 2023-02-24 20:59:56.000000 opal-common-0.5.0/opal_common/confi/confi.py
--rw-r--r--   0 asafc      (501) staff       (20)     2719 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/confi/types.py
--rw-r--r--   0 asafc      (501) staff       (20)     5805 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/config.py
--rw-r--r--   0 asafc      (501) staff       (20)     1492 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/corn_utils.py
--rw-r--r--   0 asafc      (501) staff       (20)     6050 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/emport.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.752138 opal-common-0.5.0/opal_common/fetcher/
--rw-r--r--   0 asafc      (501) staff       (20)      143 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.752772 opal-common-0.5.0/opal_common/fetcher/engine/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2653 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 asafc      (501) staff       (20)      296 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 asafc      (501) staff       (20)     1536 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 asafc      (501) staff       (20)     8484 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/events.py
--rw-r--r--   0 asafc      (501) staff       (20)     2547 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 asafc      (501) staff       (20)     3030 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 asafc      (501) staff       (20)      116 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/logger.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.753254 opal-common-0.5.0/opal_common/fetcher/providers/
--rw-r--r--   0 asafc      (501) staff       (20)       67 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1710 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 asafc      (501) staff       (20)     3525 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.753746 opal-common-0.5.0/opal_common/fetcher/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1917 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     4260 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     2140 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.755456 opal-common-0.5.0/opal_common/git/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/git/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5461 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/git/branch_tracker.py
--rw-r--r--   0 asafc      (501) staff       (20)    15616 2023-02-24 20:59:56.000000 opal-common-0.5.0/opal_common/git/bundle_maker.py
--rw-r--r--   0 asafc      (501) staff       (20)     1734 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/git/bundle_utils.py
--rw-r--r--   0 asafc      (501) staff       (20)     8685 2023-02-27 16:56:34.000000 opal-common-0.5.0/opal_common/git/commit_viewer.py
--rw-r--r--   0 asafc      (501) staff       (20)     7948 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/git/diff_viewer.py
--rw-r--r--   0 asafc      (501) staff       (20)     1580 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/git/env.py
--rw-r--r--   0 asafc      (501) staff       (20)      299 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/git/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)     8535 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/git/repo_cloner.py
--rw-r--r--   0 asafc      (501) staff       (20)     4237 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 asafc      (501) staff       (20)      182 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/http.py
--rw-r--r--   0 asafc      (501) staff       (20)     1831 2023-02-01 22:26:26.000000 opal-common-0.5.0/opal_common/logger.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.756627 opal-common-0.5.0/opal_common/logging/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      412 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/decorators.py
--rw-r--r--   0 asafc      (501) staff       (20)     1166 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/filter.py
--rw-r--r--   0 asafc      (501) staff       (20)      617 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/formatter.py
--rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/intercept.py
--rw-r--r--   0 asafc      (501) staff       (20)     1355 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/logging/thirdparty.py
--rw-r--r--   0 asafc      (501) staff       (20)     3520 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/middleware.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.757129 opal-common-0.5.0/opal_common/opa/
--rw-r--r--   0 asafc      (501) staff       (20)       88 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/opa/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      576 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/opa/parsing.py
--rw-r--r--   0 asafc      (501) staff       (20)      498 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/opa/paths.py
--rw-r--r--   0 asafc      (501) staff       (20)     3071 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/paths.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.758459 opal-common-0.5.0/opal_common/schemas/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/schemas/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6313 2023-02-24 20:59:56.000000 opal-common-0.5.0/opal_common/schemas/data.py
--rw-r--r--   0 asafc      (501) staff       (20)     1387 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/schemas/policy.py
--rw-r--r--   0 asafc      (501) staff       (20)     1767 2023-02-24 20:59:56.000000 opal-common-0.5.0/opal_common/schemas/policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)      508 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/schemas/scopes.py
--rw-r--r--   0 asafc      (501) staff       (20)     1573 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/schemas/security.py
--rw-r--r--   0 asafc      (501) staff       (20)     2003 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/schemas/store.py
--rw-r--r--   0 asafc      (501) staff       (20)     1250 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/schemas/webhook.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.758861 opal-common-0.5.0/opal_common/security/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/security/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      799 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/security/sslcontext.py
--rw-r--r--   0 asafc      (501) staff       (20)     3294 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/security/tarsafe.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.759372 opal-common-0.5.0/opal_common/sources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/sources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9414 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/sources/api_policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)     4282 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/sources/base_policy_source.py
--rw-r--r--   0 asafc      (501) staff       (20)     4237 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.759737 opal-common-0.5.0/opal_common/synchronization/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/synchronization/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1294 2023-02-01 11:46:28.000000 opal-common-0.5.0/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 asafc      (501) staff       (20)     2989 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.760081 opal-common-0.5.0/opal_common/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9622 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/tests/path_utils_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     1223 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.760688 opal-common-0.5.0/opal_common/topics/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/topics/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2371 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/topics/listener.py
--rw-r--r--   0 asafc      (501) staff       (20)     6454 2022-10-11 10:23:16.000000 opal-common-0.5.0/opal_common/topics/publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)     1053 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/topics/utils.py
--rw-r--r--   0 asafc      (501) staff       (20)      988 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/urls.py
--rw-r--r--   0 asafc      (501) staff       (20)     5917 2022-10-01 21:13:25.000000 opal-common-0.5.0/opal_common/utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:11.749055 opal-common-0.5.0/opal_common.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8380 2023-02-27 17:27:11.000000 opal-common-0.5.0/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     3198 2023-02-27 17:27:11.000000 opal-common-0.5.0/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-02-27 17:27:11.000000 opal-common-0.5.0/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      455 2023-02-27 17:27:11.000000 opal-common-0.5.0/opal_common.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-02-27 17:27:11.000000 opal-common-0.5.0/opal_common.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-02-27 17:27:11.761158 opal-common-0.5.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2601 2022-10-01 21:13:25.000000 opal-common-0.5.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.256069 opal-common-0.6.0/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8348 2023-04-21 07:57:01.255875 opal-common-0.6.0/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.244275 opal-common-0.6.0/opal_common/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      797 2022-12-08 13:45:19.000000 opal-common-0.6.0/opal_common/async_utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.246002 opal-common-0.6.0/opal_common/authentication/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/authz.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3267 2022-12-08 13:45:19.000000 opal-common-0.6.0/opal_common/authentication/casting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5016 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/signer.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.246236 opal-common-0.6.0/opal_common/authentication/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/authentication/verifier.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.246881 opal-common-0.6.0/opal_common/cli/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/cli/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/cli/commands.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      703 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/cli/docs.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/cli/typer_app.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.247418 opal-common-0.6.0/opal_common/confi/
+-rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/confi/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/confi/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13780 2023-04-18 15:25:03.000000 opal-common-0.6.0/opal_common/confi/confi.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2719 2023-04-18 15:25:03.000000 opal-common-0.6.0/opal_common/confi/types.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6648 2023-04-18 15:25:03.000000 opal-common-0.6.0/opal_common/config.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/corn_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6050 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/emport.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.248062 opal-common-0.6.0/opal_common/fetcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.248741 opal-common-0.6.0/opal_common/fetcher/engine/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8485 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/events.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.249146 opal-common-0.6.0/opal_common/fetcher/providers/
+-rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3525 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.249688 opal-common-0.6.0/opal_common/fetcher/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1917 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4260 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2140 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.251123 opal-common-0.6.0/opal_common/git/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/git/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-02-14 09:43:53.000000 opal-common-0.6.0/opal_common/git/branch_tracker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15616 2023-04-18 15:25:03.000000 opal-common-0.6.0/opal_common/git/bundle_maker.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-04-04 08:50:35.000000 opal-common-0.6.0/opal_common/git/bundle_utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-04-04 08:50:50.000000 opal-common-0.6.0/opal_common/git/commit_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/git/diff_viewer.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-02-14 09:43:53.000000 opal-common-0.6.0/opal_common/git/env.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/git/exceptions.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/git/repo_cloner.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/http.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1832 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/logger.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.251993 opal-common-0.6.0/opal_common/logging/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/decorators.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/filter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      617 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/formatter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/intercept.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/logging/thirdparty.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/middleware.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.252452 opal-common-0.6.0/opal_common/opa/
+-rw-r--r--   0 roekatz    (501) staff       (20)       88 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/opa/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      576 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/opa/parsing.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      499 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/opa/paths.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-04-20 14:50:53.000000 opal-common-0.6.0/opal_common/paths.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.253511 opal-common-0.6.0/opal_common/schemas/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/schemas/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6313 2023-04-19 08:36:33.000000 opal-common-0.6.0/opal_common/schemas/data.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/schemas/policy.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-02-14 09:43:53.000000 opal-common-0.6.0/opal_common/schemas/policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.6.0/opal_common/schemas/scopes.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1573 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/schemas/security.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2003 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/schemas/store.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-03-12 07:32:46.000000 opal-common-0.6.0/opal_common/schemas/webhook.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.253883 opal-common-0.6.0/opal_common/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/security/sslcontext.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/security/tarsafe.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.254377 opal-common-0.6.0/opal_common/sources/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/sources/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     9414 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.254764 opal-common-0.6.0/opal_common/synchronization/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/synchronization/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1294 2023-01-19 13:43:15.000000 opal-common-0.6.0/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.255155 opal-common-0.6.0/opal_common/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.255648 opal-common-0.6.0/opal_common/topics/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/topics/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/topics/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6517 2023-04-19 08:36:33.000000 opal-common-0.6.0/opal_common/topics/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-03-27 15:01:56.000000 opal-common-0.6.0/opal_common/topics/utils.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/urls.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5917 2022-12-08 13:40:17.000000 opal-common-0.6.0/opal_common/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.245051 opal-common-0.6.0/opal_common.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8348 2023-04-21 07:57:01.000000 opal-common-0.6.0/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     3198 2023-04-21 07:57:01.000000 opal-common-0.6.0/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-04-21 07:57:01.000000 opal-common-0.6.0/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      452 2023-04-21 07:57:01.000000 opal-common-0.6.0/opal_common.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-04-21 07:57:01.000000 opal-common-0.6.0/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-04-21 07:57:01.256113 opal-common-0.6.0/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.6.0/setup.py
```

### Comparing `opal-common-0.5.0/PKG-INFO` & `opal-common-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -77,17 +76,17 @@
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
 
-  - [Play with a live playground environment in docker-compose](https://docs.opal.ac/getting-started/get_started_with_opal_docker_compose_tutorial)
+  - [Play with a live playground environment in docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-playground/overview)
   <!-- - this tutorial is great for learning about OPAL core features and see what OPAL can do for you. -->
-  - [Try the getting started guide for containers](https://docs.opal.ac/getting-started/get_started_with_opal_using_docker)
+  - [Try the getting started guide for containers](https://docs.opal.ac/getting-started/running-opal/overview)
   <!-- - this tutorial will show you how to configure OPAL to your specific needs and run the official docker containers locally or in production. -->
 
   - [Check out the Helm Chart for Kubernetes](https://github.com/permitio/opal-helm-chart)
 
 - A video demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM)
 
 - You can also check out this webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
@@ -146,16 +145,14 @@
 
 ## Contributing to OPAL
 
 - Pull requests are welcome! (please make sure to include _passing_ tests and docs)
 - Prior to submitting a PR - open an issue on GitHub, or make sure your PR addresses an existing issue well.
 
 [join-slack-link]: https://i.ibb.co/wzrGHQL/Group-749.png
-[badge-slack-link]: https://bit.ly/opalslack
+[badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
-License: Apache 2.0 Platform: UNKNOWN Classifier: Operating System :: OS
-Independent Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
+WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -35,21 +34,21 @@
 interaction or API call may affect access-control decisions. OPAL runs in the
 background, supercharging policy-agents, keeping them in sync with events in
 realtime. ## Documentation - ð   [Full documentation is available here]
 (https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
 started/intro) - ð   Getting Started: OPAL is available both as **python
 packages** with a built-in CLI as well as pre-built **docker images** ready-to-
 go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/get_started_with_opal_docker_compose_tutorial)  -
-[Try the getting started guide for containers](https://docs.opal.ac/getting-
-started/get_started_with_opal_using_docker)  - [Check out the Helm Chart for
-Kubernetes](https://github.com/permitio/opal-helm-chart) - A video demo of OPAL
-is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also
-check out this webinar and Q&A about OPAL [on our YouTube channel](https://
-www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
+docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
+getting started guide for containers](https://docs.opal.ac/getting-started/
+running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
+github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
+(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
+webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
+watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -76,12 +75,13 @@
 updates, and join our Slack community to chat about authorization, open-source,
 realtime communication, tech, or anything else!   If you are using our project,
 please consider giving us a â­ï¸  [![Button][join-slack-link]][badge-slack-
 link]  [![Button][follow-twitter-link]][badge-twitter-link] ## Contributing to
 OPAL - Pull requests are welcome! (please make sure to include _passing_ tests
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
-wzrGHQL/Group-749.png [badge-slack-link]: https://bit.ly/opalslack [follow-
-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-link]:
-https://twitter.com/opal_ac ## There's more! - Check out [OPToggles](https://
-github.com/permitio/OPToggles), which enables you to create user targeted
-feature flags/toggles based on Open Policy managed authorization rules!
+wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
+[follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
+link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
+(https://github.com/permitio/OPToggles), which enables you to create user
+targeted feature flags/toggles based on Open Policy managed authorization
+rules!
```

### Comparing `opal-common-0.5.0/opal_common/async_utils.py` & `opal-common-0.6.0/opal_common/async_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/authz.py` & `opal-common-0.6.0/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/casting.py` & `opal-common-0.6.0/opal_common/authentication/casting.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/deps.py` & `opal-common-0.6.0/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/signer.py` & `opal-common-0.6.0/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/tests/jwt_signer_test.py` & `opal-common-0.6.0/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/types.py` & `opal-common-0.6.0/opal_common/authentication/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/authentication/verifier.py` & `opal-common-0.6.0/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/cli/commands.py` & `opal-common-0.6.0/opal_common/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ),
     server_url: str = typer.Option(
         "http://localhost:7002", help="url of the OPAL-server to obtain the token from"
     ),
     type: PeerType = PeerType("client"),
     ttl: Tuple[int, str] = typer.Option(
         (365, "days"),
-        help="Time-To-Live / experation for the token in `<int> <str>` e.g. `365 days`, or `1000000 milliseconds` ",
+        help="Time-To-Live / expiration for the token in `<int> <str>` e.g. `365 days`, or `1000000 milliseconds` ",
     ),
     claims: str = typer.Option(
         "{}",
         help="claims to to include in the returned signed JWT as a JSON string",
         callback=lambda x: json.loads(x),
     ),
     just_the_token: bool = typer.Option(
```

### Comparing `opal-common-0.5.0/opal_common/cli/docs.py` & `opal-common-0.6.0/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/confi/cli.py` & `opal-common-0.6.0/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/confi/confi.py` & `opal-common-0.6.0/opal_common/confi/confi.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         # entries with delayed defaults (in addition to being referenced by self._entries)
         self._delayed_defaults: Dict[str, ConfiEntry] = OrderedDict()
 
         # get members by creation order
         members = sorted(
             inspect.getmembers(self, self._is_entry), key=self._get_entry_index
         )
-        # eval class entries into values (by order of defintion - same order as in the config class lines)
+        # eval class entries into values (by order of definition - same order as in the config class lines)
         for name, entry in members:
             # unwrap delayed entries
             if isinstance(entry, ConfiDelay):
                 entry = entry.eval(self)
 
             if isinstance(entry, ConfiEntry):
                 self._entries[name] = entry
```

### Comparing `opal-common-0.5.0/opal_common/confi/types.py` & `opal-common-0.6.0/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/corn_utils.py` & `opal-common-0.6.0/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/emport.py` & `opal-common-0.6.0/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/engine/base_fetching_engine.py` & `opal-common-0.6.0/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/engine/fetch_worker.py` & `opal-common-0.6.0/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/engine/fetching_engine.py` & `opal-common-0.6.0/opal_common/fetcher/engine/fetching_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ) -> None:
         # The internal task queue (created at start_workers)
         self._queue: asyncio.Queue = None
         # Worker working the queue
         self._tasks: List[asyncio.Task] = []
         # register of the fetch providers workers can use
         self._fetcher_register = FetcherRegister(register_config)
-        # core event callback regsiters
+        # core event callback registers
         self._failure_handlers: List[OnFetchFailureCallback] = []
         # how many workers to run
         self._worker_count: int = worker_count
         # time in seconds before timeout on a fetch callback
         self._callback_timeout = callback_timeout
         # time in seconds before time out on adding a task to queue (when full)
         self._enqueue_timeout = enqueue_timeout
@@ -97,15 +97,15 @@
         Raises:
             asyncio.TimeoutError: if the given timeout has expired
             also - @see self.queue_fetch_event
         """
         timeout = self._callback_timeout if timeout is None else timeout
         wait_event = asyncio.Event()
         data = {"result": None}
-        # Callback to wait and retrive data
+        # Callback to wait and retrieve data
 
         async def waiter_callback(answer):
             data["result"] = answer
             # Signal callback is done
             wait_event.set()
 
         await self.queue_url(url, waiter_callback, **kwargs)
```

### Comparing `opal-common-0.5.0/opal_common/fetcher/events.py` & `opal-common-0.6.0/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/fetch_provider.py` & `opal-common-0.6.0/opal_common/fetcher/fetch_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 logger = get_logger("opal.providers")
 
 
 class BaseFetchProvider:
     """Base class for data fetching providers.
 
     - Override self._fetch_ to implement fetching
-    - call self.fetch() to retrive data (wrapped in retries and safe execution guards)
+    - call self.fetch() to retrieve data (wrapped in retries and safe execution guards)
     - override __aenter__ and __aexit__ for async context
     """
 
     DEFAULT_RETRY_CONFIG = {
         "wait": wait.wait_random_exponential(),
         "stop": stop.stop_after_attempt(200),
         "reraise": True,
```

### Comparing `opal-common-0.5.0/opal_common/fetcher/fetcher_register.py` & `opal-common-0.6.0/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal-common-0.6.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/providers/http_fetch_provider.py` & `opal-common-0.6.0/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/tests/failure_handler_test.py` & `opal-common-0.6.0/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """Test callback on failure."""
     got_data_event = asyncio.Event()
     got_error = asyncio.Event()
 
     async with FetchingEngine() as engine:
         # callback to handle failure
         async def error_callback(error: Exception, event: FetchEvent):
-            # check we got the expection we expected
+            # check we got the exception we expected
             assert isinstance(error, aiohttp.client_exceptions.ClientConnectorError)
             got_error.set()
 
         # register the callback
         engine.register_failure_handler(error_callback)
         # callback for success - shouldn't eb called in this test
         async def callback(result):
```

### Comparing `opal-common-0.5.0/opal_common/fetcher/tests/http_fetch_test.py` & `opal-common-0.6.0/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal-common-0.6.0/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/git/branch_tracker.py` & `opal-common-0.6.0/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/git/bundle_maker.py` & `opal-common-0.6.0/opal_common/git/bundle_maker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/git/bundle_utils.py` & `opal-common-0.6.0/opal_common/git/bundle_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from opal_common.schemas.policy import DataModule, PolicyBundle, RegoModule
 
 
 class BundleUtils:
     MAX_INDEX = 10000
 
     @staticmethod
-    def sorted_policy_modules_to_load(bundle: PolicyBundle) -> List[RegoModule]:
+    def sorted_policy_modules_to_load(
+        bundle: PolicyBundle, ignore=None
+    ) -> List[RegoModule]:
         """policy modules sorted according to manifest."""
         manifest_paths = [Path(path) for path in bundle.manifest]
 
         def key_function(module: RegoModule) -> int:
             """this method reduces the module to a number that can be act as
             sorting key.
 
@@ -37,14 +39,18 @@
             except ValueError:
                 return BundleUtils.MAX_INDEX
 
         return sorted(bundle.data_modules, key=key_function)
 
     @staticmethod
     def sorted_policy_modules_to_delete(bundle: PolicyBundle) -> List[Path]:
+        if bundle.deleted_files is None:
+            return []
         # already sorted
         return bundle.deleted_files.policy_modules
 
     @staticmethod
     def sorted_data_modules_to_delete(bundle: PolicyBundle) -> List[Path]:
+        if bundle.deleted_files is None:
+            return []
         # already sorted
         return bundle.deleted_files.data_modules
```

### Comparing `opal-common-0.5.0/opal_common/git/commit_viewer.py` & `opal-common-0.6.0/opal_common/git/commit_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,19 +117,17 @@
     path.
 
     Returns the matched glob path rather than a binary decision of
     whether there is a match to enable better logging in the case of
     matched paths in manifests.
     """
     if bundle_ignore is not None:
-        path = Path(maybe_path)
-
-        for ignore in bundle_ignore:
-            if path.match(ignore):
-                return ignore
+        return PathUtils.glob_style_match_path_to_list(
+            Path(maybe_path).as_posix(), bundle_ignore
+        )
     return None
 
 
 def is_under_directories(f: VersionedFile, directories: Set[Path]) -> bool:
     """a filter on versioned files, filters only files under certain
     directories in the repo."""
     return PathUtils.is_child_of_directories(f.path, directories)
@@ -207,15 +205,16 @@
         Args:
             filter (Optional[DirectoryFilter]): an optional predicate to filter only specific directories.
 
         Yields:
             the next directory found (only for directories passing the filter).
         """
         return filter(
-            lambda node: isinstance(node, VersionedDirectory), self.nodes(predicate)
+            lambda node: isinstance(node, VersionedDirectory),
+            self.nodes(predicate),
         )
 
     def get_node(
         self, path: Path, filterable_gen: Optional[Callable] = None
     ) -> Optional[VersionedNode]:
         """Returns the node in the given path, None if it doesn't exist."""
         return next(self.nodes(lambda n: n.path == path), None)
```

### Comparing `opal-common-0.5.0/opal_common/git/diff_viewer.py` & `opal-common-0.6.0/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/git/env.py` & `opal-common-0.6.0/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/git/repo_cloner.py` & `opal-common-0.6.0/opal_common/git/repo_cloner.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             self._base_clone_path, f"{self._clone_subdirectory_prefix}-*"
         )
         for folder in folders_with_pattern:
             yield folder
 
     def _get_single_existing_random_clone_path(self) -> Optional[str]:
         """searches for the single randomly-suffixed clone subdirectory in
-        existance.
+        existence.
 
         If found no such subdirectory or if found more than one (multiple matching subdirectories) - will return None.
         otherwise: will return the single and only clone.
         """
         subdirectories = list(self._get_randomized_clone_subdirectories())
         if len(subdirectories) != 1:
             return None
```

### Comparing `opal-common-0.5.0/opal_common/git/tar_file_to_local_git_extractor.py` & `opal-common-0.6.0/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/logger.py` & `opal-common-0.6.0/opal_common/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,9 +45,9 @@
             rotation=opal_common_config.LOG_FILE_ROTATION,
             serialize=opal_common_config.LOG_FILE_SERIALIZE,
             level=opal_common_config.LOG_FILE_LEVEL,
         )
 
 
 def get_logger(name=""):
-    """backward comptability to old get_logger."""
+    """backward compatibility to old get_logger."""
     return logger
```

### Comparing `opal-common-0.5.0/opal_common/logging/filter.py` & `opal-common-0.6.0/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/logging/formatter.py` & `opal-common-0.6.0/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/logging/intercept.py` & `opal-common-0.6.0/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/logging/thirdparty.py` & `opal-common-0.6.0/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/middleware.py` & `opal-common-0.6.0/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/opa/parsing.py` & `opal-common-0.6.0/opal_common/opa/parsing.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/paths.py` & `opal-common-0.6.0/opal_common/paths.py`

 * *Files 22% similar despite different names*

```diff
@@ -70,11 +70,32 @@
             try:
                 # we look for Path objects and not str for normalization of the path
                 found_path: Path = unsorted.pop(unsorted.index(path))
                 sorted_paths.append(found_path)
             except ValueError:
                 continue  # skip, not found in the original list
 
-        # add the remaineder to the end of the sorted list
+        # add the remainder to the end of the sorted list
         sorted_paths.extend(unsorted)
 
         return sorted_paths
+
+    @staticmethod
+    def glob_style_match_path_to_list(path: str, match_paths: List[str]):
+        """
+        Check if given path matches any of the match_paths either via glob style matching or by being nested under - when the match path ends with "/**"
+        return the match path if there's a match, and None otherwise
+        """
+        # check if any of our ignore paths match the given path
+        for match_path in match_paths:
+            # if the path is indicated as a parent via "/**" at the end
+            if match_path.endswith("/**"):
+                # check if the path is under the parent
+                if path.startswith(match_path[:-3]):
+                    return match_path
+            # otherwise check for simple (non-recursive glob matching)
+            else:
+                path_object = Path(path)
+                if path_object.match(match_path):
+                    return match_path
+        # if no match - this path shouldn't be ignored
+        return None
```

### Comparing `opal-common-0.5.0/opal_common/schemas/data.py` & `opal-common-0.6.0/opal_common/schemas/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 JsonableValue = Union[Dict[str, Any], List[Any]]
 
 DEFAULT_DATA_TOPIC = "policy_data"
 
 
 class DataSourceEntry(BaseModel):
     """
-    Data source configuration - where client's should retrive data from and how they should store it
+    Data source configuration - where client's should retrieve data from and how they should store it
     """
 
     # How to obtain the data
     url: str = Field(..., description="Url source to query for data")
     data: Optional[JsonableValue] = Field(
         None,
         description="Data payload to embed within the data update (instead of having "
@@ -53,15 +53,15 @@
 
     Answers this question for the client: from where should i get the
     full picture of data i need? (as opposed to incremental data
     updates)
     """
 
     entries: List[DataSourceEntryWithPollingInterval] = Field(
-        ..., description="list of data sources and how to fetch from them"
+        [], description="list of data sources and how to fetch from them"
     )
 
 
 class ServerDataSourceConfig(BaseModel):
     """As its data source configuration, the server can either hold:
 
     1) A static DataSourceConfig returned to all clients regardless of identity.
@@ -150,13 +150,13 @@
     # Was the entry successfully saved into the policy-data-store
     saved: Optional[bool] = False
     # Hash of the returned data
     hash: Optional[str] = None
 
 
 class DataUpdateReport(BaseModel):
-    # the UUID fo the update this report is for
+    # the UUID of the update this report is for
     update_id: Optional[str] = None
     # Each DataSourceEntry and how it was processed
     reports: List[DataEntryReport]
     # in case this is a policy update, the new hash committed the policy store.
     policy_hash: Optional[str] = None
```

### Comparing `opal-common-0.5.0/opal_common/schemas/policy.py` & `opal-common-0.6.0/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/schemas/policy_source.py` & `opal-common-0.6.0/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/schemas/security.py` & `opal-common-0.6.0/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/schemas/store.py` & `opal-common-0.6.0/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/schemas/webhook.py` & `opal-common-0.6.0/opal_common/schemas/webhook.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,7 +35,11 @@
         default=None,
         description="The JSON object key holding the event information (used instead of event_header_name)",
     )
     push_event_value: str = Field(
         ...,
         description="The event value indicating a Git push",
     )
+    match_sender_url: bool = Field(
+        True,
+        description="Should OPAL verify that the sender url matches the tracked repo URL, and drop the webhook request otherwise?",
+    )
```

### Comparing `opal-common-0.5.0/opal_common/security/sslcontext.py` & `opal-common-0.6.0/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/security/tarsafe.py` & `opal-common-0.6.0/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/sources/api_policy_source.py` & `opal-common-0.6.0/opal_common/sources/api_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/sources/base_policy_source.py` & `opal-common-0.6.0/opal_common/sources/base_policy_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         """optional task to periodically check the remote for changes (git pull
         and compare hash)."""
         while True:
             try:
                 await polling_task()
             except Exception as ex:
                 logger.error(
-                    "Error occured during polling task {task}: {err}",
+                    "Error occurred during polling task {task}: {err}",
                     task=polling_task.__name__,
                     err=ex,
                 )
             await asyncio.sleep(self._polling_interval)
 
     async def _stop_polling_task(self):
         if self._polling_task is not None:
```

### Comparing `opal-common-0.5.0/opal_common/sources/git_policy_source.py` & `opal-common-0.6.0/opal_common/sources/git_policy_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Args:
         remote_source_url(str): the base address to request the policy from
         local_clone_path(str):  path for the local git to manage policies
         branch_name(str):  name of remote branch in git to pull, default to master
         ssh_key (str, optional): private ssh key used to gain access to the cloned repo
         polling_interval(int):  how many seconds need to wait between polling
-        request_timeout(int):  how many seconds need to wait until timout
+        request_timeout(int):  how many seconds need to wait until timeout
     """
 
     def __init__(
         self,
         remote_source_url: str,
         local_clone_path: str,
         branch_name: str = "master",
```

### Comparing `opal-common-0.5.0/opal_common/synchronization/expiring_redis_lock.py` & `opal-common-0.6.0/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/synchronization/named_lock.py` & `opal-common-0.6.0/opal_common/synchronization/named_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from opal_common.logger import logger
 
 DEFAULT_LOCK_ATTEMPT_INTERVAL = 5.0
 
 
 class NamedLock:
     """creates a a file-lock (can be a normal file or a named pipe / fifo), and
-    exposes a context manager to try to acquire the lock asyncronously."""
+    exposes a context manager to try to acquire the lock asynchronously."""
 
     def __init__(
         self, path: str, attempt_interval: float = DEFAULT_LOCK_ATTEMPT_INTERVAL
     ):
         self._lock_file: str = path
         self._lock_file_fd = None
         self._attempt_interval = attempt_interval
```

### Comparing `opal-common-0.5.0/opal_common/tests/path_utils_test.py` & `opal-common-0.6.0/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/tests/url_utils_test.py` & `opal-common-0.6.0/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/topics/listener.py` & `opal-common-0.6.0/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/topics/publisher.py` & `opal-common-0.6.0/opal_common/topics/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,17 @@
             try:
                 await self._task
             except asyncio.CancelledError:
                 pass
             self._task = None
             logger.info(f"cancelled {self._task_name} to topic: {self._topic}")
 
+    async def wait_until_done(self):
+        await self._task
+
     async def _publish_task(self):
         while True:
             await asyncio.sleep(self._interval)
             logger.info(
                 f"{self._task_name}: publishing message on topic '{self._topic}', next publish is scheduled in {self._interval} seconds"
             )
             self._publisher.publish(topics=[self._topic], data=self._message)
```

### Comparing `opal-common-0.5.0/opal_common/topics/utils.py` & `opal-common-0.6.0/opal_common/topics/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 def pubsub_topics_from_directories(dirs: List[str]) -> List[str]:
     """converts a list of directories on the policy repository that the client
     wants to subscribe to into a list of topics.
 
     this method also ensures the client only subscribes to non-
     intersecting directories by dedupping directories that are
-    decendents of one another.
+    descendents of one another.
     """
     policy_directories = PathUtils.non_intersecting_directories([Path(d) for d in dirs])
     return policy_topics(policy_directories)
```

### Comparing `opal-common-0.5.0/opal_common/urls.py` & `opal-common-0.6.0/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common/utils.py` & `opal-common-0.6.0/opal_common/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/opal_common.egg-info/PKG-INFO` & `opal-common-0.6.0/opal_common.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -77,17 +76,17 @@
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
 
-  - [Play with a live playground environment in docker-compose](https://docs.opal.ac/getting-started/get_started_with_opal_docker_compose_tutorial)
+  - [Play with a live playground environment in docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-playground/overview)
   <!-- - this tutorial is great for learning about OPAL core features and see what OPAL can do for you. -->
-  - [Try the getting started guide for containers](https://docs.opal.ac/getting-started/get_started_with_opal_using_docker)
+  - [Try the getting started guide for containers](https://docs.opal.ac/getting-started/running-opal/overview)
   <!-- - this tutorial will show you how to configure OPAL to your specific needs and run the official docker containers locally or in production. -->
 
   - [Check out the Helm Chart for Kubernetes](https://github.com/permitio/opal-helm-chart)
 
 - A video demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM)
 
 - You can also check out this webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
@@ -146,16 +145,14 @@
 
 ## Contributing to OPAL
 
 - Pull requests are welcome! (please make sure to include _passing_ tests and docs)
 - Prior to submitting a PR - open an issue on GitHub, or make sure your PR addresses an existing issue well.
 
 [join-slack-link]: https://i.ibb.co/wzrGHQL/Group-749.png
-[badge-slack-link]: https://bit.ly/opalslack
+[badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: opal-common Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
-License: Apache 2.0 Platform: UNKNOWN Classifier: Operating System :: OS
-Independent Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
+WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -35,21 +34,21 @@
 interaction or API call may affect access-control decisions. OPAL runs in the
 background, supercharging policy-agents, keeping them in sync with events in
 realtime. ## Documentation - ð   [Full documentation is available here]
 (https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
 started/intro) - ð   Getting Started: OPAL is available both as **python
 packages** with a built-in CLI as well as pre-built **docker images** ready-to-
 go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/get_started_with_opal_docker_compose_tutorial)  -
-[Try the getting started guide for containers](https://docs.opal.ac/getting-
-started/get_started_with_opal_using_docker)  - [Check out the Helm Chart for
-Kubernetes](https://github.com/permitio/opal-helm-chart) - A video demo of OPAL
-is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also
-check out this webinar and Q&A about OPAL [on our YouTube channel](https://
-www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
+docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
+getting started guide for containers](https://docs.opal.ac/getting-started/
+running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
+github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
+(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
+webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
+watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -76,12 +75,13 @@
 updates, and join our Slack community to chat about authorization, open-source,
 realtime communication, tech, or anything else!   If you are using our project,
 please consider giving us a â­ï¸  [![Button][join-slack-link]][badge-slack-
 link]  [![Button][follow-twitter-link]][badge-twitter-link] ## Contributing to
 OPAL - Pull requests are welcome! (please make sure to include _passing_ tests
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
-wzrGHQL/Group-749.png [badge-slack-link]: https://bit.ly/opalslack [follow-
-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-link]:
-https://twitter.com/opal_ac ## There's more! - Check out [OPToggles](https://
-github.com/permitio/OPToggles), which enables you to create user targeted
-feature flags/toggles based on Open Policy managed authorization rules!
+wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
+[follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
+link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
+(https://github.com/permitio/OPToggles), which enables you to create user
+targeted feature flags/toggles based on Open Policy managed authorization
+rules!
```

### Comparing `opal-common-0.5.0/opal_common.egg-info/SOURCES.txt` & `opal-common-0.6.0/opal_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-common-0.5.0/setup.py` & `opal-common-0.6.0/setup.py`

 * *Files identical despite different names*

