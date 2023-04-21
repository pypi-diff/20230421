# Comparing `tmp/vnpy_portfoliostrategy-1.0.4.tar.gz` & `tmp/vnpy_portfoliostrategy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_portfoliostrategy-1.0.4.tar", last modified: Wed Feb 15 14:29:51 2023, max compression
+gzip compressed data, was "vnpy_portfoliostrategy-1.0.5.tar", last modified: Fri Apr 21 00:34:34 2023, max compression
```

## Comparing `vnpy_portfoliostrategy-1.0.4.tar` & `vnpy_portfoliostrategy-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 14:29:51.285744 vnpy_portfoliostrategy-1.0.4/
--rw-rw-rw-   0        0        0     1099 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1931 2023-02-15 14:29:51.286765 vnpy_portfoliostrategy-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-02-15 14:29:15.000000 vnpy_portfoliostrategy-1.0.4/README.md
--rw-rw-rw-   0        0        0     1100 2023-02-15 14:29:51.289346 vnpy_portfoliostrategy-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:29:50.994275 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/
--rw-rw-rw-   0        0        0     1909 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/__init__.py
--rw-rw-rw-   0        0        0    32383 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/backtesting.py
--rw-rw-rw-   0        0        0      229 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/base.py
--rw-rw-rw-   0        0        0    21181 2023-02-15 14:28:16.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/engine.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:29:51.234731 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/
--rw-rw-rw-   0        0        0        0 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/__init__.py
--rw-rw-rw-   0        0        0     5137 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/pair_trading_strategy.py
--rw-rw-rw-   0        0        0     5403 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/pcp_arbitrage_strategy.py
--rw-rw-rw-   0        0        0     5415 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/portfolio_boll_channel_strategy.py
--rw-rw-rw-   0        0        0     4887 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/trend_following_strategy.py
--rw-rw-rw-   0        0        0    10216 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/template.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:29:51.284703 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/
--rw-rw-rw-   0        0        0       46 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/strategy.ico
--rw-rw-rw-   0        0        0    14495 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/widget.py
--rw-rw-rw-   0        0        0     9727 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/utility.py
-drwxrwxrwx   0        0        0        0 2023-02-15 14:29:51.200608 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/
--rw-rw-rw-   0        0        0     1931 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-02-15 14:29:50.000000 vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 00:34:34.302260 vnpy_portfoliostrategy-1.0.5/
+-rw-rw-rw-   0        0        0     1099 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1931 2023-04-21 00:34:34.302260 vnpy_portfoliostrategy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2023-04-21 00:33:14.000000 vnpy_portfoliostrategy-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1100 2023-04-21 00:34:34.304280 vnpy_portfoliostrategy-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:34:34.253034 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/
+-rw-rw-rw-   0        0        0     1909 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/__init__.py
+-rw-rw-rw-   0        0        0    33266 2023-04-21 00:32:22.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/backtesting.py
+-rw-rw-rw-   0        0        0      229 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/base.py
+-rw-rw-rw-   0        0        0    21482 2023-04-21 00:32:22.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:34:34.297113 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/
+-rw-rw-rw-   0        0        0        0 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/__init__.py
+-rw-rw-rw-   0        0        0     5137 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/pair_trading_strategy.py
+-rw-rw-rw-   0        0        0     5403 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/pcp_arbitrage_strategy.py
+-rw-rw-rw-   0        0        0     5415 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/portfolio_boll_channel_strategy.py
+-rw-rw-rw-   0        0        0     4887 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/trend_following_strategy.py
+-rw-rw-rw-   0        0        0    10376 2023-04-21 00:32:22.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/template.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:34:34.301236 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/
+-rw-rw-rw-   0        0        0       46 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2022-12-16 07:06:46.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/strategy.ico
+-rw-rw-rw-   0        0        0    14495 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/widget.py
+-rw-rw-rw-   0        0        0     9727 2022-12-16 07:07:17.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:34:34.289419 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/
+-rw-rw-rw-   0        0        0     1931 2023-04-21 00:34:33.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-04-21 00:34:34.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 00:34:33.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 00:34:33.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-21 00:34:33.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-21 00:34:33.000000 vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/top_level.txt
```

### Comparing `vnpy_portfoliostrategy-1.0.4/LICENSE` & `vnpy_portfoliostrategy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/PKG-INFO` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy_portfoliostrategy
-Version: 1.0.4
+Name: vnpy-portfoliostrategy
+Version: 1.0.5
 Summary: Portfolio strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的投资组合策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_portfoliostrategy-1.0.4/README.md` & `vnpy_portfoliostrategy-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # VeighNa框架的投资组合策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_portfoliostrategy-1.0.4/setup.cfg` & `vnpy_portfoliostrategy-1.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 706f 7274 666f 6c69   = vnpy_portfoli
 00000020: 6f73 7472 6174 6567 790d 0a76 6572 7369  ostrategy..versi
-00000030: 6f6e 203d 2031 2e30 2e34 0d0a 7572 6c20  on = 1.0.4..url 
+00000030: 6f6e 203d 2031 2e30 2e35 0d0a 7572 6c20  on = 1.0.5..url 
 00000040: 3d20 6874 7470 733a 2f2f 7777 772e 766e  = https://www.vn
 00000050: 7079 2e63 6f6d 0d0a 6c69 6365 6e73 6520  py.com..license 
 00000060: 3d20 4d49 540d 0a61 7574 686f 7220 3d20  = MIT..author = 
 00000070: 5869 616f 796f 7520 4368 656e 0d0a 6175  Xiaoyou Chen..au
 00000080: 7468 6f72 5f65 6d61 696c 203d 2078 6961  thor_email = xia
 00000090: 6f79 6f75 2e63 6865 6e40 6d61 696c 2e76  oyou.chen@mail.v
 000000a0: 6e70 792e 636f 6d0d 0a64 6573 6372 6970  npy.com..descrip
```

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/__init__.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/backtesting.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/backtesting.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 class BacktestingEngine:
     """组合策略回测引擎"""
 
     gateway_name: str = "BACKTESTING"
 
