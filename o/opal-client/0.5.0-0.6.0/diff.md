# Comparing `tmp/opal-client-0.5.0.tar.gz` & `tmp/opal-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.5.0.tar", last modified: Mon Feb 27 17:27:12 2023, max compression
+gzip compressed data, was "opal-client-0.6.0.tar", last modified: Fri Apr 21 07:57:01 2023, max compression
```

## Comparing `opal-client-0.5.0.tar` & `opal-client-0.6.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.063235 opal-client-0.5.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8496 2023-02-27 17:27:12.063032 opal-client-0.5.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.057492 opal-client-0.5.0/opal_client/
--rw-r--r--   0 asafc      (501) staff       (20)       31 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.058793 opal-client-0.5.0/opal_client/callbacks/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/callbacks/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     3034 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/callbacks/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4329 2022-12-02 16:23:06.000000 opal-client-0.5.0/opal_client/callbacks/register.py
--rw-r--r--   0 asafc      (501) staff       (20)     2959 2022-12-02 16:23:03.000000 opal-client-0.5.0/opal_client/callbacks/reporter.py
--rw-r--r--   0 asafc      (501) staff       (20)     2184 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    14691 2022-12-02 16:02:32.000000 opal-client-0.5.0/opal_client/client.py
--rw-r--r--   0 asafc      (501) staff       (20)     8254 2023-02-24 20:59:56.000000 opal-client-0.5.0/opal_client/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.059604 opal-client-0.5.0/opal_client/data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      863 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/data/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4286 2022-10-12 14:50:19.000000 opal-client-0.5.0/opal_client/data/fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)      842 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/data/rpc.py
--rw-r--r--   0 asafc      (501) staff       (20)    19102 2023-02-24 20:59:56.000000 opal-client-0.5.0/opal_client/data/updater.py
--rw-r--r--   0 asafc      (501) staff       (20)     2220 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/limiter.py
--rw-r--r--   0 asafc      (501) staff       (20)       33 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)       96 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/main.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.060282 opal-client-0.5.0/opal_client/opa/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/opa/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.060519 opal-client-0.5.0/opal_client/opa/healthcheck/
--rw-r--r--   0 asafc      (501) staff       (20)     1123 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/opa/healthcheck/opal.rego
--rw-r--r--   0 asafc      (501) staff       (20)     3047 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/opa/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3144 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/opa/options.py
--rw-r--r--   0 asafc      (501) staff       (20)     8116 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/opa/runner.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.061384 opal-client-0.5.0/opal_client/policy/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      501 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     4968 2023-02-01 11:46:28.000000 opal-client-0.5.0/opal_client/policy/fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)     1797 2023-02-01 11:46:28.000000 opal-client-0.5.0/opal_client/policy/options.py
--rw-r--r--   0 asafc      (501) staff       (20)      596 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy/topics.py
--rw-r--r--   0 asafc      (501) staff       (20)    13407 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy/updater.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.062449 opal-client-0.5.0/opal_client/policy_store/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1248 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     9073 2022-10-12 14:50:19.000000 opal-client-0.5.0/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     2522 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 asafc      (501) staff       (20)    22629 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/opa_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     3625 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 asafc      (501) staff       (20)     1134 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.062813 opal-client-0.5.0/opal_client/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7281 2023-02-01 11:46:28.000000 opal-client-0.5.0/opal_client/tests/data_updater_test.py
--rw-r--r--   0 asafc      (501) staff       (20)     4414 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 asafc      (501) staff       (20)      322 2022-10-01 21:13:25.000000 opal-client-0.5.0/opal_client/utils.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.058205 opal-client-0.5.0/opal_client.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8496 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1408 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       67 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 asafc      (501) staff       (20)      404 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-02-27 17:27:12.000000 opal-client-0.5.0/opal_client.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-02-27 17:27:12.063271 opal-client-0.5.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2831 2022-10-01 21:13:25.000000 opal-client-0.5.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.692385 opal-client-0.6.0/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-04-21 07:57:01.692177 opal-client-0.6.0/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.683687 opal-client-0.6.0/opal_client/
+-rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.684985 opal-client-0.6.0/opal_client/callbacks/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/callbacks/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/callbacks/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.6.0/opal_client/callbacks/register.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/callbacks/reporter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2184 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    18405 2023-04-19 15:20:19.000000 opal-client-0.6.0/opal_client/client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10106 2023-04-20 15:05:49.000000 opal-client-0.6.0/opal_client/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.685579 opal-client-0.6.0/opal_client/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4286 2022-12-08 13:45:19.000000 opal-client-0.6.0/opal_client/data/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/data/rpc.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    19105 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/data/updater.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/limiter.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.686112 opal-client-0.6.0/opal_client/opa/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.686238 opal-client-0.6.0/opal_client/opa/healthcheck/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1123 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/healthcheck/opal.rego
+-rw-r--r--   0 roekatz    (501) staff       (20)     3047 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3144 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/opa/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8116 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/opa/runner.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.687993 opal-client-0.6.0/opal_client/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-01-19 13:43:15.000000 opal-client-0.6.0/opal_client/policy/fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-01-19 13:43:15.000000 opal-client-0.6.0/opal_client/policy/options.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy/topics.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13408 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/policy/updater.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.689461 opal-client-0.6.0/opal_client/policy_store/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/policy_store/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-03-12 10:36:51.000000 opal-client-0.6.0/opal_client/policy_store/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     8610 2023-04-19 15:20:19.000000 opal-client-0.6.0/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2518 2023-03-27 20:28:44.000000 opal-client-0.6.0/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    31778 2023-04-20 15:05:49.000000 opal-client-0.6.0/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5301 2023-03-27 20:28:44.000000 opal-client-0.6.0/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1795 2023-03-12 10:36:51.000000 opal-client-0.6.0/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.691938 opal-client-0.6.0/opal_client/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/tests/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1960 2023-04-19 08:36:33.000000 opal-client-0.6.0/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-03-27 15:01:56.000000 opal-client-0.6.0/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.6.0/opal_client/utils.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:01.684494 opal-client-0.6.0/opal_client.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1445 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      401 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-04-21 07:57:01.000000 opal-client-0.6.0/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-04-21 07:57:01.692428 opal-client-0.6.0/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2831 2022-12-08 13:40:17.000000 opal-client-0.6.0/setup.py
```

### Comparing `opal-client-0.5.0/PKG-INFO` & `opal-client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
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
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
-Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Platform:
-UNKNOWN Classifier: Operating System :: OS Independent Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
-:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
+Operating System :: OS Independent Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
+:: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-
+Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -36,21 +36,21 @@
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
@@ -77,12 +77,13 @@
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

### Comparing `opal-client-0.5.0/opal_client/callbacks/api.py` & `opal-client-0.6.0/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/callbacks/register.py` & `opal-client-0.6.0/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/callbacks/reporter.py` & `opal-client-0.6.0/opal_client/callbacks/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,8 +63,8 @@
                     logger.error(
                         "Failed to send report to {url}, got response code {status} with error: {error}",
                         url=url,
                         status=result.status,
                         error=error_content,
                     )
         except:
-            logger.exception("Failed to excute report_update_results")
+            logger.exception("Failed to execute report_update_results")
```

### Comparing `opal-client-0.5.0/opal_client/cli.py` & `opal-client-0.6.0/opal_client/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from opal_common.corn_utils import run_gunicorn, run_uvicorn
 
 app = get_typer_app()
 
 
 @app.command()
 def run(engine_type: str = typer.Option("uvicron", help="uvicorn or gunicorn")):
