# Comparing `tmp/vcsc_data_common-0.1.2.tar.gz` & `tmp/vcsc_data_common-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.2.tar", last modified: Thu Apr 20 08:29:02 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.3.tar", last modified: Fri Apr 21 06:19:37 2023, max compression
```

## Comparing `vcsc_data_common-0.1.2.tar` & `vcsc_data_common-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.032338 vcsc_data_common-0.1.2/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-20 08:29:02.032421 vcsc_data_common-0.1.2/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.2/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.2/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-20 08:29:02.032731 vcsc_data_common-0.1.2/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.029652 vcsc_data_common-0.1.2/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.2/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.030977 vcsc_data_common-0.1.2/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.2/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.2/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.031302 vcsc_data_common-0.1.2/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.2/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.031560 vcsc_data_common-0.1.2/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.2/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.031823 vcsc_data_common-0.1.2/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.2/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.032096 vcsc_data_common-0.1.2/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3489 2023-04-20 08:27:30.000000 vcsc_data_common-0.1.2/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-20 08:29:02.030536 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-20 08:29:02.000000 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-20 08:29:02.000000 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-20 08:29:02.000000 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-20 08:29:02.000000 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-20 08:29:02.000000 vcsc_data_common-0.1.2/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.871372 vcsc_data_common-0.1.3/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-21 06:19:37.871454 vcsc_data_common-0.1.3/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.3/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.3/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-21 06:19:37.871878 vcsc_data_common-0.1.3/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.868498 vcsc_data_common-0.1.3/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.3/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.869877 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870214 vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870542 vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.870813 vcsc_data_common-0.1.3/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.3/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.871112 vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3444 2023-04-21 06:19:05.000000 vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-21 06:19:37.869268 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-21 06:19:37.000000 vcsc_data_common-0.1.3/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.2/pyproject.toml` & `vcsc_data_common-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.3/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.3/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.3/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.3/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.3/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         self.paper_trading_db_connection = create_engine(
             paper_trading_db_connection_str).connect()
 
     def get_all_portfolio(self):
         return pd.read_sql(f""" 
             select t1."portfolioConfigId",t4."tradingModel",t4."portfolioModel",t1.username,t1.symbol,COALESCE("latestMatchPrice",0) as "latestMatchPrice",
                 "totalAmount",CASE WHEN "forceSellAmount" > "availableAmount" THEN 0 ELSE "availableAmount" - "forceSellAmount"  END as "availableAmount",
-                "pendingAmount","scheduledAmount", "averageMatchedPrice","targetPercent",
-                "balance","initBalance", t1."cutoffDate", t1."startDate",t1."endDate", "forceSellAmount" , t1."portfolioType"
+                "scheduledAmount", "averageMatchedPrice","targetPercent",
+                "balance","initBalance", t1."cutoffDate", "forceSellAmount" , t1."portfolioType"
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
                 left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
         """, con=self.paper_trading_db_connection)
 
     def update_target_percent_portfolio(self, portfolio_data: dict, cycle_length: int, portfolioModel: int):
```

### Comparing `vcsc_data_common-0.1.2/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.3/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