-    def __init__(self):
+    def __init__(self) -> None:
         """构造函数"""
         self.vt_symbols: List[str] = []
         self.start: datetime = None
         self.end: datetime = None
 
         self.rates: Dict[str, float] = 0
         self.slippages: Dict[str, float] = 0
@@ -140,41 +140,55 @@
 
         # 每次加载30天历史数据
         progress_delta: timedelta = timedelta(days=30)
         total_delta: timedelta = self.end - self.start
         interval_delta: timedelta = INTERVAL_DELTA_MAP[self.interval]
 
         for vt_symbol in self.vt_symbols:
-            start: datetime = self.start
-            end: datetime = self.start + progress_delta
-            progress = 0
-
-            data_count = 0
-            while start < self.end:
-                end = min(end, self.end)
+            if self.interval == Interval.MINUTE:
+                start: datetime = self.start
+                end: datetime = self.start + progress_delta
+                progress = 0
+
+                data_count = 0
+                while start < self.end:
+                    end = min(end, self.end)
+
+                    data: List[BarData] = load_bar_data(
+                        vt_symbol,
+                        self.interval,
+                        start,
+                        end
+                    )
+
+                    for bar in data:
+                        self.dts.add(bar.datetime)
+                        self.history_data[(bar.datetime, vt_symbol)] = bar
+                        data_count += 1
+
+                    progress += progress_delta / total_delta
+                    progress = min(progress, 1)
+                    progress_bar = "#" * int(progress * 10)
+                    self.output(f"{vt_symbol}加载进度：{progress_bar} [{progress:.0%}]")
 
+                    start = end + interval_delta
+                    end += (progress_delta + interval_delta)
+            else:
                 data: List[BarData] = load_bar_data(
                     vt_symbol,
                     self.interval,
-                    start,
-                    end
+                    self.start,
+                    self.end
                 )
 
                 for bar in data:
                     self.dts.add(bar.datetime)
                     self.history_data[(bar.datetime, vt_symbol)] = bar
