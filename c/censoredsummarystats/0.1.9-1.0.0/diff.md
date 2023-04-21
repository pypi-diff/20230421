# Comparing `tmp/censoredsummarystats-0.1.9.tar.gz` & `tmp/censoredsummarystats-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.1.9.tar", max compression
+gzip compressed data, was "censoredsummarystats-1.0.0.tar", max compression
```

## Comparing `censoredsummarystats-0.1.9.tar` & `censoredsummarystats-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-0.1.9/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    52645 2023-04-09 06:25:41.657236 censoredsummarystats-0.1.9/censoredsummarystats/censoredsummarystats.py
--rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-0.1.9/LICENSE
--rw-r--r--   0        0        0      534 2023-04-10 04:33:32.221568 censoredsummarystats-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-0.1.9/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-04-10 04:15:16.014879 censoredsummarystats-1.0.0/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    54586 2023-04-21 00:24:24.152651 censoredsummarystats-1.0.0/censoredsummarystats/censoredsummarystats.py
+-rw-r--r--   0        0        0    11558 2023-03-12 00:39:53.769556 censoredsummarystats-1.0.0/LICENSE
+-rw-r--r--   0        0        0      534 2023-04-21 00:58:48.149482 censoredsummarystats-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-03-12 00:39:53.771555 censoredsummarystats-1.0.0/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 censoredsummarystats-1.0.0/PKG-INFO
```

### Comparing `censoredsummarystats-0.1.9/censoredsummarystats/__init__.py` & `censoredsummarystats-1.0.0/censoredsummarystats/__init__.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.9/censoredsummarystats/censoredsummarystats.py` & `censoredsummarystats-1.0.0/censoredsummarystats/censoredsummarystats.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,39 +419,43 @@
         df['Result'] = df[censor_column] + df[numeric_column].astype(str)
     
     return df
 
 #%% Maximum Result
 
 def maximum_interval(df,
-                     groupby_columns = []):
+                     groupby_columns = None):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the maximum. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
     groupby_columns : list of strings, optional
         List of column names that should be used to create groups.
-        The default is [].
+        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the maximum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy().reset_index()
+    df = df.copy()
+    
+    # If no groups create empty list
+    if groupby_columns == None:
+        groupby_columns = []
     
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Maximum'
     groupby_columns.append('Statistic')
     
     # Determine left bound and boundary for maximum for each group.
     
@@ -485,35 +489,38 @@
     right['RightBoundary'] = np.where(condition,'Closed','Open')
     right = right[['RightBound','RightBoundary']]
     
     # Merge the two boundaries to create the interval for the maximum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index after groupby
