# Comparing `tmp/td_ml_autosegmentation-1.0.7.tar.gz` & `tmp/td_ml_autosegmentation-1.0.8.tar.gz`

## Comparing `td_ml_autosegmentation-1.0.7.tar` & `td_ml_autosegmentation-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/.DS_Store
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/src/td_ml_autosegmentation/.DS_Store
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/src/td_ml_autosegmentation/__init__.py
--rw-r--r--   0        0        0    32672 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/src/td_ml_autosegmentation/autosegment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/LICENSE
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/.DS_Store
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/.DS_Store
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/__init__.py
+-rw-r--r--   0        0        0    32943 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/autosegment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/LICENSE
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 td_ml_autosegmentation-1.0.8/PKG-INFO
```

### Comparing `td_ml_autosegmentation-1.0.7/.DS_Store` & `td_ml_autosegmentation-1.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.7/src/.DS_Store` & `td_ml_autosegmentation-1.0.8/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.7/src/td_ml_autosegmentation/.DS_Store` & `td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.7/src/td_ml_autosegmentation/autosegment.py` & `td_ml_autosegmentation-1.0.8/src/td_ml_autosegmentation/autosegment.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
         if plot==True:
             shap.plots.bar(shap_values[:,:,i])
             shap.plots.beeswarm(shap_values[:,:,i])
             
     shaps = pd.concat(shaps)
     shap_stats = shaps.groupby(by=["feature", "cluster", "feature_value"], dropna=False, as_index=False).agg(['sum', 'count', 'mean'])
     shap_stats.columns = [item[0] + '_' + item[1] for item in shap_stats.columns]
-    # client.load_table_from_dataframe(shap_stats.reset_index(), 'as_shap_temp', writer='bulk_import', if_exists='overwrite')
+    client.load_table_from_dataframe(shap_stats.reset_index(), 'as_shap_temp', writer='bulk_import', if_exists='overwrite')
 
     if plot==True:
         fig = px.bar(fi.sort_values('impt'), x='impt', y='feature', title='Overall Proportional Feature Importances', 
         labels={'impt': 'Proportional Importance', 'feature': 'Feature'})
         fig.show()
 
     return fi, shap_stats.reset_index()
@@ -606,28 +606,32 @@
     for f in df_clean.drop(categorical+['cluster'], axis=1).columns:
         if df_clean[f].nunique() == 2:
             categorical.append(f)
         else:
             continuous.append(f)
             
     # information gain of categorical features
