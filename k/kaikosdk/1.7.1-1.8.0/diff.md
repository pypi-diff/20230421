# Comparing `tmp/kaikosdk-1.7.1.tar.gz` & `tmp/kaikosdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaikosdk-1.7.1.tar", last modified: Tue Apr 18 08:27:10 2023, max compression
+gzip compressed data, was "kaikosdk-1.8.0.tar", last modified: Fri Apr 21 12:40:12 2023, max compression
```

## Comparing `kaikosdk-1.7.1.tar` & `kaikosdk-1.8.0.tar`

### file list

```diff
@@ -1,88 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.897806 kaikosdk-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.885806 kaikosdk-1.7.1/kaikosdk/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/core/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/sdk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/sdk_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/index_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:27:10.897806 kaikosdk-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 08:27:03.000000 kaikosdk-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.300984 kaikosdk-1.8.0/kaikosdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/sdk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29534 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/sdk_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.304984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_multi_assets_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.308984 kaikosdk-1.8.0/kaikosdk/stream/index_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:40:03.000000 kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:12.300984 kaikosdk-1.8.0/kaikosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 12:40:12.000000 kaikosdk-1.8.0/kaikosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:40:12.312984 kaikosdk-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-21 12:40:05.000000 kaikosdk-1.8.0/setup.py
```

### Comparing `kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/data_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/instrument_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/sort_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/core/source_data_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/source_data_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/core/source_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/source_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2.py` & `kaikosdk-1.8.0/kaikosdk/core/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/sdk_pb2.py` & `kaikosdk-1.8.0/kaikosdk/sdk_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,42 +21,46 @@
 from kaikosdk.stream.aggregates_vwap_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__vwap__v1_dot_response__pb2
 from kaikosdk.stream.aggregates_direct_exchange_rate_v1 import request_pb2 as sdk_dot_stream_dot_aggregates__direct__exchange__rate__v1_dot_request__pb2
 from kaikosdk.stream.aggregates_direct_exchange_rate_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__direct__exchange__rate__v1_dot_response__pb2
 from kaikosdk.stream.aggregates_spot_exchange_rate_v1 import request_pb2 as sdk_dot_stream_dot_aggregates__spot__exchange__rate__v1_dot_request__pb2
 from kaikosdk.stream.aggregates_spot_exchange_rate_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__spot__exchange__rate__v1_dot_response__pb2
 from kaikosdk.stream.index_v1 import request_pb2 as sdk_dot_stream_dot_index__v1_dot_request__pb2
 from kaikosdk.stream.index_v1 import response_pb2 as sdk_dot_stream_dot_index__v1_dot_response__pb2