+    df = df.reset_index()
+    
     return df
 
 def maximum(df,
-            groupby_columns = [[]],
+            groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant maximum and utility functions to
     generate the maxima results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
-    groupby_columns : list of lists of strings, optional
+    groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A maximum
         will be found within each group. Multiple lists can be supplied to
         perform sequential maxima before converting intervals to a result.
-        The default is [[]].
+        The default is None.
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
         provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
@@ -538,29 +545,36 @@
     Returns
     -------
     df : DataFrame
         DataFrame that contains a column with the relevant maximum or maxima
 
     '''
     
+    # Create a copy of the DataFrame
+    df = df.copy()
+    
     # If single result column provided, then split column
     if len(values) == 1:
         censor_column = 'CensorComponent'
         numeric_column = 'NumericComponent'
         df = result_to_components(df,values[0])
     # Else define the names to use for the censor and numeric columns
     else:
         censor_column = values[0]
         numeric_column = values[1]
     
     # Convert the results from censor and numeric components to an interval representation
     df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
     
-    # Cycle through each grouping
-    for grouping in groupby_columns:
+    # If multiple groupby lists, then cycle through them in order
+    if isinstance(groupby_columns[0],list):
+        for grouping in groupby_columns:
+            # Using the intervals, determine the range of possible maxima
+            df = maximum_interval(df, grouping)
+    else:
         # Using the intervals, determine the range of possible maxima
         df = maximum_interval(df, grouping)
     
     # Create interval notation for the maximum
     df = interval_notation(df, precision_rounding)
     
     # Convert the interval for the maximum into censor and numeric notation
@@ -573,40 +587,44 @@
     df = components_to_result(df, censor_column, numeric_column, precision_rounding)
     
     return df
 
 #%% Minimum Result
 
 def minimum_interval(df,
-                     groupby_columns = []):
+                     groupby_columns = None):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the minimum. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
     groupby_columns : list of strings, optional
         List of column names that should be used to create groups.
-        The default is [].
+        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the minimum (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy().reset_index()
+    df = df.copy()
     
+    # If no groups create empty list
+    if groupby_columns == None:
+        groupby_columns = []
+        
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Minimum'
     groupby_columns.append('Statistic')
     
     # Determine left bound and boundary for minimum for each group.
     
     # Consider the minimum bound for each left boundary option to determine
@@ -639,35 +657,38 @@
     right['RightBoundary'] = np.where(condition,'Closed','Open')
     right = right[['RightBound','RightBoundary']]
     
     # Merge the two boundaries to create the interval for the minimum
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index after groupby
+    df = df.reset_index()
+    
     return df
 
 def minimum(df,
-            groupby_columns = [[]],
+            groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant minimum and utility functions to
     generate the minima results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
-    groupby_columns : list of lists of strings, optional
+    groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A minimum
         will be found within each group. Multiple lists can be supplied to
         perform sequential minima before converting intervals to a result.
-        The default is [[]].
+        The default is None.
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
         provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
@@ -692,29 +713,36 @@
     Returns
     -------
     df : DataFrame
         DataFrame that contains a column with the relevant minimum or minima
 
     '''
     
+    # Create a copy of the DataFrame
+    df = df.copy()
+    
     # If single result column provided, then split column
     if len(values) == 1:
         censor_column = 'CensorComponent'
         numeric_column = 'NumericComponent'
         df = result_to_components(df,values[0])
     # Else define the names to use for the censor and numeric columns
     else:
         censor_column = values[0]
         numeric_column = values[1]
     
     # Convert the results from censor and numeric components to an interval representation
     df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
     
-    # Cycle through each grouping
-    for grouping in groupby_columns:
+    # If multiple groupby lists, then cycle through them in order
+    if isinstance(groupby_columns[0],list):
+        for grouping in groupby_columns:
+            # Using the intervals, determine the range of possible minima
+            df = minimum_interval(df, grouping)
+    else:
         # Using the intervals, determine the range of possible minima
         df = minimum_interval(df, grouping)
     
     # Create interval notation for the minimum
     df = interval_notation(df, precision_rounding)
     
     # Convert the interval for the minimum into censor and numeric notation
@@ -727,39 +755,43 @@
     df = components_to_result(df, censor_column, numeric_column, precision_rounding)
     
     return df
 
 #%% Average Result
 
 def average_interval(df,
-                     groupby_columns = []):
+                     groupby_columns = None):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for the average. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains results in a specific interval notation.
     groupby_columns : list of strings, optional
         List of column names that should be used to create groups.