-    """Run the client as a deamon."""
+    """Run the client as a daemon."""
     typer.echo(f"-- Starting OPAL client (with {engine_type}) --")
 
     if engine_type == "gunicorn":
         app: FastAPI
         from opal_client.main import app
 
         run_gunicorn(
```

### Comparing `opal-client-0.5.0/opal_client/client.py` & `opal-client-0.6.0/opal_client/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import functools
 import os
 import signal
 import uuid
 from logging import disable
 from typing import List, Optional
 
+import aiofiles
+import aiofiles.os
 import aiohttp
 import websockets
 from fastapi import FastAPI, status
 from fastapi.responses import JSONResponse
 from opal_client.callbacks.api import init_callbacks_api
 from opal_client.callbacks.register import CallbacksRegister
 from opal_client.config import PolicyStoreTypes, opal_client_config
@@ -41,14 +43,17 @@
         policy_store: BasePolicyStoreClient = None,
         data_updater: DataUpdater = None,
         data_topics: List[str] = None,
         policy_updater: PolicyUpdater = None,
         inline_opa_enabled: bool = None,
         inline_opa_options: OpaServerOptions = None,
         verifier: Optional[JWTVerifier] = None,
+        store_backup_path: Optional[str] = None,
+        store_backup_interval: Optional[int] = None,
+        offline_mode_enabled: bool = False,
     ) -> None:
         """
         Args:
             policy_store_type (PolicyStoreTypes, optional): [description]. Defaults to POLICY_STORE_TYPE.
 
             Internal components (for each pass None for default init, or False to disable):
                 policy_store (BasePolicyStoreClient, optional): The policy store client. Defaults to None.
@@ -164,14 +169,30 @@
                 audience=opal_common_config.AUTH_JWT_AUDIENCE,
                 issuer=opal_common_config.AUTH_JWT_ISSUER,
             )
         if not self.verifier.enabled:
             logger.info(
                 "API authentication disabled (public encryption key was not provided)"
             )
+        self.store_backup_path = (
+            store_backup_path or opal_client_config.STORE_BACKUP_PATH
+        )
+        self.store_backup_interval = (
+            store_backup_interval or opal_client_config.STORE_BACKUP_INTERVAL
+        )
+
+        self.offline_mode_enabled = (
+            offline_mode_enabled or opal_client_config.OFFLINE_MODE_ENABLED
+        )
+        if self.offline_mode_enabled and not inline_opa_enabled:
+            logger.warning(
+                "Offline mode was enabled, but isn't supported when using an external policy store (inline OPA is disabled)"
+            )
+            self.offline_mode_enabled = False
+        self._backup_loaded = False
 
         # init fastapi app
         self.app: FastAPI = self._init_fast_api_app()
 
     def _init_fast_api_app(self):
         """inits the fastapi app object."""
         app = FastAPI(
@@ -203,28 +224,45 @@
         app.include_router(data_router, tags=["Data Updater"])
         app.include_router(policy_store_router, tags=["Policy Store"])
         app.include_router(callbacks_router, tags=["Callbacks"])
 
         # top level routes (i.e: healthchecks)
         @app.get("/healthcheck", include_in_schema=False)
         @app.get("/", include_in_schema=False)
-        async def healthcheck():
-            resp = await self.policy_store.get_data("/system/opal/healthy")
-            healthy = resp["result"]
+        @app.get("/healthy", include_in_schema=False)
+        async def healthy():
+            """returns 200 if updates keep being successfully fetched from the
+            server and applied to the policy store."""
+            healthy = await self.policy_store.is_healthy()
 
             if healthy:
                 return JSONResponse(
                     status_code=status.HTTP_200_OK, content={"status": "ok"}
                 )
             else:
                 return JSONResponse(
                     status_code=status.HTTP_503_SERVICE_UNAVAILABLE,
                     content={"status": "unavailable"},
                 )
 
+        @app.get("/ready", include_in_schema=False)
+        async def ready():
+            """returns 200 if the policy store is ready to serve requests."""
+            ready = self._backup_loaded or await self.policy_store.is_ready()
+
+            if ready:
+                return JSONResponse(
+                    status_code=status.HTTP_200_OK, content={"status": "ok"}
+                )
+            else:
+                return JSONResponse(
+                    status_code=status.HTTP_503_SERVICE_UNAVAILABLE,
+                    content={"status": "unavailable"},
+                )
+
         return app
 
     def _configure_lifecycle_callbacks(self, app: FastAPI):
         """registers callbacks on app startup and shutdown.
 
         on app startup we launch our long running processes (async
         tasks) on the event loop. on app shutdown we stop these long
@@ -233,14 +271,17 @@
 
         @app.on_event("startup")
         async def startup_event():
             asyncio.create_task(self.start_client_background_tasks())
 
         @app.on_event("shutdown")
         async def shutdown_event():
+            if self.offline_mode_enabled:
+                await self.backup_store()
+
             await self.stop_client_background_tasks()
 
         return app
 
     async def start_client_background_tasks(self):
         """Launch OPAL client long-running tasks:
 
@@ -282,22 +323,67 @@
             tasks.append(asyncio.create_task(self.policy_updater.stop()))
 
         try:
             await asyncio.gather(*tasks)
         except Exception:
             logger.exception("exception while shutting down updaters")
 
+    async def load_store_from_backup(self):
+        """Imports the backup file, if exists, to the policy store."""
+        try:
+            if os.path.isfile(self.store_backup_path):
+                async with aiofiles.open(self.store_backup_path, "r") as backup_file:
+                    logger.debug("importing policy store from backup file...")
+                    await self.policy_store.full_import(backup_file)
+                    logger.debug("import completed")
+                    self._backup_loaded = True
+            else:
+                logger.warning("policy store backup file wasn't found")
+        except Exception:
+            logger.exception("failed to load backup data to policy store")
+
+    async def backup_store(self):
+        """Exports the policy store's data to a backup file."""
+        try:
+            async with self._backup_lock:
+                await aiofiles.os.makedirs(
+                    os.path.dirname(self.store_backup_path), exist_ok=True
+                )
+                tmp_backup_path = self.store_backup_path + ".tmp"
+                async with aiofiles.open(tmp_backup_path, "w") as backup_file:
+                    logger.debug("exporting policy store to backup file...")
+                    await self.policy_store.full_export(backup_file)
+                    logger.debug("export completed")
+
+                # Atomically replace the previous backup (only after the new one is ready)
+                await aiofiles.os.replace(tmp_backup_path, self.store_backup_path)
+        except Exception:
+            logger.exception("failed to backup policy store")
+
+    async def periodically_backup_store(self):
+        self._backup_lock = asyncio.Lock()
+
+        # Backup store periodically
+        while True:
+            await asyncio.sleep(self.store_backup_interval)
+            await self.backup_store()
+
     async def launch_policy_store_dependent_tasks(self):
         try:
             await self.maybe_init_healthcheck_policy()
         except Exception:
             logger.critical("healthcheck policy enabled but could not be initialized!")
             self._trigger_shutdown()
             return
 
+        if self.offline_mode_enabled:
+            # Immediately attempt loading from backup (waiting for failure loading from server would delay availability)
+            await self.load_store_from_backup()
+            asyncio.create_task(self.periodically_backup_store())
+
         try:
             for task in asyncio.as_completed(
                 [self.launch_policy_updater(), self.launch_data_updater()]
             ):
                 await task
         except websockets.exceptions.InvalidStatusCode as err:
             logger.error("Failed to launch background task -- {err}", err=repr(err))
@@ -332,15 +418,14 @@
             )
             raise
 
         try:
             await self.policy_store.init_healthcheck_policy(
                 policy_id=healthcheck_policy_relpath,
                 policy_code=healthcheck_policy_code,
-                data_updater_enabled=opal_client_config.DATA_UPDATER_ENABLED,
             )
         except aiohttp.ClientError as err:
             logger.error(
                 "Failed to connect to OPA agent while init healthcheck policy -- {err}",
                 err=repr(err),
             )
             raise
```

### Comparing `opal-client-0.5.0/opal_client/config.py` & `opal-client-0.6.0/opal_client/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 from opal_client.opa.options import OpaServerOptions
 from opal_client.policy.options import PolicyConnRetryOptions
-from opal_client.policy_store.schemas import PolicyStoreTypes
+from opal_client.policy_store.schemas import PolicyStoreAuth, PolicyStoreTypes
 from opal_common.confi import Confi, confi
 from opal_common.config import opal_common_config
 from opal_common.fetcher.providers.http_fetch_provider import HttpFetcherConfig
 from opal_common.schemas.data import DEFAULT_DATA_TOPIC, UpdateCallback
 
 
 # Opal Client general configuration -------------------------------------------
@@ -18,20 +18,41 @@
 
 
 class OpalClientConfig(Confi):
     # opa client (policy store) configuration
     POLICY_STORE_TYPE = confi.enum(
         "POLICY_STORE_TYPE", PolicyStoreTypes, PolicyStoreTypes.OPA
     )
-    POLICY_STORE_URL = confi.str("POLICY_STORE_URL", f"http://localhost:8181")
+    POLICY_STORE_URL = confi.str("POLICY_STORE_URL", "http://localhost:8181")
+
+    POLICY_STORE_AUTH_TYPE = confi.enum(
+        "POLICY_STORE_AUTH_TYPE", PolicyStoreAuth, PolicyStoreAuth.NONE
+    )
     POLICY_STORE_AUTH_TOKEN = confi.str(
         "POLICY_STORE_AUTH_TOKEN",
         None,
-        description="the authentication (bearer) token OPAL client will use to authenticate against the policy store (i.e: OPA agent)",
+        description="the authentication (bearer) token OPAL client will use to "
+        "authenticate against the policy store (i.e: OPA agent).",
+    )
+    POLICY_STORE_AUTH_OAUTH_SERVER = confi.str(
+        "POLICY_STORE_AUTH_OAUTH_SERVER",
+        None,
+        description="the authentication server OPAL client will use to authenticate against for retrieving the access_token.",
+    )
+    POLICY_STORE_AUTH_OAUTH_CLIENT_ID = confi.str(
+        "POLICY_STORE_AUTH_OAUTH_CLIENT_ID",
+        None,
+        description="the client_id OPAL will use to authenticate against the OAuth server.",
+    )
+    POLICY_STORE_AUTH_OAUTH_CLIENT_SECRET = confi.str(
+        "POLICY_STORE_AUTH_OAUTH_CLIENT_SECRET",
+        None,
+        description="the client secret OPAL will use to authenticate against the OAuth server.",
     )
