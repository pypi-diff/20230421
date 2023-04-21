# Comparing `tmp/zelos-demeter-0.1.8.tar.gz` & `tmp/zelos-demeter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zelos-demeter-0.1.8.tar", last modified: Tue Nov 29 08:30:18 2022, max compression
+gzip compressed data, was "zelos-demeter-0.1.9.tar", last modified: Tue Dec 27 03:39:41 2022, max compression
```

## Comparing `zelos-demeter-0.1.8.tar` & `zelos-demeter-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.101463 zelos-demeter-0.1.8/
--rw-r--r--   0 florije    (501) staff       (20)     1063 2022-11-03 09:30:12.000000 zelos-demeter-0.1.8/LICENSE
--rw-r--r--   0 florije    (501) staff       (20)     1780 2022-11-29 08:30:18.101879 zelos-demeter-0.1.8/PKG-INFO
--rw-r--r--   0 florije    (501) staff       (20)     1450 2022-11-03 09:30:12.000000 zelos-demeter-0.1.8/README.md
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.016276 zelos-demeter-0.1.8/demeter/
--rw-r--r--   0 florije    (501) staff       (20)      749 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    15001 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/_typing.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.026267 zelos-demeter-0.1.8/demeter/broker/
--rw-r--r--   0 florije    (501) staff       (20)      134 2022-11-03 09:30:12.000000 zelos-demeter-0.1.8/demeter/broker/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)    29395 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/broker/broker.py
--rw-r--r--   0 florije    (501) staff       (20)     1951 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/broker/helper.py
--rw-r--r--   0 florije    (501) staff       (20)     7073 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/broker/liquitidymath.py
--rw-r--r--   0 florije    (501) staff       (20)     4318 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/broker/types.py
--rw-r--r--   0 florije    (501) staff       (20)     3124 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/broker/v3_core.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.042818 zelos-demeter-0.1.8/demeter/core/
--rw-r--r--   0 florije    (501) staff       (20)       54 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/core/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)        0 2022-10-08 08:28:15.000000 zelos-demeter-0.1.8/demeter/core/_typing.py
--rw-r--r--   0 florije    (501) staff       (20)    16047 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/core/actuator.py
--rw-r--r--   0 florije    (501) staff       (20)     4008 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/core/evaluating_indicator.py
--rw-r--r--   0 florije    (501) staff       (20)    14832 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/data_line.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.071064 zelos-demeter-0.1.8/demeter/download/
--rw-r--r--   0 florije    (501) staff       (20)      148 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     2712 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/_typing.py
--rw-r--r--   0 florije    (501) staff       (20)     3302 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/downloader.py
--rw-r--r--   0 florije    (501) staff       (20)     2265 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/eth_req.py
--rw-r--r--   0 florije    (501) staff       (20)     3060 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/process.py
--rw-r--r--   0 florije    (501) staff       (20)     2815 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/source_bigquery.py
--rw-r--r--   0 florije    (501) staff       (20)     7722 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/source_rpc.py
--rw-r--r--   0 florije    (501) staff       (20)     3559 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/download/swap_contract.py
--rw-r--r--   0 florije    (501) staff       (20)     2098 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/download/utils.py
--rw-r--r--   0 florije    (501) staff       (20)     4402 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/downloader.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.074515 zelos-demeter-0.1.8/demeter/etc/
--rw-r--r--   0 florije    (501) staff       (20)        0 2022-10-08 08:28:15.000000 zelos-demeter-0.1.8/demeter/etc/__init__.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.082265 zelos-demeter-0.1.8/demeter/indicator/
--rw-r--r--   0 florije    (501) staff       (20)      108 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/indicator/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)      913 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/indicator/common.py
--rw-r--r--   0 florije    (501) staff       (20)     2741 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/indicator/ma.py
--rw-r--r--   0 florije    (501) staff       (20)     1645 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/indicator/volatility.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.093637 zelos-demeter-0.1.8/demeter/strategy/
--rw-r--r--   0 florije    (501) staff       (20)      176 2022-11-03 09:30:12.000000 zelos-demeter-0.1.8/demeter/strategy/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     8950 2022-11-25 09:36:54.000000 zelos-demeter-0.1.8/demeter/strategy/strategy.py
--rw-r--r--   0 florije    (501) staff       (20)     3908 2022-11-09 02:24:52.000000 zelos-demeter-0.1.8/demeter/strategy/trigger.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.095778 zelos-demeter-0.1.8/demeter/utils/
--rw-r--r--   0 florije    (501) staff       (20)        0 2022-10-08 08:28:15.000000 zelos-demeter-0.1.8/demeter/utils/__init__.py
--rw-r--r--   0 florije    (501) staff       (20)     1098 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/demeter/utils/application.py
--rw-r--r--   0 florije    (501) staff       (20)       38 2022-11-29 08:30:18.103746 zelos-demeter-0.1.8/setup.cfg
--rw-r--r--   0 florije    (501) staff       (20)      964 2022-11-29 08:29:49.000000 zelos-demeter-0.1.8/setup.py
-drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-11-29 08:30:18.100350 zelos-demeter-0.1.8/zelos_demeter.egg-info/
--rw-r--r--   0 florije    (501) staff       (20)     1780 2022-11-29 08:30:17.000000 zelos-demeter-0.1.8/zelos_demeter.egg-info/PKG-INFO
--rw-r--r--   0 florije    (501) staff       (20)     1122 2022-11-29 08:30:17.000000 zelos-demeter-0.1.8/zelos_demeter.egg-info/SOURCES.txt
--rw-r--r--   0 florije    (501) staff       (20)        1 2022-11-29 08:30:17.000000 zelos-demeter-0.1.8/zelos_demeter.egg-info/dependency_links.txt
--rw-r--r--   0 florije    (501) staff       (20)       86 2022-11-29 08:30:17.000000 zelos-demeter-0.1.8/zelos_demeter.egg-info/requires.txt
--rw-r--r--   0 florije    (501) staff       (20)        8 2022-11-29 08:30:17.000000 zelos-demeter-0.1.8/zelos_demeter.egg-info/top_level.txt
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.376802 zelos-demeter-0.1.9/
+-rw-r--r--   0 florije    (501) staff       (20)     1063 2022-11-03 09:30:12.000000 zelos-demeter-0.1.9/LICENSE
+-rw-r--r--   0 florije    (501) staff       (20)     1780 2022-12-27 03:39:41.377569 zelos-demeter-0.1.9/PKG-INFO
+-rw-r--r--   0 florije    (501) staff       (20)     1450 2022-11-03 09:30:12.000000 zelos-demeter-0.1.9/README.md
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.332854 zelos-demeter-0.1.9/demeter/
+-rw-r--r--   0 florije    (501) staff       (20)      728 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    14325 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/_typing.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.338760 zelos-demeter-0.1.9/demeter/broker/
+-rw-r--r--   0 florije    (501) staff       (20)      134 2022-11-03 09:30:12.000000 zelos-demeter-0.1.9/demeter/broker/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)    29597 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/broker/broker.py
+-rw-r--r--   0 florije    (501) staff       (20)     1951 2022-11-25 09:36:54.000000 zelos-demeter-0.1.9/demeter/broker/helper.py
+-rw-r--r--   0 florije    (501) staff       (20)     7073 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/broker/liquitidymath.py
+-rw-r--r--   0 florije    (501) staff       (20)     4329 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/broker/types.py
+-rw-r--r--   0 florije    (501) staff       (20)     3197 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/broker/v3_core.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.347449 zelos-demeter-0.1.9/demeter/core/
+-rw-r--r--   0 florije    (501) staff       (20)       54 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/core/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)       25 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/core/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)    16252 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/core/actuator.py
+-rw-r--r--   0 florije    (501) staff       (20)     4397 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/demeter/core/evaluating_indicator.py
+-rw-r--r--   0 florije    (501) staff       (20)    14832 2022-11-25 09:36:54.000000 zelos-demeter-0.1.9/demeter/data_line.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.356838 zelos-demeter-0.1.9/demeter/download/
+-rw-r--r--   0 florije    (501) staff       (20)      148 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     2712 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/_typing.py
+-rw-r--r--   0 florije    (501) staff       (20)     3302 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/downloader.py
+-rw-r--r--   0 florije    (501) staff       (20)     2265 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/eth_req.py
+-rw-r--r--   0 florije    (501) staff       (20)     3060 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/process.py
+-rw-r--r--   0 florije    (501) staff       (20)     2815 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/source_bigquery.py
+-rw-r--r--   0 florije    (501) staff       (20)     7722 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/source_rpc.py
+-rw-r--r--   0 florije    (501) staff       (20)     3559 2022-11-25 09:36:54.000000 zelos-demeter-0.1.9/demeter/download/swap_contract.py
+-rw-r--r--   0 florije    (501) staff       (20)     2098 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/download/utils.py
+-rw-r--r--   0 florije    (501) staff       (20)     4402 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/downloader.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.357745 zelos-demeter-0.1.9/demeter/etc/
+-rw-r--r--   0 florije    (501) staff       (20)        0 2022-10-08 08:28:15.000000 zelos-demeter-0.1.9/demeter/etc/__init__.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.361925 zelos-demeter-0.1.9/demeter/indicator/
+-rw-r--r--   0 florije    (501) staff       (20)      108 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/indicator/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)      913 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/indicator/common.py
+-rw-r--r--   0 florije    (501) staff       (20)     2741 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/indicator/ma.py
+-rw-r--r--   0 florije    (501) staff       (20)     1645 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/indicator/volatility.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.365469 zelos-demeter-0.1.9/demeter/strategy/
+-rw-r--r--   0 florije    (501) staff       (20)      176 2022-11-03 09:30:12.000000 zelos-demeter-0.1.9/demeter/strategy/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     8950 2022-11-25 09:36:54.000000 zelos-demeter-0.1.9/demeter/strategy/strategy.py
+-rw-r--r--   0 florije    (501) staff       (20)     3908 2022-11-09 02:24:52.000000 zelos-demeter-0.1.9/demeter/strategy/trigger.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.367720 zelos-demeter-0.1.9/demeter/utils/
+-rw-r--r--   0 florije    (501) staff       (20)        0 2022-10-08 08:28:15.000000 zelos-demeter-0.1.9/demeter/utils/__init__.py
+-rw-r--r--   0 florije    (501) staff       (20)     1098 2022-11-29 08:29:49.000000 zelos-demeter-0.1.9/demeter/utils/application.py
+-rw-r--r--   0 florije    (501) staff       (20)       38 2022-12-27 03:39:41.378536 zelos-demeter-0.1.9/setup.cfg
+-rw-r--r--   0 florije    (501) staff       (20)      964 2022-12-27 03:38:49.000000 zelos-demeter-0.1.9/setup.py
+drwxr-xr-x   0 florije    (501) staff       (20)        0 2022-12-27 03:39:41.375898 zelos-demeter-0.1.9/zelos_demeter.egg-info/
+-rw-r--r--   0 florije    (501) staff       (20)     1780 2022-12-27 03:39:41.000000 zelos-demeter-0.1.9/zelos_demeter.egg-info/PKG-INFO
+-rw-r--r--   0 florije    (501) staff       (20)     1122 2022-12-27 03:39:41.000000 zelos-demeter-0.1.9/zelos_demeter.egg-info/SOURCES.txt
+-rw-r--r--   0 florije    (501) staff       (20)        1 2022-12-27 03:39:41.000000 zelos-demeter-0.1.9/zelos_demeter.egg-info/dependency_links.txt
+-rw-r--r--   0 florije    (501) staff       (20)       86 2022-12-27 03:39:41.000000 zelos-demeter-0.1.9/zelos_demeter.egg-info/requires.txt
+-rw-r--r--   0 florije    (501) staff       (20)        8 2022-12-27 03:39:41.000000 zelos-demeter-0.1.9/zelos_demeter.egg-info/top_level.txt
```

### Comparing `zelos-demeter-0.1.8/LICENSE` & `zelos-demeter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/PKG-INFO` & `zelos-demeter-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zelos-demeter
-Version: 0.1.8
+Version: 0.1.9
 Summary: better back testing tool for uniswap v3
 Home-page: https://zelos-demeter.readthedocs.io
 Author: zelos research
 Author-email: zelos@antalpha.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

