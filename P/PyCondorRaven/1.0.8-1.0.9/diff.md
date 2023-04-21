# Comparing `tmp/PyCondorRaven-1.0.8.tar.gz` & `tmp/PyCondorRaven-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCondorRaven-1.0.8.tar", last modified: Mon Feb 13 20:48:51 2023, max compression
+gzip compressed data, was "PyCondorRaven-1.0.9.tar", last modified: Tue Apr  4 15:34:01 2023, max compression
```

## Comparing `PyCondorRaven-1.0.8.tar` & `PyCondorRaven-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:48:51.872211 PyCondorRaven-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-13 20:48:51.872211 PyCondorRaven-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:48:51.872211 PyCondorRaven-1.0.8/PyCondorRaven/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/compare_value_against_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)    21509 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/features_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/fund_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    72028 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/hyperparam_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/preprocess_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    77721 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)    21609 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/reinforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/select_features_manually.py
--rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/series_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/series_predictor_lt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    67110 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/PyCondorRaven/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:48:51.872211 PyCondorRaven-1.0.8/PyCondorRaven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-13 20:48:51.000000 PyCondorRaven-1.0.8/PyCondorRaven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-13 20:48:51.000000 PyCondorRaven-1.0.8/PyCondorRaven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:48:51.000000 PyCondorRaven-1.0.8/PyCondorRaven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-13 20:48:51.000000 PyCondorRaven-1.0.8/PyCondorRaven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 20:48:51.872211 PyCondorRaven-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-13 20:48:41.000000 PyCondorRaven-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:34:01.290780 PyCondorRaven-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-04 15:34:01.290780 PyCondorRaven-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:34:01.290780 PyCondorRaven-1.0.9/PyCondorRaven/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/compare_value_against_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21509 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/features_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/fund_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72028 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/hyperparam_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/preprocess_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77721 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21609 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/reinforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/select_features_manually.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/series_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/series_predictor_lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/PyCondorRaven/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:34:01.290780 PyCondorRaven-1.0.9/PyCondorRaven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-04 15:34:01.000000 PyCondorRaven-1.0.9/PyCondorRaven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-04 15:34:01.000000 PyCondorRaven-1.0.9/PyCondorRaven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:34:01.000000 PyCondorRaven-1.0.9/PyCondorRaven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 15:34:01.000000 PyCondorRaven-1.0.9/PyCondorRaven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:34:01.290780 PyCondorRaven-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-04 15:33:51.000000 PyCondorRaven-1.0.9/setup.py
```

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/compare_value_against_returns.py` & `PyCondorRaven-1.0.9/PyCondorRaven/compare_value_against_returns.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/database.py` & `PyCondorRaven-1.0.9/PyCondorRaven/database.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/dynamo.py` & `PyCondorRaven-1.0.9/PyCondorRaven/dynamo.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/features_selection.py` & `PyCondorRaven-1.0.9/PyCondorRaven/features_selection.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/fund_selection.py` & `PyCondorRaven-1.0.9/PyCondorRaven/fund_selection.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/gcp.py` & `PyCondorRaven-1.0.9/PyCondorRaven/gcp.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/hyperparam_optim.py` & `PyCondorRaven-1.0.9/PyCondorRaven/hyperparam_optim.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/main.py` & `PyCondorRaven-1.0.9/PyCondorRaven/main.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/models.py` & `PyCondorRaven-1.0.9/PyCondorRaven/models.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/preprocess_dataset.py` & `PyCondorRaven-1.0.9/PyCondorRaven/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/raven.py` & `PyCondorRaven-1.0.9/PyCondorRaven/raven.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/reinforcement.py` & `PyCondorRaven-1.0.9/PyCondorRaven/reinforcement.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/representation.py` & `PyCondorRaven-1.0.9/PyCondorRaven/representation.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/series_predictor.py` & `PyCondorRaven-1.0.9/PyCondorRaven/series_predictor.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/series_predictor_lt.py` & `PyCondorRaven-1.0.9/PyCondorRaven/series_predictor_lt.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/simulation.py` & `PyCondorRaven-1.0.9/PyCondorRaven/simulation.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/test_algorithms.py` & `PyCondorRaven-1.0.9/PyCondorRaven/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/test_time.py` & `PyCondorRaven-1.0.9/PyCondorRaven/test_time.py`

 * *Files identical despite different names*

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven/utils.py` & `PyCondorRaven-1.0.9/PyCondorRaven/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 	assert data.ndim == 2
 	for i in range(data.shape[1]):
 		tmp = np.zeros((data.shape[0], n_features))
 		tmp[:, 0] = data[:, i]
 		data[:, i] = scaler.inverse_transform(tmp)[:, 0]
 	return data
 
-def normalize_data(data, scale=(0,1), train_size=0.8):
+def normalize_data(data, scale=(0,1), train_size=0.8, ignore_first_col=False):
     """
         Función para normalizar los datos, es decir, escalarlos en una escala que por *default* es [-1, 1]
 
         Parámetros:
         - values -- Arreglo de numpy, los datos
         - scaler -- Tupla de 2 valores, escala a la cual se quiere escalar los datos
 
@@ -341,17 +341,22 @@
         - scaler -- Instancia de MinMaxScaler, para luego revertir el proceso de escalamiento
     """
     # Be sure all values are numbers
     n_train = int(data.values.shape[0] * (train_size or 1))
     values_train = data.iloc[:n_train, :].astype('float32')
     # scale the data
     scaler = MinMaxScaler(feature_range=scale)
-    scaler.fit(values_train)
-    train_scaled = pd.DataFrame(scaler.transform(values_train), index=data.index[:n_train], columns=data.columns)
-    val_scaled = pd.DataFrame(scaler.transform(data.iloc[n_train:, :]), index=data.index[n_train:], columns=data.columns) if train_size is not None else None
+    if ignore_first_col:
+        scaler.fit(values_train.iloc[:, 1:])
+        train_scaled = pd.concat([values_train.iloc[:,0], pd.DataFrame(scaler.transform(values_train.iloc[:, 1:]), index=data.index[:n_train], columns=data.columns[1:])], axis=1)
+        val_scaled = pd.concat([data.iloc[n_train:, 0], pd.DataFrame(scaler.transform(data.iloc[n_train:, 1:]), index=data.index[n_train:], columns=data.columns[1:])], axis=1) if train_size is not None else None
+    else:
+        scaler.fit(values_train)
+        train_scaled = pd.DataFrame(scaler.transform(values_train), index=data.index[:n_train], columns=data.columns)
+        val_scaled = pd.DataFrame(scaler.transform(data.iloc[n_train:, :]), index=data.index[n_train:], columns=data.columns) if train_size is not None else None
     return train_scaled, val_scaled, scaler
 
 def series_to_supervised(data, n_in=1, n_out=1, dropnan=True):
 	"""
 		Función que convierte la serie de tiempo en datos supervisados para el modelo, es decir cambia el formato de (número de ejemplos, número de *features*)
 		por (número de ejemplos, número de *lags*, número de *features*)
```

### Comparing `PyCondorRaven-1.0.8/PyCondorRaven.egg-info/SOURCES.txt` & `PyCondorRaven-1.0.9/PyCondorRaven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