+
     POLICY_STORE_CONN_RETRY: PolicyConnRetryOptions = confi.model(
         "POLICY_STORE_CONN_RETRY",
         PolicyConnRetryOptions,
         # defaults are being set according to PolicyStoreConnRetryOptions pydantic definitions (see class)
         {},
         description="retry options when connecting to the policy store (i.e. the agent that handles the policy, e.g. OPA)",
     )
@@ -43,14 +64,20 @@
             "max_wait": 10,
             "attempts": 5,
             "wait_time": 1,
         },
         description="retry options when connecting to the policy source (e.g. the policy bundle server)",
     )
 
+    POLICY_STORE_POLICY_PATHS_TO_IGNORE = confi.list(
+        "POLICY_STORE_POLICY_PATHS_TO_IGNORE",
+        [],
+        description="When loading policies manually or otherwise externally into the policy store, use this list of glob patterns to have OPAL ignore and not delete or override them, end paths (without any wildcards in the middle) with '\**' to indicate you want all nested under the path to be ignored",
+    )
+
     # create an instance of a policy store upon load
     def load_policy_store():
         from opal_client.policy_store.policy_store_client_factory import (
             PolicyStoreClientFactory,
         )
 
         return PolicyStoreClientFactory.create()
@@ -140,15 +167,16 @@
         description="directories in policy repo we should subscribe to",
     )
 
     # Data updater configuration --------------------------------------------------
     DATA_UPDATER_ENABLED = confi.bool(
         "DATA_UPDATER_ENABLED",
         True,
-        description="If set to False, opal client will not listen to dynamic data updates. Dynamic data fetching will be completely disabled.",
+        description="If set to False, opal client will not listen to dynamic data updates. "
+        "Dynamic data fetching will be completely disabled.",
     )
 
     DATA_TOPICS = confi.list(
         "DATA_TOPICS",
         [DEFAULT_DATA_TOPIC],
         description="Data topics to subscribe to",
     )