### Comparing `zelos-demeter-0.1.8/README.md` & `zelos-demeter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/__init__.py` & `zelos-demeter-0.1.9/demeter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ._typing import UnitDecimal, TokenInfo, Asset, ActionTypeEnum, PositionInfo, AccountStatus, RowData, BaseAction, \
-    AddLiquidityAction, CollectFeeAction, RemoveLiquidityAction, BuyAction, SellAction, EvaluatingIndicator, \
+    AddLiquidityAction, CollectFeeAction, RemoveLiquidityAction, BuyAction, SellAction, \
     DemeterError, TimeUnitEnum, EthError
 from .broker import Broker, tick_to_quote_price, PoolBaseInfo, PoolStatus, BrokerAsset, Position
 from .core import Actuator
 from .data_line import LineTypeEnum, Cursorable, Line, Lines
 from .download import ChainType, DataSource
 from .indicator import simple_moving_average, exponential_moving_average, actual_volatility
 from .strategy import Strategy, Trigger, TimeRangesTrigger, TimeRangeTrigger, TimeRange, PeriodTrigger, PeriodsTrigger, \
```

### Comparing `zelos-demeter-0.1.8/demeter/_typing.py` & `zelos-demeter-0.1.9/demeter/_typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,21 @@
         :return: formatted string
         :rtype: str
         """
         dec = self.quantize(self.__integral) if self == self.to_integral() else self.normalize()
         return "{:{}} {}".format(dec, self.output_format, self.unit)
 
 
+class EvaluatorEnum(Enum):
+    ALL = 0
+    ANNUALIZED_RETURNS = 1
+    BENCHMARK_RETURNS = 2
+    MAX_DRAEDOWN = 3
+
+
 class TokenInfo(NamedTuple):
     """
     token info
 
     :param name: token symbol, will be set as unit of a token value
     :type name: str
     :param decimal: decimal of this token