-        The default is [].
+        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the average (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy().reset_index()
+    df = df.copy()
+    
+    # If no groups create empty list
+    if groupby_columns == None:
+        groupby_columns = []
     
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = 'Average'
     groupby_columns.append('Statistic')
     
     # Change notation of 'Closed' and 'Open' boundaries to 0 and 1, respectively
     # The presence of any open boundaries on one side ensure that the interval for the average is also
@@ -780,36 +812,39 @@
     df[['LeftBoundary','RightBoundary']] = df[['LeftBoundary','RightBoundary']].replace([0,1], ['Closed','Open'])
     
     # Means with infinite values produce nan values rather than np.inf values
     # Convert nan to inf only if infinite values are included in the mean
     df['LeftBound'] = np.where(df['Minimum'] == -np.inf, -np.inf, df['LeftBound'])
     df['RightBound'] = np.where(df['Maximum'] == np.inf, np.inf, df['RightBound'])
     
+    # Reset index after groupby
+    df = df.reset_index()
+    
     return df
 
 def average(df,
-            groupby_columns = [[]],
+            groupby_columns = None,
             values = ['CensorComponent','NumericComponent'],
             focus_high_potential = True,
             include_negative_interval = False,
             precision_tolerance_to_drop_censor = 0.25,
             precision_rounding = True):
     '''
     A function that combines the relevant average and utility functions to
     generate the average results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
-    groupby_columns : list of lists of strings, optional
+    groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. An average
         will be found within each group. Multiple lists can be supplied to
         perform sequential averaging before converting intervals to a result.
-        The default is [[]].
+        The default is None.
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
         provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
@@ -837,29 +872,36 @@
     Returns
     -------
     df : DataFrame
         DataFrame that contains calculated averages
 
     '''
     
+    # Create a copy of the DataFrame
+    df = df.copy()
+    
     # If single result column provided, then split column
     if len(values) == 1:
         censor_column = 'CensorComponent'
         numeric_column = 'NumericComponent'
         df = result_to_components(df,values[0])
     # Else define the names to use for the censor and numeric columns
     else:
         censor_column = values[0]
         numeric_column = values[1]
     
     # Convert the results from censor and numeric components to an interval representation
     df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
     
-    # Cycle through each grouping
-    for grouping in groupby_columns:
+    # If multiple groupby lists, then cycle through them in order
+    if isinstance(groupby_columns[0],list):
+        for grouping in groupby_columns:
+            # Using the intervals, determine the range of possible averages
+            df = average_interval(df, grouping)
+    else:
         # Using the intervals, determine the range of possible averages
         df = average_interval(df, grouping)
     
     # Create interval notation for the minimum
     df = interval_notation(df, precision_rounding)
     
     # Convert the interval for the minimum into censor and numeric notation
@@ -874,15 +916,15 @@
     return df
 
 #%% Percentile Result
 
 def percentile_interval(df,
                         percentile,
                         method = 'hazen',
-                        groupby_columns = []):
+                        groupby_columns = None):
     '''
     A function that analyses the interval notation form of results returned
     from components_to_interval to generate a new interval for percentiles. Groups
     of results can be defined by including the columns that should be used to
     create groups.
 
     Parameters
@@ -899,26 +941,30 @@
             - tukey
             - blom
             - hazen
             - excel
         The default is hazen.
     groupby_columns : list of strings, optional
         List of column names that should be used to create groups.
-        The default is [].
+        The default is None.
 
     Returns
     -------
     df : DataFrame
         DataFrame that has the interval for the percentile (for each group if
         column names are provided for grouping)
 
     '''
     
     # Create a copy of the DataFrame
-    df = df.copy().reset_index()
+    df = df.copy()
+    
+    # If no groups create empty list
+    if groupby_columns == None:
+        groupby_columns = []
     
     # Check the percentile is between 0 and 1
     if percentile < 0 or percentile > 100:
         raise Exception(f'Percentile out of range. Attempted percentile: {percentile}')
     
     # Create column that indicates the generated statistic and append to grouping list
     df['Statistic'] = f'Percentile-{percentile}'
@@ -1057,20 +1103,23 @@
     # Convert nan to inf only if infinite values are included in the mean
     right['RightBound'] = np.where(right['Maximum'] == np.inf, np.inf, right['RightBound'])
     
     # Merge the two boundaries to create the interval for the percentile
     # Check that the merge is 1-to-1
     df = left.merge(right, how = 'outer', on = groupby_columns, validate = '1:1')
     
+    # Reset index after groupby
+    df = df.reset_index()
+    
     return df
 
 def percentile(df,
                percentile,
                method = 'hazen',
-               groupby_columns = [[]],
+               groupby_columns = None,
                values = ['CensorComponent','NumericComponent'],
                focus_high_potential = True,
                include_negative_interval = False,
                precision_tolerance_to_drop_censor = 0.25,
                precision_rounding = True):
     '''
     A function that combines the relevant percentile and utility functions to
@@ -1088,20 +1137,20 @@
             Options include the following, ordered from largest to smallest result.
             - weiball
             - tukey
             - blom
             - hazen
             - excel
         The default is hazen.
-    groupby_columns : list of lists of strings, optional
+    groupby_columns : lists of strings (or list of lists), optional
         List of column names that should be used to create groups. A percentile
         will be found within each group. Multiple lists can be supplied to
         perform sequential median percentiles before calculating a percentile
         over the final grouping.
-        The default is [[]].
+        The default is None.
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
         provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
@@ -1129,37 +1178,44 @@
     Returns
     -------
     df : DataFrame
         DataFrame that contains calculated percentiles
 
     '''
     
