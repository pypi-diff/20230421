# Comparing `tmp/nalyst-0.1.3.tar.gz` & `tmp/nalyst-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.1.3.tar", last modified: Fri Apr 21 13:06:05 2023, max compression
+gzip compressed data, was "nalyst-0.1.5.tar", last modified: Fri Apr 21 13:28:48 2023, max compression
```

## Comparing `nalyst-0.1.3.tar` & `nalyst-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:06:05.353231 nalyst-0.1.3/
--rw-rw-rw-   0        0        0      463 2023-04-21 13:05:55.000000 nalyst-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3699 2023-04-21 13:06:05.353231 nalyst-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2023-04-21 12:03:30.000000 nalyst-0.1.3/README.md
--rw-rw-rw-   0        0        0     1048 2023-04-21 12:22:58.000000 nalyst-0.1.3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:06:05.347847 nalyst-0.1.3/nalyst/
--rw-rw-rw-   0        0        0      543 2023-04-21 11:36:57.000000 nalyst-0.1.3/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0      691 2023-04-21 11:36:49.000000 nalyst-0.1.3/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.3/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2118 2023-04-21 13:03:51.000000 nalyst-0.1.3/nalyst/Error.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.3/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     2497 2023-04-21 12:14:38.000000 nalyst-0.1.3/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.3/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.3/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.3/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 11:32:07.000000 nalyst-0.1.3/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.3/nalyst/PCA.py
--rw-rw-rw-   0        0        0      857 2023-04-21 11:33:07.000000 nalyst-0.1.3/nalyst/SharpeRatio.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.3/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.3/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.1.3/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     1033 2023-04-21 13:04:24.000000 nalyst-0.1.3/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:06:05.352235 nalyst-0.1.3/nalyst.egg-info/
--rw-rw-rw-   0        0        0     3699 2023-04-21 13:06:05.000000 nalyst-0.1.3/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-04-21 13:06:05.000000 nalyst-0.1.3/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:06:05.000000 nalyst-0.1.3/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-21 13:06:05.000000 nalyst-0.1.3/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 13:06:05.000000 nalyst-0.1.3/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 13:06:05.353231 nalyst-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-21 13:05:43.000000 nalyst-0.1.3/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-21 13:05:46.000000 nalyst-0.1.3/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.507531 nalyst-0.1.5/
+-rw-rw-rw-   0        0        0      463 2023-04-21 13:27:44.000000 nalyst-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3755 2023-04-21 13:28:48.507531 nalyst-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2640 2023-04-21 13:17:28.000000 nalyst-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1088 2023-04-21 13:28:28.000000 nalyst-0.1.5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.501551 nalyst-0.1.5/nalyst/
+-rw-rw-rw-   0        0        0      543 2023-04-21 11:36:57.000000 nalyst-0.1.5/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0      691 2023-04-21 11:36:49.000000 nalyst-0.1.5/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.5/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.5/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3538 2023-04-21 13:13:13.000000 nalyst-0.1.5/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.5/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.5/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.5/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 11:32:07.000000 nalyst-0.1.5/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.5/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-0.1.5/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0      857 2023-04-21 11:33:07.000000 nalyst-0.1.5/nalyst/SharpeRatio.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.5/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.5/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.1.5/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0      988 2023-04-21 13:13:37.000000 nalyst-0.1.5/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:28:48.506534 nalyst-0.1.5/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     3755 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 13:28:48.000000 nalyst-0.1.5/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 13:28:48.507531 nalyst-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-21 13:27:39.000000 nalyst-0.1.5/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 13:27:41.000000 nalyst-0.1.5/version.py
```

### Comparing `nalyst-0.1.3/LICENSE` & `nalyst-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/PKG-INFO` & `nalyst-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.3
+Version: 0.1.5
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,18 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-NALYST
-
-
-
 INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
@@ -50,23 +46,30 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION
+INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
+```text
 pip install nalyst
 
+pip install --upgrade nalyst
+
+pip show nalyst
+```
+
+IMPORT PACKAGES
 
 ```text
-from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
 from nalyst.MaxAbsScaler import MaxAbsScaler
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
@@ -85,7 +88,8 @@
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
 Github: https://github.com/harryworlds/nalyst
+
```

### Comparing `nalyst-0.1.3/README.md` & `nalyst-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-NALYST
-
-
-
 INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