@@ -442,43 +449,14 @@
                get_formatted_str({
                    "price": self.price.to_str(),
                    "fee": self.fee.to_str(),
                    "balance": f"{self.base_balance_after.to_str()}(+{self.base_change.to_str()}), {self.quote_balance_after.to_str()}(-{self.quote_change.to_str()})"
                })
 
 
-@dataclass
-class EvaluatingIndicator:
-    """
-    Indicator to evaluate a strategy
-
-    :param annualized_returns: annualized returns
-    :type annualized_returns: UnitDecimal
-    :param benchmark_returns: benchmark returns
-    :type benchmark_returns: UnitDecimal
-
-
-    """
-    annualized_returns: UnitDecimal
-    benchmark_returns: UnitDecimal
-    max_drawdown: UnitDecimal
-
-    def get_output_str(self) -> str:
-        """
-        get colored and formatted string to output in console
-        :return: formatted string
-        :rtype: str
-        """
-        return get_formatted_str({
-            "annualized_returns": self.annualized_returns.to_str(),
-            "benchmark_returns": self.benchmark_returns.to_str(),
-            "max_drawdown": self.max_drawdown.to_str()
-        })
-
-
 class DemeterError(Exception):
     def __init__(self, message):
         self.message = message
 
 
 class EthError(Exception):
     def __init__(self, code, message):