-                    data_count += 1
-
-                progress += progress_delta / total_delta
-                progress = min(progress, 1)
-                progress_bar = "#" * int(progress * 10)
-                self.output(f"{vt_symbol}加载进度：{progress_bar} [{progress:.0%}]")
 
-                start = end + interval_delta
-                end += (progress_delta + interval_delta)
+                data_count = len(data)
 
             self.output(f"{vt_symbol}历史数据加载完成，数据量：{data_count}")
 
         self.output("所有历史数据加载完成")
 
     def run_backtesting(self) -> None:
         """开始回测"""
@@ -266,53 +280,59 @@
     def calculate_statistics(self, df: DataFrame = None, output=True) -> dict:
         """计算策略统计指标"""
         self.output("开始计算策略统计指标")
 
         if df is None:
             df: DataFrame = self.daily_df
 
-        if df is None:
-            # 如果没有成交记录则设置所有指标结果为0
-            start_date: str = ""
-            end_date: str = ""
-            total_days: int = 0
-            profit_days: int = 0
-            loss_days: int = 0
-            end_balance: float = 0
-            max_drawdown: float = 0
-            max_ddpercent: float = 0
-            max_drawdown_duration: int = 0
-            total_net_pnl: float = 0
-            daily_net_pnl: float = 0
-            total_commission: float = 0
-            daily_commission: float = 0
-            total_slippage: float = 0
-            daily_slippage: float = 0
-            total_turnover: float = 0
-            daily_turnover: float = 0
-            total_trade_count: int = 0
-            daily_trade_count: int = 0
-            total_return: float = 0
-            annual_return: float = 0
-            daily_return: float = 0
-            return_std: float = 0
-            sharpe_ratio: float = 0
-            return_drawdown_ratio: float = 0
-        else:
-            # 计算资金相关指标
+        # 初始化统计指标
+        start_date: str = ""
+        end_date: str = ""
+        total_days: int = 0
+        profit_days: int = 0
+        loss_days: int = 0
+        end_balance: float = 0
+        max_drawdown: float = 0
+        max_ddpercent: float = 0
+        max_drawdown_duration: int = 0
+        total_net_pnl: float = 0
+        daily_net_pnl: float = 0
+        total_commission: float = 0
+        daily_commission: float = 0
+        total_slippage: float = 0
+        daily_slippage: float = 0
+        total_turnover: float = 0
+        daily_turnover: float = 0
+        total_trade_count: int = 0
+        daily_trade_count: int = 0
+        total_return: float = 0
+        annual_return: float = 0
+        daily_return: float = 0
+        return_std: float = 0
+        sharpe_ratio: float = 0
+        return_drawdown_ratio: float = 0
+
+        # 检查是否发生过爆仓
+        positive_balance: bool = False
+
+        # 计算资金相关指标
+        if df is not None:
             df["balance"] = df["net_pnl"].cumsum() + self.capital
             df["return"] = np.log(df["balance"] / df["balance"].shift(1)).fillna(0)
-            df["highlevel"] = (
-                df["balance"].rolling(
-                    min_periods=1, window=len(df), center=False).max()
-            )
+            df["highlevel"] = df["balance"].rolling(min_periods=1, window=len(df), center=False).max()
             df["drawdown"] = df["balance"] - df["highlevel"]
             df["ddpercent"] = df["drawdown"] / df["highlevel"] * 100
 
-            # 计算统计指标
+            # 检查是否发生过爆仓
+            positive_balance = (df["balance"] > 0).all()
+            if not positive_balance:
+                self.output("回测中出现爆仓（资金小于等于0），无法计算策略统计指标")
+
+        # 计算统计指标
+        if positive_balance:
             start_date = df.index[0]
             end_date = df.index[-1]
 
             total_days: int = len(df)
             profit_days: int = len(df[df["net_pnl"] > 0])
             loss_days: int = len(df[df["net_pnl"] < 0])
 
@@ -687,18 +707,22 @@
         """发送邮件"""
         pass
 
     def sync_strategy_data(self, strategy: StrategyTemplate) -> None:
         """保存策略数据到文件"""
         pass
 