@@ -25,23 +21,30 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION
+INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
+```text
 pip install nalyst
 
+pip install --upgrade nalyst
+
+pip show nalyst
+```
+
+IMPORT PACKAGES
 
 ```text
-from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
 from nalyst.MaxAbsScaler import MaxAbsScaler
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
@@ -59,8 +62,9 @@
 
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
-Github: https://github.com/harryworlds/nalyst
+Github: https://github.com/harryworlds/nalyst
+
```

### Comparing `nalyst-0.1.3/__init__.py` & `nalyst-0.1.5/nalyst/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.SharpeRatio import SharpRatio
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.Error import rmse, r_squared, mse
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -24,9 +23,8 @@
     'MinMaxScaler',
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
-    'Error'
 ]
```

### Comparing `nalyst-0.1.3/nalyst/BetaFive.py` & `nalyst-0.1.5/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/BetaMax.py` & `nalyst-0.1.5/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/DecisionTree.py` & `nalyst-0.1.5/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/KMeans.py` & `nalyst-0.1.5/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/LogisticRegression.py` & `nalyst-0.1.5/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/MaxAbsScaler.py` & `nalyst-0.1.5/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/MinMaxScaler.py` & `nalyst-0.1.5/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/MonteCarloSimulator.py` & `nalyst-0.1.5/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/PCA.py` & `nalyst-0.1.5/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/SharpeRatio.py` & `nalyst-0.1.5/nalyst/SharpeRatio.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/StandardScaler.py` & `nalyst-0.1.5/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/TestTrainSplit.py` & `nalyst-0.1.5/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/ThresholdClassifier.py` & `nalyst-0.1.5/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.3/nalyst/__init__.py` & `nalyst-0.1.5/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
 from nalyst.MonteCarloSimulator import MonteCarloSimulator
 from nalyst.BetaFive import calculate_beta_five
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.SharpeRatio import SharpRatio
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
-from nalyst.Error import Error
+from nalyst.RegressionPlot import RegressionPlot
 
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
@@ -24,9 +24,10 @@
     'MinMaxScaler',
     'StandardScaler',
     'TestTrainSplit',
     'MonteCarloSimulator',
     'BetaFive',
     'BetaMax',
     'SharpRatio',
-    'Error'
+    'ThresholdClassifier',
+    'RegressionPlot'
 ]
```

### Comparing `nalyst-0.1.3/nalyst.egg-info/PKG-INFO` & `nalyst-0.1.5/nalyst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.3
+Version: 0.1.5
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,18 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-NALYST
-
-
-
 INTRODUCTION
 
 Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
@@ -50,23 +46,30 @@
 MaxAbs Scale: a tool for scaling data to the absolute maximum value of each feature.
 
 Standard Scale: a tool for standardizing data to have a mean of 0 and a standard deviation of 1.
 
 Quick model training: with this library, users can quickly and easily train machine learning models, saving time and effort.
 
 
-INSTALLATION
+INSTALLATION PACKAGE
 
 To install the library, simply run the following command in your terminal:
 
+```text
 pip install nalyst
 
+pip install --upgrade nalyst
+
+pip show nalyst
+```
+
+IMPORT PACKAGES
 
 ```text
-from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.LinearRegression import LinearRegression
 from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
 from nalyst.MaxAbsScaler import MaxAbsScaler
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
@@ -85,7 +88,8 @@
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
 
 YouTube: https://www.youtube.com/channel/UCvMhAaE-L3rwkXUf4BnIhuQ
 
 Github: https://github.com/harryworlds/nalyst
+
```

### Comparing `nalyst-0.1.3/nalyst.egg-info/SOURCES.txt` & `nalyst-0.1.5/nalyst.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 __init__.py
 pyproject.toml
 setup.py
 version.py
 nalyst/BetaFive.py
 nalyst/BetaMax.py
 nalyst/DecisionTree.py
-nalyst/Error.py
 nalyst/KMeans.py
 nalyst/LinearRegression.py
 nalyst/LogisticRegression.py
 nalyst/MaxAbsScaler.py
 nalyst/MinMaxScaler.py
 nalyst/MonteCarloSimulator.py
 nalyst/PCA.py
+nalyst/RegressionPlot.py
 nalyst/SharpeRatio.py
 nalyst/StandardScaler.py
 nalyst/TestTrainSplit.py
 nalyst/ThresholdClassifier.py
 nalyst/__init__.py
 nalyst.egg-info/PKG-INFO
 nalyst.egg-info/SOURCES.txt
```

### Comparing `nalyst-0.1.3/setup.py` & `nalyst-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.1.3',
+    version='0.1.5',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