```

### Comparing `zelos-demeter-0.1.8/demeter/broker/broker.py` & `zelos-demeter-0.1.9/demeter/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self._init_amount1 = DECIMAL_ZERO
         # status
         self._positions: dict[PositionInfo:Position] = {}
         self._pool_status = PoolStatus(None, 0, DECIMAL_ZERO, DECIMAL_ZERO, DECIMAL_ZERO, DECIMAL_ZERO)
         self._price_unit = f"{self.base_asset.name}/{self.quote_asset.name}"
         # internal temporary variable
         self.action_buffer = []
+        self.allow_negative_balance = False
 
     def __str__(self):
         return f"Pool: {self.pool_info}, position count: {len(self.positions)}, " \
                f"balance: {self.base_asset.balance}{self.base_asset.name},{self.quote_asset.balance}{self.quote_asset.name}"
 
     @property
     def positions(self) -> dict[PositionInfo:Position]:
@@ -294,16 +295,16 @@
                                                                                     lower_tick,
                                                                                     upper_tick,
                                                                                     sqrt_price_x96)
         if position_info in self._positions:
             self._positions[position_info].liquidity += liquidity
         else:
             self._positions[position_info] = Position(DECIMAL_ZERO, DECIMAL_ZERO, liquidity)
-        self._asset0.sub(token0_used)
-        self._asset1.sub(token1_used)
+        self._asset0.sub(token0_used, self.allow_negative_balance)
+        self._asset1.sub(token1_used, self.allow_negative_balance)
         return position_info, token0_used, token1_used, liquidity
 
     def __remove_liquidity(self, position: PositionInfo, liquidity: int = None, sqrt_price_x96: int = -1):
         sqrt_price_x96 = int(sqrt_price_x96) if sqrt_price_x96 != -1 else get_sqrt_ratio_at_tick(
             self.pool_status.current_tick)
         delta_liquidity = liquidity if (liquidity is not None) and liquidity < self.positions[position].liquidity \
             else self.positions[position].liquidity