@@ -164,15 +192,16 @@
         "http://localhost:8000/policy-config",
         description="Default URL to fetch data from",
     )
 
     SHOULD_REPORT_ON_DATA_UPDATES = confi.bool(
         "SHOULD_REPORT_ON_DATA_UPDATES",
         False,
-        description="Should the client report on updates to callbacks defined in DEFAULT_UPDATE_CALLBACKS or within the given updates",
+        description="Should the client report on updates to callbacks defined in "
+        "DEFAULT_UPDATE_CALLBACKS or within the given updates",
     )
     DEFAULT_UPDATE_CALLBACK_CONFIG = confi.model(
         "DEFAULT_UPDATE_CALLBACK_CONFIG",
         HttpFetcherConfig,
         {
             "method": "post",
             "headers": {"content-type": "application/json"},
@@ -209,14 +238,30 @@
         description="Unique client statistics identifier",
     )
 
     OPA_HEALTH_CHECK_POLICY_PATH = "opa/healthcheck/opal.rego"
 
     SCOPE_ID = confi.str("SCOPE_ID", "default", description="OPAL Scope ID")
 
+    STORE_BACKUP_PATH = confi.str(
+        "STORE_BACKUP_PATH",
+        "/opal/backup/opa.json",
+        description="Path to backup policy store's data to",
+    )
+    STORE_BACKUP_INTERVAL = confi.int(
+        "STORE_BACKUP_INTERVAL",
+        60,
+        description="Interval in seconds to backup policy store's data",
+    )
+    OFFLINE_MODE_ENABLED = confi.bool(
+        "OFFLINE_MODE_ENABLED",
+        False,
+        description="If set, opal client will try to load policy store from backup file and operate even if server is unreachable. Ignored if INLINE_OPA_ENABLED=False",
+    )
+
     def on_load(self):
         # LOGGER
         if self.INLINE_OPA_LOG_FORMAT == OpaLogFormat.NONE:
             opal_common_config.LOG_MODULE_EXCLUDE_LIST.append("opal_client.opa.logger")
             # re-assign to apply to internal confi-entries as well
             opal_common_config.LOG_MODULE_EXCLUDE_LIST = (
                 opal_common_config.LOG_MODULE_EXCLUDE_LIST
```

### Comparing `opal-client-0.5.0/opal_client/data/api.py` & `opal-client-0.6.0/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/data/fetcher.py` & `opal-client-0.6.0/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/data/rpc.py` & `opal-client-0.6.0/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/data/updater.py` & `opal-client-0.6.0/opal_client/data/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         data configuration on startup from OPAL-server Uses Pub/Sub to
         subscribe to data update events, and fetches (using FetchingEngine)
         data from sources.
 
         Args:
             token (str, optional): Auth token to include in connections to OPAL server. Defaults to CLIENT_TOKEN.
             pubsub_url (str, optional): URL for Pub/Sub updates for data. Defaults to OPAL_SERVER_PUBSUB_URL.
-            data_sources_config_url (str, optional): URL to retrive base data configuration. Defaults to DEFAULT_DATA_SOURCES_CONFIG_URL.
+            data_sources_config_url (str, optional): URL to retrieve base data configuration. Defaults to DEFAULT_DATA_SOURCES_CONFIG_URL.
             fetch_on_connect (bool, optional): Should the update fetch basic data immediately upon connection/reconnection. Defaults to True.
             data_topics (List[str], optional): Topics of data to fetch and subscribe to. Defaults to DATA_TOPICS.
             policy_store (BasePolicyStoreClient, optional): Policy store client to use to store data. Defaults to DEFAULT_POLICY_STORE.
         """
         # Defaults
         token: str = token or opal_client_config.CLIENT_TOKEN
         pubsub_url: str = pubsub_url or opal_client_config.SERVER_PUBSUB_URL
@@ -184,15 +184,15 @@
     async def get_base_policy_data(
         self, config_url: str = None, data_fetch_reason="Initial load"
     ):
         """Load data into the policy store according to the data source's
         config provided in the config URL.
 
         Args:
-            config_url (str, optional): URL to retrive data sources config from. Defaults to None ( self._data_sources_config_url).
+            config_url (str, optional): URL to retrieve data sources config from. Defaults to None ( self._data_sources_config_url).
             data_fetch_reason (str, optional): Reason to log for the update operation. Defaults to "Initial load".
         """
         logger.info(
             "Performing data configuration, reason: {reason}", reason=data_fetch_reason
         )
         sources_config = await self.get_policy_data_config(url=config_url)
         # translate config to a data update
@@ -339,15 +339,15 @@
         # Urls may be None - handle_urls has a default for None
         policy_data_with_urls = await data_fetcher.handle_urls(urls)
         # Save the data from the update
         # We wrap our interaction with the policy store with a transaction
         async with policy_store.transaction_context(
             update.id, transaction_type=TransactionType.data
         ) as store_transaction:
-            # for intelisense treat store_transaction as a PolicyStoreClient (which it proxies)
+            # for intellisense treat store_transaction as a PolicyStoreClient (which it proxies)
             store_transaction: BasePolicyStoreClient
             error_content = None
             for (url, fetch_config, result), entry in itertools.zip_longest(
                 policy_data_with_urls, entries
             ):
                 fetched_data_successfully = True
```

### Comparing `opal-client-0.5.0/opal_client/limiter.py` & `opal-client-0.6.0/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/opa/healthcheck/opal.rego` & `opal-client-0.6.0/opal_client/opa/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/opa/logger.py` & `opal-client-0.6.0/opal_client/opa/logger.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/opa/options.py` & `opal-client-0.6.0/opal_client/opa/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/opa/runner.py` & `opal-client-0.6.0/opal_client/opa/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         rehydration_callbacks: Optional[List[AsyncCallback]] = None,
     ):
         """factory for OpaRunner, accept optional callbacks to run in certain
         lifecycle events.
 
         Initial Start Callbacks:
             The first time we start opa, we might want to do certain actions (like launch tasks)
-            that are dependant on the policy store being up (such as PolicyUpdater, DataUpdater).
+            that are dependent on the policy store being up (such as PolicyUpdater, DataUpdater).
 
         Rehydration Callbacks:
             when opa restarts, its cache is clean and it does not have the state necessary
             to handle authorization queries. therefore it is necessary that we rehydrate the
             cache with fresh state fetched from the server.
         """
         opa_runner = OpaRunner(options=options, piped_logs_format=piped_logs_format)
```

### Comparing `opal-client-0.5.0/opal_client/policy/fetcher.py` & `opal-client-0.6.0/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/policy/options.py` & `opal-client-0.6.0/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/policy/topics.py` & `opal-client-0.6.0/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.5.0/opal_client/policy/updater.py` & `opal-client-0.6.0/opal_client/policy/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             self._topics = pubsub_topics_from_directories(
                 self._subscription_directories
             )
         else:
             self._topics = [f"{self._scope_id}:policy:."]
         # The pub/sub client for data updates
         self._client = None
-        # The task running the Pub/Sub subcribing client
+        # The task running the Pub/Sub subscribing client
         self._subscriber_task = None
         self._stopping = False
         # policy fetcher - fetches policy bundles
         self._policy_fetcher = PolicyFetcher()
         # callbacks on policy changes
         self._data_fetcher = data_fetcher or DataFetcher()
         self._callbacks_register = callbacks_register or CallbacksRegister()
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/api.py` & `opal-client-0.6.0/opal_client/policy_store/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from fastapi import APIRouter, Depends
 from opal_client.config import opal_client_config
-from opal_client.policy_store.schemas import PolicyStoreDetails
+from opal_client.policy_store.schemas import PolicyStoreAuth, PolicyStoreDetails
 from opal_common.authentication.authz import require_peer_type
 from opal_common.authentication.deps import JWTAuthenticator
 from opal_common.authentication.types import JWTClaims
 from opal_common.authentication.verifier import Unauthorized
 from opal_common.logger import logger
 from opal_common.schemas.security import PeerType
 
@@ -25,10 +25,16 @@
         except Unauthorized as e:
             logger.error(f"Unauthorized to publish update: {repr(e)}")
             raise
 
         return PolicyStoreDetails(
             url=opal_client_config.POLICY_STORE_URL,
             token=opal_client_config.POLICY_STORE_AUTH_TOKEN or None,
+            auth_type=opal_client_config.POLICY_STORE_AUTH_TYPE or PolicyStoreAuth.NONE,
+            oauth_client_id=opal_client_config.POLICY_STORE_AUTH_OAUTH_CLIENT_ID
+            or None,
+            oauth_client_secret=opal_client_config.POLICY_STORE_AUTH_OAUTH_CLIENT_SECRET
+            or None,
+            oauth_server=opal_client_config.POLICY_STORE_AUTH_OAUTH_SERVER or None,
         )
 
     return router
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.6.0/opal_client/policy_store/base_policy_store_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import uuid
+from asyncio import StreamReader, StreamWriter
 from datetime import datetime
 from functools import partial
 from inspect import signature
 from typing import Any, Dict, List, Optional, Union
 
 from opal_client.config import opal_client_config
 from opal_client.logger import logger
@@ -61,20 +62,27 @@
 
     async def get_data(self, path: str) -> Dict:
         raise NotImplementedError()
 
     async def get_data_with_input(self, path: str, input: BaseModel) -> Dict:
         raise NotImplementedError()
 
-    async def init_healthcheck_policy(
-        self, policy_id: str, policy_code: str, data_updater_enabled: bool = True
-    ):
+    async def init_healthcheck_policy(self, policy_id: str, policy_code: str):
+        raise NotImplementedError()
+
+    async def log_transaction(self, transaction: StoreTransaction):
         raise NotImplementedError()
 
-    async def persist_transaction(self, transaction: StoreTransaction):
+    async def is_healthy(self) -> bool:
+        raise NotImplementedError()
+
+    async def full_export(self, writer: StreamWriter) -> None:
+        raise NotImplementedError()
+
+    async def full_import(self, reader: StreamReader) -> None:
         raise NotImplementedError()
 
 
 class PolicyStoreTransactionContextManager(AbstractPolicyStore):
     def __init__(
         self,
         policy_store: "BasePolicyStoreClient",
@@ -226,24 +234,8 @@
                 success=True,
                 creation_time=creation_time,
                 end_time=end_time,
                 transaction_type=transaction_type,
                 remotes_status=remotes_status,
             )
 
-        if not opal_client_config.OPA_HEALTH_CHECK_POLICY_ENABLED:
-            return  # skip persisting the transaction, healthcheck policy is disabled
-
-        try:
-            await self.persist_transaction(transaction)
-        except Exception as e:
-            # The writes to transaction log in OPA cache are not done a protected
-            # transaction context. If they fail, we do nothing special.
-            transaction_data = json.dumps(
-                transaction, indent=4, sort_keys=True, default=str
-            )
-            logger.error(
-                "Cannot write to OPAL transaction log, transaction id={id}, error={err} with data={data}",
-                id=transaction.id,
-                err=repr(e),
-                data=transaction_data,
-            )
+        await self.log_transaction(transaction)
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.6.0/opal_client/policy_store/mock_policy_store_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,9 +83,9 @@
         await self.has_data_event.wait()
 
     async def init_healthcheck_policy(
         self, policy_id: str, policy_code: str, data_updater_enabled: bool = True
     ):
         pass
 
-    async def persist_transaction(self, transaction: StoreTransaction):
+    async def log_transaction(self, transaction: StoreTransaction):
         pass
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/opa_client.py` & `opal-client-0.6.0/opal_client/policy_store/opa_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import asyncio
 import functools
 import json
-from typing import Any, Dict, List, Optional, Set
+import time
+from asyncio import StreamReader, StreamWriter
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Set
+from urllib.parse import urlencode
 
 import aiohttp
 from fastapi import Response, status
 from opal_client.config import opal_client_config
 from opal_client.logger import logger
 from opal_client.policy_store.base_policy_store_client import (
     BasePolicyStoreClient,
     JsonableValue,
 )
+from opal_client.policy_store.schemas import PolicyStoreAuth
 from opal_client.utils import proxy_response
 from opal_common.git.bundle_utils import BundleUtils
 from opal_common.opa.parsing import get_rego_package
-from opal_common.schemas.policy import DataModule, PolicyBundle
+from opal_common.paths import PathUtils
+from opal_common.schemas.policy import DataModule, PolicyBundle, RegoModule
 from opal_common.schemas.store import JSONPatchAction, StoreTransaction, TransactionType
 from pydantic import BaseModel
-from tenacity import retry
+from tenacity import RetryError, retry
 
 JSONPatchDocument = List[JSONPatchAction]
 
 
 RETRY_CONFIG = opal_client_config.POLICY_STORE_CONN_RETRY.toTenacityConfig()
 
 
+def should_ignore_path(path, ignore_paths):
+    """Helper function to check if the policy-store should ignore to given
+    path."""
+    return PathUtils.glob_style_match_path_to_list(path, ignore_paths) is not None
+
+
 def fail_silently(fallback=None):
     def decorator(func):
         @functools.wraps(func)
         async def wrapper(*args, **kwargs):
             try:
                 return await func(*args, **kwargs)
             except aiohttp.ClientError as e:
@@ -45,15 +56,15 @@
     setattr(func, "affects_transaction", True)
     return func
 
 
 async def proxy_response_unless_invalid(
     raw_response: aiohttp.ClientResponse, accepted_status_codes: List[int]
 ) -> Response:
-    """throws value error if the http response recieved has an unexpected
+    """throws value error if the http response received has an unexpected
     status code."""
     response = await proxy_response(raw_response)
     if response.status_code not in accepted_status_codes:
         try:
             error = await raw_response.json()
         except json.JSONDecodeError:
             error = ""
@@ -72,22 +83,16 @@
     """
 
     POLICY_ACTIONS = ["set_policies", "set_policy", "delete_policy"]
     DATA_ACTIONS = ["set_policy_data", "delete_policy_data"]
 
     def __init__(
         self,
-        policy_store: BasePolicyStoreClient,
-        policy_id: str,
-        policy_template: str,
         data_updater_enabled: bool = True,
     ):
-        self._store = policy_store
-        self._policy_id = policy_id
-        self._policy_template = policy_template
         self._data_updater_disabled = not data_updater_enabled
         self._num_successful_policy_transactions = 0
         self._num_failed_policy_transactions = 0
         self._num_successful_data_transactions = 0
         self._num_failed_data_transactions = 0
         self._last_policy_transaction: Optional[StoreTransaction] = None
         self._last_failed_policy_transaction: Optional[StoreTransaction] = None
@@ -95,260 +100,432 @@
         self._last_failed_data_transaction: Optional[StoreTransaction] = None
 
     @property
     def ready(self) -> bool:
         is_ready: bool = self._num_successful_policy_transactions > 0 and (
             self._data_updater_disabled or self._num_successful_data_transactions > 0
         )
-        return json.dumps(is_ready)
+        return is_ready
 
     @property
     def healthy(self) -> bool:
         policy_updater_is_healthy: bool = (
             self._last_policy_transaction is not None
             and self._last_policy_transaction.success
         )
         data_updater_is_healthy: bool = (
             self._last_data_transaction is not None
             and self._last_data_transaction.success
         )
         is_healthy: bool = policy_updater_is_healthy and (
             self._data_updater_disabled or data_updater_is_healthy
         )
-        return json.dumps(is_healthy)
+        logger.info(
+            f"OPA client health: {is_healthy} (policy: {policy_updater_is_healthy}, data: {data_updater_is_healthy})"
+        )
+        return is_healthy
 
     @property
     def last_policy_transaction(self):
         if self._last_policy_transaction is None:
-            return json.dumps({})
-        return json.dumps(self._last_policy_transaction.dict())
+            return {}
+        return self._last_policy_transaction.dict()
 
     @property
     def last_data_transaction(self):
         if self._last_data_transaction is None:
-            return json.dumps({})
-        return json.dumps(self._last_data_transaction.dict())
+            return {}
+        return self._last_data_transaction.dict()
 
     @property
     def last_failed_policy_transaction(self):
         if self._last_failed_policy_transaction is None:
-            return json.dumps({})
-        return json.dumps(self._last_failed_policy_transaction.dict())
+            return {}
+        return self._last_failed_policy_transaction.dict()
 
     @property
     def last_failed_data_transaction(self):
         if self._last_failed_data_transaction is None:
-            return json.dumps({})
-        return json.dumps(self._last_failed_data_transaction.dict())
+            return {}
+        return self._last_failed_data_transaction.dict()
 
     @property
     def transaction_policy_statistics(self):
-        return json.dumps(
-            {
-                "successful": self._num_successful_policy_transactions,
-                "failed": self._num_failed_policy_transactions,
-            }
-        )
+        return {
+            "successful": self._num_successful_policy_transactions,
+            "failed": self._num_failed_policy_transactions,
+        }
 
     @property
     def transaction_data_statistics(self):
-        return json.dumps(
-            {
-                "successful": self._num_successful_data_transactions,
-                "failed": self._num_failed_data_transactions,
-            }
-        )
-
-    async def persist(self):
-        """renders the policy template with the current state, and writes it to
-        OPA."""
-        logger.info(
-            "persisting health check policy: ready={ready}, healthy={healthy}",
-            ready=self.ready,
-            healthy=self.healthy,
-        )
-        logger.info(
-            "Policy and data statistics: policy: (successful {success_policy}, failed {failed_policy});\tdata: (successful {success_data}, failed {failed_data})",
-            success_policy=self._num_successful_policy_transactions,
-            failed_policy=self._num_failed_policy_transactions,
-            success_data=self._num_successful_data_transactions,
-            failed_data=self._num_failed_data_transactions,
-        )
-        policy_code = self._policy_template.format(
-            ready=self.ready,
-            healthy=self.healthy,
-            last_policy_transaction=self.last_policy_transaction,
-            last_failed_policy_transaction=self.last_failed_policy_transaction,
-            last_data_transaction=self.last_data_transaction,
-            last_failed_data_transaction=self.last_failed_data_transaction,
-            transaction_data_statistics=self.transaction_data_statistics,
-            transaction_policy_statistics=self.transaction_policy_statistics,
-        )
-        return await self._store.set_policy(
-            policy_id=self._policy_id, policy_code=policy_code
-        )
+        return {
+            "successful": self._num_successful_data_transactions,
+            "failed": self._num_failed_data_transactions,
+        }
 
     def _is_policy_transaction(self, transaction: StoreTransaction):
         return transaction.transaction_type == TransactionType.policy
 
     def _is_data_transaction(self, transaction: StoreTransaction):
         return transaction.transaction_type == TransactionType.data
 
     def process_transaction(self, transaction: StoreTransaction):
         """mutates the state into a new state that can be then persisted as
         hardcoded policy."""
-        logger.info(
+        logger.debug(
             "processing store transaction: {transaction}",
             transaction=transaction.dict(),
         )
         if self._is_policy_transaction(transaction):
-
             if transaction.success:
                 self._last_policy_transaction = transaction
                 self._num_successful_policy_transactions += 1
             else:
                 self._last_failed_policy_transaction = transaction
                 self._num_failed_policy_transactions += 1
 
         elif self._is_data_transaction(transaction):
-
             if transaction.success:
                 self._last_data_transaction = transaction
                 self._num_successful_data_transactions += 1
             else:
                 self._last_failed_data_transaction = transaction
                 self._num_failed_data_transactions += 1
 
 
+class OpaTransactionLogPolicyWriter:
+    def __init__(
+        self,
+        policy_store: BasePolicyStoreClient,
+        policy_id: str,
+        policy_template: str,
+    ):
+        self._store = policy_store
+        self._policy_id = policy_id
+        self._policy_template = policy_template
+
+    @staticmethod
+    def _format_with_json(template, **kwargs):
+        kwargs = {k: json.dumps(v) for k, v in kwargs.items()}
+        return template.format(**kwargs)
+
+    async def persist(self, state: OpaTransactionLogState):
+        """renders the policy template with the current state, and writes it to
+        OPA."""
+        logger.info(
+            "persisting health check policy: ready={ready}, healthy={healthy}",
+            ready=state.ready,
+            healthy=state.healthy,
+        )
+        logger.info(
+            "Policy and data statistics: policy: (successful {success_policy}, failed {failed_policy});\tdata: (successful {success_data}, failed {failed_data})",
+            success_policy=state._num_successful_policy_transactions,
+            failed_policy=state._num_failed_policy_transactions,
+            success_data=state._num_successful_data_transactions,
+            failed_data=state._num_failed_data_transactions,
+        )
+        policy_code = self._format_with_json(
+            self._policy_template,
+            ready=state.ready,
+            healthy=state.healthy,
+            last_policy_transaction=state.last_policy_transaction,
+            last_failed_policy_transaction=state.last_failed_policy_transaction,
+            last_data_transaction=state.last_data_transaction,
+            last_failed_data_transaction=state.last_failed_data_transaction,
+            transaction_data_statistics=state.transaction_data_statistics,
+            transaction_policy_statistics=state.transaction_policy_statistics,
+        )
+        return await self._store.set_policy(
+            policy_id=self._policy_id, policy_code=policy_code
+        )
+
+
 class OpaClient(BasePolicyStoreClient):
     """communicates with OPA via its REST API."""
 
     POLICY_NAME = "rbac"
 
-    def __init__(self, opa_server_url=None, opa_auth_token: Optional[str] = None):
+    def __init__(
+        self,
+        opa_server_url=None,
+        opa_auth_token: Optional[str] = None,
+        auth_type: PolicyStoreAuth = PolicyStoreAuth.NONE,
+        oauth_client_id: Optional[str] = None,
+        oauth_client_secret: Optional[str] = None,
+        oauth_server: Optional[str] = None,
+        data_updater_enabled: bool = True,
+    ):
         base_url = opa_server_url or opal_client_config.POLICY_STORE_URL
         self._opa_url = f"{base_url}/v1"
         self._cached_policies: Dict[str, str] = {}
         self._policy_version: Optional[str] = None
         self._lock = asyncio.Lock()
         self._token = opa_auth_token
-        self._headers = {}
-        if opa_auth_token is not None:
-            self._headers.update({"Authorization": f"Bearer {opa_auth_token}"})
-
-        # as long as this is null, transaction log is disabled
-        self._transaction_state: Optional[OpaTransactionLogState] = None
+        self._auth_type: PolicyStoreAuth = auth_type
+        self._oauth_client_id = oauth_client_id
+        self._oauth_client_secret = oauth_client_secret
+        self._oauth_server = oauth_server
+        self._oauth_token_cache = {"token": None, "expires": 0}
+
+        if auth_type == PolicyStoreAuth.TOKEN:
+            if self._token is None:
+                logger.error("POLICY_STORE_AUTH_TOKEN can not be empty")
+                raise Exception("required variables for token auth are not set")
+
+        if auth_type == PolicyStoreAuth.OAUTH:
+            isError = False
+            if self._oauth_client_id is None:
+                isError = True
+                logger.error("POLICY_STORE_AUTH_OAUTH_CLIENT_ID can not be empty")
+
+            if self._oauth_client_secret is None:
+                isError = True
+                logger.error("POLICY_STORE_AUTH_OAUTH_CLIENT_SECRET can not be empty")
+
+            if self._oauth_server is None:
+                isError = True
+                logger.error("POLICY_STORE_AUTH_OAUTH_SERVER can not be empty")
+
+            if isError:
+                raise Exception("required variables for oauth are not set")
+
+        logger.info(f"Authentication mode for policy store: {auth_type}")
+
+        self._transaction_state = OpaTransactionLogState(data_updater_enabled)
+        # as long as this is null, persisting transaction log to OPA is disabled
+        self._transaction_state_writer: Optional[OpaTransactionLogState] = None
 
     async def get_policy_version(self) -> Optional[str]:
         return self._policy_version
 
+    @retry(**RETRY_CONFIG)
+    async def _get_oauth_token(self):
+        logger.info("Retrieving a new OAuth access_token.")
+
+        async with aiohttp.ClientSession() as session:
+            try:
+                async with session.post(
+                    self._oauth_server,
+                    headers={
+                        "accept": "application/json",
+                        "content-type": "application/x-www-form-urlencoded;charset=UTF-8",
+                    },
+                    data=urlencode({"grant_type": "client_credentials"}).encode(
+                        "utf-8"
+                    ),
+                    auth=aiohttp.BasicAuth(
+                        self._oauth_client_id, self._oauth_client_secret
+                    ),
+                ) as oauth_response:
+                    response = await oauth_response.json()
+                    logger.info(
+                        f"got access_token, expires in {response['expires_in']} seconds"
+                    )
+
+                    return {
+                        # refresh token before it expires, lets subtract 10 seconds
+                        "expires": time.time() + response["expires_in"] - 10,
+                        "token": response["access_token"],
+                    }
+            except aiohttp.ClientError as e:
+                logger.warning("OAuth server connection error: {err}", err=repr(e))
+                raise
+
+    async def _get_auth_headers(self) -> {}:
+        headers = {}
+        if self._auth_type == PolicyStoreAuth.TOKEN:
+            if self._token is not None:
+                headers.update({"Authorization": f"Bearer {self._token}"})
+
+        elif self._auth_type == PolicyStoreAuth.OAUTH:
+            if (
+                self._oauth_token_cache["token"] is None
+                or time.time() > self._oauth_token_cache["expires"]
+            ):
+                self._oauth_token_cache = await self._get_oauth_token()
+
+            headers.update(
+                {"Authorization": f"Bearer {self._oauth_token_cache['token']}"}
+            )
+
+        return headers
+
     @affects_transaction
     @retry(**RETRY_CONFIG)
     async def set_policy(
-        self, policy_id: str, policy_code: str, transaction_id: Optional[str] = None
+        self,
+        policy_id: str,
+        policy_code: str,
+        transaction_id: Optional[str] = None,
     ):
+        # ignore explicitly configured paths
+        if should_ignore_path(
+            policy_id, opal_client_config.POLICY_STORE_POLICY_PATHS_TO_IGNORE
+        ):
+            logger.info(
+                f"Ignoring setting policy - {policy_id}, set in POLICY_PATHS_TO_IGNORE."
+            )
+            return
         self._cached_policies[policy_id] = policy_code
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.put(
                     f"{self._opa_url}/policies/{policy_id}",
                     data=policy_code,
-                    headers={"content-type": "text/plain", **self._headers},
+                    headers={"content-type": "text/plain", **headers},
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
-                        opa_response, accepted_status_codes=[status.HTTP_200_OK]
+                        opa_response,
+                        accepted_status_codes=[
+                            status.HTTP_200_OK,
+                            status.HTTP_400_BAD_REQUEST,  # No point in immediate retry, this means erroneous rego (bad syntax, duplicated definition, etc)
+                        ],
                     )
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
     @fail_silently()
     @retry(**RETRY_CONFIG)
     async def get_policy(self, policy_id: str) -> Optional[str]:
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.get(
-                    f"{self._opa_url}/policies/{policy_id}", headers=self._headers
+                    f"{self._opa_url}/policies/{policy_id}", headers=headers
                 ) as opa_response:
                     result = await opa_response.json()
                     return result.get("result", {}).get("raw", None)
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
+    @fail_silently()
+    @retry(**RETRY_CONFIG)
+    async def get_policies(self) -> Optional[Dict[str, str]]:
+        async with aiohttp.ClientSession() as session:
+            try:
+                headers = await self._get_auth_headers()
+
+                async with session.get(
+                    f"{self._opa_url}/policies", headers=headers
+                ) as opa_response:
+                    result = await opa_response.json()
+                    return OpaClient._extract_modules_from_policies_json(result)
+            except aiohttp.ClientError as e:
+                logger.warning("Opa connection error: {err}", err=repr(e))
+                raise
+
     @affects_transaction
     @retry(**RETRY_CONFIG)
     async def delete_policy(self, policy_id: str, transaction_id: Optional[str] = None):
+        # ignore explicitly configured paths
+        if should_ignore_path(
+            policy_id, opal_client_config.POLICY_STORE_POLICY_PATHS_TO_IGNORE
+        ):
+            logger.info(
+                f"Ignoring deleting policy - {policy_id}, set in POLICY_PATHS_TO_IGNORE."
+            )
+            return
+
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.delete(
-                    f"{self._opa_url}/policies/{policy_id}", headers=self._headers
+                    f"{self._opa_url}/policies/{policy_id}", headers=headers
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_200_OK,
                             status.HTTP_404_NOT_FOUND,
                         ],
                     )
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
-    @fail_silently()
-    @retry(**RETRY_CONFIG)
     async def get_policy_module_ids(self) -> List[str]:
-        async with aiohttp.ClientSession() as session:
-            try:
-                async with session.get(
-                    f"{self._opa_url}/policies", headers=self._headers
-                ) as opa_response:
-                    result = await opa_response.json()
-                    return OpaClient._extract_module_ids_from_policies_json(result)
-            except aiohttp.ClientError as e:
-                logger.warning("Opa connection error: {err}", err=repr(e))
-                raise
+        modules = await self.get_policies()
+        return modules.keys()
 
     @staticmethod
-    def _extract_module_ids_from_policies_json(result: Dict[str, Any]) -> List[str]:
+    def _extract_modules_from_policies_json(result: Dict[str, Any]) -> Dict[str, str]:
         """return all module ids in OPA cache who are not:
 
         - skipped module ids (i.e: our health check policy)
         - all modules with package name starting with "system" (special OPA policies)
         """
-        modules: List[Dict[str, Any]] = result.get("result", [])
+        policies: List[Dict[str, Any]] = result.get("result", [])
         builtin_modules = [opal_client_config.OPA_HEALTH_CHECK_POLICY_PATH]
 
-        module_ids = []
-        for module in modules:
-            module_id = module.get("id", None)
-            package_name = get_rego_package(module.get("raw", ""))
+        modules = {}
+        for policy in policies:
+            module_id = policy.get("id", None)
+            module_raw = policy.get("raw", "")
+            package_name = get_rego_package(module_raw)
 
             if module_id is None:
                 continue
 
             if package_name is not None and package_name.startswith("system."):
                 continue
 
             if module_id in builtin_modules:
                 continue
 
-            module_ids.append(module_id)
+            modules[module_id] = module_raw
 
-        return module_ids
+        return modules
 
     @affects_transaction
     async def set_policies(
         self, bundle: PolicyBundle, transaction_id: Optional[str] = None
     ):
         if bundle.old_hash is None:
             return await self._set_policies_from_complete_bundle(bundle)
         else:
             return await self._set_policies_from_delta_bundle(bundle)
 
+    @staticmethod
+    async def _attempt_operations_with_postponed_failure_retry(
+        ops: List[Callable[[], Awaitable[Response]]]
+    ):
+        """Attempt to execute the given operations in the given order, where
+        failed operations are tried again at the end (recursively).
+
+        This overcomes issues of misordering (e.g. setting a renamed
+        policy before deleting the old one, or setting a policy before
+        its dependencies)
+        """
+        while True:
+            failed_ops = []
+            for op in ops:
+                # Only expected errors are retried (such as 400), so exceptions are not caught
+                response = await op()
+                if response and response.status_code != status.HTTP_200_OK:
+                    logger.warning(
+                        f"Failed policy operation, would retry again after the rest. status: {response.status_code}, body: {response.body.decode()}"
+                    )
+                    failed_ops.append(op)
+
+            if len(failed_ops) == 0:
+                # all ops succeeded
+                return
+
+            if len(failed_ops) == len(ops):
+                # all ops failed on this iteration, no point at retrying
+                raise RuntimeError("Giving up setting / deleting failed modules to OPA")
+
+            ops = failed_ops  # retry failed ops
+
     async def _set_policies_from_complete_bundle(self, bundle: PolicyBundle):
         module_ids_in_store: Set[str] = set(await self.get_policy_module_ids())
         module_ids_in_bundle: Set[str] = {
             module.path for module in bundle.policy_modules
         }
         module_ids_to_delete: Set[str] = module_ids_in_store.difference(
             module_ids_in_bundle
@@ -358,46 +535,60 @@
             # save bundled policy *static* data into store
             for module in BundleUtils.sorted_data_modules_to_load(bundle):
                 await self._set_policy_data_from_bundle_data_module(
                     module, hash=bundle.hash
                 )
 
             # save bundled policies into store
-            for module in BundleUtils.sorted_policy_modules_to_load(bundle):
-                await self.set_policy(policy_id=module.path, policy_code=module.rego)
+            await OpaClient._attempt_operations_with_postponed_failure_retry(
+                [
+                    functools.partial(
+                        self.set_policy, policy_id=module.path, policy_code=module.rego
+                    )
+                    for module in BundleUtils.sorted_policy_modules_to_load(bundle)
+                ]
+            )
 
             # remove policies from the store that are not in the bundle
             # (because this bundle is "complete", i.e: contains all policy modules for a given hash)
+            # Note: this can be ignored below by config.POLICY_STORE_POLICY_PATHS_TO_IGNORE
             for module_id in module_ids_to_delete:
                 await self.delete_policy(policy_id=module_id)
 
             # save policy version (hash) into store
             self._policy_version = bundle.hash
 
     async def _set_policies_from_delta_bundle(self, bundle: PolicyBundle):
         async with self._lock:
             # save bundled policy *static* data into store
             for module in BundleUtils.sorted_data_modules_to_load(bundle):
                 await self._set_policy_data_from_bundle_data_module(
                     module, hash=bundle.hash
                 )
 
-            # save bundled policies into store
-            for module in BundleUtils.sorted_policy_modules_to_load(bundle):
-                await self.set_policy(policy_id=module.path, policy_code=module.rego)
+            # remove static policy data from store
+            for module_id in BundleUtils.sorted_data_modules_to_delete(bundle):
+                await self.delete_policy_data(
+                    path=self._safe_data_module_path(str(module_id))
+                )
 
-            # remove deleted policies (or static policy data) from store
-            if bundle.deleted_files is not None:
-                for module_id in BundleUtils.sorted_policy_modules_to_delete(bundle):
-                    await self.delete_policy(policy_id=module_id)
-
-                for module_id in BundleUtils.sorted_data_modules_to_delete(bundle):
-                    await self.delete_policy_data(
-                        path=self._safe_data_module_path(str(module_id))
+            await OpaClient._attempt_operations_with_postponed_failure_retry(
+                # save bundled policies into store
+                [
+                    functools.partial(
+                        self.set_policy, policy_id=module.path, policy_code=module.rego
                     )
+                    for module in BundleUtils.sorted_policy_modules_to_load(bundle)
+                ]
+                + [
+                    # remove deleted policies from store
+                    functools.partial(self.delete_policy, policy_id=module_id)
+                    for module_id in BundleUtils.sorted_policy_modules_to_delete(bundle)
+                ]
+            )
 
             # save policy version (hash) into store
             self._policy_version = bundle.hash
 
     @classmethod
     def _safe_data_module_path(cls, path: str):
         if not path or path == ".":
@@ -444,18 +635,20 @@
             logger.warning(
                 "OPAL client was instructed to put a list on OPA's root document. In OPA the root document must be an object so the original value was wrapped."
             )
             policy_data = {"items": policy_data}
 
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.put(
                     f"{self._opa_url}/data{path}",
                     data=json.dumps(policy_data, default=str),
-                    headers=self._headers,
+                    headers=headers,
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_304_NOT_MODIFIED,
                         ],
@@ -471,16 +664,18 @@
     ):
         path = self._safe_data_module_path(path)
         if not path:
             return await self.set_policy_data({})
 
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.delete(
-                    f"{self._opa_url}/data{path}", headers=self._headers
+                    f"{self._opa_url}/data{path}", headers=headers
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
                         opa_response,
                         accepted_status_codes=[
                             status.HTTP_204_NO_CONTENT,
                             status.HTTP_404_NOT_FOUND,
                         ],
@@ -499,21 +694,24 @@
         path = self._safe_data_module_path(path)
         # a patch document is a list of actions
         # we render each action with pydantic, and then dump the doc into json
         json_document = json.dumps([action.dict() for action in patch_document])
 
         async with aiohttp.ClientSession() as session:
             try:
+                headers = await self._get_auth_headers()
+
                 async with session.patch(
                     f"{self._opa_url}/data{path}",
                     data=json_document,
-                    headers=self._headers,
+                    headers=headers,
                 ) as opa_response:
                     return await proxy_response_unless_invalid(
-                        opa_response, accepted_status_codes=[status.HTTP_204_NO_CONTENT]
+                        opa_response,
+                        accepted_status_codes=[status.HTTP_204_NO_CONTENT],
                     )
             except aiohttp.ClientError as e:
                 logger.warning("Opa connection error: {err}", err=repr(e))
                 raise
 
     @fail_silently()
     @retry(**RETRY_CONFIG)
@@ -521,20 +719,22 @@
         """
         wraps opa's "GET /data" api that extracts base data documents from opa cache.
         NOTE: opa always returns 200 and empty dict (for valid input) even if the data does not exist.
 
         returns a dict (parsed json).
         """
         # function accepts paths that start with / and also path that do not start with /
-        if path.startswith("/"):
-            path = path[1:]
+        if path != "" and not path.startswith("/"):
+            path = "/" + path
         try:
+            headers = await self._get_auth_headers()
+
             async with aiohttp.ClientSession() as session:
                 async with session.get(
-                    f"{self._opa_url}/data/{path}", headers=self._headers
+                    f"{self._opa_url}/data{path}", headers=headers
                 ) as opa_response:
                     return await opa_response.json()
         except aiohttp.ClientError as e:
             logger.warning("Opa connection error: {err}", err=repr(e))
             raise
 
     @retry(**RETRY_CONFIG)
@@ -549,36 +749,73 @@
         https://www.openpolicyagent.org/docs/latest/rest-api/#get-a-document-with-input
         """
         # opa data api format needs the input to sit under "input"
         opa_input = {"input": input.dict()}
         if path.startswith("/"):
             path = path[1:]
         try:
+            headers = await self._get_auth_headers()
+
             async with aiohttp.ClientSession() as session:
                 async with session.post(
                     f"{self._opa_url}/data/{path}",
                     data=json.dumps(opa_input),
-                    headers=self._headers,
+                    headers=headers,
                 ) as opa_response:
                     return await proxy_response(opa_response)
         except aiohttp.ClientError as e:
             logger.warning("Opa connection error: {err}", err=repr(e))
             raise
 
     @retry(**RETRY_CONFIG)
-    async def init_healthcheck_policy(
-        self, policy_id: str, policy_code: str, data_updater_enabled: bool = True
-    ):
-        self._transaction_state = OpaTransactionLogState(
+    async def init_healthcheck_policy(self, policy_id: str, policy_code: str):
+        self._transaction_state_writer = OpaTransactionLogPolicyWriter(
             policy_store=self,
             policy_id=policy_id,
             policy_template=policy_code,
-            data_updater_enabled=data_updater_enabled,
         )
-        return await self._transaction_state.persist()
+        return await self._transaction_state_writer.persist(self._transaction_state)
 
     @retry(**RETRY_CONFIG)
-    async def persist_transaction(self, transaction: StoreTransaction):
-        if self._transaction_state is None:
-            return
+    async def log_transaction(self, transaction: StoreTransaction):
         self._transaction_state.process_transaction(transaction)
-        return await self._transaction_state.persist()
+
+        if self._transaction_state_writer:
+            try:
+                return await self._transaction_state_writer.persist(
+                    self._transaction_state
+                )
+            except Exception as e:
+                # The writes to transaction log in OPA cache are not done a protected
+                # transaction context. If they fail, we do nothing special.
+                transaction_data = json.dumps(
+                    transaction, indent=4, sort_keys=True, default=str
+                )
+                logger.error(
+                    "Cannot write to OPAL transaction log, transaction id={id}, error={err} with data={data}",
+                    id=transaction.id,
+                    err=repr(e),
+                    data=transaction_data,
+                )
+
+    async def is_ready(self) -> bool:
+        return self._transaction_state.ready
+
+    async def is_healthy(self) -> bool:
+        return self._transaction_state.healthy
+
+    async def full_export(self, writer: StreamWriter) -> None:
+        policies = await self.get_policies()
+        data = await self.get_data("")
+        await writer.write(json.dumps({"policies": policies, "data": data}))
+
+    async def full_import(self, reader: StreamReader) -> None:
+        import_data = json.loads(await reader.read())
+
+        await OpaClient._attempt_operations_with_postponed_failure_retry(
+            [
+                functools.partial(self.set_policy, policy_id=id, policy_code=raw)
+                for id, raw in import_data["policies"].items()
+            ]
+        )
+
+        await self.set_policy_data(import_data["data"])
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.6.0/opal_client/policy_store/policy_store_client_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,127 @@
 from typing import Dict, Optional
 
 from opal_client.config import opal_client_config
 from opal_client.policy_store.base_policy_store_client import BasePolicyStoreClient
-from opal_client.policy_store.schemas import PolicyStoreTypes
+from opal_client.policy_store.schemas import PolicyStoreAuth, PolicyStoreTypes
 
 
 class PolicyStoreClientFactoryException(Exception):
     pass
 
 
 class InvalidPolicyStoreTypeException(Exception):
     pass
 
 
 class PolicyStoreClientFactory:
-
     CACHE: Dict[str, BasePolicyStoreClient] = {}
 
     @classmethod
     def get(
         cls,
         store_type: PolicyStoreTypes = None,
         url: str = None,
         save_to_cache=True,
         token: Optional[str] = None,
+        auth_type: PolicyStoreAuth = PolicyStoreAuth.NONE,
+        oauth_client_id: Optional[str] = None,
+        oauth_client_secret: Optional[str] = None,
+        oauth_server: Optional[str] = None,
     ) -> BasePolicyStoreClient:
         """Same as self.create() but with caching.
 
         Args:
             store_type (PolicyStoreTypes, optional): The type of policy-store to use. Defaults to opal_client_config.POLICY_STORE_TYPE.
             url (str, optional): the URL of the policy store. Defaults to opal_client_config.POLICY_STORE_URL.
             save_to_cache (bool, optional): Should the created value be saved to cache (To be obtained via the get method).
 
         Raises:
-            InvalidPolicyStoreTypeException: Raised when the factory doesn't have a store-client macthing the given type
+            InvalidPolicyStoreTypeException: Raised when the factory doesn't have a store-client matching the given type
 
         Returns:
             BasePolicyStoreClient: the policy store client interface
         """
         # get from cache if available - else create anew
         key = cls.get_cache_key(store_type, url)
         value = cls.CACHE.get(key, None)
         if value is None:
-            return cls.create(store_type, url, token)
+            return cls.create(
+                store_type=store_type,
+                url=url,
+                save_to_cache=save_to_cache,
+                token=token,
+                auth_type=auth_type,
+                oauth_client_id=oauth_client_id,
+                oauth_client_secret=oauth_client_secret,
+                oauth_server=oauth_server,
+            )
         else:
             return value
 
     @classmethod
     def create(
         cls,
         store_type: PolicyStoreTypes = None,
         url: str = None,
         save_to_cache=True,
         token: Optional[str] = None,
+        auth_type: PolicyStoreAuth = None,
+        oauth_client_id: Optional[str] = None,
+        oauth_client_secret: Optional[str] = None,
+        oauth_server: Optional[str] = None,
+        data_updater_enabled: Optional[bool] = None,
     ) -> BasePolicyStoreClient:
         """
         Factory method - create a new policy store by type.
 
         Args:
             store_type (PolicyStoreTypes, optional): The type of policy-store to use. Defaults to opal_client_config.POLICY_STORE_TYPE.
             url (str, optional): the URL of the policy store. Defaults to opal_client_config.POLICY_STORE_URL.
             save_to_cache (bool, optional): Should the created value be saved to cache (To be obtained via the get method).
 
         Raises:
-            InvalidPolicyStoreTypeException: Raised when the factory doesn't have a store-client macthing the given type
+            InvalidPolicyStoreTypeException: Raised when the factory doesn't have a store-client matching the given type
 
         Returns:
             BasePolicyStoreClient: the policy store client interface
         """
         # load defaults
         store_type = store_type or opal_client_config.POLICY_STORE_TYPE
         url = url or opal_client_config.POLICY_STORE_URL
         store_token = token or opal_client_config.POLICY_STORE_AUTH_TOKEN
 
+        auth_type = auth_type or opal_client_config.POLICY_STORE_AUTH_TYPE
+        oauth_client_id = (
+            oauth_client_id or opal_client_config.POLICY_STORE_AUTH_OAUTH_CLIENT_ID
+        )
+        oauth_client_secret = (
+            oauth_client_secret
+            or opal_client_config.POLICY_STORE_AUTH_OAUTH_CLIENT_SECRET
+        )
+        oauth_server = oauth_server or opal_client_config.POLICY_STORE_AUTH_OAUTH_SERVER
+        data_updater_enabled = (
+            data_updater_enabled
+            if data_updater_enabled is not None
+            else opal_client_config.DATA_UPDATER_ENABLED
+        )
+
         # OPA
         if PolicyStoreTypes.OPA == store_type:
             from opal_client.policy_store.opa_client import OpaClient
 
-            res = OpaClient(url, opa_auth_token=store_token)
+            res = OpaClient(
+                url,
+                opa_auth_token=store_token,
+                auth_type=auth_type,
+                oauth_client_id=oauth_client_id,
+                oauth_client_secret=oauth_client_secret,
+                oauth_server=oauth_server,
+                data_updater_enabled=data_updater_enabled,
+            )
         # MOCK
         elif PolicyStoreTypes.MOCK == store_type:
             from opal_client.policy_store.mock_policy_store_client import (
                 MockPolicyStoreClient,
             )
 
             res = MockPolicyStoreClient()
```

### Comparing `opal-client-0.5.0/opal_client/policy_store/schemas.py` & `opal-client-0.6.0/opal_client/policy_store/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,34 +5,56 @@
 
 
 class PolicyStoreTypes(Enum):
     OPA = "OPA"
     MOCK = "MOCK"
 
 
+class PolicyStoreAuth(Enum):
+    NONE = "none"
+    TOKEN = "token"
+    OAUTH = "oauth"
+
+
 class PolicyStoreDetails(BaseModel):
     """
     represents a policy store endpoint - contains the policy store's:
     - location (url)
     - type
     - credentials
     """
 
     type: PolicyStoreTypes = Field(
         PolicyStoreTypes.OPA,
         description="the type of policy store, currently only OPA is officially supported",
     )
     url: str = Field(
         ...,
-        description="the url that OPA can be found in. if localhost is the host - it means OPA is on the same hostname as OPAL client.",
+        description="the url that OPA can be found in. if localhost is the host - "
+        "it means OPA is on the same hostname as OPAL client.",
     )
     token: Optional[str] = Field(
         None, description="optional access token required by the policy store"
     )
 
+    auth_type: PolicyStoreAuth = Field(
+        PolicyStoreAuth.NONE,
+        description="the type of authentication is supported for the policy store.",
+    )
+
+    oauth_client_id: Optional[str] = Field(
+        None, description="optional OAuth client id required by the policy store"
+    )
+    oauth_client_secret: Optional[str] = Field(
+        None, description="optional OAuth client secret required by the policy store"
+    )
+    oauth_server: Optional[str] = Field(
+        None, description="optional OAuth server required by the policy store"
+    )
+
     @validator("type")
     def force_enum(cls, v):
         if isinstance(v, str):
             return PolicyStoreTypes(v)
         if isinstance(v, PolicyStoreTypes):
             return v
         raise ValueError(f"invalid value: {v}")
```

### Comparing `opal-client-0.5.0/opal_client/tests/data_updater_test.py` & `opal-client-0.6.0/opal_client/tests/data_updater_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 DATA_SOURCES_CONFIG = ServerDataSourceConfig(
     config=DataSourceConfig(entries=[{"url": DATA_URL, "topics": DATA_TOPICS}])
 )
 
 
 def setup_server(event):
-    # Server without git watcher and with a test specifc url for data, and without broadcasting
+    # Server without git watcher and with a test specific url for data, and without broadcasting
     server = OpalServer(
         init_policy_watcher=False,
         data_sources_config=DATA_SOURCES_CONFIG,
         broadcaster_uri=None,
         enable_jwks_endpoint=False,
     )
     server_app = server.app
@@ -139,15 +139,15 @@
         should_send_reports=False,
     )
     # start the updater (terminate on exit)
     await updater.start()
     try:
         proc = multiprocessing.Process(target=trigger_update, daemon=True)
         proc.start()
-        # wait until new data arrives into the strore via the updater
+        # wait until new data arrives into the store via the updater
         await asyncio.wait_for(policy_store.wait_for_data(), 60)
     # cleanup
     finally:
         await updater.stop()
         proc.terminate()
 
 
@@ -173,15 +173,15 @@
     async with ClientSession() as session:
         res = await session.get(CHECK_DATA_UPDATE_CALLBACK_URL)
         current_callback_count = await res.json()
 
     try:
         proc = multiprocessing.Process(target=trigger_update, daemon=True)
         proc.start()
-        # wait until new data arrives into the strore via the updater
+        # wait until new data arrives into the store via the updater
         await asyncio.wait_for(policy_store.wait_for_data(), 15)
         # give the callback a chance to arrive
         await asyncio.sleep(1)
 
         async with ClientSession() as session:
             res = await session.get(CHECK_DATA_UPDATE_CALLBACK_URL)
             count = await res.json()
@@ -208,12 +208,12 @@
         fetch_on_connect=True,
         data_topics=DATA_TOPICS,
         should_send_reports=False,
     )
     # start the updater (terminate on exit)
     await updater.start()
     try:
-        # wait until new data arrives into the strore via the updater
+        # wait until new data arrives into the store via the updater
         await asyncio.wait_for(policy_store.wait_for_data(), 5)
     # cleanup
     finally:
         await updater.stop()
```

### Comparing `opal-client-0.5.0/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.6.0/opal_client/tests/server_to_client_intergation_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 # Client settings
 CLIENT_PORT = int(os.environ.get("CLIENT_PORT") or "9321")
 CLIENT_STORE_ROUTE = "/check_store"
 CLIENT_STORE_URL = f"http://localhost:{CLIENT_PORT}{CLIENT_STORE_ROUTE}"
 
 
 def setup_server(event):
-    # Server without git watcher and with a test specifc url for data, and without broadcasting
+    # Server without git watcher and with a test specific url for data, and without broadcasting
     server = OpalServer(
         init_policy_watcher=False,
         init_publisher=False,
         data_sources_config=DATA_SOURCES_CONFIG,
         broadcaster_uri=None,
         enable_jwks_endpoint=False,
     )
```

### Comparing `opal-client-0.5.0/opal_client.egg-info/PKG-INFO` & `opal-client-0.6.0/opal_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
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
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
-Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Platform:
-UNKNOWN Classifier: Operating System :: OS Independent Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
-:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
+Operating System :: OS Independent Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP
+:: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-
+Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -36,21 +36,21 @@
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
@@ -77,12 +77,13 @@
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

### Comparing `opal-client-0.5.0/opal_client.egg-info/SOURCES.txt` & `opal-client-0.6.0/opal_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 opal_client/policy_store/base_policy_store_client.py
 opal_client/policy_store/mock_policy_store_client.py
 opal_client/policy_store/opa_client.py
 opal_client/policy_store/policy_store_client_factory.py
 opal_client/policy_store/schemas.py
 opal_client/tests/__init__.py
 opal_client/tests/data_updater_test.py
+opal_client/tests/opa_client_test.py
 opal_client/tests/server_to_client_intergation_test.py
```

### Comparing `opal-client-0.5.0/setup.py` & `opal-client-0.6.0/setup.py`

 * *Files identical despite different names*