-    information_gain = []
-    for cat in categorical:
-        information_gain.append((cat, info_gain(df_clean, cat)))
-    information_gain = sorted(information_gain, key=lambda x: x[1])
-    
-    out['cat_information_gain'] = information_gain
-    
-    # relative feature compactness
-    cont = df[continuous+['cluster']]
-    rel_std = 1 - cont.groupby('cluster').std() / cont.drop('cluster', axis=1).std()
-    
-    for c in rel_std.index:
-        t = rel_std.loc[c]
-        out[f'cluster_{c}']['compact_features'] = t[t != 0].sort_values().to_dict()
+    if categorical == []:
+        out['cat_information_gain'] == [('no categorical features', 1)]
+    else:
+        information_gain = []
+        for cat in categorical:
+            information_gain.append((cat, info_gain(df_clean, cat)))
+        information_gain = sorted(information_gain, key=lambda x: x[1])
+        out['cat_information_gain'] = information_gain
+    
+    # relative feature compactness (only for continuous variables)
+    if continuous == []:
+        pass 
+    else:
+        cont = df[continuous+['cluster']]
+        rel_std = 1 - cont.groupby('cluster').std() / cont.drop('cluster', axis=1).std()
+        for c in rel_std.index:
+            t = rel_std.loc[c]
+            out[f'cluster_{c}']['compact_features'] = t[t != 0].sort_values().to_dict()
     
     return df, out
 
 
 def impt_df(out, rf=None, k_search=None, k_min=None):
     """Create a combined importances DataFrame.
 
@@ -670,14 +674,75 @@
         
         out = pd.concat([out, wss, ss])
 
     out["rnk"] = out.groupby(["kind", "cluster"])["impt"].rank("dense", ascending=False)
         
     return out.reset_index(drop=True)
 
+
+def get_histo(df_clean, impt_df, user_id, n=50):
+    
+    cont = impt_df[impt_df.kind=='feature_compactness']['feature'].unique().tolist()
+
+    histo = df_clean.copy()[cont+['cluster']]
+
+    for c in cont:
+        bins = n
+        hist = pd.qcut(histo[c], n, duplicates='drop')
+        while hist.nunique() == 1:
+            bins = bins + n
+            hist = pd.qcut(histo[c], bins, duplicates='drop')
+        histo[c] = hist
+
+    histos = []
+    for c in cont:
+        h = histo.reset_index()[[c, 'cluster', user_id]].groupby(['cluster', c]).count().reset_index()
+        h.columns = ['cluster', 'range', 'freq']
+        h['feature'] = c
+        histos.append(h)
+
+    out = pd.concat(histos)
+    out['lower'] = out['range'].map(lambda x: x.left)
+    out['upper'] = out['range'].map(lambda x: x.right)
+    
+    cat = impt_df[impt_df.kind == 'info_gain']['feature'].tolist()
+    
+    cats = []
+    for c in cat:
+        ct = df_clean.reset_index()[[user_id, 'cluster', c]].groupby(['cluster', c]).count().reset_index()
+        ct.columns = ['cluster', 'range', 'freq']
+        ct['feature'] = c
+        cats.append(ct)
+    cats = pd.concat(cats)
+    out = pd.concat([out, cats])
+    
+    return out.reset_index(drop=True)
+
+def obj_size_fmt(num):
+    if num<10**3:
+        return "{:.2f}{}".format(num,"B")
+    elif ((num>=10**3)&(num<10**6)):
+        return "{:.2f}{}".format(num/(1.024*10**3),"KB")
+    elif ((num>=10**6)&(num<10**9)):
+        return "{:.2f}{}".format(num/(1.024*10**6),"MB")
+    else:
+        return "{:.2f}{}".format(num/(1.024*10**9),"GB")
+
+
+def memory_usage():
+    memory_usage_by_variable=pd.DataFrame({k:sys.getsizeof(v)\
+    for (k,v) in globals().items()},index=['Size'])
+    memory_usage_by_variable=memory_usage_by_variable.T
+    memory_usage_by_variable=memory_usage_by_variable.sort_values(by='Size',ascending=False).head(10)
+    memory_usage_by_variable['Size']=memory_usage_by_variable['Size'].apply(lambda x: obj_size_fmt(x))
+    return memory_usage_by_variable
+
+
+""" functions below are for TD segment creation """
+
 def add_attribute_to_parent(audienceId, td_api_key, db, table, user_id, td_api_server,
             col_name='autosegmentation_cluster', rerun_master_segment='no'):
     
     source_headers = {
     'Authorization': 'TD1 '+ td_api_key}
 
     segment_api = td_api_server.replace('api', 'api-cdp')
@@ -796,65 +861,8 @@
         else:
             try:
                 segment_creation.json()['errors']['name'][0] == 'has already been taken'
                 print(f'Segment {cl.title()} already exists')
             except:
                 print(segment_creation.json()) ### check to see if segment already exists
             
-    return segments_json
-
-def get_histo(df_clean, impt_df, user_id, n=50):
-    
-    cont = impt_df[impt_df.kind=='feature_compactness']['feature'].unique().tolist()
-
-    histo = df_clean.copy()[cont+['cluster']]
-
-    for c in cont:
-        bins = n
-        hist = pd.qcut(histo[c], n, duplicates='drop')
-        while hist.nunique() == 1:
-            bins = bins + n
-            hist = pd.qcut(histo[c], bins, duplicates='drop')
-        histo[c] = hist
-
-    histos = []
-    for c in cont:
-        h = histo.reset_index()[[c, 'cluster', user_id]].groupby(['cluster', c]).count().reset_index()
-        h.columns = ['cluster', 'range', 'freq']
-        h['feature'] = c
-        histos.append(h)
-
-    out = pd.concat(histos)
-    out['lower'] = out['range'].map(lambda x: x.left)
-    out['upper'] = out['range'].map(lambda x: x.right)
-    
-    cat = impt_df[impt_df.kind == 'info_gain']['feature'].tolist()
-    
-    cats = []
-    for c in cat:
-        ct = df_clean.reset_index()[[user_id, 'cluster', c]].groupby(['cluster', c]).count().reset_index()
-        ct.columns = ['cluster', 'range', 'freq']
-        ct['feature'] = c
-        cats.append(ct)
-    cats = pd.concat(cats)
-    out = pd.concat([out, cats])
-    
-    return out.reset_index(drop=True)
-
-def obj_size_fmt(num):
-    if num<10**3:
-        return "{:.2f}{}".format(num,"B")
-    elif ((num>=10**3)&(num<10**6)):
-        return "{:.2f}{}".format(num/(1.024*10**3),"KB")
-    elif ((num>=10**6)&(num<10**9)):
-        return "{:.2f}{}".format(num/(1.024*10**6),"MB")
-    else:
-        return "{:.2f}{}".format(num/(1.024*10**9),"GB")
-
-
-def memory_usage():
-    memory_usage_by_variable=pd.DataFrame({k:sys.getsizeof(v)\
-    for (k,v) in globals().items()},index=['Size'])
-    memory_usage_by_variable=memory_usage_by_variable.T
-    memory_usage_by_variable=memory_usage_by_variable.sort_values(by='Size',ascending=False).head(10)
-    memory_usage_by_variable['Size']=memory_usage_by_variable['Size'].apply(lambda x: obj_size_fmt(x))
-    return memory_usage_by_variable
+    return segments_json
```

### Comparing `td_ml_autosegmentation-1.0.7/README.md` & `td_ml_autosegmentation-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `td_ml_autosegmentation-1.0.7/pyproject.toml` & `td_ml_autosegmentation-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "td_ml_autosegmentation"
-version = "1.0.07"
+version = "1.0.08"
 authors = [
   { name="Yish Lim", email="limyishuen@gmail.com" },
 ]
 description = "TD Autosegmentation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `td_ml_autosegmentation-1.0.7/PKG-INFO` & `td_ml_autosegmentation-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: td_ml_autosegmentation
-Version: 1.0.7
+Version: 1.0.8
 Summary: TD Autosegmentation
 Project-URL: Homepage, https://github.com/treasure-data-ps/ml_autosegmentation
 Project-URL: Bug Tracker, https://github.com/treasure-data-ps/ml_autosegmentation
 Author-email: Yish Lim <limyishuen@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