@@ -487,15 +488,15 @@
         :type remove_dry_pool: bool
         :return: (base_got,quote_get), base and quote token amounts collected from position
         :rtype:  (Decimal,Decimal)
         """
         if (max_collect_amount0 and max_collect_amount0 < 0) or \
                 (max_collect_amount1 and max_collect_amount1 < 0):
             raise DemeterError("collect amount should large than 0")
-        token0_get, token1_get = self.__collect_fee(self._positions[position])
+        token0_get, token1_get = self.__collect_fee(self._positions[position], max_collect_amount0, max_collect_amount1)
 
         base_get, quote_get = self.__convert_pair(token0_get, token1_get)
         if self._positions[position]:
             self.action_buffer.append(
                 CollectFeeAction(
                     base_balance_after=UnitDecimal(self.base_asset.balance, self.base_asset.name),
                     quote_balance_after=UnitDecimal(self.quote_asset.balance, self.quote_asset.name),
@@ -523,15 +524,15 @@
         :rtype: (Decimal, Decimal, Decimal)
         """
         price = price if price else self.pool_status.price
         from_amount = price * amount
         from_amount_with_fee = from_amount * (1 + self.pool_info.fee_rate)
         fee = from_amount_with_fee - from_amount
         from_asset, to_asset = self.__convert_pair(self._asset0, self._asset1)
