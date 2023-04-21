# Comparing `tmp/edamame-0.48.tar.gz` & `tmp/edamame-0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.48.tar", last modified: Sun Apr 16 11:18:01 2023, max compression
+gzip compressed data, was "edamame-0.49.tar", last modified: Fri Apr 21 08:57:14 2023, max compression
```

## Comparing `edamame-0.48.tar` & `edamame-0.49.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.680333 edamame-0.48/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.48/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9914 2023-04-16 11:18:01.679942 edamame-0.48/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8160 2023-04-16 11:15:56.000000 edamame-0.48/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.674570 edamame-0.48/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-16 10:34:05.000000 edamame-0.48/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.676720 edamame-0.48/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      127 2023-04-16 11:13:18.000000 edamame-0.48/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21608 2023-04-16 11:09:39.000000 edamame-0.48/edamame/classifier/classification.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.678010 edamame-0.48/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.48/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.48/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.48/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.679391 edamame-0.48/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.48/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.48/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21388 2023-04-04 20:19:13.000000 edamame-0.48/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.676041 edamame-0.48/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9914 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-16 10:34:00.000000 edamame-0.48/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-16 11:18:01.680423 edamame-0.48/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.464614 edamame-0.49/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.49/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10798 2023-04-21 08:57:14.463685 edamame-0.49/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9044 2023-04-20 10:23:15.000000 edamame-0.49/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.456806 edamame-0.49/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-21 08:55:43.000000 edamame-0.49/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.459531 edamame-0.49/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      127 2023-04-16 11:13:18.000000 edamame-0.49/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21608 2023-04-16 11:09:39.000000 edamame-0.49/edamame/classifier/classification.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.461251 edamame-0.49/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.49/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.49/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.49/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.463037 edamame-0.49/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.49/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.49/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21361 2023-04-21 08:55:27.000000 edamame-0.49/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-21 08:57:14.458437 edamame-0.49/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10798 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-21 08:57:14.000000 edamame-0.49/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-21 08:55:48.000000 edamame-0.49/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-21 08:57:14.464711 edamame-0.49/setup.cfg
```

### Comparing `edamame-0.48/LICENSE` & `edamame-0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.48/PKG-INFO` & `edamame-0.49/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,14 @@
-Metadata-Version: 2.1
-Name: edamame
-Version: 0.48
-Summary: Exploratory data analysis tools
-Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/marcosalvalaggio/edamame
-Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/edamame/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
+<h1 align="center">
+<img src="logo.png" width="200">
+</h1><br>
+
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -161,14 +130,37 @@
 
 After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
 
 ```python
 from edamame.classifier import classifier_metrics
 ```
 
+### Example:
+
+```python
+from edamame.classifier import TrainClassifier
+from sklearn import datasets
+import edamame.eda as eda
+iris = datasets.load_iris()
+X = iris.data
+X = pd.DataFrame(X, columns=iris.feature_names)
+y = iris.target
+y = pd.DataFrame(y, columns=['y'])
+X_train, y_train, X_test, y_test = eda.setup(X,y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+classifier = TrainClassifier(X_train_s, y_train, X_test_s, y_test)
+models = classifier.auto_ml()
+svm = classifier.svm()
+classifier.model_metrics(model_name="svm")
+classifier.save_model(model_name="svm")
+svm_upload = eda.load_model(path="svm.pkl")
+classifier_metrics(svm_upload, X_train_s, y_train)
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.48/README.md` & `edamame-0.49/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,47 @@
-
+Metadata-Version: 2.1
+Name: edamame
+Version: 0.49
+Summary: Exploratory data analysis tools
+Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
+License: Copyright (c) 2018 The Python Packaging Authority
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/marcosalvalaggio/edamame
+Project-URL: Bug Tracker, https://github.com/marcosalvalaggio/edamame/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
+<h1 align="center">
+<img src="logo.png" width="200">
+</h1><br>
+
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -128,14 +163,37 @@
 
 After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
 
 ```python
 from edamame.classifier import classifier_metrics
 ```
 
+### Example:
+
+```python
+from edamame.classifier import TrainClassifier
+from sklearn import datasets
+import edamame.eda as eda
+iris = datasets.load_iris()
+X = iris.data
+X = pd.DataFrame(X, columns=iris.feature_names)
+y = iris.target
+y = pd.DataFrame(y, columns=['y'])
+X_train, y_train, X_test, y_test = eda.setup(X,y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+classifier = TrainClassifier(X_train_s, y_train, X_test_s, y_test)
+models = classifier.auto_ml()
+svm = classifier.svm()
+classifier.model_metrics(model_name="svm")
+classifier.save_model(model_name="svm")
+svm_upload = eda.load_model(path="svm.pkl")
+classifier_metrics(svm_upload, X_train_s, y_train)
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.48/edamame/classifier/classification.py` & `edamame-0.49/edamame/classifier/classification.py`

 * *Files identical despite different names*

### Comparing `edamame-0.48/edamame/eda/__init__.py` & `edamame-0.49/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.48/edamame/eda/eda.py` & `edamame-0.49/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.48/edamame/eda/tools.py` & `edamame-0.49/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.48/edamame/regressor/diagnose.py` & `edamame-0.49/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.48/edamame/regressor/regression.py` & `edamame-0.49/edamame/regressor/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 import pandas as pd
 import matplotlib.pyplot as plt 
 from IPython.display import display, Markdown
 from sklearn.linear_model import LinearRegression, Ridge, Lasso
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor
 import xgboost as xgb
-from sklearn.metrics import r2_score, mean_squared_error, mean_absolute_error, get_scorer_names
+from sklearn.metrics import r2_score, mean_squared_error, mean_absolute_error
 from sklearn.model_selection import GridSearchCV, KFold, cross_val_predict, cross_val_score
 import pickle
 from edamame.eda.tools import dataframe_review, dummy_control, setup
 from typing import Tuple, List, Literal, Union
 # pandas options
 pd.set_option('display.max_columns', None)
 pd.set_option('display.width', None)
 pd.set_option('display.max_colwidth', None)
 
 # list of metrics
-#get_scorer_names()
-
+#get_scorer
 
 class TrainRegressor:
     """
     This class represents a pipeline for training and handling regression models.
 
     Attributes: 
         X_train (pd.DataFrame): The input training data.
```

### Comparing `edamame-0.48/edamame.egg-info/PKG-INFO` & `edamame-0.49/edamame.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.48
+Version: 0.49
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,19 +27,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
-
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
+<h1 align="center">
+<img src="logo.png" width="200">
+</h1><br>
+
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -161,14 +163,37 @@
 
 After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
 
 ```python
 from edamame.classifier import classifier_metrics
 ```
 
+### Example:
+
+```python
+from edamame.classifier import TrainClassifier
+from sklearn import datasets
+import edamame.eda as eda
+iris = datasets.load_iris()
+X = iris.data
+X = pd.DataFrame(X, columns=iris.feature_names)
+y = iris.target
+y = pd.DataFrame(y, columns=['y'])
+X_train, y_train, X_test, y_test = eda.setup(X,y)
+X_train_s = eda.scaling(X_train)
+X_test_s = eda.scaling(X_test)
+classifier = TrainClassifier(X_train_s, y_train, X_test_s, y_test)
+models = classifier.auto_ml()
+svm = classifier.svm()
+classifier.model_metrics(model_name="svm")
+classifier.save_model(model_name="svm")
+svm_upload = eda.load_model(path="svm.pkl")
+classifier_metrics(svm_upload, X_train_s, y_train)
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.48/pyproject.toml` & `edamame-0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.48"
+version = "0.49"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

