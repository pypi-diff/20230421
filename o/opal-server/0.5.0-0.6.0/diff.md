# Comparing `tmp/opal-server-0.5.0.tar.gz` & `tmp/opal-server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.5.0.tar", last modified: Mon Feb 27 17:27:12 2023, max compression
+gzip compressed data, was "opal-server-0.6.0.tar", last modified: Fri Apr 21 07:57:02 2023, max compression
```

## Comparing `opal-server-0.5.0.tar` & `opal-server-0.6.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.314053 opal-server-0.5.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8590 2023-02-27 17:27:12.313857 opal-server-0.5.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.310424 opal-server-0.5.0/opal_server/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2126 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    10274 2023-02-24 20:59:56.000000 opal-server-0.5.0/opal_server/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.311451 opal-server-0.5.0/opal_server/data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5297 2022-10-12 14:50:19.000000 opal-server-0.5.0/opal_server/data/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     6109 2023-02-24 20:59:56.000000 opal-server-0.5.0/opal_server/data/data_update_publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)    12246 2023-02-24 20:59:56.000000 opal-server-0.5.0/opal_server/git_fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)      987 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/loadlimiting.py
--rw-r--r--   0 asafc      (501) staff       (20)      153 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/main.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.311576 opal-server-0.5.0/opal_server/policy/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.311745 opal-server-0.5.0/opal_server/policy/bundles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4444 2023-02-24 20:59:56.000000 opal-server-0.5.0/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.312200 opal-server-0.5.0/opal_server/policy/watcher/
--rw-r--r--   0 asafc      (501) staff       (20)       67 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4459 2023-02-27 16:56:34.000000 opal-server-0.5.0/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 asafc      (501) staff       (20)     5833 2023-02-27 16:56:34.000000 opal-server-0.5.0/opal_server/policy/watcher/factory.py
--rw-r--r--   0 asafc      (501) staff       (20)     2379 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.312749 opal-server-0.5.0/opal_server/policy/webhook/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5618 2023-02-01 11:46:28.000000 opal-server-0.5.0/opal_server/policy/webhook/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-02-24 20:59:56.000000 opal-server-0.5.0/opal_server/policy/webhook/deps.py
--rw-r--r--   0 asafc      (501) staff       (20)     1234 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/policy/webhook/listener.py
--rw-r--r--   0 asafc      (501) staff       (20)     1331 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)     3659 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/pubsub.py
--rw-r--r--   0 asafc      (501) staff       (20)     1390 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/redis.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.313269 opal-server-0.5.0/opal_server/scopes/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/scopes/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    11107 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/scopes/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     1690 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/scopes/loader.py
--rw-r--r--   0 asafc      (501) staff       (20)     1325 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/scopes/scope_repository.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.313601 opal-server-0.5.0/opal_server/security/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/security/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1423 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/security/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     1277 2022-10-01 21:13:25.000000 opal-server-0.5.0/opal_server/security/jwks.py
--rw-r--r--   0 asafc      (501) staff       (20)    19069 2022-10-14 18:40:00.000000 opal-server-0.5.0/opal_server/server.py
--rw-r--r--   0 asafc      (501) staff       (20)    12533 2023-02-01 11:46:28.000000 opal-server-0.5.0/opal_server/statistics.py
--rw-r--r--   0 asafc      (501) staff       (20)    10294 2022-10-11 10:23:16.000000 opal-server-0.5.0/opal_server/worker.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-02-27 17:27:12.311055 opal-server-0.5.0/opal_server.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8590 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1211 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       53 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 asafc      (501) staff       (20)      566 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-02-27 17:27:12.000000 opal-server-0.5.0/opal_server.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-02-27 17:27:12.314089 opal-server-0.5.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2979 2022-10-01 21:13:25.000000 opal-server-0.5.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.142644 opal-server-0.6.0/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-04-21 07:57:02.142280 opal-server-0.6.0/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.138218 opal-server-0.6.0/opal_server/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-04-19 15:20:19.000000 opal-server-0.6.0/opal_server/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    10418 2023-04-19 15:20:19.000000 opal-server-0.6.0/opal_server/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139596 opal-server-0.6.0/opal_server/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5297 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-03-27 15:01:56.000000 opal-server-0.6.0/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/git_fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/loadlimiting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139745 opal-server-0.6.0/opal_server/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139947 opal-server-0.6.0/opal_server/policy/bundles/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4444 2023-02-14 09:43:53.000000 opal-server-0.6.0/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.140439 opal-server-0.6.0/opal_server/policy/watcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4459 2023-02-28 14:04:36.000000 opal-server-0.6.0/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5669 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.140941 opal-server-0.6.0/opal_server/policy/webhook/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5675 2023-03-12 07:32:46.000000 opal-server-0.6.0/opal_server/policy/webhook/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-02-14 09:43:53.000000 opal-server-0.6.0/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-04-18 15:25:03.000000 opal-server-0.6.0/opal_server/pubsub.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1390 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/redis.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.141658 opal-server-0.6.0/opal_server/scopes/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/scopes/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12600 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/loader.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1325 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7285 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/service.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-04-19 08:36:33.000000 opal-server-0.6.0/opal_server/scopes/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.142059 opal-server-0.6.0/opal_server/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1423 2022-12-08 13:45:19.000000 opal-server-0.6.0/opal_server/security/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.6.0/opal_server/security/jwks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    16902 2023-04-19 10:07:30.000000 opal-server-0.6.0/opal_server/server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-01-19 13:43:15.000000 opal-server-0.6.0/opal_server/statistics.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-04-21 07:57:02.139207 opal-server-0.6.0/opal_server.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      546 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-04-21 07:57:02.000000 opal-server-0.6.0/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-04-21 07:57:02.142693 opal-server-0.6.0/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.6.0/setup.py
```

### Comparing `opal-server-0.5.0/PKG-INFO` & `opal-server-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
-Platform: UNKNOWN Classifier: Operating System :: OS Independent Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
-WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Classifier: Operating System :: OS Independent Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
+:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
+Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -37,21 +37,21 @@
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
@@ -78,12 +78,13 @@
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

### Comparing `opal-server-0.5.0/opal_server/cli.py` & `opal-server-0.6.0/opal_server/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 from opal_server.config import opal_server_config
 
 app = get_typer_app()
 
 
 @app.command()
 def run(engine_type: str = typer.Option("uvicron", help="uvicorn or gunicorn")):
-    """Run the server as a deamon."""
+    """Run the server as a daemon."""
     typer.echo(f"-- Starting OPAL Server (with {engine_type}) --")
 
     if engine_type == "gunicorn":
         app: FastAPI
         from opal_server.main import app
 
         run_gunicorn(
             app,
             opal_server_config.SERVER_WORKER_COUNT,
             host=opal_server_config.SERVER_HOST,
-            port=opal_server_config.SERVER_PORT,
+            port=opal_server_config.SERVER_BIND_PORT,
         )
     else:
         run_uvicorn(
             "opal_server.main:app",
             workers=opal_server_config.SERVER_WORKER_COUNT,
             host=opal_server_config.SERVER_HOST,
-            port=opal_server_config.SERVER_PORT,
+            port=opal_server_config.SERVER_BIND_PORT,
         )
 
 
 @app.command()
 def print_config():
     """To test config values, print the configuration parsed from ENV and
     CMD."""
```

### Comparing `opal-server-0.5.0/opal_server/config.py` & `opal-server-0.6.0/opal_server/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         + "see link: https://limits.readthedocs.io/en/stable/quickstart.html#rate-limit-string-notation",
     )
     # The URL for the backbone pub/sub server (e.g. Postgres, Kfaka, Redis) @see
     BROADCAST_URI = confi.str("BROADCAST_URI", None)
     # The name to be used for segmentation in the backbone pub/sub (e.g. the Kafka topic)
     BROADCAST_CHANNEL_NAME = confi.str("BROADCAST_CHANNEL_NAME", "EventNotifier")
     BROADCAST_CONN_LOSS_BUGFIX_EXPERIMENT_ENABLED = confi.bool(
-        "BROADCAST_CONN_LOSS_BUGFIX_EXPERIMENT_ENABLED", False
+        "BROADCAST_CONN_LOSS_BUGFIX_EXPERIMENT_ENABLED", True
     )
 
     # server security
     AUTH_PRIVATE_KEY_FORMAT = confi.enum(
         "AUTH_PRIVATE_KEY_FORMAT", EncryptionKeyFormat, EncryptionKeyFormat.pem
     )
     AUTH_PRIVATE_KEY_PASSPHRASE = confi.str("AUTH_PRIVATE_KEY_PASSPHRASE", None)
