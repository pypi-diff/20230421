# Comparing `tmp/nalyst-0.1.5.tar.gz` & `tmp/nalyst-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.1.5.tar", last modified: Fri Apr 21 13:28:48 2023, max compression
+gzip compressed data, was "nalyst-0.2.1.tar", last modified: Fri Apr 21 15:28:50 2023, max compression
```

## Comparing `nalyst-0.1.5.tar` & `nalyst-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.507531 nalyst-0.1.5/
--rw-rw-rw-   0        0        0      463 2023-04-21 13:27:44.000000 nalyst-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3755 2023-04-21 13:28:48.507531 nalyst-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2640 2023-04-21 13:17:28.000000 nalyst-0.1.5/README.md
--rw-rw-rw-   0        0        0     1088 2023-04-21 13:28:28.000000 nalyst-0.1.5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.501551 nalyst-0.1.5/nalyst/
--rw-rw-rw-   0        0        0      543 2023-04-21 11:36:57.000000 nalyst-0.1.5/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0      691 2023-04-21 11:36:49.000000 nalyst-0.1.5/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.5/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.5/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3538 2023-04-21 13:13:13.000000 nalyst-0.1.5/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.5/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.5/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.5/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 11:32:07.000000 nalyst-0.1.5/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.5/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.1.5/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0      857 2023-04-21 11:33:07.000000 nalyst-0.1.5/nalyst/SharpeRatio.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.5/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.5/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.1.5/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0      988 2023-04-21 13:13:37.000000 nalyst-0.1.5/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.506534 nalyst-0.1.5/nalyst.egg-info/
--rw-rw-rw-   0        0        0     3755 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 13:28:48.507531 nalyst-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-21 13:27:39.000000 nalyst-0.1.5/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 13:27:41.000000 nalyst-0.1.5/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:50.508547 nalyst-0.2.1/
+-rw-rw-rw-   0        0        0      463 2023-04-21 15:28:37.000000 nalyst-0.2.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3755 2023-04-21 15:28:50.508547 nalyst-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2640 2023-04-21 13:17:28.000000 nalyst-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1088 2023-04-21 13:29:45.000000 nalyst-0.2.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:50.503113 nalyst-0.2.1/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-0.2.1/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-0.2.1/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.2.1/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.2.1/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-0.2.1/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.2.1/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.2.1/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.2.1/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 11:32:07.000000 nalyst-0.2.1/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.2.1/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.2.1/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0      857 2023-04-21 11:33:07.000000 nalyst-0.2.1/nalyst/SharpeRatio.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.2.1/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.2.1/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.2.1/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     1088 2023-04-21 14:57:44.000000 nalyst-0.2.1/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:50.507549 nalyst-0.2.1/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     3755 2023-04-21 15:28:50.000000 nalyst-0.2.1/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-04-21 15:28:50.000000 nalyst-0.2.1/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:28:50.000000 nalyst-0.2.1/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-21 15:28:50.000000 nalyst-0.2.1/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 15:28:50.000000 nalyst-0.2.1/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:28:50.508547 nalyst-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-21 15:28:24.000000 nalyst-0.2.1/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 15:28:28.000000 nalyst-0.2.1/version.py
```

### Comparing `nalyst-0.1.5/LICENSE` & `nalyst-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/PKG-INFO` & `nalyst-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.5
+Version: 0.2.1
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.1.5/README.md` & `nalyst-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/__init__.py` & `nalyst-0.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/BetaFive.py` & `nalyst-0.2.1/nalyst/BetaFive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import yfinance as yf
 import numpy as np
 
 
 def calculate_beta_five(ticker, benchmark):
-    stock = yf.Ticker(ticker).history(period="5y", interval='1mo')
-    benchmark = yf.Ticker(benchmark).history(period="5y", interval='1mo')
+    try:
+        stock = yf.Ticker(ticker).history(period="5y", interval='1mo')
+        benchmark = yf.Ticker(benchmark).history(period="5y", interval='1mo')
 
-    stock_returns = stock['Close'].pct_change().dropna()
-    benchmark_returns = benchmark['Close'].pct_change().dropna()
+        # Align the dates of stock and benchmark DataFrames
+        stock, benchmark = stock.align(benchmark, join='inner', axis=0)
 
-    covariance = np.cov(stock_returns, benchmark_returns)[0][1]
-    benchmark_variance = np.var(benchmark_returns)
+        stock_returns = stock['Close'].pct_change().dropna()
+        benchmark_returns = benchmark['Close'].pct_change().dropna()
 
-    beta = covariance / benchmark_variance
-    return beta
+        covariance = np.cov(stock_returns, benchmark_returns)[0][1]
+        benchmark_variance = np.var(benchmark_returns)
+
+        beta = covariance / benchmark_variance
+        return beta
+    except Exception as e:
+        print(f"Error: Invalid ticker symbol - {e}")
+        return None
```

### Comparing `nalyst-0.1.5/nalyst/DecisionTree.py` & `nalyst-0.2.1/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/KMeans.py` & `nalyst-0.2.1/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/LinearRegression.py` & `nalyst-0.2.1/nalyst/LinearRegression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 from typing import List, Tuple
 
 
 class LinearRegression:
     """
     Class for building and analyzing a linear regression model.
     Attributes:
@@ -22,66 +23,50 @@
         predict(x: List[float]) -> List[float]: Generate predicted y values based on a list of x values.
         mse() -> float: Calculate the mean squared error of the model.
         rmse() -> float: Calculate the root mean squared error of the model.
         r_squared() -> float: Calculate the R-squared value of the model.
     """
 
     def __init__(self, x: List[float], y: List[float]):
