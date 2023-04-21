# Comparing `tmp/hypertrace-agent-0.9.3.tar.gz` & `tmp/hypertrace-agent-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypertrace-agent-0.9.3.tar", last modified: Thu Jan 13 16:51:50 2022, max compression
+gzip compressed data, was "hypertrace-agent-0.9.4.tar", last modified: Thu Jan 13 21:44:37 2022, max compression
```

## Comparing `hypertrace-agent-0.9.3.tar` & `hypertrace-agent-0.9.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.894187 hypertrace-agent-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-13 16:51:50.894187 hypertrace-agent-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-13 16:51:50.894187 hypertrace-agent-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/
--rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/hypertrace_instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/config/
--rw-r--r--   0 runner    (1001) docker     (121)     7959 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/__init___test.py
--rw-r--r--   0 runner    (1001) docker     (121)    22415 2022-01-13 16:51:45.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/environment_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/config/file_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/filter/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/filter/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/init/
--rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/init/__init__test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (121)    11090 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (121)     7712 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/aiohttp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/django/
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/django/django_auto_instrumentation_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/flask/
--rw-r--r--   0 runner    (1001) docker     (121)     8102 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)    11487 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/instrumentation_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/postgresql/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.890187 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/requests/
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/env_var_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-13 16:51:18.000000 hypertrace-agent-0.9.3/src/hypertrace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:51:50.894187 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-13 16:51:50.000000 hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.151746 hypertrace-agent-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/hypertrace_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/agent/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     7959 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/__init___test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22415 2022-01-13 21:44:31.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/environment_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/config/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/agent/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/filter/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/filter/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.155746 hypertrace-agent-0.9.4/src/hypertrace/agent/init/
+-rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/init/__init__test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)    11090 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (121)     7712 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/aiohttp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/django/
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/django/django_auto_instrumentation_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/flask/
+-rw-r--r--   0 runner    (1001) docker     (121)     8099 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)    11487 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/instrumentation_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/requests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/env_var_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-13 21:44:02.000000 hypertrace-agent-0.9.4/src/hypertrace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 21:44:37.159746 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-13 21:44:37.000000 hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/top_level.txt
```

### Comparing `hypertrace-agent-0.9.3/LICENSE` & `hypertrace-agent-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/PKG-INFO` & `hypertrace-agent-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypertrace-agent
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hypertrace Python Agent
 Home-page: https://github.com/hypertrace/pythonagent
 Author: Hypertrace
 Author-email: community@hypertrace.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hypertrace/pythonagent/issues
 Platform: UNKNOWN