@@ -236,53 +236,48 @@
 
     SERVER_HOST = confi.str(
         "SERVER_HOST",
         "127.0.0.1",
         description="(if run via CLI)  Address for the server to bind",
     )
 
-    SERVER_PORT = confi.int(
+    SERVER_PORT = confi.str(
         "SERVER_PORT",
+        None,
+        # Users have expirienced errors when kubernetes sets the envar OPAL_SERVER_PORT="tcp://..." (which fails to parse as a port integer).
+        description="Deprecated, use SERVER_BIND_PORT instead",
+    )
+
+    SERVER_BIND_PORT = confi.int(
+        "SERVER_BIND_PORT",
         7002,
         description="(if run via CLI)  Port for the server to bind",
     )
 
     # optional APM tracing with datadog
     ENABLE_DATADOG_APM = confi.bool(
         "ENABLE_DATADOG_APM",
         False,
         description="Set if OPAL server should enable tracing with datadog APM",
     )
 
-    SERVER_ROLE = confi.enum(
-        "SERVER_ROLE",
-        ServerRole,
-        default=ServerRole.Primary,
-        description="Server is leader or follower",
-    )
-
     SCOPES = confi.bool("SCOPES", default=False)
 
     REDIS_URL = confi.str("REDIS_URL", default="redis://localhost")
 
-    CELERY_BACKEND = confi.str("CELERY_BACKEND", None)
-
     BASE_DIR = confi.str("BASE_DIR", default=pathlib.Path.home() / ".local/state/opal")
 
     POLICY_REFRESH_INTERVAL = confi.int(
         "POLICY_REFRESH_INTERVAL",
         default=0,
         description="Policy polling refresh interval",
     )
 
-    SERVER_URL = confi.str(
-        "SERVER_URL",
-        default="http://localhost:7002",
-        description="OPAL Server URL",
-    )
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-    WORKER_TOKEN = confi.str(
-        "WORKER_TOKEN", "", description="Server/Worker access token"
-    )
+        if self.SERVER_PORT is not None and self.SERVER_PORT.isdigit():
+            # Backward compatibility - if SERVER_PORT is set with a valid value, use it as SERVER_BIND_PORT
+            self.SERVER_BIND_PORT = int(self.SERVER_PORT)
 
 
 opal_server_config = OpalServerConfig(prefix="OPAL_")
```

### Comparing `opal-server-0.5.0/opal_server/data/api.py` & `opal-server-0.6.0/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/data/data_update_publisher.py` & `opal-server-0.6.0/opal_server/data/data_update_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         # Expand the topics for each event to include sub topic combos (e.g. publish 'a/b/c' as 'a' , 'a/b', and 'a/b/c')
         for entry in update.entries:
             topic_combos = []
             if entry.topics:
                 for topic in entry.topics:
                     topic_combos.extend(DataUpdatePublisher.get_topic_combos(topic))
-                entry.topics = topic_combos  # Update entry with the exaustive list, so client won't have to expand it again
+                entry.topics = topic_combos  # Update entry with the exhaustive list, so client won't have to expand it again
                 all_topic_combos.update(topic_combos)
             else:
                 logger.warning(
                     "[{pid}] No topics were provided for the following entry: {entry}",
                     pid=os.getpid(),
                     entry=entry,
                 )
@@ -119,15 +119,15 @@
         # Create new publish entry
 
         return self.publish_data_updates(
             DataUpdate(reason="Periodic Update", entries=[update])
         )
 
     def create_polling_updates(self, sources: ServerDataSourceConfig):
-        # For every entry with a non zero period update interval, bind an inverval to it
+        # For every entry with a non zero period update interval, bind an interval to it
         updaters = []
         if hasattr(sources, "config") and hasattr(sources.config, "entries"):
             for source in sources.config.entries:
                 if (
                     hasattr(source, "periodic_update_interval")
                     and isinstance(source.periodic_update_interval, float)
                     and source.periodic_update_interval is not None
```

### Comparing `opal-server-0.5.0/opal_server/git_fetcher.py` & `opal-server-0.6.0/opal_server/git_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from opal_common.logger import logger
 from opal_common.schemas.policy import PolicyBundle
 from opal_common.schemas.policy_source import (
     GitHubTokenAuthData,
     GitPolicyScopeSource,
     SSHAuthData,
 )
-from opal_common.synchronization.expiring_redis_lock import run_locked
+from opal_common.synchronization.named_lock import NamedLock
 from pygit2 import (
     KeypairFromMemory,
     RemoteCallbacks,
     Repository,
     Username,
     UserPass,
     clone_repository,
@@ -78,14 +78,21 @@
         try:
             repo.lookup_reference(f"refs/remotes/{remote}/{branch}")
             return True
         except KeyError:
             return False
 
     @staticmethod
+    def get_local_branch(repo: Repository, branch: str) -> Optional[pygit2.Reference]:
+        try:
+            return repo.lookup_reference(f"refs/heads/{branch}")
+        except KeyError:
+            return None
+
+    @staticmethod
     def get_commit_hash(repo: Repository, branch: str, remote: str) -> Optional[str]:
         try:
             (commit, _) = repo.resolve_refish(f"{remote}/{branch}")
             return commit.hex
         except (pygit2.GitError, KeyError):
             return None
 
@@ -96,19 +103,19 @@
         remote_name: str,
     ):
         ref = RepoInterface.create_local_branch_ref(repo, branch_name, remote_name)
         repo.checkout(ref)
 
     @staticmethod
     def verify_found_repo_matches_remote(
-        expected_remote_url: str, clone_path: str
+        repo: Repository,
+        expected_remote_url: str,
     ) -> Repository:
         """verifies that the repo we found in the directory matches the repo we
         are wishing to clone."""
-        repo = Repository(clone_path)
         for remote in repo.remotes:
             if remote.url == expected_remote_url:
                 logger.debug(
                     f"found target repo url is referred by remote: {remote.name}, url={remote.url}"
                 )
                 return
         error: str = f"Repo mismatch! No remote matches target url: {expected_remote_url}, found urls: {[remote.url for remote in repo.remotes]}"
@@ -128,65 +135,70 @@
         super().__init__(callbacks)
         self._base_dir = GitPolicyFetcher.base_dir(base_dir)
         self._source = source
         self._auth_callbacks = GitCallback(self._source)
         self._repo_path = GitPolicyFetcher.repo_clone_path(base_dir, self._source)
         self._remote = remote_name
         self._scope_id = scope_id
-        logger.info(
+        logger.debug(
             f"Initializing git fetcher: scope_id={scope_id}, url={source.url}, branch={self._source.branch}, path={GitPolicyFetcher.source_id(source)}"
         )
 
-    async def concurrent_fetch(self, redis: aioredis.Redis, *args, **kwargs):
-        """makes sure the repo is already fetched and is up to date.
+    async def _get_repo_lock(self):
+        locks_dir = self._base_dir / ".locks"
+        await aiofiles.os.makedirs(str(locks_dir), exist_ok=True)
 
-        A wrapper around fetch() to ensure that there are no concurrency
-        issues when trying to fetch multiple scopes that are cloned to
-        the same file system directory. We obtain safety with redis
-        locks.
-        """
-        lock_name = GitPolicyFetcher.source_id(self._source)
-        await run_locked(redis, lock_name, self.fetch(*args, **kwargs))
+        return NamedLock(
+            locks_dir / GitPolicyFetcher.source_id(self._source), attempt_interval=0.1
+        )
 
-    async def fetch(self, hinted_hash: Optional[str] = None, force_fetch: bool = False):
+    async def fetch_and_notify_on_changes(
+        self, hinted_hash: Optional[str] = None, force_fetch: bool = False
+    ):
         """makes sure the repo is already fetched and is up to date.
 
         - if no repo is found, the repo will be cloned.
         - if the repo is found and it is deemed out-of-date, the configured remote will be fetched.
         - if after a fetch new commits are detected, a callback will be triggered.
         - if the hinted commit hash is provided and is already found in the local clone
         we use this hint to avoid an necessary fetch.
         """
-        await aiofiles.os.makedirs(str(self._base_dir), exist_ok=True)
-
-        if self._discover_repository(self._repo_path):
-            logger.info("Repo found at {path}", path=self._repo_path)
-            RepoInterface.verify_found_repo_matches_remote(
-                self._source.url, str(self._repo_path)
-            )
-            repo = self._get_valid_repo_at(str(self._repo_path))
-            if repo is not None:
-                if not (
-                    await self._should_fetch(
+        repo_lock = await self._get_repo_lock()
+        async with repo_lock:
+            if self._discover_repository(self._repo_path):
+                logger.debug("Repo found at {path}", path=self._repo_path)
+                repo = self._get_valid_repo()
+                if repo is not None:
+                    should_fetch = await self._should_fetch(
                         repo, hinted_hash=hinted_hash, force_fetch=force_fetch
                     )
-                ):
-                    logger.info("Skipping fetch")
+                    if should_fetch:
+                        logger.debug(
+                            f"Fetching remote (force_fetch={force_fetch}): {self._remote} ({self._source.url})"
+                        )
+                        await run_sync(
+                            repo.remotes[self._remote].fetch,
+                            callbacks=self._auth_callbacks,
+                        )
+                        logger.debug(f"Fetch completed: {self._source.url}")
+
+                    # New commits might be present because of a previous fetch made by another scope
+                    await self._notify_on_changes(repo)
                     return
-                await self._fetch_and_notify_on_changes(repo)
-                return
+                else:
+                    # repo dir exists but invalid -> we must delete the directory
+                    logger.warning(
+                        "Deleting invalid repo: {path}", path=self._repo_path
+                    )
+                    shutil.rmtree(self._repo_path)
             else:
-                # repo dir exists but invalid -> we must delete the directory
-                logger.info("Deleting invalid repo: {path}", path=self._repo_path)
-                shutil.rmtree(self._repo_path)
-        else:
-            logger.info("Repo not found at {path}", path=self._repo_path)
+                logger.info("Repo not found at {path}", path=self._repo_path)
 
-        # fallthrough to clean clone
-        await self._clone()
+            # fallthrough to clean clone
+            await self._clone()
 
     def _discover_repository(self, path: Path) -> bool:
         git_path: Path = path / ".git"
         return discover_repository(str(path)) and git_path.exists()
 
     async def _clone(self):
         logger.info(
@@ -206,29 +218,32 @@
             logger.exception(
                 f"Could not clone repo at {self._source.url}, checkout branch={self._source.branch}"
             )
         else:
             logger.info(f"Clone completed: {self._source.url}")
             await self.callbacks.on_update(None, repo.head.target.hex)
 
-    def _get_valid_repo_at(self, path: str) -> Optional[Repository]:
+    def _get_valid_repo(self) -> Optional[Repository]:
+        path = str(self._repo_path)
+
         try:
-            return Repository(path)
+            repo = Repository(path)
+            RepoInterface.verify_found_repo_matches_remote(repo, self._source.url)
+            return repo
         except pygit2.GitError:
             logger.warning("Invalid repo at: {path}", path=path)
             return None
 
     async def _should_fetch(
         self,
         repo: Repository,
         hinted_hash: Optional[str] = None,
         force_fetch: bool = False,
     ) -> bool:
         if force_fetch:
-            logger.info("Force-fetch was requested")
             return True  # must fetch
 
         if not RepoInterface.has_remote_branch(repo, self._source.branch, self._remote):
             logger.info(
                 "Target branch was not found in local clone, re-fetching the remote"
             )
             return True  # missing branch
@@ -242,29 +257,39 @@
                     "Hinted commit hash was not found in local clone, re-fetching the remote"
                 )
                 return True  # hinted commit was not found
 
         # by default, we try to avoid re-fetching the repo for performance
         return False
 
-    async def _fetch_and_notify_on_changes(self, repo: Repository):
-        old_revision = RepoInterface.get_commit_hash(
-            repo, self._source.branch, self._remote
-        )
-        logger.info(f"Fetching remote: {self._remote} ({self._source.url})")
-        await run_sync(repo.remotes[self._remote].fetch, callbacks=self._auth_callbacks)
-        logger.info(f"Fetch completed: {self._source.url}")
+    async def _notify_on_changes(self, repo: Repository):
+        # Get the latest commit hash of the target branch
         new_revision = RepoInterface.get_commit_hash(
             repo, self._source.branch, self._remote
         )
         if new_revision is None:
             logger.error(f"Did not find target branch on remote: {self._source.branch}")
             return
+
+        # Get the previous commit hash of the target branch
+        local_branch = RepoInterface.get_local_branch(repo, self._source.branch)
+        if local_branch is None:
+            # First sync of a new branch (the first synced branch in this repo was set by the clone (see `checkout_branch`))
+            old_revision = None
+            local_branch = RepoInterface.create_local_branch_ref(
+                repo, self._source.branch, self._remote, self._source.branch
+            )
+        else:
+            old_revision = local_branch.target.hex
+
         await self.callbacks.on_update(old_revision, new_revision)
 
+        # Bring forward local branch (a bit like "pull"), so we won't detect changes again
+        local_branch.set_target(new_revision)
+
     def _get_current_branch_head(self) -> str:
         repo = Repository(str(self._repo_path))
         head_commit_hash = RepoInterface.get_commit_hash(
             repo, self._source.branch, self._remote
         )
         if not head_commit_hash:
             logger.error("Could not find current branch head")
```

### Comparing `opal-server-0.5.0/opal_server/loadlimiting.py` & `opal-server-0.6.0/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/policy/bundles/api.py` & `opal-server-0.6.0/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/policy/watcher/callbacks.py` & `opal-server-0.6.0/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/policy/watcher/factory.py` & `opal-server-0.6.0/opal_server/policy/watcher/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 from functools import partial
 from typing import Any, List, Optional
 
-from fastapi_websocket_pubsub import Topic
+from fastapi_websocket_pubsub.pub_sub_server import PubSubEndpoint
 from opal_common.confi.confi import load_conf_if_none
 from opal_common.git.repo_cloner import RepoClonePathFinder
 from opal_common.logger import logger
 from opal_common.sources.api_policy_source import ApiPolicySource
 from opal_common.sources.git_policy_source import GitPolicySource
 from opal_common.topics.publisher import TopicPublisher
 from opal_server.config import PolicySourceTypes, opal_server_config
 from opal_server.policy.watcher.callbacks import publish_changed_directories
-from opal_server.policy.watcher.task import PolicyWatcherTask
+from opal_server.policy.watcher.task import BasePolicyWatcherTask, PolicyWatcherTask
+from opal_server.scopes.task import ScopesPolicyWatcherTask
 
 
 def setup_watcher_task(
     publisher: TopicPublisher,
+    pubsub_endpoint: PubSubEndpoint,
     source_type: str = None,
     remote_source_url: str = None,
     clone_path_finder: RepoClonePathFinder = None,
     branch_name: str = None,
     ssh_key: Optional[str] = None,
     polling_interval: int = None,
     request_timeout: int = None,
     policy_bundle_token: str = None,
     extensions: Optional[List[str]] = None,
     bundle_ignore: Optional[List[str]] = None,
-) -> PolicyWatcherTask:
+) -> BasePolicyWatcherTask:
     """Create a PolicyWatcherTask with Git / API policy source defined by env
     vars Load all the defaults from config if called without params.
 
     Args:
         publisher(TopicPublisher): server side publisher to publish changes in policy
         source_type(str): policy source type, can be Git / Api to opa bundle server
         remote_source_url(str): the base address to request the policy from
         clone_path_finder(RepoClonePathFinder): from which the local dir path for the repo clone would be retrieved
         branch_name(str):  name of remote branch in git to pull
         ssh_key (str, optional): private ssh key used to gain access to the cloned repo
         polling_interval(int):  how many seconds need to wait between polling
-        request_timeout(int):  how many seconds need to wait until timout
+        request_timeout(int):  how many seconds need to wait until timeout
         policy_bundle_token(int):  auth token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
         extensions(list(str), optional):  list of extantions to check when new policy arrive default is OPA_FILE_EXTENSIONS
         bundle_ignore(list(str), optional):  list of glob paths to use for excluding files from bundle default is OPA_BUNDLE_IGNORE
     """
+    if opal_server_config.SCOPES:
+        return ScopesPolicyWatcherTask(pubsub_endpoint)
+
     # load defaults
     source_type = load_conf_if_none(source_type, opal_server_config.POLICY_SOURCE_TYPE)
+
     clone_path_finder = load_conf_if_none(
         clone_path_finder,
         RepoClonePathFinder(
             base_clone_path=opal_server_config.POLICY_REPO_CLONE_PATH,
             clone_subdirectory_prefix=opal_server_config.POLICY_REPO_CLONE_FOLDER_PREFIX,
             use_fixed_path=opal_server_config.POLICY_REPO_REUSE_CLONE_PATH,
         ),
     )
-    clone_path = clone_path_finder.get_clone_path()
-    if not clone_path:
-        # we should never see this warning
-        logger.warning(
-            "Policy repo clone path was not found when setting up policy source!! recreating clone path..."
-        )
-        clone_path = clone_path_finder.create_new_clone_path()
+
+    clone_path = (
+        clone_path_finder.get_clone_path() or clone_path_finder.create_new_clone_path()
+    )
+    logger.info(f"Policy repo will be cloned to: {clone_path}")
+
     branch_name = load_conf_if_none(
         branch_name, opal_server_config.POLICY_REPO_MAIN_BRANCH
     )
     ssh_key = load_conf_if_none(ssh_key, opal_server_config.POLICY_REPO_SSH_KEY)
     polling_interval = load_conf_if_none(
         polling_interval, opal_server_config.POLICY_REPO_POLLING_INTERVAL
     )
@@ -112,19 +117,8 @@
         partial(
             publish_changed_directories,
             publisher=publisher,
             file_extensions=extensions,
             bundle_ignore=bundle_ignore,
         )
     )
-    return PolicyWatcherTask(watcher)
-
-
-async def trigger_repo_watcher_pull(
-    watcher: PolicyWatcherTask, topic: Topic, data: Any
-):
-    """triggers the policy watcher check for changes.
-
-    will trigger a task on the watcher's thread.
-    """
-    logger.info("webhook listener triggered")
-    watcher.trigger()
+    return PolicyWatcherTask(watcher, pubsub_endpoint)
```

### Comparing `opal-server-0.5.0/opal_server/policy/webhook/api.py` & `opal-server-0.6.0/opal_server/policy/webhook/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,17 @@
                 logger.error(
                     "Webhook config is missing both event_request_key and event_header_name. Must have at least one."
                 )
 
             policy_repo_url = opal_server_config.POLICY_REPO_URL
 
             # Check if the URL we are tracking is mentioned in the webhook
-            if policy_repo_url and is_matching_webhook_url(
-                policy_repo_url, urls, names
+            if policy_repo_url and (
+                is_matching_webhook_url(policy_repo_url, urls, names)
+                or not webhook_config.match_sender_url
             ):
                 logger.info(
                     "triggered webhook on repo: {repo}",
                     repo=opal_server_config.POLICY_REPO_URL,
                     hook_event=event,
                 )
                 # Check if this it the right event (push)
```

### Comparing `opal-server-0.5.0/opal_server/policy/webhook/deps.py` & `opal-server-0.6.0/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/policy/webhook/listener.py` & `opal-server-0.6.0/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/publisher.py` & `opal-server-0.6.0/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/pubsub.py` & `opal-server-0.6.0/opal_server/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from opal_common.confi.confi import load_conf_if_none
 from opal_common.config import opal_common_config
 from opal_common.logger import logger
 from opal_server.config import opal_server_config
 
 
 class PubSub:
-    """Warpper for the Pub/Sub channel used for both policy and data
+    """Wrapper for the Pub/Sub channel used for both policy and data
     updates."""
 
     def __init__(self, signer: JWTSigner, broadcaster_uri: str = None):
         """
         Args:
             broadcaster_uri (str, optional): Which server/medium should the PubSub use for broadcasting. Defaults to BROADCAST_URI.
             None means no broadcasting.
```

### Comparing `opal-server-0.5.0/opal_server/redis.py` & `opal-server-0.6.0/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/scopes/api.py` & `opal-server-0.6.0/opal_server/scopes/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,31 +8,41 @@
     Header,
     HTTPException,
     Path,
     Query,
     Response,
     status,
 )
+from fastapi.responses import RedirectResponse
 from fastapi_websocket_pubsub import PubSubEndpoint
 from git import InvalidGitRepositoryError
+from opal_common.async_utils import run_sync
 from opal_common.authentication.authz import (
     require_peer_type,
     restrict_optional_topics_to_publish,
 )
 from opal_common.authentication.casting import cast_private_key
-from opal_common.authentication.deps import JWTAuthenticator
+from opal_common.authentication.deps import JWTAuthenticator, get_token_from_header
 from opal_common.authentication.types import EncryptionKeyFormat, JWTClaims
 from opal_common.authentication.verifier import Unauthorized
 from opal_common.logger import logger
-from opal_common.schemas.data import DataSourceConfig, DataUpdate
+from opal_common.schemas.data import (
+    DataSourceConfig,
+    DataUpdate,
+    ServerDataSourceConfig,
+)
 from opal_common.schemas.policy import PolicyBundle, PolicyUpdateMessageNotification
 from opal_common.schemas.policy_source import GitPolicyScopeSource, SSHAuthData
 from opal_common.schemas.scopes import Scope
 from opal_common.schemas.security import PeerType
-from opal_common.topics.publisher import ScopedServerSideTopicPublisher
+from opal_common.topics.publisher import (
+    ScopedServerSideTopicPublisher,
+    ServerSideTopicPublisher,
+)
+from opal_common.urls import set_url_query_param
 from opal_server.config import opal_server_config
 from opal_server.data.data_update_publisher import DataUpdatePublisher
 from opal_server.git_fetcher import GitPolicyFetcher
 from opal_server.scopes.scope_repository import ScopeNotFoundError, ScopeRepository
 
 
 def verify_private_key(private_key: str, key_format: EncryptionKeyFormat) -> bool:
@@ -62,38 +72,31 @@
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail={"error": "private key is invalid"},
             )
 
 
 def init_scope_router(
-    scopes: ScopeRepository, authenticator: JWTAuthenticator, pubsub: PubSubEndpoint
+    scopes: ScopeRepository,
+    authenticator: JWTAuthenticator,
+    pubsub_endpoint: PubSubEndpoint,
 ):
     router = APIRouter()
 
     def _allowed_scoped_authenticator(
         claims: JWTClaims = Depends(authenticator), scope_id: str = Path(...)
     ):
         if not authenticator.enabled:
             return
 
         allowed_scopes = claims.get("allowed_scopes")
 
         if not allowed_scopes or scope_id not in allowed_scopes:
             raise HTTPException(status.HTTP_403_FORBIDDEN)
 
-    def _check_worker_token(authorization: str = Header()):
-        if authorization is None:
-            raise Unauthorized()
-
-        scheme, token = authorization.split(" ")
-
-        if scheme.lower() != "bearer" or token != opal_server_config.WORKER_TOKEN:
-            raise Unauthorized()
-
     @router.put("", status_code=status.HTTP_201_CREATED)
     async def put_scope(
         *,
         force_fetch: bool = Query(
             False,
             description="Whether the policy repo must be fetched from remote",
         ),
@@ -108,17 +111,19 @@
 
         verify_private_key_or_throw(scope_in)
         await scopes.put(scope_in)
 
         force_fetch_str = " (force fetch)" if force_fetch else ""
         logger.info(f"Sync scope: {scope_in.scope_id}{force_fetch_str}")
 
-        from opal_server.worker import sync_scope
-
-        sync_scope.delay(scope_in.scope_id, force_fetch=force_fetch)
+        # All server replicas (leaders) should sync the scope.
+        await pubsub_endpoint.publish(
+            opal_server_config.POLICY_REPO_WEBHOOK_TOPIC,
+            {"scope_id": scope_in.scope_id, "force_fetch": force_fetch},
+        )
 
         return Response(status_code=status.HTTP_201_CREATED)
 
     @router.get(
         "",
         response_model=List[Scope],
         response_model_exclude={"policy": {"auth"}},
@@ -161,20 +166,17 @@
     ):
         try:
             require_peer_type(authenticator, claims, PeerType.datasource)
         except Unauthorized as ex:
             logger.error(f"Unauthorized to delete scope: {repr(ex)}")
             raise
 
+        # TODO: This should also asynchronously clean the repo from the disk (if it's not used by other scopes)
         await scopes.delete(scope_id)
 
-        from opal_server.worker import delete_scope
-
-        delete_scope.delay(scope_id)
-
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.post("/{scope_id}/refresh", status_code=status.HTTP_200_OK)
     async def refresh_scope(
         scope_id: str,
         hinted_hash: Optional[str] = Query(
             None,
@@ -191,20 +193,27 @@
             raise
 
         try:
             _ = await scopes.get(scope_id)
 
             logger.info(f"Refresh scope: {scope_id}")
 
-            from opal_server.worker import sync_scope
-
             # If the hinted hash is None, we have no way to know whether we should
             # re-fetch the remote, so we force fetch, just in case.
             force_fetch = hinted_hash is None
-            sync_scope.delay(scope_id, hinted_hash=hinted_hash, force_fetch=force_fetch)
+
+            # All server replicas (leaders) should sync the scope.
+            await pubsub_endpoint.publish(
+                opal_server_config.POLICY_REPO_WEBHOOK_TOPIC,
+                {
+                    "scope_id": scope_id,
+                    "force_fetch": force_fetch,
+                    "hinted_hash": hinted_hash,
+                },
+            )
 
             return Response(status_code=status.HTTP_200_OK)
 
         except ScopeNotFoundError:
             raise HTTPException(
                 status.HTTP_404_NOT_FOUND, detail=f"No such scope: {scope_id}"
             )
@@ -214,17 +223,16 @@
         """sync all scopes."""
         try:
             require_peer_type(authenticator, claims, PeerType.datasource)
         except Unauthorized as ex:
             logger.error(f"Unauthorized to refresh all scopes: {repr(ex)}")
             raise
 
-        from opal_server.worker import schedule_sync_all_scopes
-
-        await schedule_sync_all_scopes(scopes)
+        # All server replicas (leaders) should sync all scopes.
+        await pubsub_endpoint.publish(opal_server_config.POLICY_REPO_WEBHOOK_TOPIC)
 
         return Response(status_code=status.HTTP_200_OK)
 
     @router.get(
         "/{scope_id}/policy",
         response_model=PolicyBundle,
         status_code=status.HTTP_200_OK,
@@ -237,65 +245,92 @@
             None,
             description="hash of previous bundle already downloaded, server will return a diff bundle.",
         ),
     ):
         try:
             scope = await scopes.get(scope_id)
         except ScopeNotFoundError:
-            raise HTTPException(
-                status.HTTP_404_NOT_FOUND, detail=f"No such scope: {scope_id}"
+            logger.warning(
+                "Requested scope {scope_id} not found, returning default scope",
+                scope_id=scope_id,
             )
+            return await _generate_default_scope_bundle(scope_id)
 
         if not isinstance(scope.policy, GitPolicyScopeSource):
             raise HTTPException(
                 status.HTTP_501_NOT_IMPLEMENTED,
                 detail=f"policy source is not yet implemented: {scope_id}",
             )
 
         fetcher = GitPolicyFetcher(
             pathlib.Path(opal_server_config.BASE_DIR),
             scope.scope_id,
             cast(GitPolicyScopeSource, scope.policy),
         )
 
         try:
-            return fetcher.make_bundle(base_hash)
+            return await run_sync(fetcher.make_bundle, base_hash)
         except (InvalidGitRepositoryError, pygit2.GitError, ValueError):
-            raise HTTPException(
-                status.HTTP_503_SERVICE_UNAVAILABLE,
-                detail=f"scope is not yet cloned: {scope_id}",
+            logger.warning(
+                "Requested scope {scope_id} has invalid repo, returning default scope",
+                scope_id=scope_id,
             )
+            return await _generate_default_scope_bundle(scope_id)
+
+    async def _generate_default_scope_bundle(scope_id: str) -> PolicyBundle:
+        try:
+            scope = await scopes.get("default")
+            fetcher = GitPolicyFetcher(
+                pathlib.Path(opal_server_config.BASE_DIR),
+                scope.scope_id,
+                cast(GitPolicyScopeSource, scope.policy),
+            )
+            return fetcher.make_bundle(None)
+        except (
+            ScopeNotFoundError,
+            InvalidGitRepositoryError,
+            pygit2.GitError,
+            ValueError,
+        ):
+            raise ScopeNotFoundError(scope_id)
 
     @router.get(
         "/{scope_id}/data",
         response_model=DataSourceConfig,
         status_code=status.HTTP_200_OK,
         dependencies=[Depends(_allowed_scoped_authenticator)],
     )
-    async def get_scope_data_config(*, scope_id: str = Path(..., title="Scope ID")):
+    async def get_scope_data_config(
+        *,
+        scope_id: str = Path(..., title="Scope ID"),
+        authorization: Optional[str] = Header(None),
+    ):
         logger.info(
             "Serving source configuration for scope {scope_id}", scope_id=scope_id
         )
-        scope = await scopes.get(scope_id)
-        return scope.data
+        try:
+            scope = await scopes.get(scope_id)
+            return scope.data
+        except ScopeNotFoundError as ex:
+            logger.warning(
+                "Requested scope {scope_id} not found, returning OPAL_DATA_CONFIG_SOURCES",
+                scope_id=scope_id,
+            )
+            try:
+                config: ServerDataSourceConfig = opal_server_config.DATA_CONFIG_SOURCES
 
-    @router.post(
-        "/{scope_id}/policy/update",
-        status_code=status.HTTP_204_NO_CONTENT,
-        dependencies=[Depends(_check_worker_token)],
-    )
-    async def notify_new_policy(
-        *,
-        scope_id: str = Path(..., description="Scope ID"),
-        notification: PolicyUpdateMessageNotification,
-    ):
-        async with ScopedServerSideTopicPublisher(pubsub, scope_id) as publisher:
-            publisher.publish(notification.topics, notification.update)
-            await publisher.wait()
-        return Response(status_code=status.HTTP_204_NO_CONTENT)
+                if config.external_source_url:
+                    url = str(config.external_source_url)
+                    token = get_token_from_header(authorization)
+                    redirect_url = set_url_query_param(url, "token", token)
+                    return RedirectResponse(url=redirect_url)
+                else:
+                    return config.config
+            except ScopeNotFoundError:
+                raise HTTPException(status.HTTP_404_NOT_FOUND, detail=str(ex))
 
     @router.post("/{scope_id}/data/update")
     async def publish_data_update_event(
         update: DataUpdate,
         claims: JWTClaims = Depends(authenticator),
         scope_id: str = Path(..., description="Scope ID"),
     ):
@@ -303,14 +338,16 @@
             require_peer_type(authenticator, claims, PeerType.datasource)
 
             restrict_optional_topics_to_publish(authenticator, claims, update)
 
             for entry in update.entries:
                 entry.topics = [f"data:{topic}" for topic in entry.topics]
 
-            async with ScopedServerSideTopicPublisher(pubsub, scope_id) as publisher:
+            async with ScopedServerSideTopicPublisher(
+                pubsub_endpoint, scope_id
+            ) as publisher:
                 DataUpdatePublisher(publisher).publish_data_updates(update)
         except Unauthorized as ex:
             logger.error(f"Unauthorized to publish update: {repr(ex)}")
             raise
 
     return router
```

### Comparing `opal-server-0.5.0/opal_server/scopes/loader.py` & `opal-server-0.6.0/opal_server/scopes/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from opal_server.config import ServerRole, opal_server_config
 from opal_server.scopes.scope_repository import ScopeRepository
 
 DEFAULT_SCOPE_ID = "default"
 
 
 async def load_scopes(repo: ScopeRepository):
-    if opal_server_config.SERVER_ROLE == ServerRole.Primary:
-        logger.info("Server is primary, loading default scope.")
-        await _load_env_scope(repo)
+    logger.info("Server is primary, loading default scope.")
+    await _load_env_scope(repo)
 
 
 async def _load_env_scope(repo: ScopeRepository):
     # backwards compatible opal scope
     if opal_server_config.POLICY_REPO_URL is not None:
         logger.info(
             "Adding default scope from env: {url}",
```

### Comparing `opal-server-0.5.0/opal_server/scopes/scope_repository.py` & `opal-server-0.6.0/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/security/api.py` & `opal-server-0.6.0/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/security/jwks.py` & `opal-server-0.6.0/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/server.py` & `opal-server-0.6.0/opal_server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,49 +2,45 @@
 import os
 import sys
 import traceback
 from functools import partial
 from typing import List, Optional
 
 from fastapi import Depends, FastAPI
-from fastapi_utils.tasks import repeat_every
 from fastapi_websocket_pubsub.event_broadcaster import EventBroadcasterContextManager
 from opal_common.authentication.deps import JWTAuthenticator, StaticBearerAuthenticator
 from opal_common.authentication.signer import JWTSigner
 from opal_common.confi.confi import load_conf_if_none
 from opal_common.config import opal_common_config
-from opal_common.git.repo_cloner import RepoClonePathFinder
 from opal_common.logger import configure_logs, logger
 from opal_common.middleware import configure_middleware
 from opal_common.schemas.data import ServerDataSourceConfig
-from opal_common.schemas.policy_source import SSHAuthData
 from opal_common.synchronization.named_lock import NamedLock
 from opal_common.topics.publisher import (
     PeriodicPublisher,
     ServerSideTopicPublisher,
     TopicPublisher,
 )
 from opal_server.config import opal_server_config
 from opal_server.data.api import init_data_updates_router
 from opal_server.data.data_update_publisher import DataUpdatePublisher
 from opal_server.loadlimiting import init_loadlimit_router
 from opal_server.policy.bundles.api import router as bundles_router
-from opal_server.policy.watcher import setup_watcher_task, trigger_repo_watcher_pull
+from opal_server.policy.watcher.factory import setup_watcher_task
 from opal_server.policy.watcher.task import PolicyWatcherTask
 from opal_server.policy.webhook.api import init_git_webhook_router
 from opal_server.publisher import setup_broadcaster_keepalive_task
 from opal_server.pubsub import PubSub
 from opal_server.redis import RedisDB
 from opal_server.scopes.api import init_scope_router
-from opal_server.scopes.loader import DEFAULT_SCOPE_ID, load_scopes
-from opal_server.scopes.scope_repository import ScopeNotFoundError, ScopeRepository
+from opal_server.scopes.loader import load_scopes
+from opal_server.scopes.scope_repository import ScopeRepository
 from opal_server.security.api import init_security_router
 from opal_server.security.jwks import JwksStaticEndpoint
 from opal_server.statistics import OpalStatistics, init_statistics_router
-from opal_server.worker import schedule_sync_all_scopes
 
 
 class OpalServer:
     def __init__(
         self,
         init_policy_watcher: bool = None,
         policy_remote_url: str = None,
@@ -104,16 +100,14 @@
         )
         self.loadlimit_notation: str = load_conf_if_none(
             loadlimit_notation, opal_server_config.CLIENT_LOAD_LIMIT_NOTATION
         )
         self._policy_remote_url = policy_remote_url
 
         configure_logs()
-        self.watcher: Optional[PolicyWatcherTask] = None
-        self.leadership_lock: Optional[NamedLock] = None
 
         self.data_sources_config: ServerDataSourceConfig = (
             data_sources_config
             if data_sources_config is not None
             else opal_server_config.DATA_CONFIG_SOURCES
         )
 
@@ -165,25 +159,26 @@
 
         if opal_common_config.STATISTICS_ENABLED:
             self.opal_statistics = OpalStatistics(self.pubsub.endpoint)
         else:
             self.opal_statistics = None
 
         # if stats are enabled, the server workers must be listening on the broadcast
-        # channel for their own syncronization, not just for their clients. therefore
+        # channel for their own synchronization, not just for their clients. therefore
         # we need a "global" listening context
         self.broadcast_listening_context: Optional[
             EventBroadcasterContextManager
         ] = None
         if self.broadcaster_uri is not None and opal_common_config.STATISTICS_ENABLED:
             self.broadcast_listening_context = (
                 self.pubsub.endpoint.broadcaster.get_listening_context()
             )
 
-        self.watcher: Optional[PolicyWatcherTask] = None
+        self.watcher: PolicyWatcherTask = None
+        self.leadership_lock: Optional[NamedLock] = None
 
         if opal_server_config.SCOPES:
             self._redis_db = RedisDB(opal_server_config.REDIS_URL)
             self._scopes = ScopeRepository(self._redis_db)
             logger.info("OPAL Scopes: server is connected to scopes repository")
 
         # init fastapi app
@@ -288,15 +283,14 @@
         """
 
         @app.on_event("startup")
         async def startup_event():
             logger.info("*** OPAL Server Startup ***")
 
             try:
-                await self.start()
                 self._task = asyncio.create_task(self.start_server_background_tasks())
 
             except Exception:
                 logger.critical("Exception while starting OPAL")
                 traceback.print_exc()
 
                 sys.exit(1)
@@ -304,19 +298,14 @@
         @app.on_event("shutdown")
         async def shutdown_event():
             logger.info("triggered shutdown event")
             await self.stop_server_background_tasks()
 
         return app
 
-    async def start(self):
-        if opal_server_config.SCOPES:
-            await load_scopes(self._scopes)
-            await schedule_sync_all_scopes(self._scopes)
-
     async def start_server_background_tasks(self):
         """starts the background processes (as asyncio tasks) if such are
         configured.
 
         all workers will start these tasks:
         - publisher: a client that is used to publish updates to the client.
 
@@ -331,72 +320,51 @@
                             "listening on broadcast channel for statistics events..."
                         )
                         await self.broadcast_listening_context.__aenter__()
                     asyncio.create_task(self.opal_statistics.run())
                     self.pubsub.endpoint.notifier.register_unsubscribe_event(
                         self.opal_statistics.remove_client
                     )
-                if self._init_policy_watcher:
-                    # repo watcher is enabled, but we want only one worker to run it
-                    # (otherwise for each new commit, we will publish multiple updates via pub/sub).
-                    # leadership is determined by the first worker to obtain a lock
-                    self.leadership_lock = NamedLock(
-                        opal_server_config.LEADER_LOCK_FILE_PATH
+
+                # We want only one worker to run repo watchers
+                # (otherwise for each new commit, we will publish multiple updates via pub/sub).
+                # leadership is determined by the first worker to obtain a lock
+                self.leadership_lock = NamedLock(
+                    opal_server_config.LEADER_LOCK_FILE_PATH
+                )
+                async with self.leadership_lock:
+                    # only one worker gets here, the others block. in case the leader worker
+                    # is terminated, another one will obtain the lock and become leader.
+                    logger.info(
+                        "leadership lock acquired, leader pid: {pid}",
+                        pid=os.getpid(),
                     )
-                    async with self.leadership_lock:
-                        # only one worker gets here, the others block. in case the leader worker
-                        # is terminated, another one will obtain the lock and become leader.
-                        logger.info(
-                            "leadership lock acquired, leader pid: {pid}",
-                            pid=os.getpid(),
-                        )
-                        logger.info(
-                            "listening on webhook topic: '{topic}'",
-                            topic=opal_server_config.POLICY_REPO_WEBHOOK_TOPIC,
-                        )
+
+                    if not opal_server_config.SCOPES:
                         # bind data updater publishers to the leader worker
                         asyncio.create_task(
                             DataUpdatePublisher.mount_and_start_polling_updates(
                                 self.publisher, opal_server_config.DATA_CONFIG_SOURCES
                             )
                         )
+                    else:
+                        await load_scopes(self._scopes)
 
-                        # init policy watcher
-                        if self.watcher is None:
-                            clone_path_finder = RepoClonePathFinder(
-                                base_clone_path=opal_server_config.POLICY_REPO_CLONE_PATH,
-                                clone_subdirectory_prefix=opal_server_config.POLICY_REPO_CLONE_FOLDER_PREFIX,
-                                use_fixed_path=opal_server_config.POLICY_REPO_REUSE_CLONE_PATH,
-                            )
-                            # only the leader should create new clone path and discard previous ones
-                            full_local_repo_path = (
-                                clone_path_finder.create_new_clone_path()
-                            )
-                            logger.info(
-                                f"Policy repo will be cloned to: {full_local_repo_path}"
-                            )
-
-                            self.watcher = setup_watcher_task(
-                                self.publisher,
-                                remote_source_url=opal_server_config.POLICY_REPO_URL,
-                                ssh_key=opal_server_config.POLICY_REPO_SSH_KEY,
-                                branch_name=opal_server_config.POLICY_REPO_MAIN_BRANCH,
-                                clone_path_finder=clone_path_finder,
-                            )
-
-                        # the leader listens to the webhook topic (webhook api route can be hit randomly in all workers)
-                        # and triggers the watcher to check for changes in the tracked upstream remote.
-                        await self.pubsub.endpoint.subscribe(
-                            [opal_server_config.POLICY_REPO_WEBHOOK_TOPIC],
-                            partial(trigger_repo_watcher_pull, self.watcher),
+                    if self.broadcast_keepalive is not None:
+                        self.broadcast_keepalive.start()
+                        if not self._init_policy_watcher:
+                            # Wait on keepalive instead to keep leadership lock acquired
+                            await self.broadcast_keepalive.wait_until_done()
+
+                    if self._init_policy_watcher:
+                        self.watcher = setup_watcher_task(
+                            self.publisher, self.pubsub.endpoint
                         )
                         # running the watcher, and waiting until it stops (until self.watcher.signal_stop() is called)
                         async with self.watcher:
-                            if self.broadcast_keepalive is not None:
-                                self.broadcast_keepalive.start()
                             await self.watcher.wait_until_should_stop()
 
                 if (
                     self.opal_statistics is not None
                     and self.broadcast_listening_context is not None
                 ):
                     await self.broadcast_listening_context.__aexit__()
```

### Comparing `opal-server-0.5.0/opal_server/statistics.py` & `opal-server-0.6.0/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.5.0/opal_server/worker.py` & `opal-server-0.6.0/opal_server/scopes/service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import shutil
 from functools import partial
 from pathlib import Path
 from typing import List, Optional, Set, cast
 
 import git
-from aiohttp import ClientError, ClientSession
-from asgiref.sync import async_to_sync
-from celery import Celery
-from fastapi import status
+from fastapi_websocket_pubsub import PubSubEndpoint
 from opal_common.git.commit_viewer import VersionedFile
-from opal_common.logger import configure_logs, logger
+from opal_common.logger import logger
 from opal_common.schemas.policy import PolicyUpdateMessageNotification
 from opal_common.schemas.policy_source import GitPolicyScopeSource
-from opal_common.schemas.scopes import Scope
-from opal_common.utils import get_authorization_header, tuple_to_dict
-from opal_server.config import opal_server_config
+from opal_common.topics.publisher import ScopedServerSideTopicPublisher
 from opal_server.git_fetcher import GitPolicyFetcher, PolicyFetcherCallbacks
 from opal_server.policy.watcher.callbacks import (
     create_policy_update,
     create_update_all_directories_in_repo,
 )
-from opal_server.redis import RedisDB
 from opal_server.scopes.scope_repository import ScopeRepository
 
 
 def is_rego_source_file(
     f: VersionedFile, extensions: Optional[List[str]] = None
 ) -> bool:
     """filters only rego files or data.json files."""
@@ -41,20 +35,20 @@
 
 class NewCommitsCallbacks(PolicyFetcherCallbacks):
     def __init__(
         self,
         base_dir: Path,
         scope_id: str,
         source: GitPolicyScopeSource,
-        http: ClientSession,
+        pubsub_endpoint: PubSubEndpoint,
     ):
         self._scope_repo_dir = GitPolicyFetcher.repo_clone_path(base_dir, source)
         self._scope_id = scope_id
         self._source = source
-        self._http = http
+        self._pubsub_endpoint = pubsub_endpoint
 
     async def on_update(self, previous_head: str, head: str):
         if previous_head == head:
             logger.info(
                 f"scope '{self._scope_id}': No new commits, HEAD is at '{head}'"
             )
             return
@@ -93,210 +87,125 @@
         if notification is not None:
             await self.trigger_notification(notification)
 
     async def trigger_notification(self, notification: PolicyUpdateMessageNotification):
         logger.info(
             f"Triggering policy update for scope {self._scope_id}: {notification.dict()}"
         )
-
-        url = f"{opal_server_config.SERVER_URL}/scopes/{self._scope_id}/policy/update"
-        try:
-            async with self._http.post(
-                url,
-                json=notification.dict(),
-                headers=tuple_to_dict(
-                    get_authorization_header(opal_server_config.WORKER_TOKEN)
-                ),
-            ) as response:
-                if response.status == status.HTTP_204_NO_CONTENT:
-                    logger.debug(
-                        f"triggered policy notification for {self._scope_id} via the api"
-                    )
-                else:
-                    logger.error(
-                        f"could not trigger policy notification for {self._scope_id} via the api, got status={response.status}"
-                    )
-        except ClientError as e:
-            logger.error("opal server connection error: {err}", err=repr(e))
+        async with ScopedServerSideTopicPublisher(
+            self._pubsub_endpoint, self._scope_id
+        ) as publisher:
+            publisher.publish(notification.topics, notification.update)
+            await publisher.wait()
 
 
-class Worker:
-    def __init__(self, base_dir: Path, scopes: ScopeRepository):
+class ScopesService:
+    def __init__(
+        self,
+        base_dir: Path,
+        scopes: ScopeRepository,
+        pubsub_endpoint: PubSubEndpoint,
+    ):
         self._base_dir = base_dir
         self._scopes = scopes
-        self._http: Optional[ClientSession] = None
-
-    async def __aenter__(self):
-        await self.start()
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.stop()
-
-    async def start(self):
-        self._http = ClientSession()
-
-    async def stop(self):
-        await self._http.close()
+        self._pubsub_endpoint = pubsub_endpoint
 
     async def sync_scope(
         self,
         scope_id: str,
         hinted_hash: Optional[str] = None,
         force_fetch: bool = False,
+        notify_on_changes: bool = True,
     ):
-        logger.info(f"Sync scope: {scope_id}")
         scope = await self._scopes.get(scope_id)
 
         if not isinstance(scope.policy, GitPolicyScopeSource):
             logger.warning("Non-git scopes are currently not supported!")
             return
-
         source = cast(GitPolicyScopeSource, scope.policy)
+
+        logger.info(
+            f"Sync scope: {scope_id} (remote: {source.url}, branch: {source.branch})"
+        )
+
+        callbacks = PolicyFetcherCallbacks()
+        if notify_on_changes:
+            callbacks = NewCommitsCallbacks(
+                base_dir=self._base_dir,
+                scope_id=scope_id,
+                source=source,
+                pubsub_endpoint=self._pubsub_endpoint,
+            )
+
         fetcher = GitPolicyFetcher(
             self._base_dir,
             scope_id,
             source,
-            callbacks=NewCommitsCallbacks(
-                base_dir=self._base_dir,
-                scope_id=scope_id,
-                source=source,
-                http=self._http,
-            ),
+            callbacks=callbacks,
         )
 
         try:
-            # using concurrent fetch so that if the celery worker is spawn with concurrency > 1,
-            # the competing processes will not modify the same dir on the filesystem at the same time
-            await fetcher.concurrent_fetch(
-                redis=self._scopes.db.redis_connection,
+            await fetcher.fetch_and_notify_on_changes(
                 hinted_hash=hinted_hash,
                 force_fetch=force_fetch,
             )
         except Exception as e:
             logger.exception(
                 f"Could not fetch policy for scope {scope_id}, got error: {e}"
             )
 
     async def delete_scope(self, scope_id: str):
         logger.info(f"Delete scope: {scope_id}")
         scope = await self._scopes.get(scope_id)
         url = scope.policy.url
 
         scopes = await self._scopes.all()
+        remove_repo_clone = True
 
         for scope in scopes:
             if scope.scope_id != scope_id and scope.policy.url == url:
                 logger.info(
-                    f"found another scope with same remote url: {scope.scope_id}"
+                    f"found another scope with same remote url ({scope.scope_id}), skipping clone deletion"
                 )
-                return
-
-        scope_dir = GitPolicyFetcher.repo_clone_path(
-            self._base_dir, cast(GitPolicyScopeSource, scope.policy)
-        )
-        shutil.rmtree(scope_dir, ignore_errors=True)
+                remove_repo_clone = False
+                break
 
-    async def periodic_check(self):
-        logger.info("Polling OPAL scopes for policy changes")
-        scopes = await self._scopes.all()
-
-        already_fetched = set()
-        for scope in scopes:
-            if scope.policy.poll_updates and scope.policy.url not in already_fetched:
-                logger.info(
-                    f"triggering sync_scope for scope {scope.scope_id} (remote: {scope.policy.url})"
-                )
-                sync_scope.delay(scope.scope_id, force_fetch=True)
-                already_fetched.add(scope.policy.url)
-
-
-def create_worker() -> Worker:
-    opal_base_dir = Path(opal_server_config.BASE_DIR)
-
-    worker = Worker(
-        base_dir=opal_base_dir,
-        scopes=ScopeRepository(RedisDB(opal_server_config.REDIS_URL)),
-    )
-
-    return worker
-
-
-def with_worker(f):
-    async def _inner(*args, **kwargs):
-        async with create_worker() as worker:
-            await f(worker, *args, **kwargs)
-
-    return _inner
+        if remove_repo_clone:
+            scope_dir = GitPolicyFetcher.repo_clone_path(
+                self._base_dir, cast(GitPolicyScopeSource, scope.policy)
+            )
+            shutil.rmtree(scope_dir, ignore_errors=True)
 
+        await self._scopes.delete(scope_id)
 
-configure_logs()
-app = Celery(
-    "opal-worker",
-    broker=opal_server_config.REDIS_URL,
-    # if none, no results backend is used
-    backend=opal_server_config.CELERY_BACKEND,
-)
-app.conf.task_default_queue = "opal-worker"
-app.conf.task_serializer = "json"
-
+    async def sync_scopes(self, only_poll_updates=False, notify_on_changes=True):
+        scopes = await self._scopes.all()
+        if only_poll_updates:
+            # Only sync scopes that have polling enabled (in a periodic check)
+            scopes = [scope for scope in scopes if scope.policy.poll_updates]
 
-@app.on_after_configure.connect
-def setup_periodic_tasks(sender, **kwargs):
-    polling_interval = opal_server_config.POLICY_REFRESH_INTERVAL
-    if polling_interval == 0:
-        logger.info("OPAL scopes: polling task is off.")
-    else:
         logger.info(
-            f"OPAL scopes: started polling task, interval is {polling_interval} seconds."
+            f"OPAL Scopes: syncing {len(scopes)} scopes in the background (polling updates: {only_poll_updates})"
         )
-        sender.add_periodic_task(polling_interval, periodic_check.s())
-
 
-@app.task(ignore_result=True)
-def sync_scope(
-    scope_id: str, hinted_hash: Optional[str] = None, force_fetch: bool = False
-):
-    return async_to_sync(with_worker(Worker.sync_scope))(
-        scope_id, hinted_hash=hinted_hash, force_fetch=force_fetch
-    )
-
-
-@app.task(ignore_result=True)
-def delete_scope(scope_id: str):
-    return async_to_sync(with_worker(Worker.delete_scope))(scope_id)
-
-
-@app.task(ignore_result=True)
-def periodic_check():
-    return async_to_sync(with_worker(Worker.periodic_check))()
-
-
-async def schedule_sync_all_scopes(scopes: ScopeRepository):
-    """Syncing all scopes found in redis.
-
-    Schedules separate sync scope tasks in celery. Git fetches are done
-    only for unique remotes.
-    """
-    all_scopes = await scopes.all()
-    logger.info(f"OPAL Scopes: syncing {len(all_scopes)} scopes in the background")
-
-    already_fetched = set()
-    already_synced_scope_ids: List[str] = []
-
-    # first we sync with git fetch all the unique repositories
-    for scope in all_scopes:
-        if scope.policy.url not in already_fetched:
-            logger.info(
-                f"Sync scope {scope.scope_id} (force fetch, remote: {scope.policy.url})"
-            )
-            sync_scope.delay(scope.scope_id, force_fetch=True)
-            already_fetched.add(scope.policy.url)
-            already_synced_scope_ids.append(scope.scope_id)
-
-    # then we sync other "same repo" scopes without git fetch to be more efficient
-    for scope in all_scopes:
-        if scope.scope_id not in already_synced_scope_ids:
-            logger.info(
-                f"Sync scope {scope.scope_id} (SKIP fetch, remote: {scope.policy.url})"
+        fetched_urls = set()
+        skipped_scopes = []
+        for scope in scopes:
+            # Give priority to scopes that have a unique url (so we'll clone all repos asap)
+            if scope.policy.url in fetched_urls:
+                skipped_scopes.append(scope)
+                continue
+
+            await self.sync_scope(
+                scope.scope_id,
+                force_fetch=True,
+                notify_on_changes=notify_on_changes,
+            )
+            fetched_urls.add(scope.policy.url)
+
+        for scope in skipped_scopes:
+            # No need to refetch the same repo, just check for changes
+            await self.sync_scope(
+                scope.scope_id,
+                force_fetch=False,
+                notify_on_changes=notify_on_changes,
             )
-            sync_scope.delay(scope.scope_id)
```

### Comparing `opal-server-0.5.0/opal_server.egg-info/PKG-INFO` & `opal-server-0.6.0/opal_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.5.0
+Version: 0.6.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.5.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.6.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
-Platform: UNKNOWN Classifier: Operating System :: OS Independent Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet ::
-WWW/HTTP :: WSGI Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Classifier: Operating System :: OS Independent Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
+:: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
+Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
 administration layer for Open_Policy_Agent_(OPA), detecting changes to both
@@ -37,21 +37,21 @@
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
@@ -78,12 +78,13 @@
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

### Comparing `opal-server-0.5.0/opal_server.egg-info/SOURCES.txt` & `opal-server-0.6.0/opal_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 opal_server/loadlimiting.py
 opal_server/main.py
 opal_server/publisher.py
 opal_server/pubsub.py
 opal_server/redis.py
 opal_server/server.py
 opal_server/statistics.py
-opal_server/worker.py
 opal_server.egg-info/PKG-INFO
 opal_server.egg-info/SOURCES.txt
 opal_server.egg-info/dependency_links.txt
 opal_server.egg-info/entry_points.txt
 opal_server.egg-info/requires.txt
 opal_server.egg-info/top_level.txt
 opal_server/data/__init__.py
@@ -31,10 +30,12 @@
 opal_server/policy/webhook/api.py
 opal_server/policy/webhook/deps.py
 opal_server/policy/webhook/listener.py
 opal_server/scopes/__init__.py
 opal_server/scopes/api.py
 opal_server/scopes/loader.py
 opal_server/scopes/scope_repository.py
+opal_server/scopes/service.py
+opal_server/scopes/task.py
 opal_server/security/__init__.py
 opal_server/security/api.py
 opal_server/security/jwks.py
```

### Comparing `opal-server-0.5.0/opal_server.egg-info/requires.txt` & `opal-server-0.6.0/opal_server.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 permit-broadcaster[kafka,postgres,redis]<1,>=0.2.0
 gitpython<4,>=3.1.27
 pyjwt[crypto]<3,>=2.1.0
 websockets<11,>=10.3
 ddtrace<2,>=1.1.4
 slowapi<1,>=0.1.5
 aioredis<3,>=2.0.1
-celery<6,>=5.2.7
 pygit2<2,>=1.9.2
 asgiref<4,>=3.5.2
 redis<5,>=4.3.4
-opal-common==0.5.0
+opal-common==0.6.0
 charset-normalizer<3,>=2.0.12
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.78.0
-fastapi_websocket_pubsub<1,>=0.3.0
+fastapi_websocket_pubsub==0.3.3
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<21,>=20.1.0
 pydantic[email]<2,>=1.9.1
 uvicorn[standard]<1,>=0.17.6
 fastapi-utils<1,>=0.2.1
 
 [:python_version < "3.8"]
```

### Comparing `opal-server-0.5.0/setup.py` & `opal-server-0.6.0/setup.py`

 * *Files identical despite different names*

