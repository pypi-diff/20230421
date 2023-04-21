# Comparing `tmp/td_ml_autosegmentation-1.0.8.tar.gz` & `tmp/td_ml_autosegmentation-1.0.9.tar.gz`

## Comparing `td_ml_autosegmentation-1.0.8.tar` & `td_ml_autosegmentation-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/.DS_Store
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/.DS_Store
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/__init__.py
--rw-r--r--   0        0        0    32943 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/autosegment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/LICENSE
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/.DS_Store
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/src/td_ml_autosegmentation/.DS_Store
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/src/td_ml_autosegmentation/__init__.py
+-rw-r--r--   0        0        0    33080 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/src/td_ml_autosegmentation/autosegment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/LICENSE
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.9/PKG-INFO
```

### Comparing `td_ml_autosegmentation-1.0.8/.DS_Store` & `td_ml_autosegmentation-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.8/src/.DS_Store` & `td_ml_autosegmentation-1.0.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/.DS_Store` & `td_ml_autosegmentation-1.0.9/src/td_ml_autosegmentation/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/autosegment.py` & `td_ml_autosegmentation-1.0.9/src/td_ml_autosegmentation/autosegment.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,25 +607,27 @@
         if df_clean[f].nunique() == 2:
             categorical.append(f)
         else:
             continuous.append(f)
             
     # information gain of categorical features
     if categorical == []:
-        out['cat_information_gain'] == [('no categorical features', 1)]
+        out['cat_information_gain'] == [('no_categorical_features', 1)]
     else:
         information_gain = []
         for cat in categorical:
             information_gain.append((cat, info_gain(df_clean, cat)))
         information_gain = sorted(information_gain, key=lambda x: x[1])
         out['cat_information_gain'] = information_gain
     
     # relative feature compactness (only for continuous variables)
     if continuous == []:
-        pass 
+        for k, v in out.items():
+            if k.startswith('cluster_'):
+                out[k] = {'compact_features': {'no_continuous_features': 0}}
     else:
         cont = df[continuous+['cluster']]
         rel_std = 1 - cont.groupby('cluster').std() / cont.drop('cluster', axis=1).std()
         for c in rel_std.index:
             t = rel_std.loc[c]
             out[f'cluster_{c}']['compact_features'] = t[t != 0].sort_values().to_dict()
```

### Comparing `td_ml_autosegmentation-1.0.8/README.md` & `td_ml_autosegmentation-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.8/pyproject.toml` & `td_ml_autosegmentation-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "td_ml_autosegmentation"
-version = "1.0.08"
+version = "1.0.09"
 authors = [
   { name="Yish Lim", email="limyishuen@gmail.com" },
 ]
 description = "TD Autosegmentation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `td_ml_autosegmentation-1.0.8/PKG-INFO` & `td_ml_autosegmentation-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: td_ml_autosegmentation
-Version: 1.0.8
+Version: 1.0.9
 Summary: TD Autosegmentation
 Project-URL: Homepage, https://github.com/treasure-data-ps/ml_autosegmentation
 Project-URL: Bug Tracker, https://github.com/treasure-data-ps/ml_autosegmentation
 Author-email: Yish Lim <limyishuen@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