+from kaikosdk.stream.index_multi_assets_v1 import request_pb2 as sdk_dot_stream_dot_index__multi__assets__v1_dot_request__pb2
+from kaikosdk.stream.index_multi_assets_v1 import response_pb2 as sdk_dot_stream_dot_index__multi__assets__v1_dot_response__pb2
 from kaikosdk.stream.market_update_v1 import request_pb2 as sdk_dot_stream_dot_market__update__v1_dot_request__pb2
 from kaikosdk.stream.market_update_v1 import response_pb2 as sdk_dot_stream_dot_market__update__v1_dot_response__pb2
 from kaikosdk.stream.trades_v1 import request_pb2 as sdk_dot_stream_dot_trades__v1_dot_request__pb2
 from kaikosdk.stream.trades_v1 import response_pb2 as sdk_dot_stream_dot_trades__v1_dot_response__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rsdk/sdk.proto\x12\x08kaikosdk\x1a,sdk/stream/aggregated_price_v1/request.proto\x1a-sdk/stream/aggregated_price_v1/response.proto\x1a,sdk/stream/aggregated_quote_v2/request.proto\x1a-sdk/stream/aggregated_quote_v2/response.proto\x1a,sdk/stream/aggregates_ohlcv_v1/request.proto\x1a-sdk/stream/aggregates_ohlcv_v1/response.proto\x1a+sdk/stream/aggregates_vwap_v1/request.proto\x1a,sdk/stream/aggregates_vwap_v1/response.proto\x1a;sdk/stream/aggregates_direct_exchange_rate_v1/request.proto\x1a<sdk/stream/aggregates_direct_exchange_rate_v1/response.proto\x1a\x39sdk/stream/aggregates_spot_exchange_rate_v1/request.proto\x1a:sdk/stream/aggregates_spot_exchange_rate_v1/response.proto\x1a!sdk/stream/index_v1/request.proto\x1a\"sdk/stream/index_v1/response.proto\x1a)sdk/stream/market_update_v1/request.proto\x1a*sdk/stream/market_update_v1/response.proto\x1a\"sdk/stream/trades_v1/request.proto\x1a#sdk/stream/trades_v1/response.proto2\x86\x01\n\x1eStreamAggregatedQuoteServiceV2\x12\x64\n\tSubscribe\x12(.kaikosdk.StreamAggregatedQuoteRequestV2\x1a).kaikosdk.StreamAggregatedQuoteResponseV2\"\x00\x30\x01\x32\x89\x01\n\x1eStreamAggregatedPriceServiceV1\x12g\n\tSubscribe\x12(.kaikosdk.StreamAggregatedPriceRequestV1\x1a).kaikosdk.StreamAggregatedPriceResponseV1\"\x03\x88\x02\x01\x30\x01\x32\x86\x01\n\x1eStreamAggregatesOHLCVServiceV1\x12\x64\n\tSubscribe\x12(.kaikosdk.StreamAggregatesOHLCVRequestV1\x1a).kaikosdk.StreamAggregatesOHLCVResponseV1\"\x00\x30\x01\x32\xa7\x01\n)StreamAggregatesSpotExchangeRateServiceV1\x12z\n\tSubscribe\x12\x33.kaikosdk.StreamAggregatesSpotExchangeRateRequestV1\x1a\x34.kaikosdk.StreamAggregatesSpotExchangeRateResponseV1\"\x00\x30\x01\x32\xad\x01\n+StreamAggregatesDirectExchangeRateServiceV1\x12~\n\tSubscribe\x12\x35.kaikosdk.StreamAggregatesDirectExchangeRateRequestV1\x1a\x36.kaikosdk.StreamAggregatesDirectExchangeRateResponseV1\"\x00\x30\x01\x32k\n\x15StreamTradesServiceV1\x12R\n\tSubscribe\x12\x1f.kaikosdk.StreamTradesRequestV1\x1a .kaikosdk.StreamTradesResponseV1\"\x00\x30\x01\x32\x83\x01\n\x1dStreamAggregatesVWAPServiceV1\x12\x62\n\tSubscribe\x12\'.kaikosdk.StreamAggregatesVWAPRequestV1\x1a(.kaikosdk.StreamAggregatesVWAPResponseV1\"\x00\x30\x01\x32v\n\x14StreamIndexServiceV1\x12^\n\tSubscribe\x12%.kaikosdk.StreamIndexServiceRequestV1\x1a&.kaikosdk.StreamIndexServiceResponseV1\"\x00\x30\x01\x32}\n\x1bStreamMarketUpdateServiceV1\x12^\n\tSubscribe\x12%.kaikosdk.StreamMarketUpdateRequestV1\x1a&.kaikosdk.StreamMarketUpdateResponseV1\"\x00\x30\x01\x42R\n\rcom.kaiko.sdkB\x08SdkProtoP\x01Z*github.com/kaikodata/kaiko-go-sdk;kaikosdk\xaa\x02\x08KaikoSdkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rsdk/sdk.proto\x12\x08kaikosdk\x1a,sdk/stream/aggregated_price_v1/request.proto\x1a-sdk/stream/aggregated_price_v1/response.proto\x1a,sdk/stream/aggregated_quote_v2/request.proto\x1a-sdk/stream/aggregated_quote_v2/response.proto\x1a,sdk/stream/aggregates_ohlcv_v1/request.proto\x1a-sdk/stream/aggregates_ohlcv_v1/response.proto\x1a+sdk/stream/aggregates_vwap_v1/request.proto\x1a,sdk/stream/aggregates_vwap_v1/response.proto\x1a;sdk/stream/aggregates_direct_exchange_rate_v1/request.proto\x1a<sdk/stream/aggregates_direct_exchange_rate_v1/response.proto\x1a\x39sdk/stream/aggregates_spot_exchange_rate_v1/request.proto\x1a:sdk/stream/aggregates_spot_exchange_rate_v1/response.proto\x1a!sdk/stream/index_v1/request.proto\x1a\"sdk/stream/index_v1/response.proto\x1a.sdk/stream/index_multi_assets_v1/request.proto\x1a/sdk/stream/index_multi_assets_v1/response.proto\x1a)sdk/stream/market_update_v1/request.proto\x1a*sdk/stream/market_update_v1/response.proto\x1a\"sdk/stream/trades_v1/request.proto\x1a#sdk/stream/trades_v1/response.proto2\x86\x01\n\x1eStreamAggregatedQuoteServiceV2\x12\x64\n\tSubscribe\x12(.kaikosdk.StreamAggregatedQuoteRequestV2\x1a).kaikosdk.StreamAggregatedQuoteResponseV2\"\x00\x30\x01\x32\x89\x01\n\x1eStreamAggregatedPriceServiceV1\x12g\n\tSubscribe\x12(.kaikosdk.StreamAggregatedPriceRequestV1\x1a).kaikosdk.StreamAggregatedPriceResponseV1\"\x03\x88\x02\x01\x30\x01\x32\x86\x01\n\x1eStreamAggregatesOHLCVServiceV1\x12\x64\n\tSubscribe\x12(.kaikosdk.StreamAggregatesOHLCVRequestV1\x1a).kaikosdk.StreamAggregatesOHLCVResponseV1\"\x00\x30\x01\x32\xa7\x01\n)StreamAggregatesSpotExchangeRateServiceV1\x12z\n\tSubscribe\x12\x33.kaikosdk.StreamAggregatesSpotExchangeRateRequestV1\x1a\x34.kaikosdk.StreamAggregatesSpotExchangeRateResponseV1\"\x00\x30\x01\x32\xad\x01\n+StreamAggregatesDirectExchangeRateServiceV1\x12~\n\tSubscribe\x12\x35.kaikosdk.StreamAggregatesDirectExchangeRateRequestV1\x1a\x36.kaikosdk.StreamAggregatesDirectExchangeRateResponseV1\"\x00\x30\x01\x32k\n\x15StreamTradesServiceV1\x12R\n\tSubscribe\x12\x1f.kaikosdk.StreamTradesRequestV1\x1a .kaikosdk.StreamTradesResponseV1\"\x00\x30\x01\x32\x83\x01\n\x1dStreamAggregatesVWAPServiceV1\x12\x62\n\tSubscribe\x12\'.kaikosdk.StreamAggregatesVWAPRequestV1\x1a(.kaikosdk.StreamAggregatesVWAPResponseV1\"\x00\x30\x01\x32v\n\x14StreamIndexServiceV1\x12^\n\tSubscribe\x12%.kaikosdk.StreamIndexServiceRequestV1\x1a&.kaikosdk.StreamIndexServiceResponseV1\"\x00\x30\x01\x32\x97\x01\n\x1fStreamIndexMultiAssetsServiceV1\x12t\n\tSubscribe\x12\x30.kaikosdk.StreamIndexMultiAssetsServiceRequestV1\x1a\x31.kaikosdk.StreamIndexMultiAssetsServiceResponseV1\"\x00\x30\x01\x32}\n\x1bStreamMarketUpdateServiceV1\x12^\n\tSubscribe\x12%.kaikosdk.StreamMarketUpdateRequestV1\x1a&.kaikosdk.StreamMarketUpdateResponseV1\"\x00\x30\x01\x42R\n\rcom.kaiko.sdkB\x08SdkProtoP\x01Z*github.com/kaikodata/kaiko-go-sdk;kaikosdk\xaa\x02\x08KaikoSdkb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sdk.sdk_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\rcom.kaiko.sdkB\010SdkProtoP\001Z*github.com/kaikodata/kaiko-go-sdk;kaikosdk\252\002\010KaikoSdk'
   _STREAMAGGREGATEDPRICESERVICEV1.methods_by_name['Subscribe']._options = None
   _STREAMAGGREGATEDPRICESERVICEV1.methods_by_name['Subscribe']._serialized_options = b'\210\002\001'
