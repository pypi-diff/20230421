# Comparing `tmp/th2_data_services_lwdp-2.0.2.0.dev4742507433.tar.gz` & `tmp/th2_data_services_lwdp-2.0.2.0.dev4766015884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4742507433.tar", last modified: Wed Apr 19 11:01:48 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4766015884.tar", last modified: Fri Apr 21 14:43:47 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433.tar` & `th2_data_services_lwdp-2.0.2.0.dev4766015884.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-19 11:01:32.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38764 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/response_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-21 14:43:26.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38821 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_data_services_lwdp
-Version: 2.0.2.0.dev4742507433
+Name: th2-data-services-lwdp
+Version: 2.0.2.0.dev4766015884
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/README.md` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     _check_response_formats,
 )
 from th2_data_services.data_source.lwdp.utils.json import BufferedJSONProcessor
 from th2_data_services.data_source.lwdp.page import PageNotFound
 
 Event = dict
 
+
 # LOG import logging
 
 # LOG logger = logging.getLogger(__name__)
 
 
 class SSEHandlerClassBase(IHTTPCommand):
     def __init__(
@@ -644,32 +645,34 @@
         super().__init__()
         self._id = id
         self._stub_status = use_stub
         self._response_formats = response_formats
 
     def handle(self, data_source: HTTPDataSource) -> dict:  # noqa: D102
         api: HTTPAPI = data_source.source_api
-        if self._response_formats in [['JSON_PARSED','BASE_64'],['BASE_64','JSON_PARSED'],None]:
+        if self._response_formats in [["JSON_PARSED", "BASE_64"], ["BASE_64", "JSON_PARSED"], None]:
             only_raw = False
-        elif self._response_formats == ['BASE_64']:
+        elif self._response_formats == ["BASE_64"]:
             only_raw = True
         else:
-            raise Exception("response_formats should be either ['BASE_64'] or ['JSON_PARSED','BASE_64']")
+            raise Exception(
+                "response_formats should be either ['BASE_64'] or ['JSON_PARSED','BASE_64']"
+            )
 
         url = api.get_url_find_message_by_id(self._id, only_raw)
         # LOG         logger.info(url)
         response = api.execute_request(url)
         if response.status_code in (404, 408) and self._stub_status:
             stub = data_source.message_stub_builder.build(
                 {data_source.message_struct.MESSAGE_ID: self._id}
             )
             return stub
         elif response.status_code in (404, 408):
             # LOG             logger.error(f"Unable to find the message. Id: {self._id}")
-            raise MessageNotFound(self._id,"Unable to find the message")
+            raise MessageNotFound(self._id, "Unable to find the message")
         else:
             return response.json()
 
 
 class GetMessagesById(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
@@ -733,15 +736,15 @@
         # +TODO - we often repeat these args. Perhaps it's better to move them to some class.
         max_url_length: int = 2048,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         cache: bool = False,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ):
-        """GetMessages constructor.
+        """GetMessagesByBookByStreams constructor.
 
         Args:
             start_timestamp: Start timestamp of search.
             book_id: Book ID for messages
             streams: List of aliases to request. If direction is not specified all directions will be requested for stream.
             message_ids: List of message IDs to restore search. If given, it has
                 the highest priority and ignores streams (uses streams from ids), startTimestamp and resumeFromId.
@@ -845,15 +848,15 @@
         # Non-data source args.
         max_url_length: int = 2048,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         cache: bool = False,
         buffer_limit=DEFAULT_BUFFER_LIMIT,
     ):
-        """GetMessagesByGroups Constructor.
+        """GetMessagesByBookByGroups Constructor.
 
         Args:
             start_timestamp: Sets the search starting point.
             end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
 
             book_id: book ID for requested groups.
             groups: List of groups to search messages from.
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from datetime import datetime
 from typing import List
-from th2_data_services.data_source.lwdp.utils.response_formats import ResponseFormats
+from th2_data_services.data_source.lwdp.utils._response_formats import ResponseFormats
+
 
 def _check_list_or_tuple(variable, var_name):  # noqa
     if not (isinstance(variable, tuple) or isinstance(variable, list)):
         raise TypeError(f"{var_name} argument has to be list or tuple type. Got {type(variable)}")
 
 
 def _check_datetime(dt: datetime):
     if not isinstance(dt, datetime):
         raise TypeError("Provided timestamp should be `datetime` object")
 
 
 def _check_response_formats(formats: List[str]):
     rf = ResponseFormats()
     if not rf.is_valid_response_format(formats):
-        raise Exception("Invalid response format")
+        raise Exception("Invalid response format")
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/response_formats.py` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import List, Union
+from th2_data_services.data_source.lwdp.message_response_format import ResponseFormat as RF
 
 
 class ResponseFormats:
     def __init__(self):  # noqa
         """ResponseFormats Constructor."""
-        self.correct_formats = ["PROTO_PARSED", "JSON_PARSED", "BASE_64"]
+        self.correct_formats = [RF.JSON_PARSED, RF.BASE64, RF.PROTO_PARSED]
 
     def is_valid_response_format(self, formats: Union[str, List[str]]):
         if formats is None:
             return True
         if isinstance(formats, str):
             formats = [formats]
         if not isinstance(formats, list):
             raise Exception("Wrong type. formats should be list or string")
-        if "PROTO_PARSED" in self.correct_formats and "JSON_PARSED" in self.correct_formats:
-            raise Exception("PROTO_PARSED and JSON_PARSED can't be used together for format")
-        return all(format in self.correct_formats for format in formats)
+        if RF.PROTO_PARSED in formats and RF.JSON_PARSED in formats:
+            raise Exception(
+                f"{RF.PROTO_PARSED} and {RF.JSON_PARSED} can't be used together for format"
+            )
+        return all(format in self.correct_formats for format in formats)
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-data-services-lwdp
-Version: 2.0.2.0.dev4742507433
+Name: th2_data_services_lwdp
+Version: 2.0.2.0.dev4766015884
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 th2_data_services/data_source/lwdp/interfaces/data_source.py
 th2_data_services/data_source/lwdp/interfaces/filter.py
 th2_data_services/data_source/lwdp/interfaces/source_api.py
 th2_data_services/data_source/lwdp/source_api/__init__.py
 th2_data_services/data_source/lwdp/source_api/grpc.py
 th2_data_services/data_source/lwdp/source_api/http.py
 th2_data_services/data_source/lwdp/utils/__init__.py
+th2_data_services/data_source/lwdp/utils/_response_formats.py
 th2_data_services/data_source/lwdp/utils/json.py
 th2_data_services/data_source/lwdp/utils/misc.py
-th2_data_services/data_source/lwdp/utils/response_formats.py
 th2_data_services_lwdp.egg-info/PKG-INFO
 th2_data_services_lwdp.egg-info/SOURCES.txt
 th2_data_services_lwdp.egg-info/dependency_links.txt
 th2_data_services_lwdp.egg-info/requires.txt
 th2_data_services_lwdp.egg-info/top_level.txt
```