-        from_asset.sub(from_amount_with_fee)
+        from_asset.sub(from_amount_with_fee, self.allow_negative_balance)
         to_asset.add(amount)
         base_amount, quote_amount = self.__convert_pair(from_amount, amount)
         self.action_buffer.append(
             BuyAction(base_balance_after=UnitDecimal(self.base_asset.balance, self.base_asset.name),
                       quote_balance_after=UnitDecimal(self.quote_asset.balance, self.quote_asset.name),
                       amount=UnitDecimal(amount, self.quote_asset.name),
                       price=UnitDecimal(price, self._price_unit),
@@ -554,15 +555,15 @@
         """
         price = price if price else self.pool_status.price
         from_amount_with_fee = amount
         from_amount = from_amount_with_fee * (1 - self.pool_info.fee_rate)
         to_amount = from_amount * price
         fee = from_amount_with_fee - from_amount
         to_asset, from_asset = self.__convert_pair(self._asset0, self._asset1)
-        from_asset.sub(from_amount_with_fee)
+        from_asset.sub(from_amount_with_fee, self.allow_negative_balance)
         to_asset.add(to_amount)
         base_amount, quote_amount = self.__convert_pair(to_amount, from_amount)
         self.action_buffer.append(
             SellAction(base_balance_after=UnitDecimal(self.base_asset.balance, self.base_asset.name),
                        quote_balance_after=UnitDecimal(self.quote_asset.balance, self.quote_asset.name),
                        amount=UnitDecimal(amount, self.quote_asset.name),
                        price=UnitDecimal(price, self._price_unit),
```

### Comparing `zelos-demeter-0.1.8/demeter/broker/helper.py` & `zelos-demeter-0.1.9/demeter/broker/helper.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/broker/liquitidymath.py` & `zelos-demeter-0.1.9/demeter/broker/liquitidymath.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/broker/types.py` & `zelos-demeter-0.1.9/demeter/broker/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     def __str__(self):
         """
         get string
         :return:
         :rtype:
         """
         return "PoolBaseInfo(Token0: {},".format(self.token0) + \
-               "Token1: {},".format(self.token1) + \
-               "fee: {},".format(self.fee_rate * Decimal(100)) + \
-               "base token: {})".format(self.token0.name if self.is_token0_base else self.token1.name)
+            "Token1: {},".format(self.token1) + \
+            "fee: {},".format(self.fee_rate * Decimal(100)) + \
+            "base token: {})".format(self.token0.name if self.is_token0_base else self.token1.name)
 
 
 class BrokerAsset(object):
     """
     Wallet of broker, manage balance of an asset.
     It will prevent excess usage on asset.
     """
@@ -59,15 +59,15 @@
     def __init__(self, token: TokenInfo, init_amount=Decimal(0)):
         self.token_info = token
         self.name = token.name
         self.decimal = token.decimal
         self.balance = init_amount
 
     def __str__(self):
-        return self.name
+        return f"{self.balance} {self.name}"
 
     def add(self, amount=Decimal(0)):
         """
         add amount to balance
         :param amount: amount to add
         :type amount: Decimal
         :return: entity itself
```

### Comparing `zelos-demeter-0.1.8/demeter/broker/v3_core.py` & `zelos-demeter-0.1.9/demeter/broker/v3_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
     @staticmethod
     def close_position(pool: PoolBaseInfo, position_info: PositionInfo, liquidity, sqrt_price_x96):
         return V3CoreLib.get_token_amounts(pool, position_info, sqrt_price_x96, liquidity)
 
     @staticmethod
     def get_token_amounts(pool: PoolBaseInfo, pos: PositionInfo, sqrt_price_x96, liquidity) -> (Decimal, Decimal):
+        if liquidity == 0: # performance improve
+            return 0, 0
         amount0, amount1 = get_amounts(sqrt_price_x96,
                                        pos.lower_tick,
                                        pos.upper_tick,
                                        liquidity,
                                        pool.token0.decimal,
                                        pool.token1.decimal)
         return amount0, amount1
```

### Comparing `zelos-demeter-0.1.8/demeter/core/actuator.py` & `zelos-demeter-0.1.9/demeter/core/actuator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
+import time
 from datetime import date, timedelta, datetime
 from decimal import Decimal
 
 import pandas as pd
 from tqdm import tqdm  # process bar
 
 from .evaluating_indicator import Evaluator
 from .. import PoolStatus
 from .._typing import AccountStatus, BarStatusNames, BaseAction, Asset, DemeterError, ActionTypeEnum, \
-    EvaluatingIndicator, RowData
+    RowData, EvaluatorEnum, UnitDecimal
 from ..broker import Broker, PoolBaseInfo
 from ..data_line import Lines
 from ..strategy import Strategy
 
 DEFAULT_DATA_PATH = "./data"
 
 
@@ -25,16 +26,17 @@
     Core component of a back test. Manage the resources in a test, including broker/strategy/data/indicator,
 
     :param pool_info: pool information
     :type pool_info: PoolBaseInfo
 
     """
 
-    def __init__(self, pool_info: PoolBaseInfo):
+    def __init__(self, pool_info: PoolBaseInfo, allow_negative_balance=False):
         self._broker: Broker = Broker(pool_info)
+        self._broker.allow_negative_balance = allow_negative_balance
         # data
         self._data: Lines = None
         # strategy
         self._strategy: Strategy = Strategy()
         # all the actions during the test(buy/sell/add liquidity)
         self._actions: [BaseAction] = []
         # actions in current bar
@@ -42,15 +44,15 @@
         self._broker.action_buffer = self.bar_actions
         # broker status in every bar, use array for performance
         self.account_status_list: [AccountStatus] = []
         # path of source data, which is saved by downloader
         self._data_path: str = DEFAULT_DATA_PATH
         # evaluating indicator calculator
         self._evaluator: Evaluator = None
-        self._enable_evaluating: bool = True
+        self._enabled_evaluator: [] = []
         # logging
         logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
         self.logger = logging.getLogger(__name__)
 
         # internal var
         self.__backtest_finished = False
 
@@ -113,22 +115,22 @@
 
         :return: action list
         :rtype: [BaseAction]
         """
         return self._actions
 
     @property
-    def evaluating_indicator(self) -> EvaluatingIndicator:
+    def evaluating_indicator(self) -> dict[EvaluatorEnum:UnitDecimal]:
         """
         evaluating indicator result
 
         :return:  evaluating indicator
         :rtype: EvaluatingIndicator
         """
-        return self._evaluator.evaluating_indicator if self._evaluator is not None else None
+        return self._evaluator.result if self._evaluator is not None else None
 
     @property
     def broker(self) -> Broker:
         """
         Broker manage assets in back testing. Including asset, positions. it also provides operations for positions,
 
         :return: Broker
@@ -311,15 +313,15 @@
         high_name, low_name = ("lowestTick", "highestTick") if self.broker.pool_info.is_token0_base \
             else ("highestTick", "lowestTick")
         df["low"] = df[high_name].map(lambda x: self.broker.tick_to_price(x))
         df["high"] = df[low_name].map(lambda x: self.broker.tick_to_price(x))
         df["volume0"] = df["inAmount0"].map(lambda x: Decimal(x) / 10 ** self.broker.pool_info.token0.decimal)
         df["volume1"] = df["inAmount1"].map(lambda x: Decimal(x) / 10 ** self.broker.pool_info.token1.decimal)
 
-    def run(self, enable_notify=True, enable_evaluating=True, print_final_status=False):
+    def run(self, enable_notify=True, evaluator=[EvaluatorEnum.ALL], print_final_status=False):
         """
         start back test, the whole process including:
 
         * reset actuator
         * initialize strategy (set object to strategy, then run strategy.initialize())
         * process each bar in data
             * prepare data in each row
@@ -333,15 +335,16 @@
         :param enable_notify: notify when new action happens
         :type enable_notify: bool
         :param enable_evaluating: enable evaluating indicator. if not enabled, no evaluating will be calculated
         :type enable_evaluating: bool
         :param print_final_status: enable output.
         :type print_final_status: bool
         """
-        self._enable_evaluating = enable_evaluating
+        run_begin_time = time.time()
+        self._enabled_evaluator = evaluator
         self.reset()
         if self._data is None:
             return
         self.logger.info("init strategy...")
         first_data = self._data.iloc[0]
         self._broker.pool_status = PoolStatus(self._data.index[0].to_pydatetime(),
                                               int(first_data.closeTick),
@@ -406,35 +409,35 @@
             self.logger.info("start notify all the actions")
             self.notify(self.strategy, self._actions)
         self.logger.info("main loop finished, start calculate evaluating indicator...")
         bar_status_df = pd.DataFrame(columns=BarStatusNames,
                                      index=self.data.index,
                                      data=map(lambda d: d.to_array(), self.account_status_list))
         self.logger.info("run evaluating indicator")
-        if self._enable_evaluating:
+        if len(self._enabled_evaluator) > 0:
             self._evaluator = Evaluator(
                 self._broker.get_init_account_status(init_price, self.data.index[0].to_pydatetime()),
                 bar_status_df)
-            self._evaluator.run()
+            self._evaluator.run(self._enabled_evaluator)
         self._strategy.finalize()
-        self.logger.info("back testing finish")
         self.__backtest_finished = True
         if print_final_status:
             self.output()
+        self.logger.info(f"back testing finish, execute time {time.time() - run_begin_time}s")
 
     def output(self):
         """
         output back test result to console
         """
         if self.__backtest_finished:
             print("Final status")
             print(self.broker.get_account_status(self.data.tail(1).price[0]).get_output_str())
-            if self._enable_evaluating:
+            if len(self._enabled_evaluator) > 0:
                 print("Evaluating indicator")
-                print(self._evaluator.evaluating_indicator.get_output_str())
+                print(self._evaluator.result)
         else:
             raise DemeterError("please run strategy first")
 
     def init_strategy(self):
         """
         initialize strategy, set property to strategy. and run strategy.initialize()
         """
```

### Comparing `zelos-demeter-0.1.8/demeter/core/evaluating_indicator.py` & `zelos-demeter-0.1.9/demeter/core/evaluating_indicator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from decimal import Decimal
+from typing import Union
 
 import pandas as pd
 
-from .._typing import AccountStatus, EvaluatingIndicator, DECIMAL_ZERO, UnitDecimal, DemeterError
-
-from typing import Union
+from .._typing import AccountStatus, UnitDecimal, DemeterError, EvaluatorEnum
 
 
 class Evaluator(object):
     """
     calculate evaluator indicator for strategy.
     """
 
@@ -16,22 +15,34 @@
         self.init_status: AccountStatus = init_status
         self.init_net_value = init_status.base_balance + init_status.quote_balance * init_status.price
         self.end_status = data.iloc[-1]
         self.data: Union[pd.DataFrame, AccountStatus] = data
         if len(data) < 2:
             raise DemeterError("not enough data")
         self.time_span_in_day = len(data.index) * (data.index[1] - data.index[0]).seconds / (60 * 60 * 24)
-        self._evaluating_indicator: EvaluatingIndicator = None
+        self._result = None
 
-    def run(self):
-        self._evaluating_indicator = EvaluatingIndicator(DECIMAL_ZERO, DECIMAL_ZERO, DECIMAL_ZERO)
-        self._evaluating_indicator.annualized_returns = UnitDecimal(self.get_annualized_returns(), "")
-        self._evaluating_indicator.benchmark_returns = UnitDecimal(self.get_benchmark_returns(), "")
-        self._evaluating_indicator.max_drawdown = UnitDecimal(Evaluator.get_max_drawdown_fast(self.data.net_value), "")
-        return self._evaluating_indicator
+    def run(self, enables: list[EvaluatorEnum]):
+        if EvaluatorEnum.ALL in enables:
+            enables = [x for x in EvaluatorEnum]
+            enables = filter(lambda x: x.value > 0, enables)
+        result_dict: dict[EvaluatorEnum:UnitDecimal] = {}
+        for request in enables:
+            match request:
+                case EvaluatorEnum.ANNUALIZED_RETURNS:
+                    result = UnitDecimal(self.get_annualized_returns(), "")
+                case EvaluatorEnum.BENCHMARK_RETURNS:
+                    result = UnitDecimal(self.get_benchmark_returns(), "")
+                case EvaluatorEnum.MAX_DRAEDOWN:
+                    result = UnitDecimal(Evaluator.get_max_drawdown_fast(self.data.net_value), "")
+                case _:
+                    raise DemeterError(f"{request} has not implied")
+            result_dict[request] = result
+        self._result = result_dict
+        return result_dict
 
     def get_annualized_returns(self):
         """Annualized return rate"""
         return (self.end_status.net_value / self.init_net_value) ** Decimal(365 / self.time_span_in_day) - 1
 
     def get_benchmark_returns(self):
         """
@@ -86,9 +97,9 @@
 
     def __get_benchmark_asset(self):
         base_amount = self.init_net_value / 2
         quote_amount = (self.init_net_value - base_amount) / self.init_status.price
         return base_amount, quote_amount
 
     @property
-    def evaluating_indicator(self):
-        return self._evaluating_indicator
+    def result(self) -> dict[EvaluatorEnum:UnitDecimal]:
+        return self._result
```

### Comparing `zelos-demeter-0.1.8/demeter/data_line.py` & `zelos-demeter-0.1.9/demeter/data_line.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/_typing.py` & `zelos-demeter-0.1.9/demeter/download/_typing.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/downloader.py` & `zelos-demeter-0.1.9/demeter/download/downloader.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/eth_req.py` & `zelos-demeter-0.1.9/demeter/download/eth_req.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/process.py` & `zelos-demeter-0.1.9/demeter/download/process.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/source_bigquery.py` & `zelos-demeter-0.1.9/demeter/download/source_bigquery.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/source_rpc.py` & `zelos-demeter-0.1.9/demeter/download/source_rpc.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/swap_contract.py` & `zelos-demeter-0.1.9/demeter/download/swap_contract.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/download/utils.py` & `zelos-demeter-0.1.9/demeter/download/utils.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/downloader.py` & `zelos-demeter-0.1.9/demeter/downloader.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/indicator/common.py` & `zelos-demeter-0.1.9/demeter/indicator/common.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/indicator/ma.py` & `zelos-demeter-0.1.9/demeter/indicator/ma.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/indicator/volatility.py` & `zelos-demeter-0.1.9/demeter/indicator/volatility.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/strategy/strategy.py` & `zelos-demeter-0.1.9/demeter/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/strategy/trigger.py` & `zelos-demeter-0.1.9/demeter/strategy/trigger.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/demeter/utils/application.py` & `zelos-demeter-0.1.9/demeter/utils/application.py`

 * *Files identical despite different names*

### Comparing `zelos-demeter-0.1.8/setup.py` & `zelos-demeter-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='zelos-demeter',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(exclude=["tests", "tests.*", "samples", "samples.*"]),
     url='https://zelos-demeter.readthedocs.io',
     license='MIT',
     author='zelos research',
     author_email='zelos@antalpha.com',
     description='better back testing tool for uniswap v3',
     long_description=long_description,
```

### Comparing `zelos-demeter-0.1.8/zelos_demeter.egg-info/PKG-INFO` & `zelos-demeter-0.1.9/zelos_demeter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zelos-demeter
-Version: 0.1.8
+Version: 0.1.9
 Summary: better back testing tool for uniswap v3
 Home-page: https://zelos-demeter.readthedocs.io
 Author: zelos research
 Author-email: zelos@antalpha.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

### Comparing `zelos-demeter-0.1.8/zelos_demeter.egg-info/SOURCES.txt` & `zelos-demeter-0.1.9/zelos_demeter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