-  _STREAMAGGREGATEDQUOTESERVICEV2._serialized_start=871
-  _STREAMAGGREGATEDQUOTESERVICEV2._serialized_end=1005
-  _STREAMAGGREGATEDPRICESERVICEV1._serialized_start=1008
-  _STREAMAGGREGATEDPRICESERVICEV1._serialized_end=1145
-  _STREAMAGGREGATESOHLCVSERVICEV1._serialized_start=1148
-  _STREAMAGGREGATESOHLCVSERVICEV1._serialized_end=1282
-  _STREAMAGGREGATESSPOTEXCHANGERATESERVICEV1._serialized_start=1285
-  _STREAMAGGREGATESSPOTEXCHANGERATESERVICEV1._serialized_end=1452
-  _STREAMAGGREGATESDIRECTEXCHANGERATESERVICEV1._serialized_start=1455
-  _STREAMAGGREGATESDIRECTEXCHANGERATESERVICEV1._serialized_end=1628
-  _STREAMTRADESSERVICEV1._serialized_start=1630
-  _STREAMTRADESSERVICEV1._serialized_end=1737
-  _STREAMAGGREGATESVWAPSERVICEV1._serialized_start=1740
-  _STREAMAGGREGATESVWAPSERVICEV1._serialized_end=1871
-  _STREAMINDEXSERVICEV1._serialized_start=1873
-  _STREAMINDEXSERVICEV1._serialized_end=1991
-  _STREAMMARKETUPDATESERVICEV1._serialized_start=1993
-  _STREAMMARKETUPDATESERVICEV1._serialized_end=2118
+  _STREAMAGGREGATEDQUOTESERVICEV2._serialized_start=968
+  _STREAMAGGREGATEDQUOTESERVICEV2._serialized_end=1102
+  _STREAMAGGREGATEDPRICESERVICEV1._serialized_start=1105
+  _STREAMAGGREGATEDPRICESERVICEV1._serialized_end=1242
+  _STREAMAGGREGATESOHLCVSERVICEV1._serialized_start=1245
+  _STREAMAGGREGATESOHLCVSERVICEV1._serialized_end=1379
+  _STREAMAGGREGATESSPOTEXCHANGERATESERVICEV1._serialized_start=1382
+  _STREAMAGGREGATESSPOTEXCHANGERATESERVICEV1._serialized_end=1549
+  _STREAMAGGREGATESDIRECTEXCHANGERATESERVICEV1._serialized_start=1552
+  _STREAMAGGREGATESDIRECTEXCHANGERATESERVICEV1._serialized_end=1725
+  _STREAMTRADESSERVICEV1._serialized_start=1727
+  _STREAMTRADESSERVICEV1._serialized_end=1834
+  _STREAMAGGREGATESVWAPSERVICEV1._serialized_start=1837
+  _STREAMAGGREGATESVWAPSERVICEV1._serialized_end=1968
+  _STREAMINDEXSERVICEV1._serialized_start=1970
+  _STREAMINDEXSERVICEV1._serialized_end=2088
+  _STREAMINDEXMULTIASSETSSERVICEV1._serialized_start=2091
+  _STREAMINDEXMULTIASSETSSERVICEV1._serialized_end=2242
+  _STREAMMARKETUPDATESERVICEV1._serialized_start=2244
+  _STREAMMARKETUPDATESERVICEV1._serialized_end=2369
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaikosdk-1.7.1/kaikosdk/sdk_pb2_grpc.py` & `kaikosdk-1.8.0/kaikosdk/sdk_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from kaikosdk.stream.aggregates_direct_exchange_rate_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__direct__exchange__rate__v1_dot_response__pb2
 from kaikosdk.stream.aggregates_ohlcv_v1 import request_pb2 as sdk_dot_stream_dot_aggregates__ohlcv__v1_dot_request__pb2
 from kaikosdk.stream.aggregates_ohlcv_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__ohlcv__v1_dot_response__pb2
 from kaikosdk.stream.aggregates_spot_exchange_rate_v1 import request_pb2 as sdk_dot_stream_dot_aggregates__spot__exchange__rate__v1_dot_request__pb2
 from kaikosdk.stream.aggregates_spot_exchange_rate_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__spot__exchange__rate__v1_dot_response__pb2
 from kaikosdk.stream.aggregates_vwap_v1 import request_pb2 as sdk_dot_stream_dot_aggregates__vwap__v1_dot_request__pb2
 from kaikosdk.stream.aggregates_vwap_v1 import response_pb2 as sdk_dot_stream_dot_aggregates__vwap__v1_dot_response__pb2