```

### Comparing `hypertrace-agent-0.9.3/README.md` & `hypertrace-agent-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/setup.py` & `hypertrace-agent-0.9.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,29 +22,29 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent"
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
-        "opentelemetry-api==1.4.0",
-        "opentelemetry-exporter-otlp==1.4.0",
-        "opentelemetry-exporter-zipkin==1.4.0",
-        "opentelemetry-instrumentation==0.23b0",
-        "opentelemetry-instrumentation-aiohttp-client==0.23b0",
-        "opentelemetry-instrumentation-wsgi==0.23b0",
-        "opentelemetry-instrumentation-flask==0.23b0",
-        "opentelemetry-instrumentation-mysql==0.23b0",
-        "opentelemetry-instrumentation-psycopg2==0.23b0",
-        "opentelemetry-instrumentation-requests==0.23b0",
-        "opentelemetry-instrumentation-grpc==0.23b0",
-        "opentelemetry-instrumentation-django==0.23b0",
-        "opentelemetry-propagator-b3==1.4.0",
-        "opentelemetry-sdk==1.4.0",
-        "opentelemetry-util-http==0.23b0",
+        "opentelemetry-api==1.8.0",
+        "opentelemetry-exporter-otlp==1.8.0",
+        "opentelemetry-exporter-zipkin==1.8.0",
+        "opentelemetry-instrumentation==0.27b0",
+        "opentelemetry-instrumentation-aiohttp-client==0.27b0",
+        "opentelemetry-instrumentation-wsgi==0.27b0",
+        "opentelemetry-instrumentation-flask==0.27b0",
+        "opentelemetry-instrumentation-mysql==0.27b0",
+        "opentelemetry-instrumentation-psycopg2==0.27b0",
+        "opentelemetry-instrumentation-requests==0.27b0",
+        "opentelemetry-instrumentation-grpc==0.27b0",
+        "opentelemetry-instrumentation-django==0.27b0",
+        "opentelemetry-propagator-b3==1.8.0",
+        "opentelemetry-sdk==1.8.0",
+        "opentelemetry-util-http==0.27b0",
         "deprecated==1.2.12",
         "google>=3.0.0",
         "pyyaml",
         "protobuf>=3.15.8"
     ],
     entry_points = {
         'console_scripts': [
```

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/hypertrace_instrument.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/hypertrace_instrument.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/autoinstrumentation/sitecustomize.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/autoinstrumentation/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/__init___test.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/__init___test.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/config_pb2.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/default.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/default.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/environment.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/environment.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/environment_test.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/environment_test.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/file.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/file.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/config/file_test.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/config/file_test.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/custom_logger.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/custom_logger.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/filter/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/filter/registry.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/filter/registry.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/filter/test_registry.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/filter/test_registry.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/init/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/init/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/init/__init__test.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/init/__init__test.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/aiohttp/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/django/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/django/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/django/django_auto_instrumentation_compat.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/django/django_auto_instrumentation_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 
     original_get_asgi_application = asgi.get_asgi_application
     asgi.get_asgi_application = lambda: apply_wrapper_get_app_fn(original_get_asgi_application, agent_init,
                                                                      instrumentation_wrapper)
 
 def apply_wrapper_get_app_fn(original_fn, agent_init, instrumentation_wrapper):
     """wrapper function that calls original app getter and then registers django instrumentation"""
+    # We need to run instrumentation first to inject middleware before we call the original function
+    # otherwise middleware stack changes are not applied
     def ht_get_application_fn():
-        app = original_fn()
         try:
             agent_init.register_library(DJANGO_KEY, instrumentation_wrapper)
         except:  # pylint:disable=W0702
             logger.error('registering django instrumentation in wsgi/asgi patch failed '
                          '- continuing without instrumenting django')
+        app = original_fn()
         return app
 
     return ht_get_application_fn()
```

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/flask/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/flask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import traceback
 import json
 import flask
 from opentelemetry.instrumentation.flask import (
     _InstrumentedFlask,
     FlaskInstrumentor,
     get_default_span_name,
-    _teardown_request,
     _ENVIRON_SPAN_KEY,
 )
 from werkzeug.exceptions import Forbidden
 
 from hypertrace.agent import constants  # pylint: disable=R0801
 from hypertrace.agent.filter.registry import Registry, TYPE_HTTP
 from hypertrace.agent.instrumentation import BaseInstrumentorWrapper
@@ -149,15 +148,15 @@
         if callable(name_callback):
             _HypertraceInstrumentedFlask.name_callback = name_callback
         _HypertraceInstrumentedFlask._tracer_provider = tracer_provider # pylint: disable=W0212
         flask.Flask = _HypertraceInstrumentedFlask
 
     # Initialize instrumentation wrapper
     @staticmethod
-    def instrument_app(app, request_hook=None, response_hook=None, tracer_provider=None):
+    def instrument_app(app, request_hook=None, response_hook=None, tracer_provider=None, excluded_urls=None):
         '''Initialize instrumentation'''
         logger.debug('Entering FlaskInstrumentorWrapper.instument_app().')
         try:
 
             # Call parent class's initialization
             FlaskInstrumentor.instrument_app(app, request_hook, response_hook, None)
```

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/grpc/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/instrumentation_definitions.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/instrumentation_definitions.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/postgresql/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace/agent/instrumentation/requests/__init__.py` & `hypertrace-agent-0.9.4/src/hypertrace/agent/instrumentation/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/PKG-INFO` & `hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypertrace-agent
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hypertrace Python Agent
 Home-page: https://github.com/hypertrace/pythonagent
 Author: Hypertrace
 Author-email: community@hypertrace.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hypertrace/pythonagent/issues
 Platform: UNKNOWN
```

### Comparing `hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/SOURCES.txt` & `hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypertrace-agent-0.9.3/src/hypertrace_agent.egg-info/requires.txt` & `hypertrace-agent-0.9.4/src/hypertrace_agent.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-opentelemetry-api==1.4.0
-opentelemetry-exporter-otlp==1.4.0
-opentelemetry-exporter-zipkin==1.4.0
-opentelemetry-instrumentation==0.23b0
-opentelemetry-instrumentation-aiohttp-client==0.23b0
-opentelemetry-instrumentation-wsgi==0.23b0
-opentelemetry-instrumentation-flask==0.23b0
-opentelemetry-instrumentation-mysql==0.23b0
-opentelemetry-instrumentation-psycopg2==0.23b0
-opentelemetry-instrumentation-requests==0.23b0
-opentelemetry-instrumentation-grpc==0.23b0
-opentelemetry-instrumentation-django==0.23b0
-opentelemetry-propagator-b3==1.4.0
-opentelemetry-sdk==1.4.0
-opentelemetry-util-http==0.23b0
+opentelemetry-api==1.8.0
+opentelemetry-exporter-otlp==1.8.0
+opentelemetry-exporter-zipkin==1.8.0
+opentelemetry-instrumentation==0.27b0
+opentelemetry-instrumentation-aiohttp-client==0.27b0
+opentelemetry-instrumentation-wsgi==0.27b0
+opentelemetry-instrumentation-flask==0.27b0
+opentelemetry-instrumentation-mysql==0.27b0
+opentelemetry-instrumentation-psycopg2==0.27b0
+opentelemetry-instrumentation-requests==0.27b0
+opentelemetry-instrumentation-grpc==0.27b0
+opentelemetry-instrumentation-django==0.27b0
+opentelemetry-propagator-b3==1.8.0
+opentelemetry-sdk==1.8.0
+opentelemetry-util-http==0.27b0
 deprecated==1.2.12
 google>=3.0.0
 pyyaml
 protobuf>=3.15.8
```