-        """
-        Initialize the LinearRegressionModel class.
-        Args:
-            x (List[float]): List of x values.
-            y (List[float]): List of y values.
+        """ Initialize the LinearRegressionModel class.
+            Args:
+                x (List[float]): List of x values.
+                y (List[float]): List of y values.
         """
         self.x = x
         self.y = y
         self.x_mean = sum(x) / len(x)
         self.y_mean = sum(y) / len(y)
-        self.x_value = list(map(lambda value: value - self.x_mean, x))
-        self.y_value = list(map(lambda value: value - self.y_mean, y))
-        self.x_value_square = list(map(lambda value: value**2, self.x_value))
+        self.x_value = [value - self.x_mean for value in x]
+        self.y_value = [value - self.y_mean for value in y]
+        self.x_value_square = [value**2 for value in self.x_value]
         self.x_value_square_total = sum(self.x_value_square)
-        self.x_y_value_square = list(
-            map(lambda xv, yv: xv * yv, self.x_value, self.y_value))
+        self.x_y_value_square = [xv * yv for xv,
+                                 yv in zip(self.x_value, self.y_value)]
         self.x_y_value_square_total = sum(self.x_y_value_square)
         self.b1 = self.x_y_value_square_total / self.x_value_square_total
         self.bo = self.y_mean - (self.b1 * self.x_mean)
         self.n = len(x)
 
     def predict(self, x: List[float]) -> List[float]:
-        """
-        Generate predicted y values based on a list of x values.
-        Args:
-            x (List[float]): List of x values.
-        Returns:
-            List[float]: List of predicted y values.
-        """
-        return list(map(lambda xi: self.bo + self.b1 * xi, x))
+        return [self.bo + self.b1 * xi for xi in x]
 
-    def mse(self) -> float:
-        """
-        Calculate the mean squared error of the model.
-        Returns:
-            float: Mean squared error of the model.
-        """
+    def mean_squared_error(self):
         y_pred = self.predict(self.x)
-        return sum(list(map(lambda y_pred_i, y_i: (y_pred_i - y_i)**2, y_pred, self.y))) / self.n
+        return sum([(y_pred_i - y_i)**2 for y_pred_i, y_i in zip(y_pred, self.y)]) / self.n
 
-    def rmse(self) -> float:
-        """
-        Calculate the root mean squared error of the model.
-        Returns:
-            float: Root mean squared error of the model.
-        """
-        return self.mse() ** 0.5
+    def root_mean_squared_error(self):
+        return self.mean_squared_error() ** 0.5
 
-    def r_squared(self) -> float:
-        """Compute the R-squared value of the linear regression model. 
-       Returns:
-           float: R-squared value.
-       """
+    def r_squared(self):
         y_mean_line = [self.y_mean for _ in self.y]
         total_sum_squares = sum(
             [(y - y_mean_line[idx])**2 for idx, y in enumerate(self.y)])
         residual_sum_squares = sum(
             [(self.y[idx] - self.predict([x])[0])**2 for idx, x in enumerate(self.x)])
         return 1 - (residual_sum_squares / total_sum_squares)
+
+    def intercept(self) -> float:
+        return self.bo
+
+    def coefficient(self) -> float:
+        return self.b1
```

### Comparing `nalyst-0.1.5/nalyst/LogisticRegression.py` & `nalyst-0.2.1/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/MaxAbsScaler.py` & `nalyst-0.2.1/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/MinMaxScaler.py` & `nalyst-0.2.1/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/MonteCarloSimulator.py` & `nalyst-0.2.1/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/PCA.py` & `nalyst-0.2.1/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/RegressionPlot.py` & `nalyst-0.2.1/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/SharpeRatio.py` & `nalyst-0.2.1/nalyst/SharpeRatio.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/StandardScaler.py` & `nalyst-0.2.1/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/TestTrainSplit.py` & `nalyst-0.2.1/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/ThresholdClassifier.py` & `nalyst-0.2.1/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/nalyst/__init__.py` & `nalyst-0.2.1/nalyst/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.SharpeRatio import SharpRatio
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+from nalyst.RegressionPlot import RegressionPlot
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -23,8 +24,10 @@
     'MinMaxScaler',
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
+    'ThresholdClassifier',
+    'RegressionPlot'
 ]
```

### Comparing `nalyst-0.1.5/nalyst.egg-info/PKG-INFO` & `nalyst-0.2.1/nalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.5
+Version: 0.2.1
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.1.5/nalyst.egg-info/SOURCES.txt` & `nalyst-0.2.1/nalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.5/setup.py` & `nalyst-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.1.5',
+    version='0.2.1',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