+from kaikosdk.stream.index_multi_assets_v1 import request_pb2 as sdk_dot_stream_dot_index__multi__assets__v1_dot_request__pb2
+from kaikosdk.stream.index_multi_assets_v1 import response_pb2 as sdk_dot_stream_dot_index__multi__assets__v1_dot_response__pb2
 from kaikosdk.stream.index_v1 import request_pb2 as sdk_dot_stream_dot_index__v1_dot_request__pb2
 from kaikosdk.stream.index_v1 import response_pb2 as sdk_dot_stream_dot_index__v1_dot_response__pb2
 from kaikosdk.stream.market_update_v1 import request_pb2 as sdk_dot_stream_dot_market__update__v1_dot_request__pb2
 from kaikosdk.stream.market_update_v1 import response_pb2 as sdk_dot_stream_dot_market__update__v1_dot_response__pb2
 from kaikosdk.stream.trades_v1 import request_pb2 as sdk_dot_stream_dot_trades__v1_dot_request__pb2
 from kaikosdk.stream.trades_v1 import response_pb2 as sdk_dot_stream_dot_trades__v1_dot_response__pb2
 
@@ -541,14 +543,79 @@
         return grpc.experimental.unary_stream(request, target, '/kaikosdk.StreamIndexServiceV1/Subscribe',
             sdk_dot_stream_dot_index__v1_dot_request__pb2.StreamIndexServiceRequestV1.SerializeToString,
             sdk_dot_stream_dot_index__v1_dot_response__pb2.StreamIndexServiceResponseV1.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
+class StreamIndexMultiAssetsServiceV1Stub(object):
+    """Service for streaming index multi assets V1
+    """
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.Subscribe = channel.unary_stream(
+                '/kaikosdk.StreamIndexMultiAssetsServiceV1/Subscribe',
+                request_serializer=sdk_dot_stream_dot_index__multi__assets__v1_dot_request__pb2.StreamIndexMultiAssetsServiceRequestV1.SerializeToString,
+                response_deserializer=sdk_dot_stream_dot_index__multi__assets__v1_dot_response__pb2.StreamIndexMultiAssetsServiceResponseV1.FromString,
+                )
+
+
+class StreamIndexMultiAssetsServiceV1Servicer(object):
+    """Service for streaming index multi assets V1
+    """
+
+    def Subscribe(self, request, context):
+        """Subscribe
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_StreamIndexMultiAssetsServiceV1Servicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'Subscribe': grpc.unary_stream_rpc_method_handler(
+                    servicer.Subscribe,
+                    request_deserializer=sdk_dot_stream_dot_index__multi__assets__v1_dot_request__pb2.StreamIndexMultiAssetsServiceRequestV1.FromString,
+                    response_serializer=sdk_dot_stream_dot_index__multi__assets__v1_dot_response__pb2.StreamIndexMultiAssetsServiceResponseV1.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'kaikosdk.StreamIndexMultiAssetsServiceV1', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class StreamIndexMultiAssetsServiceV1(object):
+    """Service for streaming index multi assets V1
+    """
+
+    @staticmethod
+    def Subscribe(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/kaikosdk.StreamIndexMultiAssetsServiceV1/Subscribe',
+            sdk_dot_stream_dot_index__multi__assets__v1_dot_request__pb2.StreamIndexMultiAssetsServiceRequestV1.SerializeToString,
+            sdk_dot_stream_dot_index__multi__assets__v1_dot_response__pb2.StreamIndexMultiAssetsServiceResponseV1.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+
 class StreamMarketUpdateServiceV1Stub(object):
     """Service for streaming market update V1
     """
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/index_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/index_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/index_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/market_update_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/trades_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2.py` & `kaikosdk-1.8.0/kaikosdk/stream/trades_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.1/kaikosdk.egg-info/SOURCES.txt` & `kaikosdk-1.8.0/kaikosdk.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
 kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
 kaikosdk/stream/aggregates_vwap_v1/__init__.py
 kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
 kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
 kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
 kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
+kaikosdk/stream/index_multi_assets_v1/__init__.py
+kaikosdk/stream/index_multi_assets_v1/request_pb2.py
+kaikosdk/stream/index_multi_assets_v1/request_pb2_grpc.py
+kaikosdk/stream/index_multi_assets_v1/response_pb2.py
+kaikosdk/stream/index_multi_assets_v1/response_pb2_grpc.py
 kaikosdk/stream/index_v1/__init__.py
 kaikosdk/stream/index_v1/commodity_pb2.py
 kaikosdk/stream/index_v1/commodity_pb2_grpc.py
 kaikosdk/stream/index_v1/request_pb2.py
 kaikosdk/stream/index_v1/request_pb2_grpc.py
 kaikosdk/stream/index_v1/response_pb2.py
 kaikosdk/stream/index_v1/response_pb2_grpc.py
```

