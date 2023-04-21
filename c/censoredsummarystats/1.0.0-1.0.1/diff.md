# Comparing `tmp/censoredsummarystats-1.0.0.tar.gz` & `tmp/censoredsummarystats-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-1.0.0.tar", max compression
+gzip compressed data, was "censoredsummarystats-1.0.1.tar", max compression
```

## Comparing `censoredsummarystats-1.0.0.tar` & `censoredsummarystats-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-1.0.0/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    54586 2023-04-21 00:24:24.152651 censoredsummarystats-1.0.0/censoredsummarystats/censoredsummarystats.py
--rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-1.0.0/LICENSE
--rw-r--r--   0        0        0      534 2023-04-21 00:58:48.149482 censoredsummarystats-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-1.0.0/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-1.0.1/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    54495 2023-04-21 01:24:00.486982 censoredsummarystats-1.0.1/censoredsummarystats/censoredsummarystats.py
+-rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-1.0.1/LICENSE
+-rw-r--r--   0        0        0      534 2023-04-21 01:26:56.290650 censoredsummarystats-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-1.0.1/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-1.0.1/PKG-INFO
```

### Comparing `censoredsummarystats-1.0.0/censoredsummarystats/__init__.py` & `censoredsummarystats-1.0.1/censoredsummarystats/__init__.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-1.0.0/censoredsummarystats/censoredsummarystats.py` & `censoredsummarystats-1.0.1/censoredsummarystats/censoredsummarystats.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,17 +113,17 @@
     df['Interval'] += np.where(df['RightBoundary'].isin(['Open']), ')', ']')
     
     return df
 
 #%%% Convert between, results, components, intervals
 
 def result_to_components(df,
-          value_column,
-          censor_column = 'CensorComponent',
-          numeric_column = 'NumericComponent'):
+                         value_column,
+                         censor_column = 'CensorComponent',
+                         numeric_column = 'NumericComponent'):
     '''
     A function that separates censors (<,≤,≥,>) from a result. Splitting the
     censor component from the numeric component enables the use of numeric
     data types. A result of <10 (string/text) is split into a censor component
     of < (string/text) and a numeric component of 10 (float/decimal).
 
     Parameters
@@ -233,19 +233,19 @@
         df['LeftBoundary'] = np.where(condition, 'Closed', df['LeftBoundary'])
         df['LeftBound'] = np.where(condition, 0.0, df['LeftBound'])
     
     return df
 
 
 def interval_to_components(df,
-                       censor_column = 'CensorComponent',
-                       numeric_column = 'NumericComponent',
-                       focus_high_potential = True,
-                       include_negative_interval = False,
-                       precision_tolerance_to_drop_censor = 0.25):
+                           censor_column = 'CensorComponent',
+                           numeric_column = 'NumericComponent',
+                           focus_high_potential = True,
+                           include_negative_interval = False,
+                           precision_tolerance_to_drop_censor = 0.25):
     '''
     A function that determines the censor and numeric components
     from intervals
 
     Parameters
     ----------
     df : DataFrame
@@ -369,14 +369,17 @@
     # If no condition is met, default to <> and NaN
     df[censor_column] = np.select(conditions, censor_results, '<>')
     df[numeric_column] = np.select(conditions, numeric_results, np.nan)
     
     # Only return the censor and numeric columns
     df = df[['Interval',censor_column,numeric_column]]
     
+    # Reset index
+    df = df.reset_index()
+    
     return df
 
 
 def components_to_result(df,
                          censor_column = 'CensorComponent',
                          numeric_column = 'NumericComponent',
                          precision_rounding = True):
@@ -443,15 +446,15 @@
     df : DataFrame
         DataFrame that has the interval for the maximum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy()
+    df = df.copy().reset_index()
     
     # If no groups create empty list
     if groupby_columns == None:
         groupby_columns = []
     
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Maximum'
@@ -489,17 +492,14 @@
     right['RightBoundary'] = np.where(condition,'Closed','Open')
     right = right[['RightBound','RightBoundary']]
     
     # Merge the two boundaries to create the interval for the maximum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
-    # Reset index after groupby
-    df = df.reset_index()
-    
     return df
 
 def maximum(df,
             groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
@@ -611,15 +611,15 @@
     df : DataFrame
         DataFrame that has the interval for the minimum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy()
+    df = df.copy().reset_index()
     
     # If no groups create empty list
     if groupby_columns == None:
         groupby_columns = []
         
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Minimum'
@@ -657,17 +657,14 @@
     right['RightBoundary'] = np.where(condition,'Closed','Open')
     right = right[['RightBound','RightBoundary']]
     
     # Merge the two boundaries to create the interval for the minimum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
-    # Reset index after groupby
-    df = df.reset_index()
-    
     return df
 
 def minimum(df,
             groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
@@ -779,15 +776,15 @@
     df : DataFrame
         DataFrame that has the interval for the average (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy()
+    df = df.copy().reset_index()
     
     # If no groups create empty list
     if groupby_columns == None:
         groupby_columns = []
     
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Average'
@@ -812,17 +809,14 @@
     df[['LeftBoundary','RightBoundary']] = df[['LeftBoundary','RightBoundary']].replace([0,1], ['Closed','Open'])
     
     # Means with infinite values produce nan values rather than np.inf values
     # Convert nan to inf only if infinite values are included in the mean
     df['LeftBound'] = np.where(df['Minimum'] == -np.inf, -np.inf, df['LeftBound'])
     df['RightBound'] = np.where(df['Maximum'] == np.inf, np.inf, df['RightBound'])
     
-    # Reset index after groupby
-    df = df.reset_index()
-    
     return df
 
 def average(df,
             groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             focus_high_potential = True,
             include_negative_interval = False,
@@ -952,15 +946,15 @@
     df : DataFrame
         DataFrame that has the interval for the percentile (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy()
+    df = df.copy().reset_index()
     
     # If no groups create empty list
     if groupby_columns == None:
         groupby_columns = []
     
     # Check the percentile is between 0 and 1
     if percentile < 0 or percentile > 100:
@@ -1103,17 +1097,14 @@
     # Convert nan to inf only if infinite values are included in the mean
     right['RightBound'] = np.where(right['Maximum'] == np.inf, np.inf, right['RightBound'])
     
     # Merge the two boundaries to create the interval for the percentile
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
-    # Reset index after groupby
-    df = df.reset_index()
-    
     return df
 
 def percentile(df,
                percentile,
                method = 'hazen',
                groupby_columns = None,
                values = ['CensorComponent','NumericComponent'],
```

### Comparing `censoredsummarystats-1.0.0/LICENSE` & `censoredsummarystats-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-1.0.0/pyproject.toml` & `censoredsummarystats-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
```

### Comparing `censoredsummarystats-1.0.0/PKG-INFO` & `censoredsummarystats-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