-    def get_pricetick(self, strategy: StrategyTemplate, vt_symbol) -> float:
-        """获取合约乘数"""
+    def get_pricetick(self, strategy: StrategyTemplate, vt_symbol: str) -> float:
+        """获取合约价格跳动"""
         return self.priceticks[vt_symbol]
 
+    def get_size(self, strategy: StrategyTemplate, vt_symbol: str) -> float:
+        """获取合约乘数"""
+        return self.sizes[vt_symbol]
+
     def put_strategy_event(self, strategy: StrategyTemplate) -> None:
         """推送事件更新策略界面"""
         pass
 
     def output(self, msg) -> None:
         """输出回测引擎信息"""
         print(f"{datetime.now()}\t{msg}")
```

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/engine.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,22 +211,31 @@
             self.write_log(f"撤单失败，找不到委托{vt_orderid}", strategy)
             return
 
         req: CancelRequest = order.create_cancel_request()
         self.main_engine.cancel_order(req, order.gateway_name)
 
     def get_pricetick(self, strategy: StrategyTemplate, vt_symbol: str) -> float:
-        """获取合约乘数"""
+        """获取合约价格跳动"""
         contract: Optional[ContractData] = self.main_engine.get_contract(vt_symbol)
 
         if contract:
             return contract.pricetick
         else:
             return None
 
+    def get_size(self, strategy: StrategyTemplate, vt_symbol: str) -> int:
+        """获取合约乘数"""
+        contract: Optional[ContractData] = self.main_engine.get_contract(vt_symbol)
+
+        if contract:
+            return contract.size
+        else:
+            return None
+
     def load_bars(self, strategy: StrategyTemplate, days: int, interval: Interval) -> None:
         """加载历史数据"""
         vt_symbols: list = strategy.vt_symbols
         dts: Set[datetime] = set()
         history_data: Dict[Tuple, BarData] = {}
 
         # 通过接口、数据服务、数据库获取历史数据
```

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/pair_trading_strategy.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/pair_trading_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/pcp_arbitrage_strategy.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/pcp_arbitrage_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/portfolio_boll_channel_strategy.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/portfolio_boll_channel_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/strategies/trend_following_strategy.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/strategies/trend_following_strategy.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/template.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,29 +272,33 @@
         """获取全部活动状态的委托号"""
         return list(self.active_orderids)
 
     def write_log(self, msg: str) -> None:
         """记录日志"""
         self.strategy_engine.write_log(msg, self)
 
-    def get_pricetick(self, vt_symbol) -> float:
+    def get_pricetick(self, vt_symbol: str) -> float:
         """查询合约最小价格跳动"""
         return self.strategy_engine.get_pricetick(self, vt_symbol)
 
+    def get_size(self, vt_symbol: str) -> int:
+        """查询合约乘数"""
+        return self.strategy_engine.get_size(self, vt_symbol)
+
     def load_bars(self, days: int, interval: Interval = Interval.MINUTE) -> None:
         """加载历史K线数据来执行初始化"""
         self.strategy_engine.load_bars(self, days, interval)
 
     def put_event(self) -> None:
         """推送策略数据更新事件"""
         if self.inited:
             self.strategy_engine.put_strategy_event(self)
 
     def send_email(self, msg: str) -> None:
         """发送邮件信息"""
         if self.inited:
             self.strategy_engine.send_email(msg, self)
 
-    def sync_data(self):
+    def sync_data(self) -> None:
         """同步策略状态数据到文件"""
         if self.trading:
             self.strategy_engine.sync_strategy_data(self)
```

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/strategy.ico` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/strategy.ico`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/ui/widget.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy/utility.py` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy/utility.py`

 * *Files identical despite different names*

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/PKG-INFO` & `vnpy_portfoliostrategy-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vnpy-portfoliostrategy
-Version: 1.0.4
+Name: vnpy_portfoliostrategy
+Version: 1.0.5
 Summary: Portfolio strategy application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 # VeighNa框架的投资组合策略模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.4-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.5-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
```

### Comparing `vnpy_portfoliostrategy-1.0.4/vnpy_portfoliostrategy.egg-info/SOURCES.txt` & `vnpy_portfoliostrategy-1.0.5/vnpy_portfoliostrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

