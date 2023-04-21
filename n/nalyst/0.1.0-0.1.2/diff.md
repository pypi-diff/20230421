# Comparing `tmp/nalyst-0.1.0.tar.gz` & `tmp/nalyst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.1.0.tar", last modified: Fri Apr 14 15:23:22 2023, max compression
+gzip compressed data, was "nalyst-0.1.2.tar", last modified: Fri Apr 21 12:17:43 2023, max compression
```

## Comparing `nalyst-0.1.0.tar` & `nalyst-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.705200 nalyst-0.1.0/
--rw-rw-rw-   0        0        0      424 2023-04-14 15:22:55.000000 nalyst-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 15:23:22.704203 nalyst-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.1.0/README.md
--rw-rw-rw-   0        0        0      655 2023-04-14 15:12:51.000000 nalyst-0.1.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.695105 nalyst-0.1.0/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.0/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.0/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 15:21:33.000000 nalyst-0.1.0/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.0/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.0/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.0/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.0/nalyst/PCA.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.0/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.0/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0      581 2023-04-14 15:21:58.000000 nalyst-0.1.0/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.703088 nalyst-0.1.0/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 15:23:22.705200 nalyst-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 15:22:21.000000 nalyst-0.1.0/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 15:22:15.000000 nalyst-0.1.0/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:17:43.907645 nalyst-0.1.2/
+-rw-rw-rw-   0        0        0      463 2023-04-21 12:06:49.000000 nalyst-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3699 2023-04-21 12:17:43.907645 nalyst-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-04-21 12:03:30.000000 nalyst-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1048 2023-04-21 12:15:20.000000 nalyst-0.1.2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:17:43.899673 nalyst-0.1.2/nalyst/
+-rw-rw-rw-   0        0        0      543 2023-04-21 11:36:57.000000 nalyst-0.1.2/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0      691 2023-04-21 11:36:49.000000 nalyst-0.1.2/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.2/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0      984 2023-04-21 12:14:36.000000 nalyst-0.1.2/nalyst/Error.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.2/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     2497 2023-04-21 12:14:38.000000 nalyst-0.1.2/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.2/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.2/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.2/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 11:32:07.000000 nalyst-0.1.2/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.2/nalyst/PCA.py
+-rw-rw-rw-   0        0        0      857 2023-04-21 11:33:07.000000 nalyst-0.1.2/nalyst/SharpeRatio.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.2/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.2/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-0.1.2/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     1048 2023-04-21 12:15:17.000000 nalyst-0.1.2/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 12:17:43.906649 nalyst-0.1.2/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     3699 2023-04-21 12:17:43.000000 nalyst-0.1.2/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-04-21 12:17:43.000000 nalyst-0.1.2/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 12:17:43.000000 nalyst-0.1.2/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-21 12:17:43.000000 nalyst-0.1.2/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 12:17:43.000000 nalyst-0.1.2/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 12:17:43.907645 nalyst-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-21 12:06:35.000000 nalyst-0.1.2/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 12:06:42.000000 nalyst-0.1.2/version.py
```

### Comparing `nalyst-0.1.0/LICENSE` & `nalyst-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/PKG-INFO` & `nalyst-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.0
+Version: 0.1.2
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -57,14 +57,31 @@
 INSTALLATION
 
 To install the library, simply run the following command in your terminal:
 
 pip install nalyst
 
 
+```text
+from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.DecisionTree import DecisionTree, Node
+from nalyst.KMeans import KMeans
+from nalyst.PCA import PCA
+from nalyst.LogisticRegression import LogisticRegression, accuracy
+from nalyst.MaxAbsScaler import MaxAbsScaler
+from nalyst.MinMaxScaler import MinMaxScaler
+from nalyst.StandardScaler import StandardScaler
+from nalyst.TestTrainSplit import TrainTestSplit
+from nalyst.MonteCarloSimulator import MonteCarloSimulator
+from nalyst.BetaFive import calculate_beta_five
+from nalyst.BetaMax import calculate_beta_max
+from nalyst.SharpeRatio import SharpRatio
+from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+```
+
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
```

### Comparing `nalyst-0.1.0/README.md` & `nalyst-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -32,14 +32,31 @@
 INSTALLATION
 
 To install the library, simply run the following command in your terminal:
 
 pip install nalyst
 
 
+```text
+from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.DecisionTree import DecisionTree, Node
+from nalyst.KMeans import KMeans
+from nalyst.PCA import PCA
+from nalyst.LogisticRegression import LogisticRegression, accuracy
+from nalyst.MaxAbsScaler import MaxAbsScaler
+from nalyst.MinMaxScaler import MinMaxScaler
+from nalyst.StandardScaler import StandardScaler
+from nalyst.TestTrainSplit import TrainTestSplit
+from nalyst.MonteCarloSimulator import MonteCarloSimulator
+from nalyst.BetaFive import calculate_beta_five
+from nalyst.BetaMax import calculate_beta_max
+from nalyst.SharpeRatio import SharpRatio
+from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+```
+
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
```

### Comparing `nalyst-0.1.0/nalyst/DecisionTree.py` & `nalyst-0.1.2/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/KMeans.py` & `nalyst-0.1.2/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/LogisticRegression.py` & `nalyst-0.1.2/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/MaxAbsScaler.py` & `nalyst-0.1.2/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/MinMaxScaler.py` & `nalyst-0.1.2/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/PCA.py` & `nalyst-0.1.2/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/StandardScaler.py` & `nalyst-0.1.2/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst/TestTrainSplit.py` & `nalyst-0.1.2/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.1.0/nalyst.egg-info/PKG-INFO` & `nalyst-0.1.2/nalyst.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.1.0
+Version: 0.1.2
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -57,14 +57,31 @@
 INSTALLATION
 
 To install the library, simply run the following command in your terminal:
 
 pip install nalyst
 
 
+```text
+from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.DecisionTree import DecisionTree, Node
+from nalyst.KMeans import KMeans
+from nalyst.PCA import PCA
+from nalyst.LogisticRegression import LogisticRegression, accuracy
+from nalyst.MaxAbsScaler import MaxAbsScaler
+from nalyst.MinMaxScaler import MinMaxScaler
+from nalyst.StandardScaler import StandardScaler
+from nalyst.TestTrainSplit import TrainTestSplit
+from nalyst.MonteCarloSimulator import MonteCarloSimulator
+from nalyst.BetaFive import calculate_beta_five
+from nalyst.BetaMax import calculate_beta_max
+from nalyst.SharpeRatio import SharpRatio
+from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
+```
+
 SUPPORT
 
 If you need help or have any questions, please feel free to reach out to
 
 COMMUNICATION 
 
 LinkedIn: https://www.linkedin.com/in/thapahemant/
```

### Comparing `nalyst-0.1.0/setup.py` & `nalyst-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.1.0',
+    version='0.1.2',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

