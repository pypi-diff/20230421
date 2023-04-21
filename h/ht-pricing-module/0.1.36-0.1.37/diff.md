# Comparing `tmp/ht_pricing_module-0.1.36.tar.gz` & `tmp/ht_pricing_module-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.1.36.tar", last modified: Wed Apr 12 10:50:36 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.1.37.tar", last modified: Fri Apr 21 01:21:28 2023, max compression
```

## Comparing `ht_pricing_module-0.1.36.tar` & `ht_pricing_module-0.1.37.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.36/MANIFEST.in
--rw-rw-rw-   0        0        0      264 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.220534 ht_pricing_module-0.1.36/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.36/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.248459 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.257435 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.201589 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.278403 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.296673 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    45777 2023-04-03 01:09:32.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.310658 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.320631 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.333625 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4499 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.345593 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.360553 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.455377 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4317 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3485 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4294 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     5195 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4472 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4277 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3539 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4526 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4603 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5243 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.463355 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.486294 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.529179 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.533168 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.556107 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.566080 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     3714 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.586133 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3452 2023-04-12 02:15:47.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.599098 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.622089 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.642069 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.646058 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    43817 2023-04-03 01:07:06.000000 ht_pricing_module-0.1.36/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:50:36.235494 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      264 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4864 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-12 10:50:36.000000 ht_pricing_module-0.1.36/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:50:36.655034 ht_pricing_module-0.1.36/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-04-12 10:50:22.000000 ht_pricing_module-0.1.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.086066 ht_pricing_module-0.1.37/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.37/MANIFEST.in
+-rw-rw-rw-   0        0        0      264 2023-04-21 01:21:28.086066 ht_pricing_module-0.1.37/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.665064 ht_pricing_module-0.1.37/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.37/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.688003 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.696979 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.653097 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.725947 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.744898 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    45824 2023-04-14 09:34:03.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.758886 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.768858 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.781823 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4499 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.793799 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.809749 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.895520 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4317 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3485 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4294 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     5195 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4472 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4277 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3539 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4526 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4603 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5270 2023-04-14 09:34:03.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.903498 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.925491 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.969377 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.972370 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.996307 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.006279 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     3714 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.017249 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3452 2023-04-12 02:15:47.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.030215 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.053154 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.074097 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.077089 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    43982 2023-04-14 09:45:29.000000 ht_pricing_module-0.1.37/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.677034 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4864 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:21:28.087063 ht_pricing_module-0.1.37/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-04-21 01:21:10.000000 ht_pricing_module-0.1.37/setup.py
```

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,17 @@
     double riskfree_rate                = 8;
     double dividend                     = 9;
     double leverage                     = 10;
     int32 year_base                     = 11;
     double payoff                       = 12;
     double barrier_price                = 13;
     double obs_freq                     = 14;
-    double final_position_multiplier    = 15;
-    repeated PayoffObservation obs_date = 16; // 观察日序列
+    double base_quantity                = 15;
+    double final_position_multiplier    = 16;
+    repeated PayoffObservation obs_date = 17; // 观察日序列
 
 }
 
 message FixedAccRequest {
     PriceType price_type                = 1;
     FixedAcc param                      = 2;
 }
```

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = self.param.payoff
             param['obs_freq'] = self.param.obs_freq
             non_leveraged_barrier = DiscreteBarrier(param)
 
-            rst = rst + (-self.param.leverage * leveraged_barrier.present_value() + non_leveraged_barrier.present_value())
+            rst = rst + self.param.base_quantity * (-self.param.leverage * leveraged_barrier.present_value() + non_leveraged_barrier.present_value())
 
         param = Struct({})
         param['option_type'] = leveraged_barrier_option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
```

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.1.37/ht_pricing_module/simple_pricer_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,14 +707,15 @@
             payoff:                     Union[int, float] = None,
             final_position_multiplier:  Union[int, float] = None,
             option_type:                int = OptionType.ACCUMULATOR,
             exercise_type:              int = ExerciseType.EUROPEAN,
             pricing_method:             int = PricingMethod.AS,
             obs_date:                   Union[dict, list, DataFrame] = None,
             obs_freq:                   Union[float, int] = 1,
+            base_quantity:              Union[float, int] = 1,
     ):
         """
 
         :param accumulator_type: 累计类型AccumulatorType属性
         :param option_type: 期权类型OptionType属性, ACCUMULATOR(累计), DECUMULATOR(累沽)
         :param exercise_type: 行权类型ExerciseType属性
         :param pricing_method: 模型方法PricingMethod属性
@@ -729,14 +730,15 @@
         :param year_base: 年化天数
         :param barrier_price: "LinearAcc，FixedAccBarrier, LinearAccAko, FixedAccAko, FixedAccEnhanced, LinearAccEnhanced必填参数" 障碍价格
         :param payoff: "FixedAcc，FixedAccBarrier, FixedAccAko, FixedAccEnhanced, LinearAccAko必填参数" rebate
         :param final_position_multiplier: 熔断累计到期日建仓乘数
         :param obs_date: 观测日，dict， Dataframe类型，默认每天到期一笔
                或RepeatedStruct返回结果: [Struct(), ...], Struct().obs_index离散观测日，Struct().obs_price为已实现价格日
         :param obs_freq 默认为1，每天到期一笔
+        :param base_quantity 每日观察数量
         :return: 累计期权定价引擎
         """
 
         assert option_type in [OptionType.ACCUMULATOR, OptionType.DECUMULATOR], option_type
 
         if accumulator_type in [AccumulatorType.LINEAR_ACC, AccumulatorType.FIXED_ACC_BARRIER]:
             assert (option_type == OptionType.ACCUMULATOR and strike_price <= barrier_price) or\
@@ -827,14 +829,15 @@
             assert payoff is not None and barrier_price is not None, "payoff & barrier is required for LinearAccFusing"
             param['payoff'] = payoff
             param['barrier_price'] = barrier_price
             param['obs_freq'] = obs_freq
             if final_position_multiplier is None:
                 final_position_multiplier = expiry_date - math.floor(current_date)
             param['final_position_multiplier'] = final_position_multiplier
+            param['base_quantity'] = base_quantity
             return LinearAccFusing(param)
 
     @classmethod
     def enhanced_asian(
             cls,
             option_type:                int,
             spot_price:                 Union[int, float],
```

### Comparing `ht_pricing_module-0.1.36/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.1.37/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.36/setup.py` & `ht_pricing_module-0.1.37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.1.36"
+VERSION = "0.1.37"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