+    # Create a copy of the DataFrame
+    df = df.copy()
+    
     # If single result column provided, then split column
     if len(values) == 1:
         censor_column = 'CensorComponent'
         numeric_column = 'NumericComponent'
         df = result_to_components(df,values[0])
     # Else define the names to use for the censor and numeric columns
     else:
         censor_column = values[0]
         numeric_column = values[1]
     
     # Convert the results from censor and numeric components to an interval representation
     df = components_to_interval(df, censor_column, numeric_column, include_negative_interval)
     
-    # Cycle through each grouping
-    for grouping in groupby_columns:
-        # Only apply percentile to final grouping
-        if grouping == groupby_columns[-1]:
-            # Using the intervals, determine the range of possible percentiles
-            df = percentile_interval(df, percentile, method, grouping)
-        # Apply median to all prior groupings
-        else:
-            # Using the intervals, determine the range of possible medians
-            df = percentile_interval(df, 50, method, grouping)
+    # If multiple groupby lists, then cycle through them in order
+    if isinstance(groupby_columns[0],list):
+        for grouping in groupby_columns:
+            # Only apply percentile to final grouping
+            if grouping == groupby_columns[-1]:
+                # Using the intervals, determine the range of possible percentiles
+                df = percentile_interval(df, percentile, method, grouping)
+            # Apply median to all prior groupings
+            else:
+                # Using the intervals, determine the range of possible medians
+                df = percentile_interval(df, 50, method, grouping)
+    else:
+        # Using the intervals, determine the range of possible percentiles
+        df = percentile_interval(df, percentile, method, grouping)
     
     # Create interval notation for the average
     df = interval_notation(df, precision_rounding)
     
     # Convert the interval for the minimum into censor and numeric notation
     df = interval_to_components(df, censor_column, numeric_column,
                                 focus_high_potential = focus_high_potential,
@@ -1168,33 +1224,33 @@
     
     # Combine the censor and numeric components into a result
     df = components_to_result(df, censor_column, numeric_column, precision_rounding)
     
     return df
 
 def median(df,
-           groupby_columns = [[]],
+           groupby_columns = None,
            values = ['CensorComponent','NumericComponent'],
            focus_high_potential = True,
            include_negative_interval = False,
            precision_tolerance_to_drop_censor = 0.25,
            precision_rounding = True):
     '''
     A function that generates median results for groups within a DataFrame.
 
     Parameters
     ----------
     df : DataFrame
         DataFrame that contains censored or uncensored results
-    groupby_columns : list of lists of strings, optional
-        List of column names that should be used to create groups. A percentile
+    groupby_columns : lists of strings (or list of lists), optional
+        List of column names that should be used to create groups. A median
         will be found within each group. Multiple lists can be supplied to
-        perform sequential median percentiles before calculating a percentile
+        perform sequential median percentiles before calculating a median
         over the final grouping.
-        The default is [[]].
+        The default is None.
     values : list of strings, optional
         The column name(s) for the column(s) that contain the results. If a 
         single column name is given, it is assumed that the column contains
         combined censor and numeric components. If two column names are
         provided, then the first should only contain one of five censors (<,≤,,≥,>)
         and the second should contain only numeric data.
         The default is ['CensorComponent','NumericComponent'].
@@ -1222,14 +1278,17 @@
     Returns
     -------
     df : DataFrame
         DataFrame that contains calculated percentiles
 
     '''
     
+    # Create a copy of the DataFrame
+    df = df.copy()
+    
     # Call percentile function with percentile = 50
     df = percentile(df,
                     50,
                     groupby_columns = groupby_columns,
                     values = values,
                     focus_high_potential = focus_high_potential,
                     include_negative_interval = include_negative_interval,
```

### Comparing `censoredsummarystats-0.1.9/LICENSE` & `censoredsummarystats-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.1.9/pyproject.toml` & `censoredsummarystats-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.1.9"
+version = "1.0.0"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 packages = [{include = "censoredsummarystats"}]
 
 [tool.poetry.dependencies]
```

### Comparing `censoredsummarystats-0.1.9/PKG-INFO` & `censoredsummarystats-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.1.9
+Version: 1.0.0
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

